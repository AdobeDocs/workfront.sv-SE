---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Skapa och redigera affärsregler
description: Med en affärsregel kan du validera Workfront-objekt och hindra användare från att skapa, redigera eller ta bort ett objekt när vissa villkor är uppfyllda. Affärsreglerna bidrar till att förbättra datakvaliteten och effektiviteten genom att förhindra åtgärder som kan äventyra dataintegriteten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: 1cf16fd93de383aae66ba810ad85dd00806b8237
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---

# Skapa och redigera affärsregler

Med en affärsregel kan du validera Workfront-objekt och hindra användare från att skapa, redigera eller ta bort ett objekt när vissa villkor är uppfyllda. Affärsreglerna bidrar till att förbättra datakvaliteten och effektiviteten genom att förhindra åtgärder som kan äventyra dataintegriteten.

En affärsregel kan bara tilldelas ett objekt. Om du t.ex. skapar en affärsregel för att inte redigera projekt under vissa förhållanden, kan du inte använda samma regel för uppgifter. Du måste skapa en separat affärsregel med samma villkor för uppgifter.

Åtkomstnivåer och objektdelning har högre prioritet än affärsregler när en användare interagerar med ett objekt. Om en användare t.ex. har en åtkomstnivå eller behörighet som inte tillåter redigering av ett projekt, har de företräde framför en affärsregel som tillåter redigering av ett projekt under vissa villkor.

När mer än en affärsregel gäller för ett objekt följs alla regler, men tillämpas inte i en viss ordning. Du har till exempel två affärsregler. Det finns en begränsning för att skapa utgifter i februari. Den andra förhindrar redigering av ett projekt när projektstatusen är Slutförd. Om en användare försöker lägga till en utgift i ett slutfört projekt i juni, kan utgiften inte läggas till eftersom den har utlöst den andra regeln.

Affärsreglerna gäller för att skapa, redigera och ta bort objekt via API:t och Workfront-gränssnittet.

>[!NOTE]
>
>Eftersom affärsreglerna blockerar vissa åtgärder bör du alltid konfigurera dina affärsregler först i en sandlåda eller förhandsvisningsmiljö och testa dem noggrant innan du aktiverar dem i produktionen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront</td> 
   <td>Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr>  
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scenarier för affärsregler

Formatet på en affärsregel är&quot;OM det definierade villkoret uppfylls förhindras användaren från att utföra åtgärden på objektet och meddelandet visas.&quot;

Syntaxen för egenskaperna och andra funktioner i en affärsregel är densamma som syntaxen för ett beräkningsfält i ett anpassat formulär. Mer information om syntaxen finns i [Lägga till beräknade fält med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Mer information om IF-satser finns i [&quot;IF&quot;-programöversikt](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) och [Villkorsoperatorer i beräknade anpassade fält](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Mer information om användarbaserade jokertecken finns i [Använda användarbaserade jokertecken för att generera rapporter](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Mer information om datumbaserade jokertecken finns i [Generera rapporter med datumbaserade jokertecken](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

Ett API-jokertecken finns också i affärsreglerna. Använd `$$ISAPI` för att utlösa regeln endast i API:t. Använd `!$$ISAPI` om du bara vill framtvinga regeln i användargränssnittet och tillåta användare att kringgå regeln via API:t.

* Den här regeln förhindrar till exempel användare från att redigera slutförda projekt via API:t. Om jokertecknet inte användes skulle regeln blockera åtgärden både i användargränssnittet och i API:t.

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

Jokertecknen `$$BEFORE_STATE` och `$$AFTER_STATE` används i uttryck för att komma åt objektets fältvärden före och efter redigeringar.

* Dessa jokertecken är båda tillgängliga för redigeringsutlösaren. Standardläget för redigeringsutlösaren (om inget läge ingår i uttrycket) är `$$AFTER_STATE`.
* Utlösaren för att skapa objekt tillåter bara `$$AFTER_STATE` eftersom det tidigare läget inte finns.
* Borttagningsutlösaren för objekt tillåter bara `$$BEFORE_STATE` eftersom efterläget inte finns.

Några enkla affärsregelscenarier är:

* Användare kan inte lägga till nya utgifter under den sista veckan i februari. Denna formel kan anges som:

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* Användare kan inte redigera projektnamnet för ett projekt med statusen Fullständigt. Denna formel kan anges som:

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

Systemet tillåter en affärsregel per objekt och utlösare. En redigeringsutlösarregel tillåts t.ex. för utgåvor. Du kan dock inkludera flera regler i en formel med kapslade IF-satser.

Ett scenario med kapslade IF-satser är:

Användare kan inte redigera slutförda projekt och kan inte redigera projekt med ett planerat slutförandedatum i mars. Denna formel kan anges som:

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

## Lägg till en ny affärsregel

{{step-1-to-setup}}

1. Klicka på **Affärsregler** i den vänstra panelen.
1. Klicka på **Ny affärsregel**.
1. Välj den objekttyp som affärsregeln ska tilldelas till och klicka sedan på **Fortsätt**.

   ![Markera ett objekt](assets/object-for-business-rule3.png)

   Du kan tillämpa affärsregler på följande objekt:

   * Projekt
   * Uppgift
   * Problem/förfrågan
   * Portfolio
   * Dokument
   * Program
   * Utgift
   * Användare
   * Företag
   * Upprepning
   * Faktureringspost
   * Grupp
   * risk
   * Tilldelning
   * Jobbroll
   * Resurspool
   * Tid av
   * Timme
   * Mall

1. Skriv **Namn** för affärsregeln i dialogrutan Regelbyggaren.
1. I fältet **Är aktiv** väljer du om regeln ska vara aktiv när du sparar den.

   Om du väljer **Nej** sparas regeln som inaktiv och du kan aktivera den senare.

1. Välj en **utlösare** för affärsregeln. Alternativen är:

   * **När objekt skapas:** Regeln används när en användare försöker skapa ett objekt.
   * **Vid objektredigering:** Regeln används när en användare försöker redigera ett objekt.
   * **Vid borttagning av objekt:** Regeln används när en användare försöker ta bort ett objekt.

1. (Valfritt) Ange en **beskrivning** av affärsregeln och vad som händer när den tillämpas.
1. Bygg formeln i formelredigeraren i mitten av dialogrutan för affärsregler.

   Formatet på en affärsregel är&quot;OM det definierade villkoret uppfylls förhindras användaren från att utföra åtgärden på objektet och meddelandet visas.&quot;

   I formelområdet är de delar av affärsregeln som du skapar villkoret och det meddelande som visas i Workfront när villkoret är uppfyllt.

   * &quot;object&quot; är den objekttyp som du valde när du skapade affärsregeln. Den visas i dialogrutans rubrik.
   * &quot;action&quot; är den utlösare som du valde för regeln: skapa, redigera eller ta bort objektet.
   * Eftersom objektet och åtgärden redan är definierade, tar du inte med dem i formeln.
   * Det anpassade felmeddelandet visas för användaren när de utlöser affärsregeln. Den ska innehålla tydliga instruktioner om vad som gick fel och hur problemet ska åtgärdas.

     Du kan inkludera en statisk URL-adress i felmeddelandet, för att länka till dokumentation eller andra användbara sidor som hjälper användaren hur de ändrar sin åtgärd inom regelbegränsningen.

     I det här exemplet kommer &quot;Läs mer&quot; att länka till webbadressen. `"You are not allowed to add a new project in November.[Learn more](http://url)"` URL:en måste vara inom parentes, men länktext inom parentes krävs inte. Du kan visa den fullständiga URL:en och det blir en klickbar länk.

   ![Dialogrutan Lägg till affärsregel](assets/add-business-rule-dialog-no-ai-button.png)

   Det här exemplet är en affärsregel för projekt. Om den aktuella månaden är november får användarna inte skapa nya projekt, och meddelandet förklarar detta.

   Mer exempel på affärsregler finns i [Scenarier för affärsregler](#scenarios-for-business-rules) i den här artikeln.

1. (Valfritt) Använd formeln **Uttryck** och **Fält** på den högra panelen för att få hjälp med att skapa regeln.

   Sök efter ett uttryck eller fält för att begränsa listan med tillgängliga objekt.

   Listan med tillgängliga fält är begränsad till fält som är relaterade till objekttypen för affärsregeln.

1. Klicka på **Spara** när du är klar med att skapa affärsregeln.

>[!NOTE]
>
>När du har lagt till en affärsregel bör du testa den genom att lägga till, redigera eller ta bort det associerade objektet för att se till att regeln tillämpas korrekt.

## Aktivera en affärsregel

När en affärsregel är inaktiv visas Falskt i fältet Är aktiv i listan med affärsregler. Du kan inte uppdatera regelns status i listvyn.

Så här aktiverar du en affärsregel:

1. Markera affärsregeln i listan med regler och klicka på ikonen Redigera.
1. Välj **Ja** för **Är aktiv** i dialogrutan för affärsregler.
1. Klicka på **Spara**.

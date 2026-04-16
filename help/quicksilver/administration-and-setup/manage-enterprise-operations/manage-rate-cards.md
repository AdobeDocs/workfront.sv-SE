---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Hantera tariffkort
description: Ett tariffkort representerar det avtalsavtal med kunden där timtaxor har definierats för de jobbroller som kommer att slutföra arbetet. I ett avgiftskort kan du definiera flera faktureringsfrekvenser per jobbroll, baserat på attribut.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 0%

---

# Hantera tariffkort

Ett tariffkort representerar det avtalsavtal med kunden där timtaxor har definierats för de jobbroller som kommer att slutföra arbetet. På ett avgiftskort kan du definiera flera faktureringstariffer per jobbroll baserat på attribut som byrå, plats eller kostnadsställe. Attributen för din unika frekvens konfigureras under Konfigurera. Mer information finns i [Definiera tariffattribut](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

Du kan till exempel ha en befattning som Designer baserad i Paris för byrå A, en annan Designer baserad i Paris för byrå B och en tredje Designer baserad i New York som inte tilldelats någon byrå, var och en med olika faktureringstaxor. Attribut krävs dock inte för jobbroller på ett tariffkort. Attributen fungerar som verktyg för att fastställa mer detaljerade frekvenser. En faktureringstaxa på ett betalkort kan också vara giltighetsdatum, så att priset börjar och slutar på angivna datum.

Du kan även låsa hastigheter på ett tariffkort för att förhindra att de åsidosätts på projekt- eller aktivitetsnivå. Låsta frekvenser är den högsta i faktureringshierarkin, med undantag för bevarade frekvenser i ett projekt. Mer information finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Om du vill redigera ett tariffkort som delas med dig måste du ha behörigheten Hantera för tariffkortet.</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till ett tariffkort

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Klicka på [!UICONTROL **Nytt tariffkort**] och sedan på [!UICONTROL **Skapa nytt tariffkort**].
1. Ange ett namn och en beskrivning för tariffkortet i rutan [!UICONTROL **Nytt tariffkort**].

   Namnet måste vara unikt.

   ![Dialogrutan Nytt tariffkort](assets/new-rate-card-dialog.png)

1. (Valfritt) Välj en [!UICONTROL **grupp**] som tariffkort. Det här är byrån som definierar rabattkortet.
1. (Valfritt) Välj ett [!UICONTROL **företag**] som rabattkort. Detta är kunden som priserna avtalas för.

   >[!NOTE]
   >
   >Gruppen och företaget används inte bara i tariffkortsinformationen, utan också som filter när du kopplar ett kurskort till ett projekt.

1. Klicka på **Skapa**.

   Skärmen Klassificeringskort > Jobbroller och graderingar visas.

1. Klicka på [!UICONTROL **Lägg till jobbroll**].
1. I rutan [!UICONTROL **Ny faktureringstakt**] väljer du en [!UICONTROL **jobbroll**] som du vill definiera faktureringstariffer för.

   ![Dialogrutan Ny faktureringshastighet](assets/new-job-role-rate-on-rate-card.png)

1. (Valfritt) Välj attribut för faktureringssatsen, t.ex. byrå, plats eller kostnadsställe.

   >[!NOTE]
   >
   >Dessa attribut definieras separat och kan påverka intäkter och kostnadsberäkningar. Mer information finns i [Definiera tariffattribut](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Välj en [!UICONTROL **valuta**] som faktureringsränta.
1. (Valfritt) Ange ett [!UICONTROL **Jobbrollalias**] för jobbrollen.

   Om aliasnamnet du skriver inte redan finns kan du lägga till det.

   När hastighetskortet är kopplat till ett projekt visas aliaset på information som platshållartilldelningar, utgifter och rapporter i stället för den interna jobbrollens namn.

   >[!NOTE]
   >
   >* Endast ett alias kan finnas för varje jobbroll och attributkombination inom ett kreditkort.
   >* Ett alias måste uppdateras på tariffkortet och kan inte redigeras i ett projekt.

1. I fältet [!UICONTROL **Faktureringsgrad**] anger du faktureringsfrekvensen för den här jobbrollen och dess attribut.
1. (Valfritt) Välj [!UICONTROL **Lås frekvens**] om du vill låsa hastigheten och inte tillåta att den ändras på projekt- eller aktivitetsnivå. Du kan låsa upp den senare om det behövs.
1. (Valfritt) Klicka på [!UICONTROL **Lägg till giltighetsdatum**] om du vill använda giltighetsdatum för faktureringssatsen.
1. (Valfritt) Klicka på [!UICONTROL **Lägg till giltighetsfrekvens**] igen om du vill lägga till fler faktureringstariffer med giltighetsdatum för den här jobbrollen och dess attribut.
1. (Villkorligt) Om du lägger till mer än en faktureringsfrekvens för den här jobbrollen anger du följande information:

   * [!UICONTROL **Faktureringsränta**]: Värdet på faktureringssatsen för tidsperioden.
   * [!UICONTROL **Startdatum**]: Det datum då tariffen börjar.
   * [!UICONTROL **Slutdatum**]: Det datum då hastigheten slutar.

     Den första faktureringstakten behöver inte ha något startdatum och den sista faktureringstakten behöver inte ha något slutdatum. Mellanrum tillåts mellan hastighetsdatum, men överlappande datum tillåts inte. Under en lucka används andra områden i faktureringshierarkin för att fastställa faktureringssatsen baserat på en uppgifts intäktstyp. Mer information finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

1. Klicka på [!UICONTROL **Spara**].
1. (Valfritt) Om du vill lägga till en annan faktureringsfrekvens, antingen för samma jobbroll med olika attribut eller för en separat jobbroll, klickar du på [!UICONTROL **Lägg till jobbroll**].

   Kurserna för varje roll läggs till i tariffkortet när du skapar dem. Aktuell gällande kurs, baserat på datum, anges med ikonen ![Aktuell frekvens](assets/current-rate-icon.png).

   ![Betygsätt kort med visade frekvenser](assets/rates-on-rate-card.png)

## Redigera information om tariffkort och tariffer

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Om du vill redigera ett befintligt tariffkort klickar du på namnet på tariffkortet i listan Klassificeringskort.
1. Klicka på [!UICONTROL **Information**] i den vänstra panelen om du vill uppdatera information om tariffkort.
1. (Valfritt) Om du vill bifoga ett anpassat formulär till tariffkortet klickar du på fältet [!UICONTROL **Lägg till anpassat formulär**] i det övre högra hörnet på detaljsidan och väljer ett anpassat formulär i listan som visas.

   Mer information om hur du bifogar ett anpassat formulär finns i [Lägga till ett anpassat formulär till ett objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicka på [!UICONTROL **Spara ändringar**] när du har redigerat hastighetskortsinformationen.
1. Klicka på [!UICONTROL **Jobbroller och frekvenser**] i den vänstra panelen för att redigera faktureringstarifferna.
1. Om du vill redigera en frekvens markerar du kryssrutan bredvid hastigheten och klickar på [!UICONTROL **Redigera**] i åtgärdsfältet längst ned på skärmen.

   Mer information om åtgärdsfältet finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   >[!NOTE]
   >
   >Eftersom varje frekvens är associerad med kombinationen av rollen och attribut för att skapa en unik frekvens, kan rollen och attributen inte ändras när du redigerar en frekvens.

1. Om du vill ta bort en faktureringstaxa från tariffkortet markerar du kryssrutan bredvid tariffen och klickar på [!UICONTROL **Ta bort**] i åtgärdsfältet.
1. Om du vill låsa en frekvens markerar du kryssrutan bredvid hastigheten och klickar på [!UICONTROL **Lås**] i åtgärdsfältet.

   Låsta frekvenser kan inte ändras på projekt- eller aktivitetsnivå. En låsikon visas bredvid låsta frekvenser i listan.

   Du kan även låsa upp en låst frekvens från åtgärdsfältet.

1. Följ de här stegen för att justera frekvenser med en procentandel:

   1. Välj alla hastigheter som du vill justera på tariffkortet > Jobbroller och hastigheter.

      Du kan välja en eller flera priser. Alla justeras med samma procentsats.

   1. Klicka på [!UICONTROL **Justera frekvenser**] i åtgärdsfältet.
   1. I rutan [!UICONTROL **Justera jobbrollfrekvenser**] väljer du om du vill att hastighetsjusteringen ska ske under den valda tidsperioden (de befintliga giltighetsdatumen) eller ett anpassat datumintervall som du definierar.

      ![Justera jobbrollfrekvenser, ruta](assets/adjust-job-role-rates-dialog.png)

   1. Ange justeringsvärdet för tarifferna.

      Det här värdet används som en procentandel. Om du t.ex. anger 10 kommer de valda satserna att öka med 10 %.

   1. Klicka på [!UICONTROL **Uppdatera frekvenser**].
   1. Klicka på [!UICONTROL **Uppdatera**] i bekräftelsemeddelandet.

      De valda satserna ökas med procentandelen.

## Importera ett tariffkort

Se artikeln [Importera tariffkort från en mall](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md).

## Kopiera ett priskort

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Markera kryssrutan bredvid tariffkortet i listan och klicka på ikonen **Kopiera** ![Kopiera](assets/copy-icon.png) .
1. Ange ett namn för det nya tariffkortet i rutan [!UICONTROL **Kopiera tariffkort**]. Klicka sedan på [!UICONTROL **Skapa**].

   Det nya tariffkortet sparas. Redigera tariffkortsinformation, jobbroller och tariffer efter behov.

## Ta bort ett helt tariffkort

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Markera kryssrutan bredvid tariffkortet i listan och klicka på ikonen **Ta bort** ![Ta bort](assets/delete.png) .

   >[!NOTE]
   >
   >Ett tariffkort som är kopplat till ett projekt tas bort från projektet.


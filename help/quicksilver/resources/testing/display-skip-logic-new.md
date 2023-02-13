---
title: Lägga till visningslogik och hoppa över logik i ett anpassat formulär
description: Lägga till visningslogik och hoppa över logik i ett anpassat formulär
draft: Probably
source-git-commit: c0722924d6621b382050a10e9aac549fc1204d72
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# Lägga till visningslogik och hoppa över logik i ett anpassat formulär

Du kan använda smarta regler för att göra ett anpassat formulär dynamiskt och mer relevant för de användare som fyller i det. När en användare svarar på ett visst sätt i ett flervalsfält i ett formulär, visar en smart regel vad du vill att de ska se härnäst, baserat på det svaret.

De olika fälttyperna är listrutor, kryssrutor och alternativknappar.

* **Visningslogik**: Du konfigurerar en visningslogikregel för fältet, widgeten eller avsnittet som du vill att användaren ska se först när användaren har valt ett visst alternativ i ett föregående flervalsfält.

   **Exempel:** Du skapar ett formulär för begäran om marknadsföringsinnehåll där personer i organisationen kan begära en ny logotyp, webbplatsuppdatering, broschyr eller andra typer av marknadsföringsinnehåll. Beroende på vilken typ av innehåll som användaren vill ha måste du be dem om olika typer av detaljer, t.ex. färger och designidéer om de behöver en logotyp eller en lista med produktfunktioner om de behöver en broschyr.

   I fältet där du tillfrågas om färger och detaljer för en ny logotyp kan du lägga till en visningslogikregel som visar det fältet först när användaren har valt alternativknappen Logo i det första fältet.

   På samma sätt kan du i fältet som frågar efter produktfunktioner lägga till en visningslogikregel som visar det fältet först när en användare har markerat alternativknappen Broschyr i det första fältet.

   ![](assets/display-logic-logo-request-350x196.png)

   Du kan konfigurera visningslogikregler för alla anpassade fält-, widget- och avsnittsbrytningar som följer efter ett flervalsfält.

* **Hoppa över logikregel**: Du konfigurerar den här regeln för att dölja delar av ett formulär som användaren inte behöver. När användaren markerar ett visst objekt i ett föregående flervalsfält, hoppar logikregeln över dem i slutet av formuläret eller i ett anpassat fält, widget eller avsnitt som du vill att de ska se.

   **Exempel:** Någon använder formuläret för begäran om marknadsföringsinnehåll ovan för att be om en rapport som tillhandahålls av Försäljning, inte Marknadsföring. För den här användaren kan en regel för hopplogik dölja frågan som frågar efter information och hoppa till en textrad som refererar till den avdelning användaren behöver.

   ![](assets/skip-logic-white-paper-request-350x221.png)

   I det här fallet kan du lägga till ett beskrivande textfält som refererar användaren till försäljningsavdelningen. På det första anpassade fältet som frågar efter vilken typ av marknadsföringsinnehåll användaren behöver kan du lägga till en hopplogikregel som bara visar textraden när användaren väljer alternativknappen Vitbok i det första fältet.

   Detta är särskilt användbart om du lägger till många andra fält om logotyper, webbplatsuppdateringar och broschyrer som användaren inte behöver se.
Du kan bara tillämpa en hopplogikregel på ett anpassat fält, inte på en widget eller ett avsnitt.

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Skapa ett exempel på ett anpassat formulär som har visnings- och hopplogik

Det bästa sättet att lära sig att lägga till visnings- och hopplogik i ett anpassat formulär är att använda det praktiska exemplet som förklaras i de två följande avsnitten:

* [Visningslogik - praktiskt exempel](#display-logic-practical-example)
* [Hopplogik - praktiskt exempel](#skip-logic-practical-example)

### Visningslogik - praktiskt exempel {#display-logic-practical-example}

I det här exemplet skapar du ett anpassat formulär med ett flervalsfält med alternativknappar. Sedan lägger du till visningslogik som kopplar det här fältet till ett andra fält.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Välj **Anpassad Forms** ![](assets/custom-forms-icon.png).

1. Klicka **Nytt anpassat formulär**, markera **Projekt** i rutan som visas väljer du **Fortsätt**.

1. I **Formulärtitel** textruta, skriva **Exempel på eget formulär - Utbildningslogik och hopplogik** för att namnge formuläret.

   ![](assets/form-title-box-350x247.png)

1. Så här lägger du till det första fältet i formuläret:

   1. Öppna **Lägg till ett fält** -fliken.

      ![](assets/add-a-field-tab-350x237.png)

   1. Välj **Alternativknappar** fälttyp, sedan typ *Vilken typ av marknadsföringsinnehåll behöver du?* som **Etikett** för fältet.

   1. Under **Val**, ersätt **Alternativ 1** och **Val 2** med följande text för att skapa två alternativ som användare kan välja i fältet:

      *Webbplatsuppdatering*

      *Logotypdesign*

1. Så här lägger du till nästa anpassade fält och lägger till en visningslogikregel:

   1. Öppna **Lägg till ett fält** tabb igen och lägga till en ny **Alternativknappar** fältet anropades *Vilken typ av webbplatsuppdatering behöver du?*

      Vi lägger till alternativen för det här fältet senare.

   1. I **Ytterligare inställningar** avsnitt, markera **Lägg till logik**.

      ![](assets/add-logic-btn-350x408.png)

1. I rutan som visas med **Display Logic** öppna konfigurerar du det andra fältet så att det bara visas för användare som har markerat *Webbplatsdesign* i det första fältet:

   1. I den första listrutan väljer du **Vilken typ av marknadsföringsinnehåll behöver du?**
   1. I den andra listrutan väljer du **Webbplatsdesign**.
   1. Lämnar den tredje listrutan inställd på **Markerad**, markera **Spara**.

   Lägg märke till de små färgade fyrkanterna med ett D, vilket anger att det andra fältet är kopplat med visningslogik till användarens val i det första fältet:

   ![](assets/red-display-logic-indicators-350x250.png)

1. Välj **Förhandsgranska** för att vara säker på att logiken fungerar som du vill i formuläret, och sedan väljer du **Avsluta förhandsgranskning**.

1. Klicka **Spara + Stäng** spara formuläret och sedan fortsätta [Hopplogik - praktiskt exempel](#skip-logic-practical-example) nedan.

### Hopplogik - praktiskt exempel {#skip-logic-practical-example}

Hopplogik fungerar ungefär som visningslogik, men fungerar som omvänd: I stället för att göra så att specifika anpassade flervalsfält visas baserat på tidigare användarval, bestämmer du vilka som ska döljas (hoppas över) eftersom de inte är relevanta för användaren.

Du kan lära dig mer om detta genom att fortsätta att arbeta med exempelformuläret som du skapade i avsnittet [Visningslogik - praktiskt exempel](#display-logic-practical-example) i den här artikeln.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms**.
1. Klicka på formulärets namn **Exempel på eget formulär - Utbildningslogik och hopplogik** som du skapade i stegen ovan för att öppna den för redigering.
1. Välj det nedrullningsbara fält som du skapade med namnet *Vilken typ av webbplats behöver du?*, lägger till följande alternativ för fältet och klickar sedan på **Använd**:

   *E-handel*

   *Broschyr*

   *medlemskap*

1. Öppna **Lägg till ett fält** skapar du ett **Textfält med formatering **fält med namnet *Vad är målet för webbplatsen?* och sedan klicka **Använd**.

   I den här organisationen skapas en hjälpdokumentationswebbplats av det tekniska skrivteamet, inte av marknadsföringsavdelningen. Ingen ytterligare information behövs från en användare som väljer hjälpdokumentation i det andra fältet. Vi ska skapa en textrad (ett beskrivande textfält) som talar om för dem att de ska besöka Teknikskribenten istället. Och vi ska använda en logikregel som hoppar över användaren till den textraden.

1. Så här skapar du textraden:

   1. Öppna **Lägg till ett fält** och skapa en **Beskrivande textfält**.

   1. För **Etikett**, typ *Se Teknikskribent*.

   1. För **Beskrivande text**, typ *Om du vill skapa onlinehjälpdokumentation läser du i det tekniska skrivteamet*.

   1. Välj **Använd**.

1. Så här skapar du hopplogiksregeln:

   1. Välj det andra nedrullningsbara fältet, *Vilken typ av webbplats behöver du?*
   1. I **Ytterligare inställning** s-avsnitt, välja **Redigera logik**.
   1. I rutan som visas öppnar du **Hoppa över logik** -fliken.
   1. Ange den första listrutan till **Hjälpdokumentation** lämnar du den andra listrutan till **Markerad** och ange den tredje listrutan till **Se Teknikskribentteamet**.
   1. Välj **Spara**.

   Lägg märke till att den lilla skiftologiken är fyrkantig med ett S, vilket anger att användaren kommer att hoppa över något efter att ha valt ett visst alternativ i det andra fältet.

   ![](assets/notice-skip-logic-squares-350x249.png)

1. Klicka **Förhandsgranska**  för att säkerställa att logiken används på det sätt du vill.
1. Klicka **Spara +Stäng**.

Om du skapar ett formulär som detta kan du lägga till fler textfält för att fråga efter information från användare som väljer E-handel eller Broschyr i det andra fältet. Dessa fält kan fråga vem målgruppen är för webbplatsen, vad målet är att skapa den, vad budgeten är och så vidare.

Och med logiska regler kan du skapa förgreningssökvägar för frågor.

För användare som väljer E-handel kan du till exempel skapa fält med frågor om produktfoton, beskrivningar, priser och betalningsalternativ. För användare som väljer Broschyr kan du skapa fält som frågar om innehåll.

En användare som har valt hjälpdokumentation kommer aldrig att se något av dessa ytterligare fält som inte är relevanta för dem.

>[!TIP]
>
>Du kan lägga till både visningslogik och hopplogik i ett anpassat fält om allt av följande gäller fältet:
>
>* Det är ett flervalsfält (alternativknappar, listrutor eller kryssrutor)
>* Det föregås av ett flervalsfält
>* Därefter kommer ett annat anpassat fält
>


<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Multi-field display logic statements</h2>
-->


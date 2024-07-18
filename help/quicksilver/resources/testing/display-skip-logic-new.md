---
title: Lägga till visningslogik och hoppa över logik i ett anpassat formulär
description: Lägga till visningslogik och hoppa över logik i ett anpassat formulär
draft: Probably
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1475'
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

* **Hoppa över logikregel**: Du konfigurerar den här regeln så att delar av ett formulär som användaren inte behöver döljs. När användaren markerar ett visst objekt i ett föregående flervalsfält, hoppar logikregeln över dem i slutet av formuläret eller i ett anpassat fält, widget eller avsnitt som du vill att de ska se.

  **Exempel:** Någon använder formuläret för begäran om marknadsföringsinnehåll ovan för att be om en rapport som tillhandahålls av Försäljning, inte Marknadsföring. För den här användaren kan en regel för hopplogik dölja frågan som frågar efter information och hoppa till en textrad som refererar till den avdelning som han/hon behöver.

  ![](assets/skip-logic-white-paper-request-350x221.png)

  I det här fallet kan du lägga till ett beskrivande textfält som refererar användaren till försäljningsavdelningen. På det första anpassade fältet som frågar efter vilken typ av marknadsföringsinnehåll användaren behöver kan du lägga till en hopplogikregel som bara visar textraden när användaren väljer alternativknappen Vitbok i det första fältet.

  Detta är särskilt användbart om du lägger till många andra fält om logotyper, webbplatsuppdateringar och broschyrer som användaren inte behöver se.
Du kan bara tillämpa en hopplogikregel på ett anpassat fält, inte på en widget eller ett avsnitt.


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
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront-administratörer beviljar åtkomst finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Skapa ett exempel på ett anpassat formulär som har visnings- och hopplogik

Det bästa sättet att lära sig att lägga till visnings- och hopplogik i ett anpassat formulär är att använda det praktiska exemplet som förklaras i de två följande avsnitten:

* [Visningslogik - praktiskt exempel](#display-logic-practical-example)
* [Hopplogik - praktiskt exempel](#skip-logic-practical-example)

### Display logic - praktiskt exempel {#display-logic-practical-example}

I det här exemplet skapar du ett anpassat formulär med ett flervalsfält med alternativknappar. Sedan lägger du till visningslogik som kopplar det här fältet till ett andra fält.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Välj **Anpassad Forms** ![](assets/custom-forms-icon.png) i den vänstra panelen.

1. Klicka på **Nytt anpassat formulär**, välj **Projekt** i rutan som visas och välj sedan **Fortsätt**.

1. I textrutan **Formulärtitel** skriver du **Eget exempelformulär - Utbildningslogik och hopplogik** för att namnge formuläret.

   ![](assets/form-title-box-350x247.png)

1. Så här lägger du till det första fältet i formuläret:

   1. Öppna fliken **Lägg till ett fält**.

      ![](assets/add-a-field-tab-350x237.png)

   1. Välj fälttypen **Alternativknappar** och skriv sedan *Vilken typ av marknadsföringsinnehåll behöver du?* som **Label** för fältet.

   1. Under **Alternativ** ersätter du **Alternativ 1** och **Alternativ 2** med följande text för att skapa två alternativ som användare kan välja i fältet:

      *Webbplatsuppdatering*

      *Logotypdesign*

1. Så här lägger du till nästa anpassade fält och lägger till en visningslogikregel:

   1. Öppna fliken **Lägg till ett fält** igen och lägg till ett nytt **alternativknappsfält** med namnet *Vilken typ av webbplatsuppdatering behöver du?*

      Vi lägger till alternativen för det här fältet senare.

   1. Välj **Lägg till logik** i avsnittet **Ytterligare inställningar**.

      ![](assets/add-logic-btn-350x408.png)

1. I rutan som visas när fliken **Display Logic** är öppen konfigurerar du det andra fältet så att det bara visas för användare som har valt *Webbplatsdesign* i det första fältet:

   1. I den första listrutan väljer du **Vilken typ av marknadsföringsinnehåll behöver du?**
   1. Välj **Webbplatsdesign** i den andra listrutan.
   1. Välj **Spara** om den tredje listrutan ska vara **Markerad**.

   Lägg märke till de små färgade fyrkanterna med ett D, vilket anger att det andra fältet är kopplat med visningslogik till användarens val i det första fältet:

   ![](assets/red-display-logic-indicators-350x250.png)

1. Välj **Förhandsgranska** för att kontrollera att logiken fungerar som du vill i formuläret och välj sedan **Avsluta förhandsgranskning**.

1. Klicka på **Spara + stäng** och spara formuläret. Fortsätt sedan till [Hoppa över logik - praktiskt exempel](#skip-logic-practical-example) nedan.

### Hopplogik - praktiskt exempel {#skip-logic-practical-example}

Hopplogik fungerar på liknande sätt som visningslogik, men fungerar som omvänd: i stället för att visa specifika anpassade flervalsfält baserat på tidigare användarval, bestämmer du vilka som ska döljas (hoppas över) eftersom de inte är relevanta för användaren.

Om du vill veta mer kan du fortsätta att arbeta med exempelformuläret som du skapade i avsnittet [Visningslogik - praktiskt exempel](#display-logic-practical-example) i den här artikeln.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Anpassad Forms**.
1. Klicka på namnet på formuläret **Exempel på anpassat formulär - Utbildningslogik och hopplogik** som du skapade i stegen ovan för att öppna det för redigering.
1. Välj det nedrullningsbara fältet som du skapade med namnet *Vilken typ av webbplats behöver du?*, lägg till följande alternativ för fältet och klicka sedan på **Använd**:

   *E-handel*

   *Broschyr*

   *Medlemskap*

1. Öppna fliken **Lägg till ett fält** och skapa ett **textfält med formateringen **fält med namnet *Vad är målet för webbplatsen?* och klicka sedan på **Använd**.

   I den här organisationen skapas en hjälpdokumentationswebbplats av det tekniska skrivteamet, inte av marknadsföringsavdelningen. Ingen ytterligare information behövs från en användare som väljer hjälpdokumentation i det andra fältet. Vi ska skapa en textrad (ett beskrivande textfält) som talar om för dem att de ska besöka Teknikskribenten istället. Och vi ska använda en logikregel som hoppar över användaren till den textraden.

1. Så här skapar du textraden:

   1. Öppna fliken **Lägg till ett fält** och skapa ett **beskrivande textfält**.

   1. För **Label** skriver du *See Technical Writing team*.

   1. **Beskrivande text** finns i *Teknikskribenten om hur man skapar onlinehjälpsdokumentation*.

   1. Välj **Använd**.

1. Så här skapar du hopplogiksregeln:

   1. Välj det andra nedrullningsbara fältet, *Vilken typ av webbplats behöver du?*
   1. Välj **Redigera logik** i avsnittet **Ytterligare inställningar** s.
   1. Öppna fliken **Hoppa över logik** i rutan som visas.
   1. Ställ in den första listrutan till **hjälpdokumentation**, ge den andra listrutan värdet **Markerad** och ställ in den tredje listrutan till **Se gruppen för tekniska skribenter**.
   1. Välj **Spara**.

   Lägg märke till att den lilla skiftologiken är fyrkantig med ett S, vilket anger att användaren kommer att hoppa över något efter att ha valt ett visst alternativ i det andra fältet.

   ![](assets/notice-skip-logic-squares-350x249.png)

1. Klicka på **Förhandsgranska**  för att säkerställa att logiken används på det sätt du vill.
1. Klicka på **Spara +Stäng**.

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


---
title: Importera tariffkort från en mall
description: Du kan använda en mallfil för att skapa dina tariffkort i Excel och importera dem till Adobe Workfront.
author: Lisa
hide: true
hidefromtoc: true
source-git-commit: 1deb72953599c24fa40eb7a5d77214f6576fec1e
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 0%

---


# Importera tariffkort från en mall

Du kan använda en mallfil för att skapa dina tariffkort i Excel och importera dem till Adobe Workfront, i stället för att lägga till alla jobbroller och frekvenser manuellt.

## Viktiga regler för att arbeta med mallfilen

* Ange antingen jobbrollen eller resurskategorin Ej arbetsplats, men inte båda.
* Hastighetskortssekvensen på fliken RATE_RTCRD måste matcha ordningen på korten på fliken RTCRD (1 för första, 2 för andra, osv.).
* Startdatum och slutdatum måste följa de tillåtna formaten.
* Gradkort kan importeras utan priser och uppdateras senare.
* Anpassade attribut (myndighet, kostnadsställe osv.) kan variera. Kontakta systemadministratören för att få information om de exakta kraven.
* Rader som tas bort i mallen tar inte bort befintliga poster i systemet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till [!UICONTROL Rate Cards]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fylla i mallfilen

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Klicka på **Nytt tariffkort** och sedan på **Hämta Excel-mall**.
1. Spara mallfilen på datorn genom att följa instruktionerna i webbläsaren.
1. Öppna mallfilen i Excel.

   >[!TIP]
   >
   > Spara filen med ett nytt namn om du vill behålla den tomma mallfilen och använda den igen senare.

   Mallen har två flikar. Båda flikarna måste ha rätt information för att det ska gå att importera tariffkorten.

   * RTCRD: Definiera tariffkort (grundläggande information)
   * RATE_RTCRD: Definiera de detaljerade hastigheterna som är kopplade till varje tariffkort

### Fyll i fliken RTCRD (Rate Card Setup)

Skapa och visa alla tariffkort på den här fliken. Varje rad representerar ett tariffkort.

![Fliken RTCRD i mallfilen för tariffkortsimport](assets/rate-card-import-template-tab1.png)

1. Ange information för ett tariffkort på varje rad:

   * **Namn** (obligatoriskt): Namnet på tariffkortet, till exempel&quot;Global Billing 2025&quot;.

     Det här namnet är den huvudsakliga identifieraren för tariffkortet. Varje tariffkort måste ha ett unikt namn.

   * **Beskrivning** (valfritt): En fritextbeskrivning av tariffkortet. Använd detta för att beskriva syfte, omfattning eller giltighet, till exempel&quot;Gäller nordamerikanska projekt&quot;.
   * **Företag** (valfritt): Detta kan vara antingen företagsnamnet eller företags-ID:t. Importen känner igen båda.

     Exempel: Coffesta eller _68c0234e0000541dd8c0757723daa68_

   * **Grupp** (valfritt): Detta kan vara antingen gruppnamnet eller grupp-ID:t. Importen känner igen båda.

     Exempel: Marknadsföring eller _68c0234e0000541dd8c0757723daa68_

   * **Anpassade fält** (valfritt): Du kan lägga till ytterligare kolumner med anpassade fältnamn om miljön har särskilda krav.

   >[!NOTE]
   >
   >* Du måste ange ett namn för varje betalningskort.
   >* Varje tariffkort får automatiskt ett sekvensnummer baserat på radpositionen. Det kort som du definierar för första priset (i rad 2) är sekvens 1, nästa är 2 och så vidare. Dessa sekvensnummer används på fliken RATE_RTCRD för att koppla frekvenser.

### Fyll i fliken RATE_RTCRD (Rates Setup)

Definiera alla hastigheter som hör till priskorten på den här fliken.

Varje rad på fliken definierar en specifik frekvens. Du kan skapa flera priser under samma tariffkort genom att upprepa tariffkortssekvensen.

Se till att datum inte överlappar om det inte är tänkt.

![Fliken RATE_RTCRD i mallfilen för tariffkortsimport](assets/rate-card-import-template-tab2.png)

1. Ange information om en frekvens på varje rad:

   * **Namn** (obligatoriskt): En etikett för radens hastighet.

     Det bästa sättet är att återanvända priskortsnamnet för tydlighet, till exempel&quot;Global Billing 2025 - Developer Rate&quot;.

   * **Gradkortsreferens** (obligatoriskt): Sekvensnumret för det tariffkort som den här hastigheten tillhör.

     Om kurskortet var det första du angav på fliken RTCRD (rad 2) anger du 1. Om det är den andra anger du 2 och så vidare.

   * **Jobbroll** (krävs om resurskategori som inte är arbetsplats inte används): Jobbrollen som tariffen gäller för. Detta kan vara antingen jobbrollens namn eller jobbrollens ID. Importen känner igen båda.

     Exempel: Designer eller _68c0234e0000541dd8c0757723daa68_

   * **Resurskategori utan arbete** (krävs om jobbrollen inte används): Resurskategorin som inte är arbetskostnad som tariffen gäller för. Detta kan vara antingen kategorinamnet eller kategori-ID:t. Importen känner igen båda.

     Exempel: Kamera eller _68c0234e0000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >Du kan inte ange data i både kolumnerna **Jobbroll** och **Resurskategori** som inte är arbetsplats. En krävs.

   * **Startdatum** (valfritt): Det datum då tariffen börjar gälla.

     Datumet måste följa något av de format som stöds (beroende på var du befinner dig): MM/dd/åååå, dd/MM/åååå, MM/DD/YY, DD/MM/YY, M/d/yy, d/M/åååå/MM/dd, åååå/dd/MM, ååååå-MM-dd, ååååå-dd-MM

     Exempel: 01/01/2025

     Mer information finns i [Datumformateringskrav](#date-formatting-requirements) nedan.

   * **Slutdatum** (valfritt): Det datum då hastigheten slutar att gälla.

     Detta datum måste följa samma format som startdatumet som stöds.

     Mer information finns i [Datumformateringskrav](#date-formatting-requirements) nedan.

   * **Värde** (valfritt): Det numeriska hastighetsvärdet, till exempel 150. Standardvärdet är 0.
   * **Valuta** (valfritt): Valutan för kursen, till exempel USD, EUR, GBP. Standardvärdet är systemvalutan.
   * **Låst** (valfritt): Anger om hastigheten är låst. Giltiga värden är True eller False.
   * **Attribut** (valfritt/anpassat): De sista kolumnerna (Byrå, Plats, Kostnadscenter osv.) är Attribut som skiljer sig åt beroende på kundkonfiguration. Det här är anpassningsbara fält och kan variera mellan olika kundmiljöer.

     Exempel: Agency = &quot;1: Agency,&quot; Location = &quot;Chicago,&quot; Cost Center = &quot;22: Cost Centre&quot;

### Formateringskrav för datum

När du förbereder tariffkortsdata för import måste du se till att datumkolumnerna formateras som **Allmänt**, inte som **Datum**.

Om kolumnerna är inställda på datumformat kan systemet feltolka värden under importprocessen, vilket kan leda till fel eller misslyckade överföringar. Om du använder formatet Allmänt bevaras datumets numeriska råformat eller textbeteckning, vilket gör att systemet kan validera och använda värdena korrekt.

Om du följer dessa steg förhindras onödiga problem och en smidig och korrekt import av tariffdata säkerställs.

1. Markera datumkolumnerna i kalkylbladet innan du sparar eller överför filen.
1. Ändra kolumnformatet till **Allmänt**.
1. Kontrollera att värdena fortfarande visas korrekt (till exempel 01/01/2025 eller 2025-01-01).

## Importera mallfilen

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Klicka på **Nytt tariffkort** och sedan på **Importera nya tariffkort**.
1. Dra och släpp filen i dialogrutan eller klicka på Välj en Excel-fil för att bläddra till filen på datorn.
1. Klicka på **Börja importera**.

   Om det inte är några problem med filen visas ett bekräftelsemeddelande och de nya priskorten visas i listan.

1. Om filen innehåller problem visas ett felmeddelande. Klicka på **Visa problem** om du vill visa problemen på en separat skärm.

   Du måste korrigera problemen i Excel-filen och importera den igen innan tariffkorten finns i Workfront.




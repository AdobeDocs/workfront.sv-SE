---
user-type: administrator
product-area: system-administration;setup
title: Importera tariffkort från en mall
description: Du kan använda en mallfil för att skapa dina tariffkort i Excel och importera dem till Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: debe90e7-08c2-4385-96fb-8d349dec6741
source-git-commit: aa774419e65e9e4a5785382d3cb2b22bdb0389c9
workflow-type: tm+mt
source-wordcount: '1807'
ht-degree: 0%

---

# Importera tariffkort från en mall

Du kan använda en mallfil för att skapa dina tariffkort i Excel och importera dem till Adobe Workfront, i stället för att lägga till alla jobbroller och frekvenser manuellt.

Om du vill se exempelkorten som beskrivs i den här artikeln hämtar du [exempelfilen](assets/rate-cards-sample.zip).

Mer information om tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

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
     >Du kan inte ange data i både kolumnerna **Jobbroll** och **Resurskategori** som inte är arbetsplats. One is required.

   * **Start Date** (optional): The date when the rate becomes effective.

     The date must follow one of the supported formats (depending on your location): MM/dd/yyyy, dd/MM/yyyy, MM/DD/YY, DD/MM/YY, M/d/yy, d/M/yy, yyyy/MM/dd, yyyy/dd/MM, yyyy-MM-dd, yyyy-dd-MM

     Example: 01/01/2025

     For more information, see [Date formatting requirements](#date-formatting-requirements), below.

   * **End Date** (optional): The date when the rate stops being effective.

     This date must follow the same supported formats as the start date.

     For more information, see [Date formatting requirements](#date-formatting-requirements), below.

   * **Value** (optional): The numeric rate value, for example 150. Standardvärdet är 0.
   * **Currency** (optional): The currency for the rate, for example USD, EUR, GBP. The default is the system currency.
   * **Locked** (optional): Indicates if the rate is locked. Valid values are True or False.
   * **Attributes** (optional / custom): The last columns (Agency, Location, Cost Center, etc.) are Rate Attributes that differ by customer configuration. These are customizable fields and may vary per customer environment.

     Example: Agency = &quot;1: Agency,&quot; Location = &quot;Chicago,&quot; Cost Center = &quot;22: Cost Center&quot;

### Fill out the RSALS (Rate Card Alias) tab

Create and list all of the aliases on this tab. Each row represents one alias.

When the rate card is attached to a project, the alias appears on information such as placeholder assignments, expenses, and reports, instead of the internal job role name. Only one alias can exist for each job role and attribute combination within a single rate card.

An alias is added to the system, but it is not connected to a job role based on the information on this tab.

![RSALS tab on rate card import template file](assets/rsals-tab-rate-card-import.png)

1. Ange namnet på ett alias på varje rad.

   Ange endast ett aliasnamn per rad: ett jobbrollalias, ett icke-arbetsplats-resursalias eller ett utgiftstypalias.

### Fyll i fliken RCRMET_RTCRD_RSALS (tariffkortsmetadata)

På den här fliken kan du definiera anslutningar mellan resurser och alias för ett visst tariffkort.

![Fliken RCRMET_RTCRD_RSALS i mallfilen för tariffkortsimport](assets/rcrmet-tab-rate-card-import.png)

1. Ange informationen på varje rad:

   * **Gradkort** (obligatoriskt): Namnet eller sekvensnumret på det tariffkort som resursen och aliaset tillhör. Hastighetskortet måste anges på fliken RTCRD.

     För ett sekvensnummer: Om tariffkortet var det första du angav på fliken RTCRD (rad 2) anger du 1. Om det är den andra anger du 2 och så vidare.

   * **Jobbroll** (krävs om Utgiftstyp och Resurskategori som inte är arbetskostnad inte används): Den jobbroll som aliaset är anslutet till. Detta kan vara antingen jobbrollens namn eller jobbrollens ID. Importen känner igen båda.

     Exempel: Designer eller _68c0234e0000541dd8c0757723daa68_

   * **Utgiftstyp** (krävs om Jobbroll och Resurskategori som inte är arbetskostnad inte används): Utgiftstypen som aliaset är anslutet till. Detta kan vara antingen utgivartypens namn eller utgifts-ID. Importen känner igen båda.

     Exempel: Resa eller _68c0234e0000541dd8c0757723daa68_

   * **Resurskategori utan arbetskostnad** (krävs om jobbroll och utgiftstyp inte används): Resurskategorin som inte är arbetsplats som aliaset är anslutet till. Detta kan vara antingen kategorinamnet eller kategori-ID:t. Importen känner igen båda.

     Exempel: Kamera eller _68c0234e0000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >Du kan inte ange alla tre kolumnerna **Jobbroll**, **Utgiftstyp** och **Resurskategori som inte är arbetsplats**. En krävs.

   * **Resursalias**: Det alias som anges på fliken RSALS.

### Date formatting requirements

When preparing rate card data for importing, you must ensure that the date columns are formatted as **General**, not as **Date**.

If the columns are set to Date format, the system may misinterpret values during the import process, leading to errors or failed uploads. Using the General format preserves the raw numeric or text representation of the date, allowing the system to correctly validate and apply the values.

Following these steps will prevent unnecessary issues and ensure a smooth and accurate import of rate data.

1. Before saving or uploading the file, select the date columns in the spreadsheet.
1. Change the column format to **General**.
1. Verify that the values still display correctly (for example, 01/01/2025 or 2025-01-01).

## Import the template file

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Click **New rate card**, then click **Import new rate cards**.
1. Drag and drop your file into the dialog, or click **Select an Excel file** to browse to the file on your computer.
1. Click **Start importing**.

   If there are no issues with the file, then a confirmation message appears and the new rate cards appear in the list.

1. If the file contains issues, an error message appears. Click **See issues** to view the issues on a separate screen.

   You must correct the issues in the Excel file and import it again before the rate cards will exist in Workfront.

## Update existing rate cards

You can update the rates in your existing rate cards using the same Excel template and upload those changes to Workfront.

Only the RATE_RTCRD (Rates Setup) tab is required for updating existing rates.

>[!NOTE]
>
>Uploading rates for an existing rate card overwrites all of the current job roles and rates on the rate card.
>
>For example, if you have 5 job roles with rates on the existing rate card and the Excel file has 1 job role, then the rate card will have 1 job role after you upload. To keep the other 5 job roles and their rates on the rate card, you must include them in the Excel file.

To update existing rate cards:

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Klicka på **Nytt tariffkort** och sedan på **Importera tariffkortsuppdateringar**.
1. Dra och släpp filen i dialogrutan eller klicka på **Välj en Excel-fil** om du vill bläddra till filen på datorn.
1. Klicka på **Börja importera**.

   Om det inte är några problem med filen visas ett bekräftelsemeddelande och de nya priskorten visas i listan.

1. Om filen innehåller problem visas ett felmeddelande. Klicka på **Visa problem** om du vill visa problemen på en separat skärm.

   Du måste korrigera problemen i Excel-filen och importera den igen innan tariffkortsuppdateringarna finns i Workfront.



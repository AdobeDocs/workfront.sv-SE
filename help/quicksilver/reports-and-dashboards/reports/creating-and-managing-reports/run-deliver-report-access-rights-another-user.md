---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Kör och leverera en rapport med åtkomsträttigheter för en annan användare
description: Som standard kan användare bara se de objekt i en rapport som de har behörighet att visa.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 0%

---

# Kör och leverera en rapport med åtkomsträttigheter för en annan användare

Som standard kan användare bara se de objekt i en rapport som de har behörighet att visa.

Du kan tillåta alla användare att se samma resultat i en rapport som en annan användare, oavsett åtkomstnivå eller behörighetsnivå för objekten i rapporten.

Om du kör en rapport med åtkomsträttigheter för en annan användare som har högre behörighet (till exempel behörigheten för en Adobe Workfront-administratör), kan alla användare som har behörighet att visa rapporten se informationen i rapporten som den användare som har angetts i rapportbyggaren. Du kan konfigurera detta för båda rapporter som användarna hittar i Workfront gränssnitt, eller för rapporter som levereras till användarna som en bilaga till ett e-postmeddelande.

>[!TIP]
>
>Du bör ersätta **Kör den här rapporten med åtkomstbehörigheten för**-fältet med en aktiv användare endast om du vill att rapporten ska visas med den användarens åtkomstbehörighet. En arbetslicensanvändare kanske inte har behörighet att se alla objekt i en rapport som skapats av en planlicensanvändare eller systemadministratör, såvida inte rapporten visas med behörigheten för en planerare eller systemadministratör.\
>Om rapporten delas med användare med liknande åtkomst som användaren som anges i fältet **Kör den här rapporten med åtkomstbehörigheten** kan du lämna det här fältet tomt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till en rapport (för att visa den levererade rapporten)</p> <p>Hantera behörigheter till en rapport (för att köra rapporten)</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa en rapport med åtkomsträttigheter för en annan användare

Om du fyller i **Kör den här rapporten med åtkomsträttigheterna för fältet** säkerställs att en rapport innehåller samma data, oavsett vilken användare som använder rapporten. Rapporten visas på samma sätt som för den angivna användaren.

De användare som får åtkomst till rapporten måste ha minst behörigheten Visa i rapporten för att kunna se den. Om användaren som anges i fältet **Kör den här rapporten med åtkomsträttigheter för:** är inaktiverad visas inte längre rapporten för andra användare som rapporten delas med.

Så här kör du en rapport med åtkomsträttigheter för en annan användare:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.

1. Markera den rapport som du vill visa med en annan användares åtkomsträttigheter.
1. Klicka på **Rapportåtgärder** och sedan på **Redigera**.

1. Klicka på **Rapportinställningar**.

1. I fältet **Kör den här rapporten med åtkomsträttigheterna för:** börjar du skriva namnet på den användare som du vill att rapporten ska visas som och markerar den när du ser den i listan.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   >
   >Användare med en lägre åtkomstnivå som kan skapa rapporter kan inte välja någon annan användare än sig själva för fältet **Kör den här rapporten med åtkomstbehörigheten**.

1. Klicka på **Klar**.
1. Klicka på **Spara + Stäng**.\
   Rapporten visas nu för alla användare som rapporten delas med som om den visades av användaren som anges i fältet **Kör den här rapporten med åtkomstbehörigheten**.

>[!IMPORTANT]
>
>Om du anger en annan användare än den inloggade användaren för **Kör den här rapporten med åtkomsträttigheten** påverkas den information som visas i rapporten om rapporten innehåller ett filter som använder ett jokertecken som refererar till den inloggade användaren. Rapporten visas enligt det värde som anges i **Kör den här rapporten med åtkomstbehörigheten** i stället för det som definieras i jokerteckensfiltret.
>
>Mer information om jokertecken för användarfält finns i avsnittet om användarbaserade variabler i [Översikt över jokerteckenfiltervariabler](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Leverera en rapport med åtkomsträttigheter för en annan användare

Du kan konfigurera rapporter som ska levereras som bilagor till ett e-postmeddelande. Du kan konfigurera de här levererade rapporterna så att de visas för användare med högre åtkomstnivå, så att alla användare kan se samma information i de levererade rapporterna. De användare som ska se rapporten som levereras i e-postmeddelandet måste läggas till i listan Skicka till för mottagare i rapportleveransen. Mer information om hur du konfigurerar en leveransrapport finns i artikeln [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Så här skickar du en rapport med åtkomsträttigheter för en annan användare:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.

1. Välj den rapport som du vill leverera med en annan användares åtkomstbehörighet.
1. Klicka på rapportens namn för att markera den.
1. Klicka på **Rapportera åtgärder**.
1. Klicka på **Skicka rapport**.

1. I fältet **Leverera den här rapporten med åtkomsträttigheterna för:** börjar du skriva namnet på den användare som du vill att rapporten ska visas som när den levereras i ett e-postmeddelande och markerar den när du ser den i listan. Standardvärdet är namnet på den användare som skapar rapporten.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   >
   >Användare med en lägre åtkomstnivå som kan skapa rapporter kan inte välja någon annan användare än sig själva för fältet **Leverera den här rapporten med åtkomstbehörigheten**.

1. Välj det **format** som du vill att rapporten ska visas i e-postmeddelandet:

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. Klicka på **Skicka nu** för att skicka det direkt.\
   eller\
   Klicka på **Skapa upprepad leverans** om du vill schemalägga en återkommande leverans för rapporten.\
   Mer information om rapportleveranser finns i artikeln [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Begränsningar för rapporter med en Source-kolumn

I följande rapporter visas en Source-kolumn där du kan visa information om det överordnade objektet:

* Utfallsrapporter
* Timrapporter
* Dokumentrapporter

Om användare inte har behörighet till det överordnade objektet för ett problem, en timme eller ett dokument visas kolumnen Source i rapporten tom, även om rapporten är konfigurerad att visas eller levereras med en annan användares åtkomstbehörighet.

Om du vill visa information om det överordnade objektet i rapporten rekommenderar vi att du lägger till en kolumn för det överordnade objektet där du kan visa namnet på det överordnade objektet.

Du kan till exempel lägga till något av följande i en rapport med en Source-kolumn:

* Kolumnerna Projektnamn, Aktivitetsnamn eller Utleveransnamn till ett dokument eller en timrapport.
* Kolumnerna Projektnamn eller Aktivitetsnamn i en problemrapport.
* En kolumn som använder textlägesuttryck som refererar till alla tre objekten. Följande är ett exempel för en timrapport:

  `displayname=Custom Source`

  `linkedname=opTask`

  `namekey=view.relatedcolumn`

  `namekeyargkey.0=opTask`

  `namekeyargkey.1=name`

  `textmode=true`

  `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

  `valueformat=HTML`

  Mer information om visningslägen för text finns i [Redigera en vy i textläge](../text-mode/edit-text-mode-in-view.md).
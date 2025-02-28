---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Använda Workfront-tillägget för Illustrator och InDesign
description: Du kan använda Workfront Extension för att exportera digitalt innehåll som du sparar och skapar i Adobe Illustrator och Adobe InDesign till Workfront. Detta snabbar upp gransknings- och godkännandeprocessen.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '3107'
ht-degree: 0%

---

# Använda Workfront-tillägget för Illustrator och InDesign

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Vi ersätter Workfront-tillägget för Illustrator och InDesign med [uppdaterade Creative Cloud-plugin-program](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). Från slutet av 2022 stöds inte längre det här tillägget och är tillgängligt som det är.

Du kan använda Workfront Extension för att exportera digitalt innehåll som du sparar och skapar i Adobe Illustrator och Adobe InDesign till Workfront. Detta snabbar upp gransknings- och godkännandeprocessen.

Workfront-tillägget stöds för Adobe Creative Cloud 2017 och senare i följande program:

* InDesign
* Illustrator
* Photoshop

  >[!NOTE]
  >
  >Vi rekommenderar att du använder det nya plugin-programmet [Adobe Workfront för Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell: Pro eller högre</p>
   eller
   <p>Nytt: Alla planer</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell: Arbete eller högre</p>
   eller
   <p>Nytt: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en Adobe Creative Cloud-licens förutom en Workfront-licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till det objekt som du vill interagera med.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Logga in på Workfront Extension från Illustrator eller InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

När du loggar in på Workfront från ett av de Adobe-program som stöds loggas du in på alla Adobe-program som stöds.

1. Gå till det Adobe-program där du vill använda tillägget Workfront.

   En lista över de format som stöds för varje program som stöds finns i [Exporterade filformat som stöds](#supported-exported-file-formats) i den här artikeln.

1. Klicka på **Fönster** > **Tillägg** > Workfront.

1. (Valfritt) Dra panelen Workfront till den plats där du vill att den ska visas i Adobe-programmet.
1. Följ instruktionerna för att logga in på Workfront.

   >[!NOTE]
   >
   >* Workfront ansluter till Adobe Creative Cloud med OAuth 2.0, en säker standard som används av de flesta webbaserade integreringar för autentisering och behörighet av användare.
   >* När du uppmanas att ange [domänen eller värddatorn] för ditt Workfront-konto skriver du in den med följande format:`yourCompany'sDomain.my.workfront.com`. Företagets domän är vanligtvis namnet på ditt företag.

   En lista över arbetsobjekt som du har tilldelats visar om projektet är en aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

## Överföra en fil till ett Workfront-projekt, en uppgift eller ett problem {#upload-a-file-to-a-workfront-project-task-or-issue}

Du kan överföra en fil från datorns filsystem eller exportera en fil som är öppen i ett Adobe Creative Cloud-program till ett Workfront-projekt, -uppgift eller -problem. 

Tänk på följande när du överför eller exporterar en fil från Adobe Creative Cloud:

* Åtkomstnivån måste tillåta överföring av dokument till Workfront. Mer information finns i [Bevilja åtkomst till dokument](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* Du måste ha behörighet att överföra dokument till objektet där du vill ha det. Mer information finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Filen överförs till dokumentområdet för det Workfront-objekt som du väljer.
* Du kan inte exportera ett dokument till området Dokument på huvudmenyn ![Huvudmenyikonen](assets/main-menu-icon.png) från ett Adobe Creative Cloud-program.

Följande avsnitt förklarar följande:

* [Överför en fil](#upload-a-file)
* [Exportera en fil som är öppen i Illustrator eller InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Överföra en ny version av en fil från Illustrator eller InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Överföra en fil {#upload-a-file}

Du kan överföra filer till ett projekt, en uppgift eller ett problem utan att behöva lämna ditt Adobe Creative Cloud-program.

1. Om du inte ser Workfront-tillägget när du öppnar ditt Adobe Creative Cloud-program klickar du på **Fönster** > **Tillägg** > **Workfront**.

   En lista över arbetsobjekt som du har tilldelats visar om projektet har aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

1. Klicka på namnet på det projekt, den uppgift eller det problem som du vill överföra filen till.

   Du kan söka efter detta genom att skriva namnet i rutan **Sök** och välja **Projekt**, **Aktivitet** eller **Problem** i listrutan till höger om rutan **Sök** . Om arbetsobjektets namn inte visas i listan trycker du på **Retur** för att söka efter alla Workfront-objekt som du har åtkomst till för att visa.

1. Klicka på **Markera** i det nedre högra hörnet av Workfront-tillägget.
1. I listrutan **Klicka för att välja format** och klicka på det format som du vill spara filen i Workfront.

   En lista över de format som stöds för varje program som stöds finns i [Exporterade filformat som stöds](#supported-exported-file-formats) i den här artikeln.

1. (Villkorligt) Om arbetsposten där du vill överföra filen har dokumentmappar väljer du en dokumentmapp i fältet **Klicka för att välja en dokumentmapp** och klickar sedan på **Välj**.

1. Klicka på **Överför en lokal fil**.
1. Leta reda på filen i filsystemet i rutan **Öppna fil** och klicka sedan på **Öppna**.

1. (Valfritt) Ange ett nytt namn för filen.

   ![Byt namn på filen](assets/rename-file-uploading.png)

1. Klicka på **Överför**.

   I Workfront visas dokumentet nu i området Dokument för det projekt, den uppgift eller det ärende du valde.

1. (Valfritt) Klicka på dokumentets namn för att öppna dokumentinformationssidan i Workfront.

   Workfront öppnas i en ny webbläsarflik.

### Exportera en fil som är öppen i Illustrator eller InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. Öppna en fil som du vill exportera till Workfront i ett Adobe Creative Cloud-program som stöds.
1. Om Workfront-tillägget inte visas klickar du på **Fönster** > **Tillägg** > **Workfront**.

   En lista över arbetsobjekt som du har tilldelats visar om projektet har aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

1. Klicka på namnet på det projekt, den uppgift eller det problem som du vill exportera filen till.

   Du kan söka efter detta genom att skriva namnet i rutan **Sök** och välja **Projekt**, **Aktivitet** eller **Problem** i listrutan till höger om rutan **Sök** . Om arbetsobjektets namn inte visas i listan trycker du på **Retur** för att söka efter alla Workfront-objekt som du har åtkomst till för att visa.

1. I listrutan **Klicka för att välja format** och klicka på det format som du vill spara filen i Workfront.

   En lista över de format som stöds för varje program som stöds finns i [Exporterade filformat som stöds](#supported-exported-file-formats) i den här artikeln.

1. (Villkorligt) Om arbetsposten där du vill överföra filen har dokumentmappar väljer du en dokumentmapp i fältet **Klicka för att välja en dokumentmapp** och klickar sedan på **Välj**.
1. (Valfritt) Om du vill byta namn på dokumentet klickar du på dokumentnamnet och skriver ett nytt namn.

   ![Byt namn på dokument vid export](assets/rename-doc-exporting.png)

1. Klicka på **Exportera**.

   Ett meddelande visas som bekräftar att dokumentet har exporterats till Workfront.

   I Workfront visas dokumentet under Dokument för det objekt du har angett i Workfront.

1. (Valfritt) Klicka på dokumentets namn för att öppna det i Workfront.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront öppnas i en ny webbläsarflik.

### Överföra en ny version av en fil från Illustrator eller InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Om du vill exportera en fil som du arbetar med i ett Adobe-program som stöds som en ny version av en fil i Workfront, öppnar du filen i Adobe-programmet.
1. Om Workfront-tillägget inte visas klickar du på **Fönster** > **Tillägg** > **Workfront**.

   En lista över arbetsobjekt som du har tilldelats visar om projektet är en aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

1. Klicka på namnet på projektet, uppgiften eller utgåvan där det befintliga dokumentet finns med.

   Du kan söka efter detta genom att skriva namnet i rutan **Sök** och välja **Projekt**, **Aktivitet** eller **Problem** i listrutan till höger om rutan **Sök** . Om arbetsobjektets namn inte visas i listan trycker du på **Retur** för att söka efter alla Workfront-objekt som du har åtkomst till för att visa.

   Alla dokument som överförts till projekt, uppgifter eller utgåvor visas i en lista, oavsett om de har överförts från Adobe-programmet eller inte.

1. I listrutan **Klicka för att välja format** och klicka på det format som du vill spara filen i Workfront.

   Detta är nödvändigt om du exporterar en fil som är öppen i Adobe. En lista över de format som stöds för varje program som stöds finns i [Exporterade filformat som stöds](#supported-exported-file-formats) i den här artikeln.

1. Om du exporterar en fil som du har öppnat i Adobe-programmet som en ny version av det Workfront-dokument som du har valt klickar du på **Exportera**.

   eller

   Om du vill överföra en fil från datorns filsystem som en ny version av det Workfront-dokument du har valt klickar du på **Överför en lokal fil**, letar upp filen i rutan som visas, klickar på **Öppna** och sedan på **Överför**.

1. (Valfritt) Klicka på dokumentets namn för att se den nya versionen i Workfront.

   >[!NOTE]
   >
   >Dokumentnamnet i Workfront fylls i som standard och kan inte redigeras. Det ändras inte heller till namnet på filen som du överför eller exporterar som en ny version.
   >
   >
   >![Dokumentnamnet kan inte ändras](assets/doc-name-cant-be-changed.png)

## Kommentera ett Workfront-dokument från Illustrator eller InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Du kan lägga till kommentarer direkt i ett Workfront-dokument i ett Adobe-program. I Workfront visas dina kommentarer i dokumentets uppdateringsområde och i uppdateringsområdet för det Workfront-objekt där dokumentet sparas.

1. Öppna ett av de Adobe-program som stöds.
1. Om Workfront-tillägget inte visas klickar du på **Fönster** > **Tillägg** > **Workfront**.

   En lista över arbetsobjekt som du har tilldelats visar om projektet är en aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

1. Klicka på det projekt, den uppgift eller det problem där det befintliga dokumentet listas.

   Du kan söka efter detta genom att skriva namnet i rutan **Sök** och välja **Projekt**, **Aktivitet** eller **Problem** i listrutan till höger om rutan **Sök** . Om arbetsobjektets namn inte visas i listan trycker du på **Retur** för att söka efter alla Workfront-objekt som du har åtkomst till för att visa.

1. Klicka på det befintliga dokumentets namn och klicka sedan på **Markera** i det nedre högra hörnet av Workfront-tillägget.
1. Klicka på fliken **Kommentar** och skriv sedan uppdateringen i rutan.

1. (Valfritt) Om du vill inkludera andra Workfront-användare eller -team i kommentaren börjar du skriva namnet på en användare eller ett team i rutan **Meddela personer eller team** och klickar sedan på namnet när det visas i listrutan.
1. (Valfritt) Om du vill begära godkännande av dokumentet väljer du **Gör en godkännandebegäran**.
1. Klicka på **Uppdatera**.

   En uppdatering registreras på fliken Uppdateringar i dokumentet. Workfront-användare som du tar med i kommentaren får ett meddelande i appen och, beroende på hur Workfront är konfigurerat, kan även få ett e-postmeddelande.

   Mer information om meddelanden i Workfront finns i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

   Mer information om hur du tar emot e-postmeddelanden finns i [Adobe Workfront-meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

## Begär dokumentgodkännande från Illustrator eller InDesign

Du kan begära godkännande av ett Workfront-dokument direkt från ett Adobe-program.

Du kan begära dokumentgodkännande från följande enheter:

* En Workfront-användare
* En extern användare utan ett Workfront-konto

Du kan begära ett godkännande av ett dokument från ett Adobe-program på följande sätt:

* Genom att bifoga en godkännare till dokumentet.
* Genom att kommentera ett dokument, meddela personen när du gör en kommentar och bifoga dem som godkännare till dokumentet.

  Mer information om hur du begär ett godkännande när du kommenterar ett dokument finns i avsnittet [Kommentera ett Workfront-dokument från Illustrator eller InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) i den här artikeln.

Så här begär du godkännande av ett dokument från ett Adobe-program:

1. Öppna ett av de Adobe-program som stöds.
1. Om Workfront-tillägget inte visas klickar du på **Fönster** > **Tillägg** > **Workfront**.

   En lista över arbetsobjekt som du har tilldelats visar om projektet är en aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

1. Klicka på det projekt, den uppgift eller det problem där det befintliga dokumentet listas och klicka sedan på namnet på det befintliga dokumentet.

   Du kan söka efter detta genom att skriva namnet i rutan **Sök** och välja **Projekt**, **Aktivitet** eller **Problem** i listrutan till höger om rutan **Sök** . Om arbetsobjektets namn inte visas i listan trycker du på **Retur** för att söka efter alla Workfront-objekt som du har åtkomst till för att visa.

1. Klicka på namnet på det befintliga dokumentet och klicka sedan på **Markera** i det nedre högra hörnet av Workfront-tillägget.
1. Klicka på fliken **Godkännande**.
1. Om du vill lägga till en godkännare gör du något av följande i **Börja skriva ett namn**:

   * Skriv namnet på en godkännare och markera den när den visas i listan.

     ![Lägg till en dokumentgodkännare](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Skriv e-postadressen till en extern användare.

1. Klicka på **Begär godkännande**.

   Workfront-användare som du tar med i kommentaren eller lägger till som godkännare får ett meddelande i appen och, beroende på hur Workfront är konfigurerat, kan även få ett e-postmeddelande.\
   Externa användare får ett e-postmeddelande där de kan fatta beslut om godkännandet.

   Mer information om meddelanden i Workfront finns i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Mer information om hur du tar emot e-postmeddelanden finns i [Adobe Workfront-meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

## Generera ett bevis från Illustrator eller InDesign {#generate-a-proof-from-illustrator-or-indesign}

Om ni använder automatiserade arbetsflödesmallar kan ni generera ett korrektur för ett dokument som ni skapar i ett Adobe-program utan att lämna programmet. Mer information om hur du skapar korrektur finns i [Skapa korrektur](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md). Mer information om automatiserade arbetsflödesmallar finns i [Automatiserade arbetsflödesmallar](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) i [Översikt över automatiserat arbetsflöde](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Öppna ett av de Adobe-program som stöds.
1. Om Workfront-tillägget inte visas klickar du på **Fönster** > **Tillägg** > Workfront.

   En lista över arbetsobjekt som du har tilldelats visar om projektet är en aktuell status. Om en lista inte visas loggar du in på Workfront.

   Personliga aktiviteter listas under **Inget projekt**.

1. Om dokumentet redan har överförts till Workfront väljer du projekt, uppgift eller utgåva i tillägget Workfront där dokumentet finns med och klickar sedan på dokumentets namn.

   eller

   Överför ett Adobe-dokument till ett Workfront-objekt, enligt beskrivningen i avsnittet [Överför en fil till ett Workfront-projekt, en aktivitet eller ett problem](#upload-a-file-to-a-workfront-project-task-or-issue) i den här artikeln och klicka sedan på dokumentets namn.

1. I listrutan **Klicka för att välja format** och klicka på det format som du vill spara filen i Workfront.

   Vissa format är inte tillgängliga när du har aktiverat korrekturfunktionen i det följande steget. Mer information finns i [Exporterade filformat som stöds](#supported-exported-file-formats) i den här artikeln.

1. Klicka på **Överför som ett nytt korrektur** för att aktivera det.
1. Välj den **arbetsflödesmall** som du vill att personer ska använda när de granskar dokumentet.

   Din Workfront-administratör konfigurerar automatiska arbetsflödesmallar, enligt beskrivningen i [Skapa och hantera automatiska arbetsflödesmallar](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). Kontakta administratören om du har frågor.

   1. Lägg till minst en **ny mottagare** i varje fas i arbetsflödesmallen.

      Du kan börja skriva ett namn och markera det när du ser det i listrutan som visas.

   1. Ange **korrekturrollen** och frekvensen för **e-postaviseringar** för varje mottagare som du lägger till.

   1. (Valfritt) I avsnittet **E-postmeddelande** väljer du om du vill skicka ett e-postmeddelande med ett anpassat meddelande om korrekturet till alla korrekturmottagare som du har lagt till.

1. Klicka på **Skapa bevis**.

   Du kan visa förloppet för korrekturskapande. En varning visas när genereringen är klar. Du kan öppna uppgiften där du skapade korrekturet och den finns där.

## Ladda upp en ny version av ett korrektur utan att behöva lämna Illustrator eller InDesign

1. Klicka på ett befintligt dokument som har ett korrektur och klicka sedan på **Markera** i det nedre högra hörnet.
1. Klicka på **Överför som nytt korrekturversion** för att aktivera det.
1. (Valfritt) Välj den **arbetsflödesmall** som du vill att personer ska använda när de granskar den nya versionen.

   Om du inte väljer en annan mall gäller den mall som valts för den tidigare versionen. Om du har ändrat mallen för den tidigare versionen gäller ändringarna även för den nya versionen.

   Din Workfront-administratör konfigurerar automatiska arbetsflödesmallar, enligt beskrivningen i [Skapa och hantera automatiska arbetsflödesmallar](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). Kontakta administratören om du har frågor.

   1. Lägg till minst en **ny mottagare** i varje fas i arbetsflödesmallen.

      Du kan börja skriva ett namn och markera det när du ser det i listrutan som visas.

   1. Ange **korrekturrollen** och frekvensen för **e-postaviseringar** för varje mottagare som du lägger till.
   1. (Valfritt) I avsnittet **E-postmeddelande** väljer du om du vill skicka ett e-postmeddelande med ett anpassat meddelande om korrekturet till alla korrekturmottagare som du har lagt till.

1. Klicka på **Skapa ny korrekturversion**.

   Du kan visa förloppet för korrekturskapande. En varning visas när genereringen är klar. Du kan öppna uppgiften där du skapade korrekturet och den finns där.

## Logga ut från Workfront Extension

1. I Adobe-programmet klickar du på **Fönster** > **Tillägg** > **Workfront**.

1. Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) i panelens övre högra hörn.

1. (Valfritt) Klicka på **Feedback** för att öppna en kort enkät och skicka dina synpunkter om Workfront för Adobe Creative Cloud till Workfront.
1. Klicka på **Logga ut**.\
   Inloggningsskärmen visas. Mer information om inloggning finns i [Logga in på Workfront Extension från Illustrator eller InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) i den här artikeln.

## Exporterade filformat som stöds {#supported-exported-file-formats}

* [Exporterade filformat som stöds för Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Exporterade filformat som stöds för Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Exporterade filformat som stöds för Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

Workfront stöder följande filformat för export av en fil från InDesign till Workfront:

* EPS - Encapsulated PostScript
* EPUB - elektronisk publikation med fast layout
* EPUB - flödningsbar elektronisk publikation &#42;
* HTML - HyperText Markup Language
* IDML - InDesign Markup Language &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PDF - Adobe Portable Document File
* PNG - Portable Network Graphics
* SWF - Flash Player &#42;
* XML - Extensible Markup Language &#42;

&#42; Det här filformatet är inte tillgängligt när **Överför ett nytt korrektur** är aktiverat (mer information om det här alternativet finns i [Skapa ett korrektur från Illustrator eller InDesign](#generate-a-proof-from-illustrator-or-indesign) i den här artikeln). Om det här filformatet redan har valts innan du aktiverar **Överför ett nytt korrektur** ändras filformatet till PDF. Du kan välja ett annat format i listan.

### Exporterade filformat som stöds för Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront stöder följande filformat för export av en fil från Illustrator till Workfront:

* DWG - AutoCAD-ritning, AutoCAD Interchange-fil &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PNG - Portable Network Graphics
* PSD - Photoshop-dokument
* SWF - Flash Player &#42;
* TIFF - filformat för taggad bild

&#42; Det här filformatet är inte tillgängligt när **Överför ett nytt korrektur** är aktiverat (mer information om det här alternativet finns i [Skapa ett korrektur från Illustrator eller InDesign](#generate-a-proof-from-illustrator-or-indesign) i den här artikeln). Om det här filformatet redan har valts innan du aktiverar **Överför ett nytt korrektur** ändras filformatet till PNG. Du kan välja ett annat format i listan.

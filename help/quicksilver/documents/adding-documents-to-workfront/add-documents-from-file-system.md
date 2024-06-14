---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Lägga till dokument i Adobe Workfront från filsystemet
description: Du kan lägga till dokument i projekt, uppgifter eller problem i flera områden i Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: 187e33c088177affd246aaf90cea33d6201e7a1b
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 1%

---

# Lägga till dokument i Adobe Workfront från filsystemet

Du kan lägga till dokument i projekt, uppgifter eller problem i följande områden i Adobe Workfront:

* Det globala dokumentområdet
* Dokumentområdet för ett Workfront-objekt
* Ett anslutet kort på Workfront

Du kan också överföra nya versioner av dokument och lägga till länkar till dokument från tredjepartsleverantörer i molnet, som Google Drive, Dropbox och Microsoft OneDrive. Mer information om hur du lägger till nya versioner av dokument finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md). Mer information om hur du lägger till dokument från tredjepartsleverantörer i molnet finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Det finns inga begränsningar för vilka filtyper och filstorlekar du kan överföra till Workfront. För att överföringen ska lyckas måste den slutföras inom fem minuter och du måste ha tillräckligt med lagringsutrymme tillgängligt.

Om du behöver information om hur du överför nya versioner av ett dokument till Workfront går du till [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Lägga till dokument i Workfront

Du kan lägga till nya dokument i Workfront från filsystemet på din arbetsstation. Du kan även länka dokument från tredjepartsprogram som Google Drive och SharePoint.

>[!IMPORTANT]
>
>* Du kan överföra upp till 150 dokument samtidigt.
>* Det finns ingen gräns för filstorleken.
>* Nedladdningen av dokument är begränsad till 4 GB.

Så här lägger du till ett dokument:

1. Gå till projektet, uppgiften eller utgåvan där du vill lägga till ett nytt dokument.
1. Klicka på **Dokument** klickar du på **Lägg till ny** listruta.

   ![](assets/add-new-doc.png)

1. Beroende på vilken typ av dokument du vill lägga till gör du något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Överför dokument från filsystemet till din arbetsstation</td> 
      <td> 
       <ol> 
        <li value="1">Från <strong>Lägg till ny</strong> nedrullningsbar meny, välja <strong>Dokument.</strong></li> 
        <li value="2"> <p>Bläddra till och välj det dokument som du vill lägga till i filsystemet på din arbetsstation.<br></p> <p>Du kan markera flera dokument genom att hålla ned Skift-tangenten när du markerar ytterligare filer.</p> </li> 
        <li value="3">Klicka <strong>Öppna</strong>.</li> 
       </ol> 
       <p><b>ANMÄRKNING</b>: Du kan också dra och släppa filer direkt från filhanteraren i dokumentlistan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Överför dokument från ett tredjepartsprogram som Google Drive eller SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Från <strong>Lägg till ny</strong> nedrullningsbar meny, välja <strong>Från &lt;name_of_third-party_application&gt;</strong>.</p> <p>Om du till exempel vill överföra ett dokument från Google Drive klickar du på <strong>Från Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Följ instruktionerna för att välja dokumentet i tredjepartsprogrammet.<br></p> <p>Mer information om länkade dokument finns i <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Länka dokument från externa program</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begär ett dokument från en annan Workfront-användare</td> 
      <td> 
       <ol> 
        <li value="1">Från <strong>Lägg till ny</strong> nedrullningsbar meny, välja <strong>Begär ett dokument</strong>.</li> 
        <li value="2">I <strong>Vilka begär du det från?</strong> anger du namnet på den användare som du begär dokumentet från.</li> 
        <li value="3">I <strong>Berätta för dem vad du begär</strong> anger du namnet på dokumentet.</li> 
        <li value="4"> <p>Klicka <strong>Skicka förfrågan</strong>.</p> <p>Din förfrågan visas på fliken Dokument.</p> <p>Mer information om hur du begär dokument finns i <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Begär ett dokument</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

## Dokumentsäkerhet

Workfront webbplats förhindrar att virus och annat skadligt innehåll kommer in på webbplatsen via dokument på följande sätt:

* [Hur Workfront identifierar skadade filer](#how-workfront-detects-corrupted-files)
* [Filnamnsbegränsningar](#file-name-restrictions)

### Hur Workfront identifierar skadade filer {#how-workfront-detects-corrupted-files}

Dokumentskanning är bara aktiverat för din organisation på begäran.

Om dokumentskanning är aktiverat skannas filer under 25 MB när de överförs. Filer som är större än 25 MB genomsöks inte.

Om Workfront upptäcker ett skadat dokument avbryter Workfront överföringsprocessen och ett meddelande visas som anger att filen är skadad. Du får också ett e-postmeddelande när Workfront upptäcker potentiellt skadligt innehåll och filen är separerad för borttagning.

Skadade filer tas bort inom 24 timmar efter att de identifierats, såvida du inte tar bort dem manuellt. Om du tar bort en skadad fil spårar Workfront den här åtgärden som en uppdatering. Om du tillåter att Workfront tar bort den registreras inga uppdateringar.

### Filnamnsbegränsningar {#file-name-restrictions}

Filer som överförs till Workfront får inte innehålla vissa tecken i filnamn. Om en fil innehåller något av följande tecken i filnamnet, tas tecknen bort från filnamnet när filen överförs: `! # % * \ | ' " / ? < > { } [ ]`.

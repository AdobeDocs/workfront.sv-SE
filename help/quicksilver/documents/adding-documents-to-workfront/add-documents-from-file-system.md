---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Lägga till dokument i Adobe Workfront från filsystemet
description: Du kan lägga till dokument i projekt, uppgifter eller problem i flera områden i Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Lägga till dokument i Adobe Workfront från filsystemet

Workfront har för närvarande två versioner av dokumentområdet: det gamla dokumentområdet och det nya dokumentområdet. Vilken version din organisation använder beror på om din organisation använder äldre Workfront-lagring eller Enterprise-lagring. Mer information om de här lagringstyperna finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

Hur du lägger till dokument i Workfront varierar beroende på vilken version av dokumentområdet som används i organisationen.

* [Lägg till dokument i från filsystemet i det äldre dokumentområdet](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Lägga till dokument i Workfront i området för nya dokument](#add-documents-to-workfront-in-the-new-documents-area)



## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Äldre Workfront-lagring: Redigera åtkomst till dokument</p> 
   <p>Enterprise-lagring: Redigera åtkomst till dokument är aktiverat som standard och kan inte ändras</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägga till dokument från filsystemet i det äldre dokumentområdet

Om din organisation använder äldre Workfront-lagring visas det äldre dokumentområdet när du öppnar dokument i Workfront. Mer information om Workfront-lagring finns i [Skillnader mellan Adobe Enterprise-lagring och äldre Workfront-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

Du kan lägga till dokument i projekt, uppgifter eller problem i följande områden i Adobe Workfront:

* Det globala dokumentområdet
* Dokumentområdet för ett Workfront-objekt
* Ett anslutet kort på Workfront

Du kan också överföra nya versioner av dokument och lägga till länkar till dokument från tredjepartsleverantörer i molnet, som Google Drive, Dropbox och Microsoft OneDrive. Mer information om hur du lägger till nya versioner av dokument finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md). Mer information om hur du lägger till dokument från tredjepartsleverantörer i molnet finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Det finns inga begränsningar för vilka filtyper och filstorlekar du kan överföra till Workfront. För att överföringen ska lyckas måste den slutföras inom fem minuter och du måste ha tillräckligt med lagringsutrymme tillgängligt.

Om du behöver information om hur du överför nya versioner av ett dokument till Workfront läser du [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).


### Lägga till dokument i Workfront i det äldre dokumentområdet

Du kan lägga till nya dokument i Workfront från filsystemet på din arbetsstation. Du kan även länka dokument från tredjepartsprogram som Google Drive och SharePoint.

>[!IMPORTANT]
>
>* Du kan överföra upp till 150 dokument samtidigt.
>* Det finns ingen gräns för filstorleken.
>* Nedladdningen av dokument är begränsad till 4 GB.

Så här lägger du till ett dokument:

1. Gå till projektet, uppgiften eller utgåvan där du vill lägga till ett nytt dokument.
1. Klicka på fliken **Dokument** och klicka sedan på listrutan **Lägg till ny** .

   ![Lägg till nytt dokument](assets/add-new-doc.png)

1. Beroende på vilken typ av dokument du vill lägga till gör du något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Överför dokument från filsystemet till din arbetsstation</td> 
      <td> 
       <ol> 
        <li value="1">I listrutan <strong>Lägg till ny</strong> väljer du <strong>Dokument.</strong></li> 
        <li value="2"> <p>Bläddra till och välj det dokument som du vill lägga till i filsystemet på din arbetsstation.<br></p> <p>Du kan markera flera dokument genom att hålla ned Skift-tangenten när du markerar ytterligare filer.</p> </li> 
        <li value="3">Klicka på <strong>Öppna</strong>.</li> 
       </ol> 
       <p><b>Obs!</b> Du kan också dra och släppa filer direkt från filhanteraren i dokumentlistan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Överför dokument från ett tredjepartsprogram som Google Drive eller SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>I listrutan <strong>Lägg till ny</strong> väljer du <strong>Från &lt;name_of_third-party_application&gt;</strong>.</p> <p>Om du till exempel vill överföra ett dokument från Google Drive klickar du på <strong>Från Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Följ instruktionerna för att välja dokumentet i tredjepartsprogrammet.<br></p> <p>Mer information om länkade dokument finns i <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Länka dokument från externa program</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begär ett dokument från en annan Workfront-användare</td> 
      <td> 
       <ol> 
        <li value="1">Välj <strong>Begär ett dokument</strong> i listrutan <strong>Lägg till nytt</strong>.</li> 
        <li value="2">I rutan <strong>Vem begär det från</strong> skriver du namnet på den användare du begär dokumentet från.</li> 
        <li value="3">Skriv namnet på dokumentet i rutan <strong>Ange vad du begär</strong>.</li> 
        <li value="4"> <p>Klicka på <strong>Skicka begäran</strong>.</p> <p>Din förfrågan visas på fliken Dokument.</p> <p>Mer information om hur du begär dokument finns i <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Begär ett dokument</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## Lägga till dokument i Workfront i området för nya dokument

Du kan lägga till dokument i projekt, uppgifter eller utgåvor med hjälp av Enterprise-lagringsmodellen. Mer information om Enterprise-lagring finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

Funktionen stöds för närvarande inte i området för nya dokument:

* Överföra dokument till det globala dokumentområdet
* Lägga till länkar till dokument från tredjepartsleverantörer i molnet, som Google Drive, Dropbox och Microsoft OneDrive.
* Begära dokument
* Kopiera en länk till en mapp
* Checka ut dokument
* Klistra in bilder från Urklipp
* Lägga till smarta mappar


### Lägga till dokument i Workfront i området för nya dokument

Om ditt företag använder Enterprise-lagring visas det nya dokumentområdet när du öppnar dokument i Workfront. Mer information om Enterprise-lagring finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

Så här lägger du till ett dokument:

1. Gå till projektet, uppgiften eller utgåvan där du vill lägga till ett nytt dokument.
1. Klicka på **Dokument** i den vänstra panelen.
1. Klicka på **Nytt** till höger på sidan eller dra och släpp filen i släppzonen som visas. Du kan lägga till flera dokument samtidigt.

   ![Lägg till ett nytt dokument](assets/add-new-doc-new-doc.png)

Om du behöver information om hur du överför nya versioner av ett dokument till Workfront läser du [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

## Dokumentsäkerhet för företagslagring

Workfront förhindrar att virus och annat skadligt innehåll kommer in på webbplatsen via dokument på följande sätt:

**Så här identifierar Workfront skadade filer**

Dokumentskanning aktiveras automatiskt för objekt som använder Enterprise-lagringsmodellen.

Alla filer under 500 MB genomsöks när de överförs. Filer som är större än 500 MB genomsöks inte. Om Workfront upptäcker ett skadat dokument tas det bort automatiskt.

**Filnamnsbegränsningar**

Eftersom integreringen byggs med Adobe Enterprise-lagring finns det vissa tvingande struktur- och namnkonventioner som du bör känna till när du hanterar projekt och dokument.

* Objektnamn måste vara unika och kan inte dupliceras
* Adobe Enterprise-lagring kräver unika namn för peer-objekt med samma överordnade i hierarkiträdet
* Dokument kan inte ha samma namn om de tillhör samma projekt
* Dokumentnamn får inte innehålla något av följande specialtecken: `\ / : * ? " | < >`
* Dokumentnamn får innehålla högst 255 tecken

Med dessa begränsningar i åtanke byter Workfront automatiskt namn på objekt och dokument efter behov för att förhindra konflikter.


## Dokumentsäkerhet för äldre Workfront-lagring

Workfront webbplats förhindrar att virus och annat skadligt innehåll kommer in på webbplatsen via dokument på följande sätt:

**Så här identifierar Workfront skadade filer**

Dokumentskanning är bara aktiverat för din organisation på begäran.

Om dokumentskanning är aktiverat skannas filer under 25 MB när de överförs. Filer som är större än 25 MB genomsöks inte.

Om Workfront upptäcker ett skadat dokument visas ett meddelande om att filen är skadad. Du får också ett e-postmeddelande när Workfront upptäcker potentiellt skadligt innehåll och filen är separerad för borttagning.

Skadade filer tas bort inom 24 timmar efter att de identifierats, såvida du inte tar bort dem manuellt. Om du tar bort en skadad fil spårar Workfront den här åtgärden som en uppdatering. Om du tillåter att Workfront tar bort den registreras inga uppdateringar.

**Filnamnsbegränsningar**

Filer som överförs till Workfront får inte innehålla vissa tecken i filnamn. Om en fil innehåller något av följande tecken i filnamnet, tas tecknen bort från filnamnet när filen överförs: `! # % * \ | ' " / ? < > { } [ ]`.

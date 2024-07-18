---
content-type: overview
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-desktop-proofing-viewer
title: Förstå Desktop Proofing Viewer
description: Desktop Proofing Viewer är avsedd för korrektur av interaktivt innehåll, men du kan också använda den för att korrekturgranska statiskt innehåll och videomaterial.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 4610f24f-345a-4ebc-8a0c-382e34cac7b0
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Förstå Desktop Proofing Viewer

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Desktop Proofing Viewer är avsedd för korrektur av interaktivt innehåll, men du kan också använda den för att korrekturgranska statiskt innehåll och videomaterial.

Till skillnad från Web Proofing Viewer är Desktop Proofing Viewer ett program som körs på din arbetsstation. Du kommer dock åt det från [!DNL Workfront] eller från [!DNL Workfront Proof] när du startar korrektur, i stället för att köra det som ett fristående program (mer information om hur du installerar Desktop Proofing Viewer finns i [Installera Desktop Proofing Viewer](../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)).

## Jämföra Desktop Proofing Viewer med andra korrekturläsare

* [Desktop Proofing Viewer vs. Web Proofing Viewer](#desktop-proofing-viewer-vs-web-proofing-viewer)
* [Desktop Proofing Viewer kontra Legacy Proofing Viewer](#desktop-proofing-viewer-vs-legacy-proofing-viewer)

### Desktop Proofing Viewer vs. Web Proofing Viewer {#desktop-proofing-viewer-vs-web-proofing-viewer}

Två huvudegenskaper skiljer Desktop Proofing Viewer från Web Proofing Viewer:

* Med Desktop Proofing Viewer kan du granska interaktivt material som en webbplats, en direktuppspelad video eller en interaktiv banner. Med Web Proofing Viewer kan du endast granska statiskt material och videoklipp.
* Desktop Proofing Viewer körs på den lokala datorn som ett program. Web Proofing Viewer körs i webbläsaren.

  >[!NOTE]
  >
  >   * Om din organisation inte kan använda appen Desktop Proofing Viewer av säkerhetsskäl kan din [!DNL Workfront]-administratör konfigurera ditt system så att du kan granska interaktivt innehåll som paketerats i en ZIP-arkivfil i Web Proofing Viewer.
  >   * Korrekturhanteringsåtgärder som att skapa och bläddra igenom korrektur utförs i [!DNL Workfront] eller [!DNL Workfront Proof]. Desktop Proofing Viewer är bara till för granskning av korrektur.


Mer information om funktionerna för de olika korrekturläsarna finns i [Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer - översikt](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)

### Desktop Proofing Viewer kontra Legacy Proofing Viewer {#desktop-proofing-viewer-vs-legacy-proofing-viewer}

Du kanske inte har tillgång till det äldre korrekturläsaren eftersom den stöds av Flashen, som har tagits bort i de flesta miljöer.

Desktop Proofing Viewer innehåller följande förbättringar jämfört med det äldre korrekturläsaren:

* Granska oskyddade (HTTP) platser, inte bara säkra (HTTPS) platser.
* Granska iFrame-skyddade webbplatser (webbplatser som inte kan visas i en iFrame).
* Visa innehåll med förkonfigurerade upplösningar för olika enheter.\
   Du kan till exempel se hur innehåll visas på olika vanliga skrivbordsupplösningar eller på enskilda enheter som iPhone 8.

Det äldre korrekturläsaren tas bort från [!DNL Workfront] med version 2018.3 i slutet av kalenderåret 2018.

Det äldre korrekturläsaren ingår inte för kunder som köper [!DNL Workfront] efter version 2018.2 i juli 2018.

## Användarinställning för att öppna icke-interaktiva korrektur i korrekturläsaren för skrivbordet

Även om huvudsyftet med Desktop Proofing Viewer är att korrekturgranska interaktivt innehåll kan du även använda det för att korrekturgranska statiskt material och videoklipp.

Användare kan konfigurera Desktop Proofing Viewer så att den startas automatiskt när de öppnar korrektur av alla slag, inklusive statiskt eller videokort. Mer information finns i [Konfigurera inställningar för korrekturläsare](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

## Ange en korrektur-URL

Om du startar Desktop Proofing Viewer direkt från din arbetsstation kan du öppna ett korrektur genom att ange korrektur-URL:en. För att kunna göra detta måste du ha ett korrektur-URL för det korrektur som du vill visa.

Du bör öppna korrektur direkt från [!DNL Workfront]. Mer information finns i [Granska ett korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Skapa ett statiskt webbplatskorrektur med  [!DNL Workfront Proof]
description: Du kan skapa statiska korrektur av dina webbsidor. Dessutom kan du simulera olika enheter genom att definiera skärmupplösningen för klippen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Skapa ett statiskt webbplatskorrektur med [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan skapa statiska korrektur av dina webbsidor. Dessutom kan du simulera olika enheter genom att definiera skärmupplösningen för klippen.

## Skapa ett statiskt korrektur av en webbplats

1. Öppna sidan [!UICONTROL New proof] enligt beskrivningen i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Klistra in eller skriv din URL i rutan **www.shareyourlink.com**.
1. Du kan upprepa det här steget om du vill lägga till flera URL-adresser.
1. Precis nedanför den här rutan klickar du på upplösningen (standardvärdet är 1 366 × 768) och väljer sedan önskade upplösningar i rutan **[!UICONTROL Screensot resolution]**.
Välj en mindre upplösning om du vill korrekturgranska designer för mobila enheter. Vanligtvis läses designen in enligt upplösningen för skärm-/webbläsarfönster.

1. Klicka på **[!UICONTROL Look for subpages]** om du vill inkludera anslutna sidor som finns i samma domän/underdomän som den angivna URL:en.
   [!DNL Workfront Proof] skannar de anslutna sidorna och visar dem under alternativet **[!UICONTROL Look for subpages]**. Du kan markera de sidor som du vill inkludera.

1. Med funktionen [!UICONTROL Combine proofs] kan du skicka alla webbsidor som ett enda flersidigt korrektur.
1. Klicka på **[!UICONTROL Done]** och avsluta sedan konfigurationen av ditt korrektur enligt beskrivningen i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Om lösenordsskyddade sidor och sidor som kräver behörighet

[!DNL Workfront Proof] kan inte hämta en lösenordsskyddad webbplats som ett statiskt korrektur.

För att kunna skapa korrektur från sidor som kräver tillstånd måste IT-teamet lägga till en av följande URL:er till företagets Tillåtelselista som vårt webbhämtningsverktyg är kopplat till:

**AWS-kluster i USA**: webcapture.proofhq.com

**GCP-kluster i USA**: webcapture.gcp.proofhq.com

**EMEA-kluster**: webcapture.proofhq.eu

>[!NOTE]
>
>Vi rekommenderar interaktiv korrektur i stället för statisk korrektur för interna sidor som kräver auktorisering och lösenordsskyddade webbplatser. Mer information finns i [Översikt över korrektur för interaktivt innehåll](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Bearbeta statiska korrektur av webbplatser

* Animeringar, inbäddade videor, skript och interaktioner kan inte inkluderas i statiska korrektur för webbplatser. Om du vill korrekturgranska interaktivt innehåll kan du läsa [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Korrektursidor förbereds vanligtvis med en hastighet på cirka 20 sekunder per sida. Den totala beredningstiden beror dock också på de servrar där sidorna finns. Verktyget väntar 60 sekunder på att varje skickad URL-adress ska läsas in. Om väntetiden överskrids misslyckas korrekturet.
* För kombinerade korrektur misslyckas korrekturet om någon av URL:erna inte svarar på hämtningsverktyget.
* [!DNL Workfront Proof] hämtar webbsidor upp till 195 tum långt efter rastreringen. Om webbsidan är längre än så misslyckas korrekturet.
* Textextrahering är tillgängligt för alla textelement, men text som monterats som bilder extraheras inte.
* Texthyperlänkar kan klickas på korrektur och de länkade sidorna öppnas på de nya webbläsarflikarna.
* Det går inte att klicka på hyperlänkarna i bilderna om elementen style=&quot;display:block&quot; används i taggarna `<a>`. Vi rekommenderar att du justerar dessa delar av siddesignen.
* För bästa resultat rekommenderar vi att du skapar sidorna enligt de bästa kodningspraxis och erkända standarder.

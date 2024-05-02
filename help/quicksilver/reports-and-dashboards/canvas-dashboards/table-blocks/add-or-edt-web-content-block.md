---
title: Lägga till eller redigera ett webbinnehållsblock i rapportarbetsytan
description: Med webbinnehållsblock kan du visa information från externa webbplatser direkt i rapporten.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Lägga till eller redigera ett webbinnehållsblock i rapportarbetsytan

Med webbinnehållsblock kan du visa information från externa webbplatser direkt i rapporten.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Lägga till eller redigera ett webbinnehållsblock

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på&#x200B;**Rapportering**.
1. Klicka **Ny rapport**.

   eller

   Klicka på **Mer** icon ![](assets/more-icon-27x15.png) i rapportrubriken och klicka sedan på **Redigera**.

1. Till höger på skärmen, under **Lägg till ett block**, antingen:

   Dra **Webbinnehåll** på arbetsytan direkt till önskad plats.

   eller

   Dubbelklicka på **Webbinnehåll** om du vill lägga till ett block högst upp på arbetsytan.

   >[!TIP]
   >
   >Du kan ändra storleken på blocket efter att det har placerats genom att dra i hörnhandtagen.

1. Klicka **Namnlöst webbinnehåll** i blockhuvudet och skriv en rubrik för blocket.
1. Klicka på **Redigera** icon ![](assets/edit-icon.png) i blockhuvudet.

   ![](assets/web-content-block-header-350x76.png)

1. I **Inställningar** som öppnas anger du den fullständiga URL-adressen till sidan som du vill visa (inklusive&quot;https://&quot;) i dialogrutan **URL** fält.

   >[!NOTE]
   >
   >För närvarande kan bara webbplatser från vissa domäner visas. Följande domäner kan användas:
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   En varning visas under den angivna URL:en om den inte kan bäddas in. Dessa varningar omfattar:

   | Varningsnamn | Orsak |
   |---|---|
   | Ogiltig URL | Den angivna URL:en returnerar ingen giltig plats. |
   | Begränsningar för leverantörens webbplats | Den webbplats som du försöker bädda in är inte tillåten. |

   {style="table-layout:auto"}

1. (Valfritt) Klicka på **Godkänn parametrar** för att öppna en lista över tillgängliga lösenordsparametrar.

   >[!WARNING]
   >
   >Godkänd-parametrar är för närvarande inaktiverade.

1. Klicka **Bädda in URL** för att spara dina val och återgå till rapporten.

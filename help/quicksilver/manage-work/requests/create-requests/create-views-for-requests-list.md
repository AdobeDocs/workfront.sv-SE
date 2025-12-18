---
product-area: requests
navigation-topic: create-requests
title: Skapa vyer i området Förfrågningar
description: Om du använder den nya begärandefunktionen kan du skapa och spara vyer för området Förfrågningar.
author: Becky
feature: Work Management
source-git-commit: d2e938cabc5123a89335a42ed06bccaa77fcad83
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Skapa eller redigera vyer i området Förfrågningar

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Om du använder den nya begärandefunktionen kan du skapa och spara vyer för området Förfrågningar. De här vyerna innehåller filter och kolumnupplägg.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  <p>Du måste vara Workfront-administratör för att kunna lägga till vyer i layoutmallar</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Du måste ha Adobe Workfront Planning för att kunna visa planeringsförfrågningar eller begära formulär</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en vy i området Förfrågningar

{{step1-to-requests}}

1. (Valfritt och villkorligt) Välj inställningen **Byt till ny upplevelse** i skärmens övre högra hörn om följande saker gäller för din organisation och din Workfront-instans:

   * Din organisation har köpt ett Workfront-paket
   * Din organisation har anslutit sig till Adobe Unified Experience.
   * Din administratör har gett dig åtkomst till Workfront Planning
   * Du har minst behörighet att visa en Workfront Planning-arbetsyta

   Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md)

1. Klicka på listrutan **Vyer** ![Vyer](assets/view-icon-requests.png) och välj **Ny vy**.

   ![Ny vy](assets/create-new-view.png)

1. Ange ett namn för den nya vyn och klicka på **Skapa**.
1. Fortsätt till [Redigera en vy i området Förfrågningar](#edit-a-view-in-the-requests-area).

## Redigera en vy i området Förfrågningar

Du kan redigera befintliga vyer, inklusive vyer som du just har skapat.

{{step1-to-requests}}

1. (Valfritt och villkorligt) Välj inställningen **Byt till ny upplevelse** i skärmens övre högra hörn om följande saker gäller för din organisation och din Workfront-instans:

   * Din organisation har köpt ett Workfront-paket
   * Din organisation har anslutit sig till Adobe Unified Experience.
   * Din administratör har gett dig åtkomst till Workfront Planning
   * Du har minst behörighet att visa en Workfront Planning-arbetsyta

   Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md)1.

1. (Valfritt) Om du vill byta namn på en vy klickar du på listrutan **Vyer** ![Vyer](assets/view-icon-requests.png) och klickar på menyn med tre punkter bredvid vyn. Välj sedan **Byt namn** och skriv in det nya namnet för vyn.
1. Klicka på listrutan **Vyer** ![Vyer](assets/view-icon-requests.png) och välj den vy som du vill redigera.
1. <span class="preview">Om du vill lägga till ett anpassat fält som en kolumn klickar du på ikonen **Lägg till kolumn** ![Lägg till kolumn](assets/add-column.png) till höger på skärmen och sedan på plusikonen bredvid det anpassade formulärfältet som du vill lägga till som en kolumn i vyn.</span>

   <span class="preview">Anpassade fält i formulär som är kopplade till objektet i listan kan läggas till som kolumner.</span>

   >[!TIP]
   >
   >Du kan för närvarande inte lägga till kolumner i produktionsmiljön.
1. (Valfritt) Klicka på **Kolumner** och dölj, visa eller ordna om kolumnerna i listan med förfrågningar.

   ![Kolumnruta](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Du kan inte lägga till fler kolumner i produktionsmiljön.

1. (Valfritt) Klicka på **Filter** och börja lägga till villkor för vilka begäranden du vill visa på fliken Planering.

   ![Redigeringsfilter på fliken Planeringsbegäranden](assets/filters-editing-box-in-requests-planning-tab.png)

   Du kan filtrera efter följande fält:

   * **Workspace**: Den arbetsyta som förfrågningsformuläret är associerat med.
   * **Posttyp**: Posttyp som begärandeformuläret är associerat med.
   * **Anmälningsdatum**: Datumet då begäran skickades.
   * **Formulär för begäran**: Namnet på det begärandeformulär som användes för att skicka begäran.
   * **Status**: Status för begäran.
   * **Anges av**: Namnet på den användare som lade till begäran. Om begäran har lagts till av någon utanför Workfront visas **Angivet av**-fältet `N/A`.

   <span class="preview">I förhandsvisningsmiljön kan du även filtrera efter anpassade fält som har lagts till i vyn.</span>

   Du kan ha flera filter kopplade av antingen **And** eller **Or**.
Begärandelistan filtreras automatiskt när du lägger till filtervillkoren.



>[!IMPORTANT]
>
> * Ändringar av vyer sparas automatiskt.
> * Ändringar av vyer är synliga för alla som använder vyn.

## Lägg till vyn i en layoutmall.

En Workfront-administratör kan lägga till den nya vyn i layoutmallar.

Instruktioner finns i [Anpassa filter, vyer och grupperingar med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

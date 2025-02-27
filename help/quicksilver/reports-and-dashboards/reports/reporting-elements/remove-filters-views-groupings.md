---
product-area: reporting
navigation-topic: reporting-elements
title: Ta bort filter, vyer och grupperingar
description: Du kan ta bort ett filter, en vy eller en gruppering från listor och rapporter om du har skapat dem eller om de har delats med dig. Du kan inte ta bort standardfilter, vyer eller grupperingar.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Ta bort filter, vyer och grupperingar

<!-- Audited: 11/2024 -->

Du kan ta bort ett filter, en vy eller en gruppering från listor och rapporter om du har skapat dem eller om de har delats med dig. Du kan inte ta bort standardfilter, vyer eller grupperingar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Medarbetare eller högre</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Begäran eller senare</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td><p>Visa eller ge senare åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td><p>Visa behörigheter med åtkomst för delning till filtret, vyn eller grupperingen som du vill ta bort</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort ett filter med standardverktyget

Du kan ta bort ett filter som delats med dig från listor med projekt, uppgifter eller problem med hjälp av standardgränssnittet i Builder. Standardbygggränssnittet är inte tillgängligt för andra objekt eller för vyer eller grupperingar.

Du kan även ta bort filter som du äger från listor med projekt, uppgifter eller problem med hjälp av standardgränssnittet i Builder.

Systemstandardfilter kan inte tas bort eller tas bort.

### Att tänka på när du tar bort eller tar bort filter med standardverktyget

Följande scenarier gäller när du tar bort eller tar bort ett filter med standardverktyget:

* Om filtret delades med dig och du tar bort det, tas filtret bara bort åt dig. Den användare som ursprungligen skapade det och alla andra användare som det har delats med har fortfarande tillgång till filtret.
* Om du äger filtret och tar bort det tas det bort från Workfront-systemet. Filtret är inte längre tillgängligt för användare som du tidigare delat det med.
* Om du är Workfront-administratör kan du ta bort filtret och det tas bort permanent för alla användare, inklusive ägaren.

### Ta bort ett filter med standardverktyget

1. Gå till en lista med projekt, uppgifter, utgåvor, portfolior, program, användare, mallar eller grupper.
1. Klicka på ikonen **Filter** ![Filter ](assets/filter-nwepng.png) .
1. Hovra över ett filter under **Delat med mig**, klicka på **Mer**-menyn ![Mer-ikonen](assets/more-icon-spectrum.png) och klicka sedan på **Ta bort**.
1. Välj **Ta bort** i bekräftelsemeddelandet om du vill ta bort filtret permanent.

### Ta bort ett filter med standardverktyget

1. Gå till en lista med projekt, uppgifter, utgåvor, portfolior, program, användare, mallar eller grupper.
1. Klicka på ikonen **Filter** ![Filter ](assets/filter-nwepng.png) .
1. Håll pekaren över ett filter som du har behörighet att ta bort, klicka på ikonen **Mer** ![Mer](assets/more-icon-spectrum.png) och klicka sedan på **Ta bort**.

   ![Ta bort filter](assets/new-filters-more-menu-options-with-delete.png)

1. (Valfritt) Klicka på **Avbryt** i bekräftelsemeddelandet för att undvika borttagningen och återgå till filterlistan.
1. Bekräfta borttagningen genom att klicka på **Ta bort** i bekräftelsemeddelandet.

   Filtret tas bort för dig och alla användare som har behörighet till det.

## Ta bort ett filter, en vy eller en gruppering med det äldre verktyget

Du kan ta bort ett filter, en vy eller en gruppering för alla objektlistor med det äldre Builder-gränssnittet.

### Att tänka på när du tar bort filter, vyer och grupperingar med hjälp av det äldre verktyget

Hur du tar bort ett rapportelement beror på om du skapade det eller om det delades med dig.

Följande scenarier gäller när du tar bort ett filter, en vy eller en gruppering:

* **Om du skapade elementet och tog bort det** tas elementet bort från Workfront-systemet. Det är inte längre tillgängligt för användare som du tidigare delat det med.
* **Om elementet delades med dig och du tar bort det** tas elementet bara bort åt dig. Den användare som ursprungligen skapade den och alla andra användare som den har delats med har fortfarande åtkomst till den.

### Ta bort ett filter, en vy eller en gruppering med det äldre verktyget

1. Gå till en lista med objekt eller en rapport.
1. (Villkorligt) Klicka på ikonen **Filter**, **Visa** eller **Gruppering** i en lista, hovra sedan över filtret, vyn eller grupperingen som du vill ta bort, klicka på ikonen **Mer** ![Mer](assets/more-icon.png) och sedan på ikonen **Ta bort** . Filtret, vyn eller grupperingen tas bort.
1. (Villkorligt) Klicka på listrutan **Gruppering**, **Filter** eller **Visa** och välj **Ta bort gruppering**, **Ta bort filter** eller **Ta bort vy** i en rapport.

   Dialogrutan **Mina grupperingar**, **Mina filter** eller **Mina vyer** visas.

   Alla rapportelement som du har behörighet att ta bort kan tas bort. Andra rapportelement visas som nedtonade.

1. Klicka på ikonen **x** bredvid ett rapportelement som du vill ta bort.
1. (Villkorligt) Klicka på **Ja, ta bort** om du valt att ta bort ett filter, en vy eller en gruppering som du har skapat och senare delat med andra. Filtret, vyn eller grupperingen tas bort från Workfront-systemet.

   >[!TIP]
   >
   >Om du tar bort ett filter, en vy eller en gruppering som du har skapat utan att dela det med andra tas det bort från systemet utan att någon bekräftelse behöver skickas.

1. Klicka på **Klar**.


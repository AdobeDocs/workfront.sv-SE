---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: visa endast objekt med godkännandestatus'
description: Du kan bara visa objekt med en viss status som är under Väntar på godkännande. Detta fungerar på samma sätt för alla andra objekt med godkännandestatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Filter: visa endast objekt med godkännandestatus

<!--Audited: 10/2024-->

Du kan bara visa objekt med en viss status som är under Väntar på godkännande. Detta fungerar på samma sätt för alla andra objekt med godkännandestatus.

Du kan placera följande objekt i en godkännandestatus:

* Uppgifter
* Problem
* Projekt

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
    <p>Nytt:</p>
   <ul><li><p>Medarbetare som ändrar ett filter </p></li>
   <li><p>Standard för att ändra en rapport</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Begäran om att ändra ett filter </p></li>
   <li><p>Planera att ändra en rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa endast objekt med godkännandestatus

1. Gå till en lista med projekt.
1. Välj **Nytt filter** i listrutan **Filter**.
1. Välj att filtrera efter **Projekt: Status** och välj sedan den status som du vill filtrera efter i listan.

   I en projektrapport lägger du till exempel till **Status som är lika med planering** om du bara vill visa projekt som har statusen **Planering - Väntar på godkännande**.
1. Klicka på **Textläge**.
1. Ändra raden `status` genom att lägga till **:A** i statusens 3-bokstavskod:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Klicka på **Använd** > **Spara som ny**.

   I listan visas endast projekt som har statusen Planering - Väntar på godkännande.

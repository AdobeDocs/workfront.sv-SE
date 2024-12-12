---
product-area: projects
navigation-topic: financials
title: Ange PIM (Performance Index Method)
description: Performance Index Method (PIM) for the project controls the method Adobe Workfront uses to calculate project performance metrics such as Cost Performance Index (CPI), Cost Schedule Performance Index (CSI), Schedule Performance Index (SPI), and Estimate At Completion (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Ange PIM (Performance Index Method)

Performance Index Method (PIM) for the project controls the method Adobe Workfront uses to calculate project performance metrics such as Cost Performance Index (CPI), Cost Schedule Performance Index (CSI), Schedule Performance Index (SPI), and Estimate At Completion (EAC).

Workfront beräknar dessa värden enligt följande:

* Timmar
* Kostnad

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller PIM i Workfront

* Workfront-administratören eller en gruppadministratör ställer in standardinställningen för om PIM (Performance Index Method) ska vara timbaserad eller kostnadsbaserad. Beräkningarna för prestandamätningarna ändras beroende på hur den här standardinställningen ställs in. Mer information om hur du ändrar standardinställningen för hur du beräknar PIM finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Projektledare kan också ändra inställningen för PIM på projektnivå för enskilda projekt på projektfliken Ekonomi i projektet. Du måste ha behörigheten Hantera för projektet för att kunna redigera projektets finansunderflik.

## Ange PIM (Performance Index Method) för ett projekt

1. Gå till ett projekt som du är ägare till.

   >[!IMPORTANT]
   >
   >Du måste ha behörigheten Hantera för projektet för att kunna utföra följande steg. Vi rekommenderar också att endast projektägaren ska göra ändringar i projektets finansieringsdel.

1. Klicka på **Projektinformation** i den vänstra panelen och gå sedan till området **Ekonomi**.
1. Dubbelklicka på värdet i fältet **Resultatindexmetod** för att redigera det.
1. Välj bland följande alternativ i fältet **Resultatindexmetod**:

   | Timbaserad | Workfront använder de planerade timmarna för att beräkna projektets CPI och EAC, och projektets EAC visas som ett tal i timmar. |
   |---|---|
   | Kostnadsbaserad | Workfront använder den planerade arbetskostnaden vid beräkning av projektets CPI och EAC och EAC visas som ett valutavärde. När du väljer det här alternativet kontrollerar du att dina uppgiftstilldelningar (jobbroller eller användare) är kopplade till kostnadstariffer. |

   {style="table-layout:auto"}

1. Klicka på **Spara** **Ändringar**.

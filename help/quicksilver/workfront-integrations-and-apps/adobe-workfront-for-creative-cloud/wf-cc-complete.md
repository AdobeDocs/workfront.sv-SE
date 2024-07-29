---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Markera arbetsobjekt som slutförda med Adobe Workfront-plugin
description: Du kan vara kvar i Adobe Creative Cloud-programmen och slutföra arbetet i Adobe Workfront utan problem.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d94a2b10-51d5-4995-b7b3-793d7911fca9
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Markera arbetsobjekt som slutförda med plugin-programmet [!DNL Adobe Workfront]

Du kan stanna i följande [!DNL Adobe Creative Cloud]-program och slutföra ditt arbete i [!DNL Adobe Workfront] med plugin-programmet:

{{cc-app-list}}

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> --> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till det objekt som du vill slutföra.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

{{cc-install-prereq}}

## Slutför en arbetsuppgift

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Välj den uppgift eller det problem som du vill markera som slutförd i **[!UICONTROL Work List]**.
1. Klicka på **[!UICONTROL Done]**.  Om du är den enda användaren som är tilldelad den här uppgiften eller utgåvan markeras objektet [!UICONTROL Complete] eller [!UICONTROL Resolved] i [!DNL Workfront].
1. (Villkorligt) Om flera användare har tilldelats till den här uppgiften eller problemet, öppnas en listruta när du klickar på [!UICONTROL Done]. Då kan du:

   Klicka på **[!UICONTROL Done with my part]** om andra användare också måste göra sitt arbete för att uppgiften eller utgåvan ska kunna slutföras.

   eller

   Klicka på **[!UICONTROL Complete]** (för aktiviteter) eller **[!UICONTROL Resolved]** (för problem) om ingen ytterligare åtgärd behöver utföras för uppgiften eller problemet. Detta markerar objektet [!UICONTROL Complete] eller [!UICONTROL Resolved] i [!DNL Workfront].

   >[!NOTE]
   >
   >Om arbetsposten har föregångare är knappen Klar grå tills dessa föregångare har markerats som slutförda. Om du vill visa föregående aktiviteter i [!DNL Workfront] klickar du på aktivitetsnamnet.
   >![](assets/navigate-to-workfront.png)

<!-- I dont think we need this one ![](assets/complete-work-350x529.png) -->

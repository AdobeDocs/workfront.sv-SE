---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Inaktivera eller återaktivera ett företag
description: Du kan inaktivera ett företag som du inte längre använder samtidigt som alla tillhörande historiska data bevaras. Om du inaktiverar ett företag som redan används någonstans i systemet fortsätter det att fungera precis som vanligt. Den har inte tagits bort eller blockerats.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Inaktivera eller återaktivera ett företag

Du kan inaktivera ett företag som du inte längre använder samtidigt som alla tillhörande historiska data bevaras. Om du inaktiverar ett företag som redan används någonstans i systemet fortsätter det att fungera precis som vanligt. Den har inte tagits bort eller blockerats.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td><p>Aktuell: [!UICONTROL Team] eller högre</p>
   <p>eller</p>
   <p>Nytt: Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>eller</p>
   <p>Nytt: [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Åtkomstnivåkonfigurationer</strong> </td> 
   <td> <p>Något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån [!UICONTROL System Administrator], som gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
     <li> <p>Administrativ åtkomst för att hantera företag, vilket gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
    </ul> <p><b>OBS</b>:  
     <ul> 
      <li> <p>Du kan också hantera företag som är kopplade till en grupp där du har tilldelats som gruppadministratör.</p> </li> 
      <li> <p>Om du vill lägga till och ta bort användare från systemet [!DNL Workfront] måste du ha något av följande:</p> 
       <ul> 
        <li> <p>Åtkomstnivån [!UICONTROL System Administrator].</p> </li> 
        <li> <p>I din åtkomstnivå måste [!UICONTROL Edit] väljas för inställningen [!UICONTROL Users]. Dessutom måste alternativet [!UICONTROL Create] och minst ett av de två alternativen [!UICONTROL User Admin] aktiveras för inställningen [!UICONTROL Users], under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Om du använder alternativet [!UICONTROL User Admin (Group Users)] måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inaktivera eller återaktivera ett företag

{{step-1-to-setup}}

1. Klicka på ikonen **[!UICONTROL Companies]** ![Företag](assets/companies-icon-left-panel.png) i den vänstra panelen.

1. Välj ett eller flera företag att inaktivera eller återaktivera.
1. Klicka på **[!UICONTROL Edit]**.
1. Inaktivera alternativet **[!UICONTROL Is Active]** för ett enskilt företag om du vill inaktivera det, eller aktivera alternativet för att aktivera det.

   eller

   För flera företag väljer du **[!UICONTROL No]** i listrutan **[!UICONTROL Is Active]** för att inaktivera dem, eller **[!UICONTROL Yes]** för att aktivera dem.

1. Klicka på **[!UICONTROL Save Changes]**.

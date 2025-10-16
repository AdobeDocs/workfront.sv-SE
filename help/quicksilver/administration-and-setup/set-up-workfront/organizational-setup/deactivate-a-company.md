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
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Inaktivera eller återaktivera ett företag

Du kan inaktivera ett företag som du inte längre använder samtidigt som alla tillhörande historiska data bevaras. Om du inaktiverar ett företag som redan används någonstans i systemet fortsätter det att fungera precis som vanligt. Den har inte tagits bort eller blockerats.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
  <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån [!UICONTROL System Administrator], som gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
     <li> <p>Administrativ åtkomst för att hantera företag, vilket gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
    </ul> <p><b>OBS</b>:  
     <ul> 
      <li> <p>Du kan också hantera företag som är kopplade till en grupp där du har tilldelats som gruppadministratör.</p> </li> 
      <li> <p>Om du vill lägga till och ta bort användare från systemet [!DNL Workfront] måste du ha något av följande:</p> 
       <ul> 
        <li> <p>Åtkomstnivån [!UICONTROL System Administrator]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> inställningen i din åtkomstnivå konfigurerad till <b>[!UICONTROL Edit]</b> åtkomst, med <b>[!UICONTROL Create]</b> och minst ett av de två <b>[!UICONTROL User Admin]</b> alternativen aktiverade under <b>[!UICONTROL Fine-tune your settings]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Om <b>[!UICONTROL User Admin (Group Users)]</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

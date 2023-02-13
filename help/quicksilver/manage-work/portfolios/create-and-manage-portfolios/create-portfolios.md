---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Skapa en portfölj
description: Ett Portfolio är en samling projekt som konkurrerar om samma resurser, budget och tidsplan. Projekten i Portfolio är tillräckligt lika så att de skulle använda samma resurspool och mätas mot samma styrkort.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Skapa en portfölj

Ett Portfolio är en samling projekt som konkurrerar om samma resurser, budget och tidsplan. Projekten i Portfolio är tillräckligt lika så att de skulle använda samma resurspool och mätas mot samma styrkort.

Du kan använda Portfolio för att gruppera projekt som tillhör samma produktlinjer, avdelningar, avdelningar, företag eller andra affärsenheter.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Business] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL Edit] behörighet till Portfolio</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>När du har skapat en portfölj har du som standard behörighet att hantera den</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Skapa en portfölj

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **[!UICONTROL Portfolios]**.
1. Klicka på **[!UICONTROL New Portfolio]**.
1. Ersätt **[!UICONTROL Untitled Portfolio]** med det namn du vill ha för portföljen.

   Namnet kan innehålla upp till 255 tecken.

1. (Valfritt) Klicka på namnet under **[!UICONTROL Portfolio Manager]** i sidhuvudet högst upp på sidan om du vill tilldela en annan portföljförvaltare.

   ![](assets/portfolio-manager-name-350x51.jpg)

   Som skapare av portföljen tilldelas du som standard som portföljförvaltare.

1. Klicka **[!UICONTROL Portfolio Details]** i den vänstra panelen.
1. I **[!UICONTROL Overview]** kan du ändra följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Skriv en beskrivning av Portfolio för att ange vad som är unikt med det. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Börja skriva namnet på en användare som du vill ange som portföljförvaltare och markera den sedan när den visas i listan. Detta är samma sak som [!UICONTROL Portfolio Owner]. Detta är den person som kan övervaka arbetet som definieras i portföljens projekt och godkänna affärsärendet.</p> <p>Viktigt: När du anger någon som [!UICONTROL Portfolio Manager]får de automatiskt [!UICONTROL Manage] behörigheter till portföljen, programmen och projekten i portföljen. </p> <p>Tips: Du kan även uppdatera [!UICONTROL Portfolio Manager] i sidhuvudet högst upp på sidan.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Grupp </td> 
      <td> <p>Lägg till namnet på en enskild grupp om gruppen äger portföljen eller har ansvar för att slutföra den. </p> <p>Du kan se till att du väljer rätt grupp genom att hålla markören över den och klicka på [!UICONTROL information] icon <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Klicka inuti **[!UICONTROL Add custom form]** i det övre högra hörnet av [!UICONTROL Portfolio Details] sida för att välja ett anpassat formulär för portföljen och uppdatera anpassade fält.

   >[!TIP]
   >
   >Du måste ha egna portföljformulär som redan har skapats innan du kan bifoga dem till portföljer.

1. Klicka på **[!UICONTROL Save Changes]**.
1. (Valfritt) Klicka på **[!UICONTROL Programs]** i den vänstra panelen och **[!UICONTROL Add Programs]** för att lägga till program i portföljen.

   Mer information om hur du skapar program finns i [Skapa ett program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Valfritt) Klicka på **[!UICONTROL Projects]** i den vänstra panelen och **[!UICONTROL Add Projects]** för att lägga till projekt i portföljen.

   Mer information om hur du lägger till projekt på en Portfolio finns i [Lägga till projekt i en portfölj](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->

---
product-area: programs
navigation-topic: create and manage programs
title: Skapa ett program
description: Ett program representerar en samling projekt som delar en gemensam strategi, mål eller mål som överskrider projektgränserna. Program får inte finnas utanför en portfölj.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# Skapa ett program

Ett program representerar en samling projekt som delar en gemensam strategi, mål eller mål som överskrider projektgränserna. Program får inte finnas utanför en portfölj.

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
   <td> <p>[!UICONTROL Edit] tillgång till Portfolio och program </p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen</p> <p>När du har skapat ett program har du [!UICONTROL Manage] behörighet till den som standard</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Skapa ett program

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Gör något av följande.

   * Skapa ett program från [!UICONTROL Programs] område:

      1. Klicka **[!UICONTROL Programs]** på huvudmenyn.
      1. Klicka på **[!UICONTROL New Program]**.
      1. I rutan som visas skriver du namnet på en befintlig Portfolio i **[!UICONTROL Select Portfolio]** fält.
      1. Skriv namnet på det nya programmet i **[!UICONTROL Name]** fält.
      1. Klicka på **[!UICONTROL Save]**.
   * Skapa ett program från [!UICONTROL Portfolios] område:

      1. Klicka **[!UICONTROL Portfolios]** i [!UICONTROL Main Menu]och klickar sedan på en portfölj.
      1. Klicka på i den vänstra panelen **[!UICONTROL Programs]**.
      1. Klicka på **[!UICONTROL New Program]** nedrullningsbar meny, och **[!UICONTROL New Program]**.


1. Ange namnet på programmet i **[!UICONTROL Untitled Program]** fält.

   Namnet kan innehålla upp till 255 tecken.

1. (Valfritt) Klicka på **[!UICONTROL Program Manager]** i programmets huvud för att uppdatera det.

   >[!TIP]
   >
   >Som skapare av programmet anges du som programhanterare som standard.

1. Klicka **[!UICONTROL Program Details]** i den vänstra panelen.
1. Dubbelklicka på ett fält för att uppdatera informationen i **[!UICONTROL Overview]** område.
1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Fält</th> 
      <th>Beskrivning</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Ange en beskrivning för programmet.</p> <p>Beskrivningen visas på programmets landningssida.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>Börja skriva namnet på den användare som du vill ska fungera som programhanterare och klicka sedan på användarens namn när det visas i listrutan. Detta är samma sak som [!UICONTROL Program Owner]. </p> <p>Tips: Du kan även uppdatera Program Manager i programhuvudet. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Group] </td> 
      <td> <p>Lägg till namnet på en enskild grupp om gruppen äger programmet eller har ansvar för att slutföra det. </p> <p>Du kan se till att du väljer rätt grupp genom att hålla markören över den och klicka på [!UICONTROL information] icon <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt och villkorligt) Klicka inuti **[!UICONTROL Add custom form]** för att välja ett anpassat formulär för portföljen och uppdatera de anpassade fälten.

   >[!TIP]
   >
   >Du måste ha skapat anpassade programformulär innan du kan koppla dem till program.

1. (Valfritt) Dubbelklicka på ett fält för att uppdatera information i det anpassade formuläret.
1. Klicka **[!UICONTROL Projects]** i den vänstra panelen och **[!UICONTROL Add Projects]** för att lägga till projekt i programmet.

   Mer information om hur du lägger till projekt i program finns i [Lägga till ett projekt i ett program](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Klicka på **[!UICONTROL Save Changes]**.
1. (Valfritt) Klicka på **[!UICONTROL More menu]** ![](assets/more-icon.png) bredvid programnamnet och klicka på **[!UICONTROL Deactivate Program]**.

   När du inaktiverar ett program visas det inte längre i en lista över program när användare försöker lägga till det i ett projekt. Du kan fortfarande komma åt programmet från [!UICONTROL Programs] område.

## Översikt över programrubriken

Du hittar begränsad information om programmet i rubriken.

Följande information visas i programmets huvud:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Huvudinformation</td> 
   <td> <p><strong>Anteckningar</strong> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bredcrumb med namnet på portföljen</td> 
   <td>Du kan komma åt den portfölj som programmet tillhör från programmets huvud. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programmets namn</td> 
   <td>Du kan redigera programnamnet i sidhuvudet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Namn på objekttyp och aktiveringsstatus</td> 
   <td>Ordet "Program" visas i en grön ram när du visar ett program. Ordet "[!UICONTROL Deactivated]" visas bredvid den och dispositionen är grå om programmet inte är markerat som [!UICONTROL Active]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programmets verksamhetsområde </td> 
   <td> <p>Klicka på något av följande om du vill ha mer information eller redigeringsalternativ för programmet:</p> 
    <ul> 
     <li>Stjärnikonen som lägger till programmet i din favoritlista</li> 
     <li> <p>The [!UICONTROL More] meny <img src="assets/qs-more-menu.png"> om du vill göra något av följande: </p> 
      <ul> 
       <li>Redigera programmet</li> 
       <li>Inaktivera den. När ett program inaktiveras kan du inte längre koppla det till projekt på projektnivå. </li> 
       <li> <p>Ta bort den. När du tar bort programmet tas inte projekten i programmet bort. Det tar bort kopplingen mellan projekten och programmet. </p> </li> 
       <li>Dela det med andra</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>Du kan inte redigera [!UICONTROL Percent Complete] för programmet i sidhuvudet. Den här informationen uppdateras från projekten i programmet. Som standard är procentandelen slutförd av programmet ett genomsnitt av procentvärdena för slutförda projekt i en [!UICONTROL Current] och [!UICONTROL Approved] status som tillhör programmet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>Du kan redigera Program Manager i sidhuvudet. Detta är samma sak som [!UICONTROL Program Owner]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date]</td> 
   <td>Du kan inte redigera procentandelen färdig av programmet i sidhuvudet. Procent färdigt av programmet är ett genomsnitt av andelen slutförda projekt i sidhuvudet. De projekt som visas här är projekt med statusen [!UICONTROL Current] och [!UICONTROL Approved]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Active Projects Condition]</td> 
   <td>Detta är en beräkning av hur stor procentandel av projekten i programmet som har [!UICONTROL Condition] ange som [!UICONTROL On Target], [!UICONTROL At Risk], eller [!UICONTROL In Trouble]. De projekt som visas här är projekt med statusen [!UICONTROL Current] och [!UICONTROL Approved]. </td> 
  </tr> 
 </tbody> 
</table>

## Flytta ett program

Du kan lägga till befintliga program i en portfölj. Eftersom program inte kan finnas i två olika portföljer flyttas det om du lägger till ett befintligt program permanent från en portfölj till en annan.

Mer information finns i [Lägg till ett befintligt program i en portfölj](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).

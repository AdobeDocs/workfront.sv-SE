---
product-area: programs
navigation-topic: create and manage programs
title: Skapa ett program
description: Ett program representerar en samling projekt som delar en gemensam strategi, mål eller mål som överskrider projektgränserna. Program får inte finnas utanför en portfölj.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: e4cd543aa9f47e6b93aa148ea3fb972fbd356c02
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Skapa ett program

<!-- Audited: 1/2024 -->

Ett program representerar en samling projekt som delar en gemensam strategi, mål eller mål som överskrider projektgränserna. Program får inte finnas utanför en portfölj.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Nytt: Alla</p><p>eller</p><p>Aktuell: [!UICONTROL Business] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>Nytt: [!UICONTROL Standard] </p><p>eller </p><p>Aktuell: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL Edit] tillgång till Portfolio och program </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen</p> <p>När du har skapat ett program har du [!UICONTROL Manage] behörighet till den som standard.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Skapa ett program

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) längst upp till vänster.

1. Gör något av följande.

   * Skapa ett program från [!UICONTROL Programs] område:

      1. Klicka **[!UICONTROL Programs]** på huvudmenyn.
      1. Klicka på **[!UICONTROL New Program]**.
      1. Skriv namnet på en befintlig Portfolio i rutan som visas **[!UICONTROL Select Portfolio]** fält.
      1. Skriv namnet på det nya programmet i **[!UICONTROL Name]** fält.
      1. Klicka på **[!UICONTROL Save]**.
   * Skapa ett program från [!UICONTROL Portfolios] område:

      1. Klicka **[!UICONTROL Portfolios]** i [!UICONTROL Main Menu]öppnar du sedan en portfölj.
      1. Klicka på i den vänstra panelen **[!UICONTROL Programs]**.
      1. Klicka på **[!UICONTROL New Program]** nedrullningsbar meny, och **[!UICONTROL New Program]**.


1. (Villkorligt) Om du har skapat programmet från en portfölj anger du namnet på programmet i **[!UICONTROL Untitled Program]** fält.

   Namnet kan innehålla upp till 255 tecken.

1. (Valfritt) Klicka på **[!UICONTROL Program Manager]** i programmets huvud för att uppdatera det.

   >[!TIP]
   >
   >Som skapare av programmet anges du som programhanterare som standard.

1. Klicka **[!UICONTROL Program Details]** till vänster.
1. Dubbelklicka på ett fält för att uppdatera informationen i **[!UICONTROL Overview]** område.

Du kan ange följande information:

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
      <td> <p>Börja skriva namnet på den användare som du vill ska fungera som programhanterare och klicka sedan på användarens namn när det visas i listrutan. Detta är samma sak som [!UICONTROL Program Owner]. </p> <p>Tips! Du kan även uppdatera programhanteraren i programhuvudet. </p> </td> 
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

1. (Valfritt och villkorligt) Om du lägger till ett anpassat formulär kan du uppdatera informationen i det fältet genom att klicka på ett fält i det anpassade formuläret.
1. Klicka på **[!UICONTROL Save Changes]**.
1. Klicka **[!UICONTROL Projects]** i den vänstra panelen och sedan **[!UICONTROL Add Projects]** för att lägga till projekt i programmet.

   Mer information om hur du lägger till projekt i program finns i [Lägga till ett projekt i ett program](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Klicka på **[!UICONTROL Save Changes]**.
1. (Valfritt) Klicka på **[!UICONTROL More menu]** ![](assets/more-icon.png) bredvid programnamnet och klicka på **[!UICONTROL Deactivate Program]**.

   När du inaktiverar ett program visas det inte längre i en lista över program när användare försöker lägga till det i ett projekt. Du kan fortfarande komma åt programmet från [!UICONTROL Programs] område.

## Översikt över programrubriken

Du hittar viss information om programmet i rubriken.

Följande information visas i programmets huvud:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Rubrikinformation</td> 
   <td> <strong>Anteckningar</strong> </td> 
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
   <td>Ordet "Program" visas med en orange ikon när du visar ett program. Ordet "[!UICONTROL Deactivated]" visas bredvid den och dispositionen är grå om programmet inte är markerat som [!UICONTROL Active]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programmets verksamhetsområde </td> 
   <td> <p>Klicka på något av följande om du vill ha mer information eller redigeringsalternativ för programmet:</p> 
    <ul> 
     <li>Stjärnikonen som lägger till programmet i din lista över favoriter</li> 
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
   <td> <p>Du kan inte redigera [!UICONTROL Percent Complete] för programmet i sidhuvudet. Den här informationen uppdateras från projekten i programmet. Som standard är procentandelen slutförd av programmet ett genomsnitt av procentvärdena för slutförda projekt i en [!UICONTROL Current] eller [!UICONTROL Approved] status som tillhör programmet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>Du kan redigera Program Manager i sidhuvudet. Detta är samma sak som [!UICONTROL Program Owner]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date]</td> 
   <td>Du kan inte redigera programmets planerade slutförandedatum i rubriken.  </td> 
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

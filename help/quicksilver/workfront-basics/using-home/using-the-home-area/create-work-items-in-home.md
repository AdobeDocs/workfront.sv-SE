---
product-area: projects
navigation-topic: use-the-home-area
title: Skapa arbetsobjekt från hemområdet
description: Skapa arbetsobjekt från hemområdet
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# Skapa arbetsobjekt från hemområdet

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

Du kan skapa arbetsobjekt från [!UICONTROL Home] område. Du kan skapa personliga uppgifter för dig själv, begära arbete från andra användare eller lägga till uppgifter i specifika projekt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Edit] behörighet eller högre för uppgifter</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Skapa en personlig uppgift

Du kan skapa en personlig uppgift som bara är tillgänglig för dig i [!UICONTROL Home] område:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL New Task]** > **[!UICONTROL Personal]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. I **[!UICONTROL Name]** anger du ett namn för uppgiften.
1. (Valfritt) Klicka på **[!UICONTROL Select date]** väljer du sedan datumet då uppgiften förfaller. Detta anger [!UICONTROL Planned Completion Date] för uppgiften.\
   Du kan ändra **[!UICONTROL Planned Completion Date]** genom att klicka på datumet i den högra panelen eller redigera **[!UICONTROL This will be done by]** datum direkt i uppgiften.

1. Klicka **[!UICONTROL Create]** för att spara uppgiften.\
   Uppgiften är tilldelad dig och tillgänglig i [!UICONTROL Home] område.

>[!NOTE]
>
>* När du skapar en personlig uppgift lagras den i ett&quot;dolt&quot; projekt som inte är sökbart i [!UICONTROL Workfront]. Projektet heter &quot;&lt; Användarnamn > Uppgifter&quot;. &quot;Användarnamn&quot; är det fullständiga namnet på den användare som skapade uppgiften. Du kan bara komma åt det här projektet när du klickar på den personliga uppgiften i [!UICONTROL Home] -området, till exempel från uppgiftens vägbeskrivningar.
>
>* Till skillnad från vanliga projektuppgifter har personliga uppgifter en begränsad uppsättning fält som visas i Workfront-gränssnittet och påverkar inte tidslinjen eller förloppet för något projekt. Om du tilldelar en personlig uppgift till en annan användare, läggs alla uppgiftsfält till i en personlig uppgift, men uppgiften blir kvar i det personliga projektet för den användare som skapade uppgiften.
>
>* Vi rekommenderar att du skapar ett projekt och flyttar alla personliga uppgifter till det om du vill göra personliga uppgifter till en del av det vanliga arbetsflödet.
>
> ![[!UICONTROL Project for personal tasks]](assets/createworkitems-personal--project-350x105.png)

## Begär arbete från en annan användare

Du kan begära arbete från en annan användare direkt från hemområdet. När du begär arbete från en annan användare enligt beskrivningen i det här avsnittet, visas uppgiften som en begäran i användarens hemsida tills användaren klickar **[!UICONTROL Work On It]**.

Om du vill begära arbete från en annan användare från [!UICONTROL Home] område:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka **[!UICONTROL New Task]** väljer **[!UICONTROL Request]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. I **[!UICONTROL Name]** anger du ett namn för uppgiften.
1. I **[!UICONTROL Assign to]** börjar du skriva namnet på den användare, det team eller den roll som du vill tilldela och klickar sedan på namnet i listrutan.
1. I [!UICONTROL Add As] väljer du om du vill lägga till en uppgift eller ett problem.
1. Klicka **[!UICONTROL Select date]** väljer du sedan datum och tid då uppgiften förfaller.
1. Klicka **[!UICONTROL Create]** för att spara uppgiften.\
   Uppgiften visas som en arbetsförfrågan i [!UICONTROL Home] området för den användare som du har angett.

## Lägga till en aktivitet eller ett problem i ett projekt

Du kan lägga till en uppgift eller ett problem i ett befintligt projekt direkt från Hem-området:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Startsida**.
1. Klicka **[!UICONTROL New Task]** väljer **[!UICONTROL Project Task]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. I **[!UICONTROL Name]** anger du ett namn för uppgiften eller problemet.
1. I **[!UICONTROL Assign to]** börjar du skriva namnet på den användare, det team eller den roll som du vill tilldela och klickar sedan på namnet i listrutan.
1. Börja skriva namnet på det projekt där du vill skapa uppgiften eller problemet och klicka sedan på namnet när det visas i listrutan.

   >[!IMPORTANT]
   >
   >Uppgiften eller problemet visas på [!UICONTROL Work List] endast när projektet [!UICONTROL Status] är inställd på [!UICONTROL Current].

1. (Villkorligt) Om du vill skapa ett problem väljer du **[!UICONTROL Issue]** från **[!UICONTROL Add As]** nedrullningsbar meny. Som standard **[!UICONTROL Task]** är markerat.

1. Klicka **[!UICONTROL Select date]** väljer du sedan datum och tid då uppgiften förfaller.
1. Klicka **[!UICONTROL Create]** för att spara uppgiften.

---
product-area: projects
navigation-topic: use-the-home-area
title: Skapa arbetsobjekt från startdelen
description: Du kan skapa arbetsobjekt från området [!UICONTROL Home]. Du kan skapa personliga uppgifter för dig själv, begära arbete från andra användare eller lägga till uppgifter i specifika projekt.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 0%

---

# Skapa arbetsobjekt från startdelen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

Du kan skapa arbetsobjekt från området [!UICONTROL Home]. Du kan skapa personliga uppgifter för dig själv, begära arbete från andra användare eller lägga till uppgifter i specifika projekt.

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
   <td> <p>[!UICONTROL Worker]</p> <p><b>ANMÄRKNING</b></p> 
   <p>Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Edit] behörighet eller högre för uppgifter</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Skapa en personlig uppgift

Du kan skapa en personlig uppgift som bara är tillgänglig för dig i området [!UICONTROL Home]:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL New Task]** > **[!UICONTROL Personal]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. Ange ett namn för aktiviteten i fältet **[!UICONTROL Name]**.
1. (Valfritt) Klicka på **[!UICONTROL Select date]** och välj sedan det datum då uppgiften förfaller. Detta anger [!UICONTROL Planned Completion Date] för aktiviteten.\
   Du kan ändra **[!UICONTROL Planned Completion Date]** genom att klicka på datumet i den högra panelen eller redigera **[!UICONTROL This will be done by]**-datumet direkt i uppgiften.

1. Klicka på **[!UICONTROL Create]** för att spara uppgiften.\
   Uppgiften har tilldelats dig och är tillgänglig i området [!UICONTROL Home].

>[!NOTE]
>
>* När du skapar en personlig uppgift lagras den i ett dolt projekt som inte är sökbart i [!UICONTROL Workfront]. Projektet heter &quot;&lt; Användarnamn > Uppgifter&quot;. &quot;Användarnamn&quot; är det fullständiga namnet på den användare som skapade uppgiften. Du kan bara komma åt det här projektet om du klickar på den personliga uppgiften i området [!UICONTROL Home], till exempel från uppgiftens vägbeskrivningar.
>
>* Till skillnad från vanliga projektuppgifter har personliga uppgifter en begränsad uppsättning fält som visas i Workfront-gränssnittet och påverkar inte tidslinjen eller förloppet för något projekt. Om du tilldelar en personlig uppgift till en annan användare, läggs alla uppgiftsfält till i en personlig uppgift, men uppgiften blir kvar i det personliga projektet för den användare som skapade uppgiften.
>
>
>* Personliga uppgifter visas bara på tidrapporter när de har loggat timmar eller när de är fästa på tidrapporten. Du kan bara fästa en personlig uppgift på en tidrapport när det finns timmar loggade för uppgiften. Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).
> 
>* Vi rekommenderar att du skapar ett projekt och flyttar alla personliga uppgifter till det om du vill göra personliga uppgifter till en del av det vanliga arbetsflödet.
>
> ![[!UICONTROL Project for personal tasks]](assets/createworkitems-personal--project-350x105.png)

## Begär arbete från en annan användare

Du kan begära arbete från en annan användare direkt från hemområdet. När du begär arbete från en annan användare enligt beskrivningen i det här avsnittet, visas uppgiften som en begäran i användarens hemområde tills användaren klickar på **[!UICONTROL Work On It]**.

Så här begär du arbete från en annan användare från området [!UICONTROL Home]:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL New Task]** och välj sedan **[!UICONTROL Request]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. Ange ett namn för aktiviteten i fältet **[!UICONTROL Name]**.
1. I fältet **[!UICONTROL Assign to]** börjar du skriva namnet på den användare, det team eller den roll som du vill tilldela och klickar sedan på namnet när det visas i listrutan.
1. I listrutan [!UICONTROL Add As] väljer du om du vill lägga till en uppgift eller ett problem.
1. Klicka på **[!UICONTROL Select date]** och välj sedan datum och tid när uppgiften förfaller.
1. Klicka på **[!UICONTROL Create]** för att spara uppgiften.\
   Uppgiften visas som en arbetsförfrågan i området [!UICONTROL Home] för den användare du har angett.

## Lägga till en aktivitet eller ett problem i ett projekt

Du kan lägga till en uppgift eller ett problem i ett befintligt projekt direkt från Hem-området:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Hem**.
1. Klicka på **[!UICONTROL New Task]** och välj sedan **[!UICONTROL Project Task]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. I fältet **[!UICONTROL Name]** anger du ett namn för aktiviteten eller problemet.
1. I fältet **[!UICONTROL Assign to]** börjar du skriva namnet på den användare, det team eller den roll som du vill tilldela och klickar sedan på namnet när det visas i listrutan.
1. Börja skriva namnet på det projekt där du vill skapa uppgiften eller problemet och klicka sedan på namnet när det visas i listrutan.

   >[!IMPORTANT]
   >
   >Aktiviteten eller problemet visas bara på [!UICONTROL Work List] när projektet [!UICONTROL Status] är inställt på [!UICONTROL Current].

1. (Villkorligt) Om du vill skapa ett problem väljer du **[!UICONTROL Issue]** i listrutan **[!UICONTROL Add As]**. Som standard är **[!UICONTROL Task]** markerat.

1. Klicka på **[!UICONTROL Select date]** och välj sedan datum och tid när uppgiften förfaller.
1. Klicka på **[!UICONTROL Create]** för att spara uppgiften.

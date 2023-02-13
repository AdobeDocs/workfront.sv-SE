---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Hantera arbets- och teamförfrågningar på Hem-området
description: När arbetsuppgifter och ärenden tilldelas dig visas de på [!UICONTROL Work List] i [!UICONTROL Home] område. Du kan visa, omtilldela, svara på, arbeta med eller ta bort en begäran. Arbetsförfrågningar i [!UICONTROL Home] området är inte begränsat till problem som är kopplade till frågeköer.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Hantera arbets- och teamförfrågningar i [!UICONTROL Home] area

När arbetsuppgifter och ärenden tilldelas dig visas de på [!UICONTROL Work List] i [!UICONTROL Home] område. Du kan visa, omtilldela, svara på, arbeta med eller ta bort en begäran. Arbetsförfrågningar i [!UICONTROL Home] området är inte begränsat till problem som är kopplade till frågeköer.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[!UICONTROL Edit] tillgång till uppgifter och ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Contribute-behörigheter eller högre för de uppgifter och ärenden du behöver arbeta med</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Visa en arbetsförfrågan

Arbetsförfrågningar som har tilldelats dig visas i den vänstra panelen i [!UICONTROL Home]. Du kan konfigurera vilka begäranden som ska visas i [!UICONTROL Home] med filtret längst upp på [!UICONTROL Work List].

Du kan välja filter som visar objekt som du kan arbeta med, eller objekt som du redan arbetar med.

I den här artikeln beskrivs hur du använder filtren i [!UICONTROL Home] för att visa objekt som du för närvarande arbetar med eller kan överväga att börja arbeta med. Mer information om alla filter i [!UICONTROL Home] område, se [Visa objekt i arbetslistan i [!UICONTROL Home] area](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL Filter]** nedrullningsbar meny.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Klicka på något eller båda av följande alternativ för uppgifter:

   **[!UICONTROL Ready to Start]:** Visar endast aktiviteter och ärenden som är klara att starta. Båda följande programsatser måste vara sanna:

   * Aktiviteterna och deras föräldrar har inga föregående aktiviteter eller uppgiftsbegränsningar som hindrar dem från att arbeta.
   * The [!UICONTROL Planned Start Date] av uppgifterna eller problemen har inträffat tidigare eller upp till två veckor i framtiden.

   **[!UICONTROL Not Ready]**: Visar endast aktiviteter och problem som inte är klara att starta än. Någon av följande programsatser måste vara true:

   * Aktiviteterna och deras överordnade kan ha föregångare eller uppgiftsbegränsningar som förhindrar att de bearbetas.
   * Aktiviteter och problem har en [!UICONTROL Planned Start Date] det är mer än två veckor i framtiden.



1. Klicka **[!UICONTROL Working On]** under [!UICONTROL Tasks] eller [!UICONTROL Issues] för att visa uppgifter och problem som du arbetar med just nu.
1. Klicka **[!UICONTROL Requested]** under [!UICONTROL Issues] för att visa problem som har begärts från dig (du har tilldelats dem), men som du ännu inte har godkänt för arbete.

## Åtkomst till en teamförfrågan

Du kan komma åt en förfrågan som tilldelats ditt team direkt från [!UICONTROL Home] område. Mer information om gruppförfrågningar finns i [Översikt över gruppförfrågningar](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. I **[!UICONTROL Work List]** området, klicka för att expandera **[!UICONTROL Team Requests]** gruppering.

   Om inga begäranden har tilldelats ditt team visas inte grupperingen.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Klicka på teamnamnet.\
   The **[!UICONTROL Team Requests]** visas och visas alla förfrågningar som har tilldelats ditt team. Mer information om hur du arbetar med gruppförfrågningar finns i [Hantera arbets- och teamförfrågningar](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Tilldela om en begäran

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. I **[!UICONTROL Work List]** markerar du den begäran som du vill tilldela om.

1. Klicka på **[!UICONTROL Assignments]** och ta bort dig själv från begäran. Skriv sedan namnet på den användare som du vill tilldela om begäran till.

   >[!TIP]
   >
   >Om arbetsbegäran fortfarande är i tillståndet Ready to Start eller Not Ready (Klart) kan du använda **[!UICONTROL Reassign]** i **[!UICONTROL More]** i [!UICONTROL Work List].\
   >![Knappen Tilldela igen](assets/reassign-in-left-panel-350x204.png)

1. Om en uppgifts status ändras till [!UICONTROL New] eller [!UICONTROL In Progress] När uppgiften är klar måste du ta bort användartilldelningen, spara uppgiften och sedan tilldela användaren på nytt för att uppgiften ska visas igen i hemarbetslista.

## Svara på en förfrågan

Du kan svara på en begäran om att ytterligare klargöra begäran eller föreslå ett nytt datum.

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. I **[!UICONTROL Work List]** markerar du den förfrågan du vill svara på.
1. Leta reda på den person som tilldelade begäran till dig.

   Den här informationen finns på [!UICONTROL Updates] aktivitetens flik. Se till att alternativet **[!UICONTROL Show System Updates]** är aktiverat.

1. Klicka **[!UICONTROL Start new update]** och börja skriva ditt svar.
1. Ange namnet på mottagaren i dialogrutan **[!UICONTROL Notify]** och klicka sedan på **[!UICONTROL Update]**.

   >[!TIP]
   >
   >Om arbetsbegäran fortfarande finns i Klar att starta eller [!UICONTROL Not Ready] kan du använda **[!UICONTROL Reply]** i **[!UICONTROL More]** i [!UICONTROL Work List].\
   >![[!UICONTROL Reply button]](assets/reassign-in-left-panel-350x204.png)   >

## Arbeta med en begäran

När du klickar på [!UICONTROL Work On It] anger du för den användare som skickade begäran och för alla andra användare som kan ha tilldelats begäran att du ska börja arbeta med begäran. Mer information om hur du arbetar med begäranden finns i  [Hantera arbets- och teamförfrågningar](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. I **[!UICONTROL Work List]** markerar du den förfrågan du vill arbeta med och klickar sedan på **[!UICONTROL Work On It]**.\
   Information om problemet visas på den högra panelen.

## Ta bort en begäran

Om du beslutar att du inte ska arbeta med begäran kan du antingen konvertera uppgiften eller utgåvan till en begäran eller ta bort den från listan.

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. I **[!UICONTROL Work List]**, peka på objektet som väntar på att bearbetas.
1. Klicka på **[!UICONTROL Assignments]** och ta bort dig själv. Detta tar bort arbetsobjektet från din arbetslista. Om begäran inte är tilldelad någon annan, eller någon annan team eller jobbroll, lämnas begäran utan tilldelning.

   eller

   Klicka på **[!UICONTROL More]** menyikon ![](assets/more-icon.png) till höger om uppgifts- eller utgivarens namn i [!UICONTROL Home Work] Lista.

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Välj bland följande alternativ:

   * **[!UICONTROL Convert to work request]:** Välj det här alternativet om du vill konvertera arbetsuppgiften tillbaka till en arbetsförfrågan.\

      Arbetsuppgiften överförs tillbaka till en begäran och du förblir tilldelad till begäran.\
      Du kan godkänna begäran vid ett senare tillfälle genom att klicka på **[!UICONTROL Work on It]** igen.

   * **[!UICONTROL Remove]:** Välj det här alternativet om du vill ta bort en begäran från [!UICONTROL Work List].\

      Du har inte tilldelats från din begäran och din begäran är inte längre kopplad till ditt namn i [!DNL Adobe Workfront].\
      Om begäran inte är tilldelad någon annan, eller någon annan team eller jobbroll, lämnas begäran utan tilldelning.

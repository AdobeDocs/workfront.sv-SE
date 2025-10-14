---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Konfigurera ledig tid
description: Det är viktigt att ange i Adobe Workfront när en godkänd tid är ledig, eftersom detta påverkar ditt schema och påverkar de planerade datumen för slutförande av de uppgifter du har tilldelats.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: f10b0a4897d6250f0c4decf1fad069c598536a38
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Konfigurera ledig tid

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

[!DNL Adobe Workfront] är inte utformat för att replikera eller ersätta dina befintliga system för hantering, upplupning och spårning av ledig tid.

Det är dock viktigt att ange när en godkänd tid är ledig, eftersom detta påverkar både ditt schema och [!UICONTROL Planned Completion Dates] för de uppgifter du är tilldelad.

Om du till exempel har tilldelats en aktivitet som är schemalagd att ta två veckor och du planerar att ta tre dagar ledigt under den tiden, lägger [!DNL Workfront] till tre dagar i tidslinjen för aktiviteten för att ta hänsyn till den lediga tiden.

Resurshanteringsverktygen använder också din personliga ledig tid för att ange när du är tillgänglig för schemalagt arbete.

>[!NOTE]
>
>För att säkerställa att inga inkonsekvenser inträffar med de datum som du anger din ledig tid för rekommenderar vi att användarprofilens tidszon matchar den som du har schemalagt. Mer information finns i följande artiklar:
>
>* [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: Standard (för att konfigurera din personliga tid till ledig)</p>
        <p>eller</p>
        <p>Aktuell: Arbeta eller högre (för att konfigurera din personliga tid till ledig)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL Manager] med [!UICONTROL Edit User] åtkomst (för att ändra tid för andra användares kalender)<br>
   <strong>Obs!</strong> Om en hanterare redigerar en annan användares personliga tid i kalendern visas alla poster i användarens tidszon och inte i hanterarens tidszon.</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Konfigurera personlig tid av i [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Om du använder Adobe Unified Experience kan du komma åt din Workfront-profil genom att klicka på Adobe-kontomenyn (din profilbild) i det övre navigeringsområdet och sedan välja Workfront-profil.
>
>![arbetsprofil](assets/aue-profile.png)

1. Klicka på **[!UICONTROL Time Off]** i den vänstra panelen.
1. Välj önskat datum för din personliga ledig tid.

   <!--<span class="preview">Sample image in the Preview environment:</span>
   ![Personal time off calendar](assets/personal-time-off-calendar-0925.png)-->

   <!--Sample image in the Production environment:-->
   ![Personlig tid för kalendern](assets/personal-time-off-calendar.png)

1. Välj **[!UICONTROL All day]** om du vill ta en hel dag ledigt.

   Låt kryssrutan vara avmarkerad om du tar mindre än en hel dag bort och ange start- och sluttider för din tid.

1. Klicka på **[!UICONTROL Save]**.

   Din lediga tid är nu synlig i hela [!DNL Workfront]-systemet i resurshanteringsverktyg som Resursplanering och Arbetsbelastningsutjämning. När du har tilldelats arbete under den här tiden får användaren ett verktygstips om att du har schemalagt en ledig tid.

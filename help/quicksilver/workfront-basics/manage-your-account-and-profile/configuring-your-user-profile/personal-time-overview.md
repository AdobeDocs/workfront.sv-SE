---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Konfigurera personlig timeout i [!DNL Adobe Workfront]
description: Adobe Workfront är inte utformat för att replikera eller ersätta dina befintliga system för hantering, upplupning och spårning av ledig tid. Det är dock viktigt att ange när en godkänd tid är ledig, eftersom detta påverkar schemat och påverkar de planerade slutförandedatumen för de uppgifter du har tilldelats.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 91eb8770c07396b5772029e9d2370f0b1f10d4a1
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Konfigurera personlig timeout i [!DNL Adobe Workfront]

[!DNL Adobe Workfront] är inte utformat för att replikera eller ersätta dina befintliga system för att hantera, periodisera och spåra ledig tid.

Det är dock viktigt att ange när en godkänd tid är borta, eftersom detta påverkar ditt schema och påverkar [!UICONTROL Planned Completion Dates] av de uppgifter du har tilldelats.

Om du till exempel har tilldelats en aktivitet som är schemalagd att ta två veckor och du planerar att ta tre dagar ledigt under den tiden, [!DNL Workfront] lägger till tre dagar i aktivitetstidslinjen för att ta hänsyn till ledigt.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td>[!UICONTROL Work] eller högre (för att konfigurera din personliga tid av)</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td>[!UICONTROL Manager] med [!UICONTROL Edit User] åtkomst (för att ändra tiden i kalendern för andra användare)<br>
   <strong>OBS!</strong> Om en chef redigerar en annan användares personliga tid i kalendern visas alla poster i användarens tidszon och inte i hanterarens tidszon.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Konfigurera personlig timeout i [!DNL Workfront]

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ditt användarnamn bredvid din profilbild. Eller (om det är tillgängligt) klicka på din profilbild i det övre navigeringsområdet och klicka sedan på **[!UICONTROL Workfront Profile]**.
1. Klicka på i den vänstra panelen **[!UICONTROL Time Off]**.
1. Välj önskat datum för din personliga ledig tid.

   ![Personlig tid i kalendern](assets/personal-time-off-calendar.png)

1. Välj **[!UICONTROL All day]**, om du tar en hel dag ledigt.

   Låt det vara omarkerat om du tar mindre än en hel dag ledigt och ange start- och sluttider för din tid.

1. Klicka på **[!UICONTROL Save]**.

   Din lediga tid syns nu tvärs över [!DNL Workfront] i resurshanteringsverktyg som Resursplanering och Arbetsbelastningsutjämnare. När du har tilldelats arbete under den här tiden visas ett verktygstips som informerar användaren om att du har schemalagt en ledig tid.

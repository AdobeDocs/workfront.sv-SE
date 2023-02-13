---
content-type: reference
navigation-topic: notifications
title: '''Meddelanden: Mål'
description: '''Meddelanden: Mål'
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Meddelanden: Mål

Du kan aktivera e-postmeddelanden för händelser som inträffar i [!DNL Adobe Workfront Goals] i din profil. En användare med [!UICONTROL Plan] licenser kan även aktivera dem för andra användare. Mer information finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

## Åtkomstkrav

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produkt</strong></td> 
   <td>[!DNL Workfront Goals] <p>Mer information om [!DNL Workfront Goals], se <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] behörighet till [!DNL Goals] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Den användare vars [!DNL Goals] Aviseringar uppdateras måste ha följande:

* En layoutmall som innehåller [!DNL Goals] området i [!UICONTROL Main Menu].
* Tillgång till nya [!DNL Adobe Workfront] upplevelse.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!DNL Goals] meddelanden i [!UICONTROL user profile] area

De meddelanden som visas i följande tabell varnar dig om händelser som inträffar i [!DNL Workfront Goals], till exempel någon som tilldelar dig ett mål, resultat eller en aktivitet eller någon som gör en uppdatering av ett mål, resultat eller en aktivitet som du äger. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>Snabbmeddelanden för [!DNL Goals] är inaktiverade som standard. Du kan inte aktivera eller inaktivera dagliga meddelanden och du får inte dagliga sammandrag via e-post för händelserna i den här kategorin. Du kan aktivera eller inaktivera enskilda snabbmeddelanden för [!DNL Goals] kategori.

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Meddelande</strong></td> 
   <td> <p><strong>Inkluderade fält</strong> </p> <p><strong>*Endast snabbmeddelanden</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon tilldelade mig ett resultat/en aktivitet</strong></td> 
   <td> <p>Namnet på den person som tilldelade resultatet eller aktiviteten till dig</p> <p>Målets period för resultatet eller aktiviteten</p> <p>Namnet på resultatet eller aktiviteten</p> <p>The <strong>[!UICONTROL Open in web app]</strong> knappen som öppnar [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon skapade ett nytt personligt mål för mig</strong> </td> 
   <td> <p>Namnet på den person som tilldelade målet</p> <p>Målets period</p> <p>Målets namn</p> <p>The <strong>[!UICONTROL Open in web app]</strong> knappen som öppnar [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon lämnade en kommentar om mitt mål</strong></td> 
   <td> <p>Namnet på personen som lämnade kommentaren</p> <p>Målets period </p> <p>Målets namn</p> <p>Texten i kommentaren</p> <p>The <strong>[!UICONTROL Open in web app]</strong> knappen som öppnar [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon gillade min kommentar på ett mål</strong></td> 
   <td> <p>Namnet på den person som gillade kommentaren</p> <p>Målets period </p> <p>Målets namn</p> <p>Texten i kommentaren </p> <p>The <strong>[!UICONTROL Open in web app]</strong> knappen som öppnar [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon gillade en uppdatering av mitt mål</strong></td> 
   <td> <p>Du får ett e-postmeddelande när någon gillar en kommentar som du har gjort på ett mål eller när du uppdaterar förloppet för dina resultat eller aktiviteter på målet. </p> <p>Namnet på den person som gillade uppdateringen</p> <p>Målets period </p> <p>Målets namn</p> <p>The <strong>[!UICONTROL Open in web app]</strong> knappen som öppnar [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->

---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: mål'
description: 'Meddelanden: mål'
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Meddelanden: Mål

Du kan aktivera e-postmeddelanden för händelser som inträffar i [!DNL Adobe Workfront Goals] i din profil. En användare med en [!UICONTROL Plan]-licens kan även aktivera dem för andra användare. Mer information finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

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
   <td>[!DNL Workfront Goals] <p>Mer information om [!DNL Workfront Goals] finns i <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] behörighet till [!DNL Goals] eller senare</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Användaren vars [!DNL Goals] meddelanden uppdateras måste ha följande:

* En layoutmall som innehåller området [!DNL Goals] i [!UICONTROL Main Menu].
* Åtkomst till den nya [!DNL Adobe Workfront]-upplevelsen.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!DNL Goals] meddelanden i området [!UICONTROL user profile]

Meddelandena i följande tabell varnar dig om händelser som inträffar i [!DNL Workfront Goals], t.ex. någon som tilldelar dig ett mål, resultat eller en aktivitet eller någon som gör en uppdatering av ett mål, resultat eller en aktivitet som du äger. Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>Snabbmeddelanden för [!DNL Goals] är inaktiverade som standard. Du kan inte aktivera eller inaktivera dagliga meddelanden och du får inte dagliga sammandrag via e-post för händelserna i den här kategorin. Du kan aktivera eller inaktivera enskilda snabbmeddelanden för kategorin [!DNL Goals].

Se även [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Meddelande</strong></td> 
   <td> <p><strong>Fält som ingår</strong> </p> <p><strong>*Endast snabbmeddelanden</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon tilldelade mig ett resultat/en aktivitet</strong></td> 
   <td> <p>Namnet på den person som tilldelade resultatet eller aktiviteten till dig</p> <p>Målets period för resultatet eller aktiviteten</p> <p>Namnet på resultatet eller aktiviteten</p> <p>Knappen <strong>[!UICONTROL Open in web app]</strong> som öppnar panelen [!UICONTROL Goal Details]</p> <p>Knappen <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon har skapat ett nytt personligt mål för mig</strong> </td> 
   <td> <p>Namnet på den person som tilldelade målet</p> <p>Målets period</p> <p>Målets namn</p> <p>Knappen <strong>[!UICONTROL Open in web app]</strong> som öppnar panelen [!UICONTROL Goal Details]</p> <p>Knappen <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon lämnade en kommentar om mitt mål</strong></td> 
   <td> <p>Namnet på personen som lämnade kommentaren</p> <p>Målets period </p> <p>Målets namn</p> <p>Texten i kommentaren</p> <p>Knappen <strong>[!UICONTROL Open in web app]</strong> som öppnar panelen [!UICONTROL Goal Details]</p> <p>Knappen <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon gillade min kommentar på ett mål</strong></td> 
   <td> <p>Namnet på den person som gillade kommentaren</p> <p>Målets period </p> <p>Målets namn</p> <p>Texten i kommentaren </p> <p>Knappen <strong>[!UICONTROL Open in web app]</strong> som öppnar panelen [!UICONTROL Goal Details]</p> <p>Knappen <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Någon tyckte om en uppdatering för mitt mål</strong></td> 
   <td> <p>Du får ett e-postmeddelande när någon gillar en kommentar som du har gjort på ett mål eller när du uppdaterar förloppet för dina resultat eller aktiviteter på målet. </p> <p>Namnet på den person som gillade uppdateringen</p> <p>Målets period </p> <p>Målets namn</p> <p>Knappen <strong>[!UICONTROL Open in web app]</strong> som öppnar panelen [!UICONTROL Goal Details]</p> <p>Knappen <strong>[!UICONTROL Change Notifications Settings]</strong> som gör att du kan hantera dina meddelanden.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->

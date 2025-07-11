---
title: Logga in som en annan användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du ibland behöva få åtkomst till Workfront för en annan användares räkning.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 6068c9c53568d3ebec9fae294bfee1cbd365714b
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Logga in som en annan användare

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

Som Adobe Workfront-administratör kan du ibland behöva få åtkomst till Workfront för en annan användares räkning. Som gruppadministratör kan du behöva få åtkomst till Workfront för en användare som är medlem i en grupp som du hanterar.

Om en uppgift till exempel inte kan fortsätta förrän en användare på semester utför en viss åtgärd, kan du logga in som den användaren och utföra åtgärden i stället.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Eftersom en dokumentintegrering kan ansluta till privata personliga filer, kan administratörer inte komma åt dokumentintegreringar när de är inloggade som en annan användare.
>
>Mer information om dokumentintegreringar finns i [Konfigurera dokumentintegreringar](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Med åtkomstnivån Systemadministratör kan du logga in som vem som helst.</p> <p>Med åtkomstnivån Standard eller Planner kan du logga in som en användare med en lägre licensnivå om inställningen Användare i åtkomstnivån är konfigurerad för att redigera åtkomst, med alternativet Skapa och minst ett av de två alternativen för användaradministration är aktiverat under Finjustera inställningarna <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p>Obs! Om användaradministratör (gruppanvändare) är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem av dessa två alternativ.</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Logga in och utför åtgärder som en annan användare

1. Logga in på Workfront som Workfront-administratör eller gruppadministratör.

   >[!NOTE]
   >
   >* Om du är gruppadministratör kan du bara logga in som användare i de grupper som du hanterar. Behörigheten Användaradministratör (gruppanvändare) måste även aktiveras på din åtkomstnivå:
   >   
   >  ![Gruppadministratörsanvändare](assets/group-admin-user.png)
   >   
   >  Den här inställningen är inaktiverad som standard. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Du kan inte återställa lösenordet för en Workfront-administratör.

{{step-1-to-setup}}

1. Klicka på **Logga in som** i den vänstra panelen.

1. I rutan **Börja skriva namn..** på fliken **Logga in som** börjar du skriva namnet på användaren och klickar sedan på namnet när det visas i listrutan.


   >[!NOTE]
   >* Den användare du väljer måste ha en åtkomstnivå definierad i Workfront. Du kan inte logga in på Workfront som en användare som inte har behörighet att logga in.
   >* Gruppadministratörer kan bara logga in som användare som är medlemmar i de grupper som de hanterar. De kan inte logga in som Workfront-administratör.

1. Klicka på **Logga in**. Du är inloggad som en annan användare och ett meddelande visas högst upp på skärmen som anger detta.

   <!--
   <p> Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->



1. När du har utfört de nödvändiga åtgärderna som användare klickar du på **Logga ut** längst upp på skärmen.

## Spårnings- och granskningsaktivitet medan en administratör är inloggad som en annan användare

Workfront innehåller mekanismer för att spåra och granska aktiviteter som sker när administratören är inloggad som en annan användare.

När du loggar in som en annan användare ändras det senaste inloggningsdatumet för den användaren till det datum då system- eller gruppadministratören loggar in som den användaren.

* [Visa indikatorer för objekt](#view-indicators-on-items)
* [Visa granskningsinformation](#view-audit-information)

### Visa indikatorer för artiklar {#view-indicators-on-items}

När du loggar in på Workfront som en annan användare och utför en åtgärd, visar Workfront tydligt att alla åtgärder du utför görs av dig för den användare som du är inloggad som.

Om du till exempel kommenterar ett objekt när du är inloggad som en annan användare, visar en programsats att du har gjort kommentaren å användarens vägnar när du visar uppdateringsavsnittet för ett objekt.

### Visa granskningsinformation {#view-audit-information}

1. Logga in på Workfront som Workfront-administratör eller gruppadministratör.
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. Klicka på **Logga in som** i den vänstra panelen och klicka sedan på fliken **Åtkomstlogg** .

   >[!NOTE]
   >
   >Varje gång en system- eller gruppadministratör loggar in på Workfront som en annan användare loggas händelsen i granskningsspåret. Dessutom loggas alla ändringsbara åtgärder som utförs när administratören är inloggad som en annan användare i granskningsspåret.

1. (Valfritt) Du kan filtrera resultaten som visas i granskningsspåret på följande sätt:

   * Av den användare som har loggat in
   * Av den användare som har loggat in som
   * Efter datum och tid

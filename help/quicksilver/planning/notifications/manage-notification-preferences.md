---
title: Hantera aviseringsinställningar för Adobe Workfront Planning
description: Du kanske kan hantera dina meddelandeinställningar för Adobe Workfront Planning. I den här artikeln beskrivs hur du konfigurerar dina meddelandeinställningar.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---


# Hantera aviseringsinställningar för Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan få meddelanden i programmet eller via e-post när följande åtgärder inträffar i Workfront Planning:

* Någon lägger till dig i en kommentar på postsidan
* Någon ber om behörighet att komma åt en vy eller arbetsyta
* Någon ger dig behörighet att komma åt en vy eller arbetsyta <!--I could not test this but Isk confirmed-->
* Du skickar en Workfront Planning-förfrågan.
* Någon godkänner eller avvisar en Workfront Planning-begäran som du har skickat in.
* Statusen ändras till en Workfront Planning-förfrågan som du har skickat in.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience.</p> 
<p>Användarna i din organisation får meddelanden från Workfront Planning endast när din organisation är registrerad på Adobe Unified Experience. </p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p><p>Standard, Light eller Contributor
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Visa eller högre behörigheter på en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Mer information om Workfront Planning-meddelanden finns i följande artiklar:

* Mer information om kommentarer om poster finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).
* Information om meddelanden i appen från Workfront Planning finns i [Hantera meddelanden i appen för Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Information om e-postmeddelanden från Workfront Planning finns i [Hantera e-postmeddelanden för Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Hantera meddelandeinställningar

1. Logga in på Workfront med dina Adobe Experience Cloud-uppgifter.
1. Klicka på ikonen **kontomeny** ![Konto-meny på Experience Cloud](assets/account-menu-icon-on-experience-cloud.png) i skärmens övre högra hörn och klicka sedan på **Inställningar**.
1. Klicka på **Workfront** under avsnittet **Meddelanden**.
1. Markera de meddelanden som du vill ta emot.
eller
Avmarkera de meddelanden som du vill sluta ta emot.

   ![Adobe Experience Cloud-meddelandepanel för Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Följande meddelanden är tillgängliga för Workfront:

   * **Meningar**: Du får ett meddelande när någon taggar dig i en kommentar i Workfront Planning
   * **Begäranden**: Du får ett meddelande när någon har gjort något av följande:

      * Begär eller ger dig behörighet till ett Workfront Planning-objekt
      * Du har skickat in en begäran om Workfront Planning
      * Status för en Workfront Planning-begäran som du har skickat in ändringar för
      * Begär, beviljar eller avvisar ett godkännande av en Workfront Planning-begäran

   Mer information om hur du hanterar meddelanden finns i [Kontoinställningar och meddelanden](https://experienceleague.adobe.com/sv/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/sv/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->

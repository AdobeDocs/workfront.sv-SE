---
user-type: administrator
product-area: system-administration;user-management
keywords: visa,grupp,händelse,meddelanden,konfigurera,aktivera,inaktivera
navigation-topic: create-and-manage-groups
title: Visa och konfigurera händelsemeddelanden för en grupp
description: Som gruppadministratör kan du visa händelsemeddelanden som aktiveras för en grupp som du hanterar. Om en Adobe Workfront-administratör låser upp ett händelsemeddelande kan du konfigurera det för en toppnivågrupp som du hanterar. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Visa och konfigurera händelseaviseringar för en grupp

Som gruppadministratör kan du visa händelsemeddelanden som aktiveras för en grupp som du hanterar.

Om en Adobe Workfront-administratör låser upp ett händelsemeddelande kan du konfigurera det för en toppnivågrupp som du hanterar. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.

En Workfront-administratör kan även göra detta för alla grupper.

Om du konfigurerar ett händelsemeddelande för en grupp påverkas användare för vilka gruppen, eller en av dess undergrupper, är deras hemgrupp. I sina användarprofiler ser dessa användare händelsemeddelanden som aktiveras för hemgruppen i stället för händelsemeddelanden som aktiveras i hela systemet.

Mer information om hur en Workfront-administratör låser upp ett händelsemeddelande finns i [Lås upp eller låsa konfigurationen för händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Mer information om standardinställningen för meddelanden för en händelse finns i [Händelsemeddelandetyper](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Visa och konfigurera en grupps händelsemeddelanden

>[!TIP]
>
>Om du är Workfront-administratör och redan är på sidan E-postaviseringar (Inställningar > E-post > Meddelanden) kan du göra följande och sedan gå vidare till steg 6: Ta bort **systemhändelsemeddelanden** i rutan ovanför listan, börja skriva gruppens namn i rutan och klicka på den när den visas.

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen på den översta nivån.
1. Klicka på **Händelsemeddelanden** på den vänstra menyn.

   I listan som visas visar kolumnen **Aktiv** till vänster vilka meddelanden som är aktiva (blå) och inaktiva (grå) för gruppen.

1. Så här aktiverar eller inaktiverar du ett olåst händelsemeddelande: Klicka på knappen i kolumnen <strong>Aktiv</strong> för att aktivera <img src="assets/email-notification-enabled-unlocked.png"> eller inaktivera <img src="assets/email-notification-disabled-unlocked.png"> den.

   >[!INFO]
   >
   >**Exempel:** Du kan konfigurera de två viktigaste händelsemeddelandena för marknadsföringsgrupper som visas nedan och som har låsts upp för grupper.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Om en knapp i kolumnen <strong>Aktiv</strong> är grå och nedtonad <img src="assets/email-notification-disabled-locked.png">, händelsemeddelandet inaktiveras för alla användare och gruppadministratörer kan inte aktivera det eller redigera e-postens ämnesrad
   >* Om en knapp i kolumnen <strong>Aktiv</strong> är grå och inte nedtonad <img src="assets/email-notification-disabled-unlocked.png">, händelsemeddelandet är <strong>inaktiverat för alla användare och </strong> gruppadministratörer kan aktivera det för sina grupper.
   >* Om en knapp i kolumnen <strong>Aktiv</strong> är blå och nedtonad <img src="assets/email-notification-enabled-locked.png">, händelsemeddelandet aktiveras för alla användare och gruppadministratörer kan inte inaktivera det eller redigera dess e-postämnesrad för sina grupper.
   >* Om en knapp i kolumnen <strong>Aktiv</strong> är blå och inte nedtonad <img src="assets/email-notification-enabled-unlocked.png">, händelsemeddelandet är <strong>aktiverat för alla användare och</strong> gruppadministratörer kan inaktivera det för sina grupper.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->


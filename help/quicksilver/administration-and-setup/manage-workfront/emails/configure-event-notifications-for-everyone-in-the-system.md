---
title: Konfigurera händelsemeddelanden för alla i systemet
description: Händelsemeddelanden utlöser e-postmeddelanden till användare när en viss händelse inträffar. Som Adobe Workfront-administratör eller en användare med en planeraråtkomstnivå kan du konfigurera ett händelsemeddelande för alla användare i systemet. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Konfigurera händelsemeddelanden för alla i systemet

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Händelsemeddelanden utlöser e-postmeddelanden till användare när en viss händelse inträffar. Som Adobe Workfront-administratör eller en användare med en planeraråtkomstnivå kan du konfigurera ett händelsemeddelande för alla användare i systemet. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Beroende på vilken händelse du aktiverar och användaren fortsätter att vara aktiverad i sin egen profil får användarna e-postmeddelanden direkt, dagligen eller både direkt och dagligen när en händelse inträffar.

Du måste först ange vilka meddelanden du vill att alla användare ska få under Konfigurera i Workfront-instansen. När du har aktiverat ett meddelande i inställningsområdet visas det som aktiverat för varje användare på deras profilsida.

När meddelanden har aktiverats i inställningsområdet och visas på användarens profilsidor, kan enskilda användare eller en annan användare med en planlicens även konfigurera aktiverade meddelanden i en användarprofil för att styra vilka meddelanden som en viss användare får och hur ofta. Mer information finns i [Ändra dina egna e-postmeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

En lista med alla händelsemeddelanden som du kan aktivera och inaktivera finns i [Händelsemeddelandetyper](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Information om hur du låser upp ett händelsemeddelande så att gruppadministratörer kan konfigurera det för sina grupper finns i [Lås upp eller låsa konfigurationen för händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) och [Visa och konfigurera händelsemeddelanden för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

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
<p>Aktuell: Planera</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Planering eller senare, med administrativ åtkomst till påminnelsemeddelanden</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera händelsemeddelanden för alla användare

Du måste aktivera meddelanden under Konfigurera i Workfront innan användare kan aktivera eller inaktivera dem i sina enskilda profiler.

>[!TIP]
>
>Du kan inte aktivera meddelanden för Workfront-mål under Konfigurera. Användarna kan bara aktivera de här meddelandena i sina profiler. Användare med Planera licenser kan aktivera dem för andra användare. Mer information om hur du aktiverar Workfront-målmeddelanden för användare finns i [Meddelanden: Mål](../../../workfront-basics/using-notifications/notifications-goals.md).

{{step-1-to-setup}}

1. Klicka på **E-post** > **Meddelanden**.

   ![](assets/notifications-area-under-setup-emails.png)


1. Kontrollera att fliken **Händelsemeddelanden** är öppen.
1. Växla till vänster om händelsenamnet för att aktivera eller inaktivera den.

   Information om standardmeddelandestatus för en händelse finns i [Händelsemeddelanden](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Valfritt) Klicka på namnet på ett händelsemeddelande för att anpassa ämnesraden i e-postmeddelandet.

   Mer information om hur du anpassar ämnesraderna i e-postmeddelanden finns i [Anpassa e-postämnen för händelsemeddelanden](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Valfritt) Om du vill låsa upp konfigurationen för ett e-postmeddelande så att gruppadministratörer kan konfigurera den separat för sina grupper klickar du på knappen ![](assets/lock-toggle-button.png) till höger om meddelandet för att växla till den olåsta positionen ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Den här funktionaliteten är inledningsvis bara tillgänglig för kunder i kluster 4 som en del av en fasad utrullning. Det kommer att bli tillgängligt för andra kluster kort därefter. Artikeln uppdateras när detta inträffar.

   Mer information finns i [Lås upp eller låsa konfigurationen för händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

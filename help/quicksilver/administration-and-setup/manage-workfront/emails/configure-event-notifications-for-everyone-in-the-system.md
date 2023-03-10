---
title: Konfigurera händelsemeddelanden för alla i systemet
description: Händelsemeddelanden utlöser e-postmeddelanden till användare när en viss händelse inträffar. Som Adobe Workfront-administratör eller en användare med en planeraråtkomstnivå kan du konfigurera ett händelsemeddelande för alla användare i systemet. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Konfigurera händelsemeddelanden för alla i systemet

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Händelsemeddelanden utlöser e-postmeddelanden till användare när en viss händelse inträffar. Som Adobe Workfront-administratör eller en användare med en planeraråtkomstnivå kan du konfigurera ett händelsemeddelande för alla användare i systemet. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Beroende på vilken händelse du aktiverar och användaren fortsätter att vara aktiverad i sin egen profil får användarna e-postmeddelanden direkt, dagligen eller både direkt och dagligen när en händelse inträffar.

Du måste först ange vilka meddelanden du vill att alla användare ska få under Konfigurera i Workfront-instansen. När du har aktiverat ett meddelande i inställningsområdet visas det som aktiverat för varje användare på deras profilsida.

När meddelanden har aktiverats i inställningsområdet och visas på användarens profilsidor, kan enskilda användare eller en annan användare med en planlicens även konfigurera aktiverade meddelanden i en användarprofil för att styra vilka meddelanden som en viss användare får och hur ofta. Mer information finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

En lista över alla händelsemeddelanden som du kan aktivera och inaktivera finns i [Händelsemeddelanden är tillgängliga i Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Mer information om hur du låser upp ett händelsemeddelande så att gruppadministratörer kan konfigurera det för sina grupper finns i [Lås upp eller lås konfigurationen av händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) och [Visa och konfigurera händelsemeddelanden för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Planering eller senare, med administrativ åtkomst till påminnelsemeddelanden</p> <p>Mer information om hur du ger en Plan-användare administratörsåtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera händelsemeddelanden för alla användare

Du måste aktivera meddelanden under Konfigurera i Workfront innan användare kan aktivera eller inaktivera dem i sina profiler.

>[!TIP]
>
>Du kan inte aktivera meddelanden för Workfront-mål under Konfigurera. Användarna kan bara aktivera dessa meddelanden i sina profiler. Användare med Planera licenser kan aktivera dem för andra användare. Mer information om hur du aktiverar meddelanden om Workfront-mål för användare finns i [Meddelanden: Mål](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **E-post** > **Meddelanden**.

1. Se till att **Händelsemeddelanden** -fliken är öppen.
1. Klicka på växeln till vänster om händelsenamnet för att aktivera eller inaktivera den.

   Information om standardmeddelandestatus för en händelse finns i [Händelsemeddelanden](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Valfritt) Klicka på namnet på ett händelsemeddelande för att anpassa ämnesraden i e-postmeddelandet.

   Mer information om hur du anpassar ämnesraderna i e-postmeddelanden finns i [Anpassa e-postämnen för händelsemeddelanden](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Valfritt) Om du vill låsa upp konfigurationen för ett e-postmeddelande så att gruppadministratörer kan konfigurera den separat för sina grupper klickar du på knappen ![](assets/lock-toggle-button.png) till höger om meddelandet för att växla till den olåsta positionen ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Den här funktionaliteten är inledningsvis bara tillgänglig för kunder i kluster 4 som en del av en fasad utrullning. Det kommer att bli tillgängligt för andra kluster kort därefter. Artikeln uppdateras när detta inträffar.

   Mer information finns i [Lås upp eller lås konfigurationen av händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

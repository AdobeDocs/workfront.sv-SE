---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Ta bort en anpassad status
description: Du kan ta bort en anpassad systemstatus om den inte längre är användbar för din organisation.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Ta bort en anpassad status

Du kan ta bort en anpassad systemstatus om den inte längre är användbar för din organisation.

Om statusen är låst eller olåst avgör om statusen tas bort för alla grupper i systemet:

* När du tar bort en systemstatus som för närvarande är låst tas statusen bort för alla grupper i systemet, oavsett om gruppen har bytt namn på den eller inte.
* Omvänt gäller att när du tar bort en systemstatus som för närvarande är olåst behålls statusen för alla grupper i systemet.


>[!NOTE]
>
>Du kan inte ta bort följande:
>
>* En låst eller olåst systemstatus används i en systemgodkännandeprocess som för närvarande väntar på godkännande för minst ett objekt i systemet.
>
>  Du kan dock ta bort en olåst systemstatus som används i en enanvändningsprocess eller en godkännandeprocess på gruppnivå som väntar på godkännande.
>
>  Du kan köra en rapport för att hitta objekten och lösa väntande godkännanden och sedan försöka ta bort statusen igen. Instruktioner finns i [Visa objekt med väntande godkännandeprocesser med en viss status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Status som används i godkännandeprocesser som för närvarande väntar på godkännande för minst ett objekt i systemet.

Instruktioner om hur du tar bort en gruppstatus finns i [Ta bort en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Åtkomstkrav

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ta bort en anpassad systemstatus

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Projektinställningar** > **Status** i den vänstra panelen.

1. Om du vill ta bort statusen i hela systemet (inklusive för enskilda grupper) håller du musen över statusen och klickar på **Redigera**. Kontrollera sedan att **Lås för alla grupper** är markerat. Klicka på **Spara**.

   eller

   Om du vill ta bort systemstatusen men behålla den för enskilda grupper håller du musen över statusen, klickar på **Redigera** och kontrollerar sedan att **Lås för alla grupper** inte är markerat. Klicka på **Spara**.

1. Håll markören över den status som du vill ta bort och klicka sedan på **Ta bort**.
1. Klicka på **Ta bort status** i det meddelande som visas.
1. I rutan **Ta bort status** som visas väljer du en status i fältet **Ange alla projekt med den här statusen till**.

   Projekt som använder den status som du tar bort har den status som du väljer.

   Statuser är bara tillgängliga i listrutan om de är lika med samma status som den du håller på att ta bort.

   Om du t.ex. tar bort en status som är lika med Aktuell är bara statusvärden som är lika med Aktuell tillgängliga att välja.

1. Klicka på **Ta bort status**.

---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Ta bort en anpassad status
description: Du kan ta bort en anpassad systemstatus om den inte längre är användbar för din organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '435'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort en anpassad systemstatus

{{step-1-to-setup}}

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

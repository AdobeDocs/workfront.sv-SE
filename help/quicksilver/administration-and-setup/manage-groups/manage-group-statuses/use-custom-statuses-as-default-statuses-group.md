---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Använd en anpassad status som standardstatus för en grupp
description: Som gruppadministratör kan du konfigurera en anpassad status som standardstatus för en grupp eller undergrupp som du hanterar.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Använd en anpassad status som standardstatus för en grupp

Som gruppadministratör kan du konfigurera en anpassad status som standardstatus för en grupp eller undergrupp som du hanterar. Detta är användbart när systemet automatiskt behöver tilldela en Workfront-status till ett projekt, en uppgift eller ett problem. Ett projekt, en uppgift eller ett problem visar alltid den anpassade status som du anger som standardstatus i stället för att visa den Workfront-status som det motsvarar.

Statusen som du konfigurerar kan vara vilken anpassad status som helst som har skapats för gruppen, ärvts från en grupp ovanför gruppen eller ärvts från systemnivån.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!INFO]
>
>**Exempel:** Du kan skapa en anpassad status med namnet Slutförd och ange den som en standardstatus med statusen Fullständig för Workfront.
>
>För uppgifter som ställs in på att ändras till statusen Fullständig när de når 100 % visas statusen Slutförd i stället för Fullständig.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Utfärdandestatus

Om den anpassade statusen är Problem, måste alla fyra problemtyperna aktiveras för den (Felrapport, Ändra ordning, Problem och Begäran). I den utgivningsstatus som visas nedan kan statusen Återöppnad inte användas som standardstatus eftersom typen Ändra ordning inte har valts:

![](assets/all-4-issue-types-enabled.png)

## Ange en anpassad status som standardstatus för en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen och klicka sedan på namnet på gruppen där du vill skapa eller anpassa statusvärden.
1. Klicka på **Status** ![](assets/gear-icon-settings.png) i den vänstra panelen.
1. Öppna fliken **Projekt**, **Åtgärder** eller **Problem**, beroende på vilken typ av status du vill ange som standardstatus.
1. Klicka på **Ange standardstatus** i det övre högra hörnet.
1. I listrutan som visas, bredvid den status där du vill ange standardstatus, väljer du den standardstatus du vill ange.
1. Klicka på **Spara**.

   Statusen är nu tillgänglig som standardstatus för projekt som är kopplade till gruppen.

1. Koppla den anpassade statusen till det projekt där du vill använda den.

   Du kopplar statusen till projektet genom att associera gruppen där statusen finns med projektet. Användare kan bara använda den anpassade statusen om gruppen där statusen finns är associerad med projektet.

   >[!NOTE]
   >
   >Om du tilldelar projektet till en annan grupp läses projektstatusen in igen och kan ändras.

   1. Gå till det projekt där du vill använda den anpassade statusen.
   1. Klicka på menyn Mer ![](assets/more-icon.png) och sedan på **Redigera**.
   1. I rutan **Redigera projekt** som visas i fältet **Grupp** under **Projektassociation** markerar du gruppen som den anpassade statusen är associerad med.

   1. Klicka på **Spara ändringar**.

## Grupper ärver standardstatuskonfigurationer

När en Workfront-administratör har konfigurerat en anpassad status som standardstatus ärver nya grupper den konfigurationen.

När en gruppadministratör har angett en anpassad status som standardstatus ärver nya undergrupper som skapas direkt under gruppen den konfigurationen.

Mer information finns i [Hur grupper ärver statusvärden](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## När en standardstatus är dold

Om du döljer en standardstatus (genom att aktivera alternativet Dölj status för den) försöker systemet i stället ange en annan status med motsvarande typ som standard.

Om det inte finns någon tillgänglig status av motsvarande typ visas statustypen som **Dold** och är inte tillgänglig för arbetsobjekt.

![](assets/when-hide-default-status-no-equivalent.png)

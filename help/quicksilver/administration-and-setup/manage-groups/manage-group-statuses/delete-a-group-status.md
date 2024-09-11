---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Ta bort en gruppstatus
description: Som gruppadministratör kan du ta bort en status för en grupp som du hanterar om den inte är konfigurerad som obligatorisk eller låst på systemnivå, eller för en högre grupp i hierarkin.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Ta bort en gruppstatus

Som gruppadministratör kan du ta bort en status för en grupp som du hanterar om den inte är konfigurerad som obligatorisk eller låst på systemnivå, eller för en högre grupp i hierarkin.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>Du kan inte ta bort följande:
>
>* De inbyggda statusarna Planning, Current och Complete. Du kan uppdatera deras namn, redigera deras färger och låsa eller låsa upp dem, men de kan inte tas bort.
>* Status som väntar på godkännande för minst ett objekt som är associerat med gruppen eller en av dess undergrupper.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort en gruppstatus

{{step-1-to-setup}}

1. Klicka på **Grupper** i den vänstra panelen.
1. Klicka på namnet på gruppen på den översta nivån.
1. Klicka på **Status** i den vänstra panelen.
1. Håll markören över den status som du vill ta bort i listan med statusar som visas och klicka sedan på **Ta bort** när den visas längst till höger.

   ![](assets/hover-click-delete.jpg)

1. I den ruta som visas väljer du en status för att ange en ersättningsstatus för objekt (projekt, uppgifter, utgåvor och godkännandeprocesser) som använder den status som du håller på att ta bort.

   Endast statusvärden som motsvarar den status du håller på att ta bort är tillgängliga. Om du till exempel tar bort en status som är lika med Aktuell kan du bara se statusvärden som är lika med Aktuell.

   Statusen som visas beror dessutom på om statusen du tar bort är olåst eller låst:

   * **Om den är olåst**: Ej dolda låsta och olåsta statusar är tillgängliga.

     Tillsammans med de statusvärden som skapades för undergruppen inkluderas statusvärden som ärvts från grupper på systemnivå och övernivå.

   * **Om den är låst**: Något av följande är sant:

      * Om det finns andra låsta, icke-dolda statusar är bara dessa tillgängliga.
      * Om det inte finns någon låst status som inte är dold är standardstatusen för Workfront tillgänglig, även om den är dold eller olåst.

        Mer information om standardstatusvärdena för Workfront finns i [Åtkomst till listan över status för systemprojekt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Åtkomst till listan över status för systemaktivitet](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) och information om de fyra nödvändiga utfärdandestatusarna i [Åtkomst till listan över status för systemproblem](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Klicka på **Ta bort status**.

   Om borttagen status var standardstatus för den typen i gruppen ersätts ersättningsstatusen.

   Om den borttagna statusen har angetts som standardprojektstatus i projektinställningarna, ställs inställningen nu in på ersättningsstatus.

## När en grupp tas bort

När en grupp tas bort och ersätts av en annan grupp, läggs eventuella unika statusvärden som den borttagna gruppen hade till i statusarna för ersättningsgruppen. Mer information finns i [Anpassade statusvärden i en grupp som har flyttats eller tagits bort](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).

---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Ändra ordning på systemnivå och gruppstatus
description: Som Workfront-administratör kan du ändra ordningen för projekt-, uppgifts- och utfärdandestatus för alla i systemet eller för en enskild grupp.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Ändra ordning på systemnivå och gruppstatus

Som Workfront-administratör kan du ändra ordningen för projekt-, uppgifts- och utfärdandestatus för alla i systemet eller för en enskild grupp.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Om du ändrar ordning på statusarna på systemnivå påverkas inte ordningen på statusarna i grupper.
>
>  Statuserna i en nyligen skapad grupp på den översta nivån ärver dock ordningen för statusvärdena på systemnivå. (En ny undergrupp ärver ordningen för statusarna i gruppen en nivå upp.)
>
>* Du kan ändra ordningen på låsta statusar. Mer information om låsta statusar finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Gruppadministratörer kan också ändra ordningen på de statusar som används i deras grupper. Mer information finns i [Ändra gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan* </td> 
   <td>Alla</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara Workfront-administratör. Mer information om Workfront-administratörer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Standardordning för statusvärden

Som standard visas statusvärden i följande ordning:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Projekt</th> 
   <th width="33.33%">Uppgift</th> 
   <th width="33.33%">Problem</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Aktuell</li> 
     <li>Död</li> 
     <li> Parkerad </li> 
     <li> Planering </li> 
     <li> Complete </li> 
     <li> Begärd </li> 
     <li> Godkänd </li> 
     <li> Avvisad </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nytt</li> 
     <li>Pågår</li> 
     <li>Complete</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nytt</li> 
     <li>Pågår</li> 
     <li>Återöppnad</li> 
     <li>Väntar på feedback</li> 
     <li>Parkerad</li> 
     <li>Kan inte duplicera</li> 
     <li>Stängd</li> 
     <li>Löst</li> 
     <li>Verifierad slutförd</li> 
     <li>Lös inte</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ändra ordning på status för uppgifter och projekt i hela systemet eller för en grupp

{{step-1-to-setup}}

1. Klicka på **Projektinställningar > Status** i den vänstra panelen.
1. (Villkorligt) Om du ändrar ordning på statusarna för en grupp börjar du skriva namnet på gruppen i rutan i det övre högra hörnet och klickar sedan på namnet när det visas.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Ovanför statuslistan som visas klickar du på fliken **Projekt** eller **Åtgärder** .

1. Dra och släpp statusarna i önskad ordning.

   Den nya statusordern sparas automatiskt.

1. Om du vill testa den nya statusordningen går du till en uppgift eller ett projekt, klickar på statusen i det övre högra hörnet och ser till att statusvärdena som visas är i den ordning som du har konfigurerat.

## Ändra ordning på statusvärden för utgåvor

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Projektinställningar > Status.**
1. (Villkorligt) Om du ändrar ordning på statusarna för en grupp börjar du skriva namnet på gruppen i rutan i det övre högra hörnet och klickar sedan på namnet när det visas.

   ![](assets/issue-statuses-group-name.png)

1. Klicka på fliken **Problem**.
1. (Valfritt) Välj en problemtyp (**Felrapport**, **Ändra ordning**, **Problem** eller **Begäran**).

   >[!NOTE]
   >
   >* Du kan inte anpassa statusordningen för huvudlistan.
   >* Vi rekommenderar att du beställer statusar för varje utgåva på samma sätt. Mer information om problemtyper finns i [Konfigurera frågetyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Dra och släpp statusarna i önskad ordning.

   Den nya statusordern sparas automatiskt.

1. Om du vill testa den nya statusordningen går du till ett problem, klickar på statusen i det övre högra hörnet och ser till att statusvärdena som visas är i den ordning som du har konfigurerat.

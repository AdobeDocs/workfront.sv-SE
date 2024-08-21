---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Ändra ordning på gruppstatus
description: Som gruppadministratör kan du ändra ordningen för projekt-, uppgifts- och utfärdandestatus för en grupp som du hanterar.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Ordna om gruppstatus

Som gruppadministratör kan du ändra ordningen för projekt-, uppgifts- och utfärdandestatus för en grupp som du hanterar.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>* En Workfront-administratör kan ändra ordningen på statusarna på systemnivå. Detta påverkar inte ordningen på statusar i grupper.
>
>  Statuserna i en nyligen skapad grupp på den översta nivån ärver dock ordningen för statusvärdena på systemnivå. (En ny undergrupp ärver ordningen för statusarna i gruppen en nivå upp.)
>
>* Du kan ändra ordningen på låsta statusar. Mer information om låsta statusar finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
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
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
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
     <p>Aktuell</p> 
     <p>Död</p> 
     <p> Parkerad </p> 
     <p> Planering </p> 
     <p> Complete </p> 
     <p> Begärd </p> 
     <p> Godkänd </p> 
     <p> Avvisad </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>Nytt</p> 
     <p>Pågår</p> 
     <p>Complete</p> 
   </td> 
   <td> 
     <p>Nytt</p> 
     <p>Pågår</p> 
     <p>Återöppnad</p> 
     <p>Väntar på feedback</p> 
     <p>Parkerad</p> 
     <p>Kan inte duplicera</p> 
     <p>Stängd</p> 
     <p>Löst</p> 
     <p>Verifierad slutförd</p> 
     <p>Lös inte</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Ändra ordning på statusvärden för uppgifter och projekt i en grupp som du hanterar

{{step-1-to-setup}}

1. Klicka på **Grupper** i den vänstra panelen och klicka sedan på gruppens namn.
1. Klicka på **Status** i den vänstra panelen.
1. Ovanför statuslistan som visas klickar du på fliken **Projekt** eller **Åtgärder** .

1. Dra och släpp statusarna i önskad ordning.

   Den nya statusordern sparas automatiskt.

1. Om du vill testa den nya statusordningen går du till en uppgift eller ett projekt som är kopplat till gruppen, klickar på statusen i det övre högra hörnet och ser till att statusvärdena som visas är i den ordning som du har konfigurerat.

## Ändra ordning på statusvärden för utgåvor

{{step-1-to-setup}}

1. Klicka på **Grupper** i den vänstra panelen och klicka sedan på gruppens namn.
1. Klicka på **Status** i den vänstra panelen.
1. Klicka på fliken **Problem**.
1. (Valfritt) Välj en problemtyp (**Felrapport**, **Ändra ordning**, **Problem** eller **Begäran**).

   >[!NOTE]
   >
   >* Du kan inte anpassa statusordningen för huvudlistan.
   >* Vi rekommenderar att du beställer statusar för varje utgåva på samma sätt. Mer information om problemtyper finns i [Konfigurera frågetyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Dra och släpp statusarna i önskad ordning.

   Den nya statusordern sparas automatiskt.

1. Om du vill testa den nya statusordningen går du till ett problem som är kopplat till gruppen, klickar på statusen i det övre högra hörnet och ser till att statusvärdena som visas är i den ordning som du har konfigurerat.

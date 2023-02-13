---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Ordna om gruppstatus
description: Som gruppadministratör kan du ändra ordningen för projekt-, uppgifts- och utfärdandestatus för en grupp som du hanterar.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
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
>* Du kan ändra ordningen på låsta statusar. Mer information om låsta lägen finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## Åtkomstkrav

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
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

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
     <p> Slutförd </p> 
     <p> Begärd </p> 
     <p> Godkänd </p> 
     <p> Avvisad </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>Nytt</p> 
     <p>Pågår</p> 
     <p>Slutförd</p> 
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

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** klickar du sedan på gruppens namn.
1. Klicka på i den vänstra panelen **Status**.
1. Ovanför statuslistan som visas klickar du på **Projekt** eller **Uppgifter** -fliken.

1. Dra och släpp statusarna i önskad ordning.

   Den nya statusordern sparas automatiskt.

1. Om du vill testa den nya statusordningen går du till en uppgift eller ett projekt som är kopplat till gruppen, klickar på statusen i det övre högra hörnet och ser till att statusvärdena som visas är i den ordning som du har konfigurerat.

## Ändra ordning på statusvärden för utgåvor

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** klickar du sedan på gruppens namn.
1. Klicka på i den vänstra panelen **Status**.
1. Klicka på **Problem** -fliken.
1. (Valfritt) Välj en problemtyp (**Felrapport**, **Ändra ordning**, **Problem**, eller **Begäran**).

   >[!NOTE]
   >
   >* Du kan inte anpassa statusordningen för den Överordnad listan.
   >* Vi rekommenderar att du beställer statusar för varje utgåva på samma sätt. Mer information om problemtyper finns i [Konfigurera begärandetyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Dra och släpp statusarna i önskad ordning.

   Den nya statusordern sparas automatiskt.

1. Om du vill testa den nya statusordningen går du till ett problem som är kopplat till gruppen, klickar på statusen i det övre högra hörnet och ser till att statusvärdena som visas är i den ordning som du har konfigurerat.

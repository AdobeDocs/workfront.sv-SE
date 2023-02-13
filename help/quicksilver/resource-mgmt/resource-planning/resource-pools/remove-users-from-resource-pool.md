---
product-area: resource-management
navigation-topic: resource-pools
title: Ta bort användare från resurspooler
description: Även om det inte finns någon gräns för hur många användare du kan ha i en resurspool visas endast de första 2 000 användarna i listan i bokstavsordning.
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Ta bort användare från resurspooler

Även om det inte finns någon gräns för hur många användare du kan ha i en resurspool visas endast de första 2 000 användarna i listan i bokstavsordning.

Vi rekommenderar att du tar bort användare som har inaktiverats eller flyttat roller eller avdelningar, så att du alltid har en korrekt lista över användare i alla resurspooler.

Mer information om resurspooler finns i [Översikt över resurspooler](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Hantera resurspooler</p> <p>Visa eller ge användare högre åtkomst</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Ta bort användare från en resurspool

Du kan ta bort användare från en resurspool när dessa användare inte längre behövs i den poolen.

Så här tar du bort en användare från en resurspool:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Resurser**.
1. Klicka **Resurspooler** i den vänstra panelen.
1. Välj en resurspool och klicka på **Redigera.**Eller\
   Klicka på namnet på en resurspool.

1. Börja skriva namnet på en användare som du vill ta bort i dialogrutan **Sök i den här resurspoolen** fält.\
   eller\
   Börja skriva namnet på ett företag, en jobbroll, ett team eller en grupp om du vill ta bort alla användare som är associerade med de entiteterna.\
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. Klicka på x-ikonen på användarnivå för att ta bort en användare från resurspoolen. De tas bort från alla listor som de visas i.\
   eller\
   Om du vill ta bort alla användare som är kopplade till en jobbroll, grupp, team eller företag klickar du på **Ta bort** på jobbnivå, gruppnivå, teamnivå eller företagsnivå. Detta tar bort alla användare som är associerade med den jobbrollen, gruppen, teamet eller företaget från resurspoolen.

1. Klicka **Spara**.

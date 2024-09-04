---
product-area: resource-management
navigation-topic: resource-pools
title: Ta bort användare från resurspooler
description: Även om det inte finns någon gräns för hur många användare du kan ha i en resurspool visas endast de första 2 000 användarna i listan i bokstavsordning.
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Ta bort användare från resurspooler

{{preview-and-fast-release-Q424}}

Även om det inte finns någon gräns för hur många användare du kan ha i en resurspool visas endast de första 2 000 användarna i listan i bokstavsordning.

Vi rekommenderar att du tar bort användare som har inaktiverats eller flyttat roller eller avdelningar, så att du alltid har en korrekt lista över användare i alla resurspooler.

Mer information om resurspooler finns i [Översikt över resurspooler](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Hantera resurspooler</p> <p>Visa eller ge användare högre åtkomst</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort användare från en resurspool

Du kan ta bort användare från en resurspool när dessa användare inte längre behövs i den poolen.

Så här tar du bort en användare från en resurspool:

{{step1-to-resourcing}}

1. Klicka på **Resurspooler** i den vänstra panelen.
1. Välj en resurspool och klicka på **Redigera**.
eller\
   Klicka på namnet på en resurspool.

1. Börja skriva namnet på en användare som du vill ta bort i fältet **Sök i den här resurspoolen**.\
   eller\
   Börja skriva namnet på ett företag, en jobbroll, ett team eller en grupp om du vill ta bort alla användare som är associerade med de entiteterna.

   <span class="preview">Exempelbild i förhandsvisningsmiljön:<span>

   ![Ta bort användare från resurspoolen](assets/remove-users-from-resource-pool.png)

   Exempelbild i produktionsmiljön:
   ![Sök i resurspoolen](assets/search-inside-new-resource-pool-350x314.png)

1. Klicka på x-ikonen på användarnivå för att ta bort en användare från resurspoolen. De tas bort från alla listor som de visas i.\
   eller\
   Om du vill ta bort alla användare som är associerade med en jobbroll, grupp, team eller företag klickar du på **Ta bort** på jobbrollen, gruppnivån eller företagsnivån. Detta tar bort alla användare som är associerade med den jobbrollen, gruppen, teamet eller företaget från resurspoolen.

1. Klicka på **Spara**.

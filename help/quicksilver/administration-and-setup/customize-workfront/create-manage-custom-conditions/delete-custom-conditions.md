---
title: Ta bort ett anpassat villkor
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Du kan ta bort anpassade villkor.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Ta bort ett anpassat villkor

Du kan ta bort ett anpassat villkor om det inte längre behövs.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Ta bort ett anpassat villkor

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Villkor**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Välj fliken för objekttypen (**Projekt**, **Aktivitet** eller **Problem**) där villkoret som du vill ta bort finns.

1. Håll pekaren över det villkor som du vill ta bort och klicka sedan på ikonen **Ta bort** ![](assets/delete.png) som visas längst till höger.
1. Klicka på **Ta bort villkor** i bekräftelsemeddelandet som visas.

1. I rutan **Ta bort villkor** som visas väljer du ett nytt villkor i listrutan för alla projekt som använder villkoret som du tar bort.

   Anpassade villkor är bara tillgängliga i listrutan om de motsvarar samma inbyggda villkor som det du tar bort. Om du t.ex. tar bort ett villkor som är lika med Vid risk, kan du bara välja anpassade villkor som också är lika med Vid risk.

1. Klicka på **Ta bort villkor**.

>[!NOTE]
>
>Du kan inte ta bort de inbyggda villkoren, som är On Target, At Risk och In Trouble. Du kan dock ändra deras namn och färger.

Mer information om anpassade villkor finns i [Anpassade villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

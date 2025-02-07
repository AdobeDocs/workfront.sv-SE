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
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '250'
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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort ett anpassat villkor

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Villkor**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Välj fliken för objekttypen (**Projekt**, **Aktivitet** eller **Problem**) där villkoret som du vill ta bort finns.

1. Håll pekaren över villkoret som du vill ta bort och klicka sedan på ikonen **Ta bort** ![Ta bort](assets/delete.png) som visas längst till höger.
1. Klicka på **Ta bort villkor** i bekräftelsemeddelandet som visas.

1. I rutan **Ta bort villkor** som visas väljer du ett nytt villkor i listrutan för alla projekt som använder villkoret som du tar bort.

   Anpassade villkor är bara tillgängliga i listrutan om de motsvarar samma inbyggda villkor som det du tar bort. Om du t.ex. tar bort ett villkor som är lika med Vid risk, kan du bara välja anpassade villkor som också är lika med Vid risk.

1. Klicka på **Ta bort villkor**.

>[!NOTE]
>
>Du kan inte ta bort de inbyggda villkoren, som är On Target, At Risk och In Trouble. Du kan dock ändra deras namn och färger.

Mer information om anpassade villkor finns i [Anpassade villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

---
title: Ge åtkomst till Adobe Workfront mål
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till Workfront-mål.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8639da14-d545-4f9a-894b-12c29699b0db
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Ge åtkomst till Adobe Workfront mål

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till Adobe Workfront-mål, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Åtkomstkrav

Du måste ha följande för att ge användare åtkomst till Workfront-mål:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Workfront-mål <p>Kontakta er kontoansvarige på Workfront för att få veta mer om en Workfront Goals-licens. </p> <p>Workfront Goals finns endast i den nya Adobe Workfront-upplevelsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration*</td> 
   <td> <p>Du måste ha åtkomstnivån Systemadministratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomstnivå du har.

Mer information om åtkomst till Workfront-mål finns i [Krav för att använda Workfront-mål](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

## Ge användare åtkomst till Workfront-mål med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på alternativet till höger om **Mål** som du vill använda för den här åtkomstnivån.

   ![](assets/edit-access-level-goals.png)

   >[!NOTE]
   >
   >Den externa licenstypen tillåter inte Visa eller Redigera åtkomst till Workfront-mål.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

## Tillgång till Workfront-mål per licenstyp

En Workfront-administratör kan använda en åtkomstnivå för att bevilja åtkomst till Workfront-mål för användare med en plan-, arbets-, begärande- eller granskningslicens.

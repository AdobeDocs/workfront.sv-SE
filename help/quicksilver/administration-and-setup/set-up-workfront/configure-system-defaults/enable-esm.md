---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivera Adobe Enterprise-lagring för din organisation
description: Du kan aktivera Adobe Enterprise-lagring för din organisation så att den kan använda en enhetlig lagringslösning för alla Adobe-produkter.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
source-git-commit: e70a65447fe508d055809271edad399d823f66dd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Aktivera Adobe Enterprise-lagring för din organisation

Adobe Enterprise-lagring är en enhetlig lagringslösning för alla Adobe-produkter. Det är en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter.

Adobe Enterprise-lagring är aktiverat som standard för nya kunder och kan aktiveras för befintliga kunder när avtalet förnyas.

Mer information om Adobe Enterprise-lagring finns i [Adobe Enterprise-lagringsöversikt](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara Workfront-administratör. </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivera Adobe Enterprise-lagring för din organisation

Så här aktiverar du Adobe Enterprise-lagring för din organisation:

{{step-1-to-setup}}

1. Välj **System** i den vänstra navigeringen och välj sedan **Inställningar**.
1. Bläddra ned till avsnittet **Lagringsinställningar**.
1. I listrutan Standard väljer du **Adobe Enterprise Storage**.
1. (Valfritt) Om du vill använda en kombination av Adobe Enterprise-lagring och äldre Workfront-lagring markerar du kryssrutan **Tillåt användare att välja lagringsprovider**.

   >[!NOTE]
   >
   >Om du aktiverar det här alternativet kan användarna välja lagringsleverantör när de skapar ett nytt projekt. Enterprise-lagring är märkt som&quot;Nytt projekt&quot; eftersom det är standardlagringsprovidern. Äldre Workfront-lagring är märkt som ett äldre projekt.
   >
   >![nya projekt och äldre projektalternativ](assets/new-esm-project.png)

1. Välj något av följande alternativ i listrutan Tillämpa på:

   - **Hela organisationen**: Med det här alternativet används standardlagringsprovidern i hela Workfront-miljön. När en användare skapar ett nytt projekt används standardlagringsprovidern.
   - **Specifika grupper**: Med det här alternativet används standardlagringsprovidern endast för specifika grupper i organisationen. När en användare i de angivna grupperna skapar ett nytt projekt används standardlagringsprovidern

1. Klicka på **Spara**.

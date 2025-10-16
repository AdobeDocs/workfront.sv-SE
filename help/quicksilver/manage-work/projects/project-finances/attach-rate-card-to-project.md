---
title: Koppla ett tariffkort till ett projekt
description: När du kopplar ett betalningskort till ett projekt läggs alla roller efter plats och deras associerade faktureringstaxor till i projektet.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Koppla ett tariffkort till ett projekt

{{highlighted-preview-article-level}}

Hastighetskort lagrar flera faktureringspriser per jobbroll, baserat på plats. Du kan vara Designer-baserad i Paris och en andra Designer-baserad i New York, var och en med olika faktureringstaxor. Det krävs dock ingen plats för jobbroller på ett tariffkort. En faktureringsfrekvens för en jobbroll (och eventuell plats) på ett kurskort kan även innehålla giltighetsdatum.

När du kopplar ett betalningskort till ett projekt läggs alla roller efter plats och deras associerade faktureringstaxor till i projektet.

>[!NOTE]
>
>Om du bifogar ett betalkort åsidosätts alla befintliga faktureringspriser för projektet.

Du kan redigera faktureringstarifferna direkt från tariffkortet i projektet. Detta påverkar inte de hastigheter som lagras på standardtariffkortet.

Mer information om hur du skapar tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Allmän information om hur du åsidosätter faktureringssatser för jobbroller för projekt och beräknar projektintäkter finns i [Översikt över åsidosättande av faktureringssatser för jobbroller och beräkning av intäkter för ett projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Administrativ åtkomst för jobbroller</p></td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för det projekt som innehåller Redigera ekonomiska data </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Koppla ett tariffkort till ett projekt

1. Gå till projektet.
1. Klicka på **Faktureringstariffer** i den vänstra panelen.
1. Klicka på **Lägg till faktureringstakt > Koppla ett tariffkort**.

   Sidan Bifoga ett tariffkort öppnas. Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Välj det tariffkort som ska läggas till i projektet och klicka på **Bifoga**.

   Kurskortet och alla dess rollpriser för jobb läggs till i faktureringsrabattlistan.

   ![Gradkort tillagt i projekt](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >I faktureringsrabattlistan kan du ta bort en eller flera jobbroller som kommer från ett betalkort. Om du tar bort en faktureringsfrekvens för en jobbroll från projektet tas den inte bort från standardtariffkortet.

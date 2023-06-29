---
title: Koppla ett tariffkort till ett projekt
description: När du kopplar ett betalningskort till ett projekt läggs alla roller efter plats och deras associerade faktureringstaxor till i projektet.
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Koppla ett tariffkort till ett projekt

{{highlighted-preview-article-level}}

Hastighetskort lagrar flera faktureringspriser per jobbroll, baserat på plats. Du kan ha en jobbroll som Designer baserad i Paris och en andra Designer baserad i New York, där alla har olika faktureringstaxor. Det krävs dock ingen plats för jobbroller på ett tariffkort. En faktureringsfrekvens för en jobbroll (och eventuell plats) på ett kurskort kan även innehålla giltighetsdatum.

När du kopplar ett betalningskort till ett projekt läggs alla roller efter plats och deras associerade faktureringstaxor till i projektet.

>[!NOTE]
>
>Om du bifogar ett betalkort åsidosätts alla befintliga faktureringspriser för projektet.

Du kan redigera faktureringstarifferna direkt från tariffkortet i projektet. Detta påverkar inte de hastigheter som lagras på standardtariffkortet.

Mer information om hur du skapar tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Allmän information om hur du åsidosätter faktureringssatser för jobbroller för projekt och beräknar projektintäkter finns i [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Standard</p><p>eller</p><p>Äldre plan: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Administrativ åtkomst för jobbroller</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Koppla ett tariffkort till ett projekt

1. Gå till projektet.
1. Klicka **Faktureringstaxor** i den vänstra panelen. Du måste kanske först klicka **Visa fler**.
1. Klicka **Lägg till faktureringstakt > Koppla ett tariffkort**.

   Sidan Bifoga ett tariffkort öppnas. Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Välj det tariffkort som ska läggas till i projektet och klicka på **Bifoga**.

   Kurskortet och alla dess rollpriser för jobb läggs till i faktureringsrabattlistan.

   ![Kurskort som lagts till i projekt](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >I faktureringsrabattlistan kan du ta bort en eller flera jobbroller som kommer från ett betalkort. Om du tar bort en faktureringsfrekvens för en jobbroll från projektet tas den inte bort från standardtariffkortet.


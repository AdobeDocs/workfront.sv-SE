---
title: Koppla ett tariffkort till ett projekt
description: När du kopplar ett betalningskort till ett projekt läggs alla roller efter plats och deras associerade faktureringstaxor till i projektet.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Koppla ett tariffkort till ett projekt

Hastighetskort lagrar flera faktureringsfrekvenser per jobbroll, baserat på attribut. Du kan till exempel ha en befattning som Designer baserad i Paris för byrå A, en annan Designer baserad i Paris för byrå B och en tredje Designer baserad i New York som inte tilldelats någon byrå, var och en med olika faktureringstaxor. Attribut krävs dock inte för jobbroller på ett tariffkort. Attributen fungerar som verktyg för att fastställa mer detaljerade frekvenser. En faktureringstaxa på ett betalkort kan också vara giltighetsdatum, så att priset börjar och slutar på angivna datum.

När du bifogar ett betalkort till ett projekt läggs alla roller och tillhörande faktureringstaxor till i projektet.

>[!NOTE]
>
>Om du bifogar ett betalkort åsidosätts alla befintliga faktureringspriser för betalkort i projektet. Åsidosättningar av faktureringsfrekvens som lades till direkt i projektet tas inte bort.

Mer information om hur du skapar tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Allmän information om hur du åsidosätter faktureringstaxor för jobbroller för projekt och beräknar projektintäkter finns i [Översikt över åsidosatta faktureringstariffer och beräkning av intäkter för ett projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt, ekonomiska data och tariffkort</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter till projektet med behörighet att redigera faktureringstariffer</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Koppla ett tariffkort till ett projekt

1. Gå till projektet.
1. Klicka på **Priser** i den vänstra panelen och välj sedan **Fakturering**.
1. Klicka på **Lägg till faktureringstakt > Koppla ett tariffkort**.

   Rutan **Koppla ett tariffkort** öppnas. Du kan söka efter ett kurskort i listan.

   ![Koppla en tariffkortsruta](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >Grupp och företag på priskortet används som filter i den här listan. Eftersom projekt även innehåller fält för grupper och företag använder Workfront dessa värden för att begränsa listan med tillgängliga kort till dem som är relevanta för projektets sammanhang, och inte alla tariffkort i hela systemet.
   >
   >Matchen behöver inte vara exakt. Klassificeringskort med tomma värden för Grupp och/eller Företag kan fortfarande visas beroende på projektets Group/Company-konfiguration. Om till exempel ett projekt har en Grupp vald men företaget är tomt, kan du se priskort som är kopplade till den gruppen även om priskortets företag är ett annat eller tomt.

1. Välj det tariffkort som ska läggas till i projektet och klicka på **Bifoga**.

   Kurskortet och alla dess rollpriser för jobb läggs till i faktureringsrabattlistan.

   ![Gradkort tillagt i projekt](assets/rate-card-on-project.png)

## Ta bort ett tariffkort från ett projekt

När du tar bort ett kurskort från ett projekt tas alla dess jobbrollfrekvenser bort. Du kan inte ta bort en individuell avgift från projektet som kommer från ett tariffkort.

Åsidosättningar av faktureringsfrekvens för användare eller jobbroller som har lagts till direkt i projektet kan tas bort utan att hela avgiftskortet tas bort.

1. Gå till projektet.
1. Klicka på **Priser** i den vänstra panelen och välj sedan **Fakturering**.
1. Klicka på ikonen **Ta bort** ![Ta bort](assets/remove-icon.png).
1. Klicka på **Bekräfta** i bekräftelsemeddelandet för att ta bort tariffkortet.


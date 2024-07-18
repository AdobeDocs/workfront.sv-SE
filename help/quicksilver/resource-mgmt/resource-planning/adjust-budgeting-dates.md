---
product-area: resource-management
navigation-topic: resource-planning
title: Justera budgeteringsdatum i resursplaneraren
description: Om du upptäcker att det finns överbeläggningar av dina resurser efter att du har budgeterat dem i Resursplaneraren kan du utforska dessa scenarier genom att flytta budgeterade timmar, heltidsekvivalenter eller kostnader till en annan tidsram. Baserat på resultatet i dessa scenarier kan du sedan justera dina budgeterade timmar, heltidsekvivalenter eller kostnad.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Justera budgeteringsdatum i resursplaneraren

Om du upptäcker att det finns överbeläggningar av dina resurser efter att du har budgeterat dem i Resursplaneraren kan du utforska dessa scenarier genom att flytta budgeterade timmar, heltidsekvivalenter eller kostnader till en annan tidsram. Baserat på resultatet i dessa scenarier kan du sedan justera dina budgeterade timmar, heltidsekvivalenter eller kostnad.

Överbeläggningar kan uppstå när resurserna för budgeterade timmar, heltidsekvivalenter eller kostnader är högre än deras tillgängliga timmar, heltidsekvivalenter eller kostnader. Detta genererar ett negativt nettovärde.

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
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Redigera prioriteringar och budgettimmar i Resursplanering</p> <p>Redigera åtkomst till finansiella data, projekt och användare</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för de projekt som du vill budgetera information för med möjlighet att hantera finanser</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Justera budgetdatum

1. Gå till resursplaneraren och välj **Visa efter projekt**.

   >[!NOTE]
   >
   >Du kan bara använda alternativet Justera budgeterade datum när du visar resursplaneraren efter projekt.

1. Håll muspekaren över namnet på ett projekt och klicka sedan på menyn **Mer** .
1. Klicka på **Justera budgetdatum**.\
   Tidslinjen för projektallokering visas.\
   Tidsperioden där timmarna för närvarande budgeteras är orange om det finns en budgeteringskonflikt och blå om det inte finns några konflikter.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Dra och släpp den markerade tidsramen till en annan tidpunkt för att förstå var det inte finns några budgeteringskonflikter för det valda projektet. När du hittar en tidsram där nettovärdet är positivt ändras den markerade tidsramen till blå.
1. Klicka på&quot;x&quot; i det övre högra hörnet av tidslinjen för projekttilldelning för att stänga den.
1. Ta bort budgeterade timmar från den befintliga tidslinjen i projektet och lägg till dem på tidslinjen som visar den mest tillgängliga tiden.
1. Klicka på **Spara**.
1. (Villkorligt och valfritt) Om tidsramarna utan budgeteringskonflikter ligger utanför tidslinjen för projektet klickar du på namnet på projektet för att få åtkomst till projektet.
1. (Villkorligt och valfritt) Klicka på **Redigera projekt** och redigera sedan **Planerat startdatum** eller **Planerat slutförandedatum** för att ändra tidslinjen för projektet för tidsperioden utan budgeteringskonflikter.\
   Mer information om hur du redigerar projekt finns i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Villkorligt och valfritt) Klicka på **Spara ändringar**.
1. Gå tillbaka till resursplaneraren och ange budgeterade timmar, heltidsekvivalenter eller kostnader igen i tidsramen utan budgeteringskonflikter.
1. Klicka på **Spara**.

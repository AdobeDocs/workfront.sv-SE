---
product-area: projects
navigation-topic: financials
title: Hantera projektutgifter
description: Processen för att skapa och hantera utgifter är densamma för både projekt- och uppgiftsrelaterade utgifter. Alla utgifter som läggs till i projektet i affärsärendet läggs till på fliken Utgifter som planerade utgifter. Mer information om affärsärendet finns i artikeln Skapa ett affärsärende för ett projekt.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Hantera projektutgifter

Processen för att skapa och hantera utgifter är densamma för både projekt- och uppgiftsrelaterade utgifter. Alla utgifter som läggs till i projektet i affärsärendet läggs till på fliken Utgifter som planerade utgifter. Mer information om affärsärendet finns i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Det totala beloppet för dina utgifter för alla uppgifter och projektet bidrar till den totala kostnaden för projektet. Det planerade beloppet för utgifterna bidrar till projektets planerade kostnad och det faktiska beloppet för utgifterna bidrar till projektets faktiska kostnad.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Arbete eller högre</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td>Redigera åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Contribute eller högre behörigheter för projektet med behörighet att visa eller hantera ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till utgifter

1. Gå till projektet där du vill ange utgifter.\
   Om du vill lägga till utgifter för en uppgift navigerar du till en uppgift i stället.
1. Klicka på **Utgifter** i den vänstra panelen.
1. Klicka på **Lägg till en utgift**.
Dialogrutan **Lägg till en utgift** visas.
1. Uppdatera följande:

   * **Beskrivning:** Beskrivning av utgiften.
   * **Utgiftstyp:** (obligatoriskt) Välj den kategori som bäst beskriver utgiften.
   * **Aktivitet:** Börja skriva namnet på aktiviteten som utgiften är associerad med och klicka sedan på den när den visas i listrutan.
   * **Planerat belopp:** Det planerade budgeterade beloppet för utgiften.\
     Detta påverkar projektets budgeterade kostnad.

   * **Faktiskt belopp:** Det belopp som den faktiska kostnaden för utgiften uppgår till.\
     Detta påverkar projektets faktiska kostnad.

   * **Planerat datum:** Det förväntade datumet för utgiften. Du kan skriva datumet i fältet med formatet *mm/dd/åå* eller klicka på kalenderikonen  ![Kalenderikon](assets/calendar-icon.png) och välj datumet dynamiskt.

   * **Betalningsdatum:** Datumet då utgiften betalades.
   * **Fakturerbar:** Välj det här alternativet om du vill fakturera den här utgiften. Det är viktigt att kategorisera en utgift som fakturerbar när du skapar faktureringsposter.
   * **Återbetalningsbar:** Välj det här alternativet om utgiften behöver återbetalas. Du kan sedan markera utgiften som återbetald när utgiften har återbetalats.

1. Välj ett **anpassat formulär** och ange eventuell ytterligare information som krävs. Du måste skapa ett anpassat formulär innan du kan koppla det till en utgift. Endast aktiva anpassade formulär visas i listan. Mer information om hur du skapar anpassade formulär finns i artikeln [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på **Spara ändringar**.

## Ta bort utgifter

1. Gå till projektet där du vill ta bort utgifter.
1. Klicka på **Utgifter** i den vänstra panelen.
1. Markera de utgifter du vill ta bort och klicka sedan på **Ta bort** ![Ta bort](assets/delete.png).
1. Klicka på **Ja, ta bort** för att bekräfta borttagningen.

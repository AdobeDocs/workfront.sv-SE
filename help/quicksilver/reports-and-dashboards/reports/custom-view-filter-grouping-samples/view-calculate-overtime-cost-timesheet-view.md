---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: beräkna övertidskostnad i en tidrapportvy'
description: Övertid beräknas inte som standard i Adobe Workfront, men du kan skapa en tidrapport som beräknar övertid.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Visa: beräkna övertidskostnad i en tidrapportvy

Övertid beräknas inte som standard i Adobe Workfront, men du kan skapa en tidrapport som beräknar övertid.

Om användaren är kopplad till en kostnad per timme i sin profil kan du även beräkna kostnadsbeloppet för den användarens övertid.\
Mer information om hur du associerar användare med kostnad per timme finns i artikeln [Konfigurera mina inställningar](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Fältet Övertid som du kan lägga till i en tidrapportvy i en lista eller rapport visar informationen som finns i fältet Övertid i tidrapporten. Den här informationen uppdateras manuellt av en användare som har behörighet att ändra tidrapporten. Mer information om fältet Övertid i en tidrapport finns i artikeln [Översikt över tidrapportslayouten](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Beräkna övertidskostnad i en tidrapportvy

Så här lägger du till en beräknad övertidskolumn i en tidrapportvy:

1. Gå till en lista med tidrapporter eller skapa en tidrapport.

   Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klicka på **Anpassa vy** i en lista över tidrapporter.

   eller

   Välj fliken **Kolumner (Visa)** i en tidrapportrapport.

1. Klicka på **Lägg till kolumn**.
1. Klicka på **Växla till textläge**.
1. Klicka på **Klicka för att redigera text** i området **Visa i den här kolumnen**.
1. Kopiera och klistra in följande textlägeskod i dialogrutan **Textläge**.
   <pre>displayname=Calculated Overtime Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>värdeformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >I den här beräkningen antas att användaren vanligtvis arbetar en 40-timmarsvecka.

1. Klicka på **Spara**, ge den nya vyn ett namn och klicka sedan på **Spara vy** i en lista över tidrapporter.

   eller

   Klicka på **Spara + stäng** i en tidrapportrapport.

1. (Valfritt och villkorligt) Om du skapar en tidrapportrapport anger du ett namn för rapporten och klickar sedan på **Spara rapport**.

   Kostnaden för övertid för varje användare visas i kolumnen **Beräknad övertidskostnad** .

   ![calculate_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

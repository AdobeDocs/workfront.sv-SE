---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Använd rapporten för godkännande av korrektur
description: Du kan använda rapporten för godkännande av korrektur för att visa information om korrektur i din miljö.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Använd rapporten för godkännande av korrektur

Du kan använda rapporten för godkännande av korrektur för att visa information om korrektur i din miljö.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Översikt över Adobe Workfront-licenser*</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Åtkomstnivå*</strong> </td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Använd rapporten för godkännande av korrektur

{{step1-to-reports}}

1. Klicka på **Ny rapport** och rulla sedan för att välja **Korrekturgodkännande**.

   ![Rapport om godkännande av korrektur](assets/proof-approval-report.png)

1. (Valfritt) Lägg till ytterligare fält.
1. Klicka på **Spara + Stäng**.

## Ytterligare fält

Du kan lägga till följande fält i korrekturrapporten:

* **Beslutsdatum**: Visar det datum då en godkännare fattar ett beslut om ett bevis. Det här datumet finns också på sidan Skriv ut sammanfattning av korrekturet.
* **Godkännarstadium**: Visar aktuell sceninformation.
* **Arbetsflödesmall**: Visar alla arbetsflödesmallar som är kopplade till korrekturet. Om ingen mall är kopplad är kolumnen tom.
* **Väntar på beslut**: Visar sant för att signalera att ett beslut inte har uppfyllts för den senaste versionen när följande är sant:

   * Beviset har inte arkiverats
   * Den fas som godkännaren är aktiv
   * Beviset väntar på godkännande

* **Korrekturdeadline**: Visar korrekturens deadline. Alla faser måste ha en tilldelad tidsgräns för att det här fältet ska kunna fyllas i. Fältet visar tidsgränsen för den senast aktiverade fasen.

 

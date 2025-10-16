---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Använd rapporten för godkännande av korrektur
description: Du kan använda rapporten för godkännande av korrektur för att visa information om korrektur i din miljö.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Använd rapporten för godkännande av korrektur

Du kan använda rapporten för godkännande av korrektur för att visa information om korrektur i din miljö.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront package</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licens</p> </td> 
   <td> 
   <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong> </td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

 

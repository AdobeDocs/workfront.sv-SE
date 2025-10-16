---
title: Visa information om användarinloggning
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan se hur ofta användare loggar in på Workfront, liksom den senaste gången de loggade in, genom att ange att du vill inkludera informationen i en lista över användare eller i en rapport för användare.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Visa inloggningsinformation för användare

Du kan se hur ofta användare loggar in på Adobe Workfront, liksom den senaste gången de loggade in, genom att ange att du vill inkludera informationen i en lista över användare eller i en rapport för användare.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hur Workfront registrerar inloggningsinformation

Workfront registrerar följande information om användare som loggar in på systemet:

* **Inloggningsantal**: Workfront räknar en användare som loggar in i programmet en gång var 24:e timme. Om en användare loggar in flera gånger med olika webbläsare, datorer eller mobila enheter räknas alla inloggningar som sker en dag som en inloggning i Workfront. Inloggningsantalet innehåller information som börjar med när användaren skapades.
* **Senaste inloggningsdatum**: Det senaste datumet när en användare loggade in. Datumet för varje inloggning från en webbläsare, mobil enhet eller andra program registreras i det här fältet.

Logga in på Workfront på något av följande sätt som en inloggning på Workfront:

* Workfront webbprogram
* Workfront mobilappar (iOS- eller Android-enheter)
* Alla Workfront-integreringar som stöds med andra program från tredje part (som Slack)
* Anpassad integrering mellan Workfront och andra program från tredje part.
* WORKFRONT API

  >[!NOTE]
  >
  >Logga in på Workfront via Workfront API är endast tillgängligt för organisationer som ännu inte har anslutit sig till Adobe Business Platform.

## Visa användningsinformation i en användarlista eller rapport

Du kan visa fälten Antal inloggningar och Senaste inloggningsdatum i en lista över användare eller i en rapport för användare.\
Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Så här visar du användningsinformation i en lista över användare:

1. Gå till en lista över användare i Workfront.
1. Välj **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** i skärmens nedre högra hörn.
1. I fältet **Visa i den här kolumnen** börjar du skriva **Inloggningsantal** och markerar det när det visas i listan under **Användare**.

1. Klicka på **Lägg till kolumn** igen.
1. I fältet **Visa i kolumnen** börjar du skriva **Senaste inloggningsdatum** och markerar det när det visas i listan under **Användare**.

1. (Valfritt) Klicka på **Avancerade alternativ** och välj sedan ett **fältformat** i listrutan för att inkludera tid eller veckodag för den senaste inloggningen i kolumnen.

1. Klicka på **Spara vy**.\
   Vyn innehåller information om hur många gånger användarna har loggat in och när de senast loggade in.

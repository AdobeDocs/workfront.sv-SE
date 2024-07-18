---
title: Visa inloggningsinformation för användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan se hur ofta användare loggar in på Workfront, liksom den senaste gången de loggade in, genom att ange att du vill inkludera informationen i en lista över användare eller i en rapport för användare.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Visa inloggningsinformation för användare

Du kan se hur ofta användare loggar in på Adobe Workfront, liksom den senaste gången de loggade in, genom att ange att du vill inkludera informationen i en lista över användare eller i en rapport för användare.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om användaren <b>Admin (gruppanvändare)</b> är aktiverad måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om inställningen <b>Användare</b> på en åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Hur Workfront registrerar inloggningsinformation

Workfront registrerar följande information om användare som loggar in på systemet:

* **Inloggningsantal**: Workfront räknar en användare som loggar in i programmet en gång var 24:e timme. Om en användare loggar in flera gånger med olika webbläsare, datorer eller mobila enheter räknas alla inloggningar som sker en dag som en inloggning i Workfront. Inloggningsantalet innehåller information som börjar med när användaren skapades.
* **Senaste inloggningsdatum**: Det senaste datumet när en användare loggade in. Datumet för varje inloggning från en webbläsare, mobil enhet eller andra program registreras i det här fältet.

Logga in på Workfront på något av följande sätt som en inloggning på Workfront:

* Workfront webbprogram
* Workfront mobilappar (iOS- eller Android-enheter)
* Alla Workfront-integreringar som stöds med andra program från tredje part (Slack, Jira)
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

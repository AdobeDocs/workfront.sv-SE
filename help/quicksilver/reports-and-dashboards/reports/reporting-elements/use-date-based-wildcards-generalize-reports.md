---
product-area: reporting
navigation-topic: reporting-elements
title: Generera rapporter med datumbaserade jokertecken
description: Du kan generera en rapport genom att använda jokertecken i stället för specifik information när du skapar vissa rapportelement.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Generera rapporter med datumbaserade jokertecken

Du kan generera en rapport genom att använda jokertecken i stället för specifik information när du skapar vissa rapportelement.

Om du till exempel vill skapa en rapport som visar uppgifter med ett visst planerat startdatum kan du använda kalenderdatumväljaren i ett filter för att välja ett specifikt datum. Om du vill skapa en rapport som visar uppgifter som har det planerade startdatumet inom en viss tidsram från det datum då rapporten öppnas, kan du använda ett jokertecken som anger att när någon visar rapporten visas information under en tidsram som är relevant för den tidpunkt då rapporten visas.

Exempel: under den senaste veckan, under det senaste året, under de kommande två veckorna, osv. På så sätt skapar du rapporten en gång, men eftersom du använder ett jokertecken i filtret skapas olika resultat varje gång någon läser den, eftersom den anpassas till dagen då rapporten körs.

Du kan använda datumbaserade jokertecken när du skapar följande rapportelement:

* Filter
* Anpassade uppmaningar
* Vyer när regler för kolumner läggs till

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera rapportelement i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera rapportelement i en rapport</p> <p>Hantera behörigheter till en vy eller ett filter för att redigera dem</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste skapa en rapport innan du kan lägga till jokertecken i den.

Mer information om hur du skapar en rapport finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Instruktioner

Infoga ett datumbaserat jokertecken i en rapport:

1. Gå till en rapport som du vill infoga ett datumbaserat jokertecken för.
1. Klicka på **Rapportera åtgärder** och sedan på **Redigera**.
1. Klicka på fliken **Filter**.
1. Klicka på **Lägg till en filterregel**.
1. Börja skriva namnet på fältet som du vill filtrera efter.\
   Du måste skriva fält som refererar till ett datum.
1. Välj **Lika med** i listrutan för filtervariabeln.

   >[!TIP]
   >
   >Du måste alltid markera filtervariabeln **Lika med** när du arbetar med jokertecken i Adobe Workfront.

1. Klicka på växlingsknappen **Ange relativt datum** och skriv sedan `$$TODAY` i textrutan om du vill visa information om något som inträffar samma dag som rapporten körs.

   eller

   Skriv `$$NOW` om du vill visa information om något som inträffar vid samma datum och tid som rapporten körs.

   Det här datumet är alltid annorlunda eftersom det ändras med det datum som rapporten faktiskt visas av en användare. så informationen i rapporten skiljer sig från dag till dag.

1. (Valfritt) Om du vill visa information som inträffar inom en tidsram efter datumet när rapporten körs skriver du `$$TODAY+1w` om du vill visa information nästa vecka eller `$$TODAY+2m` om du vill visa information under de kommande två månaderna. Du kan också ange tidsramar för kvartal, timmar, dagar eller år.
1. (Valfritt) Om du vill visa information om något som har inträffat inom en tidsram före datumet då rapporten körs skriver du `$$TODAY-1w` om du vill visa information från föregående vecka eller `$$TODAY-2m` om du vill visa information från de senaste två månaderna. Du kan också ange tidsramar för kvartal, timmar, dagar eller år.

   En fullständig lista över attribut, kvalificerare och operatorer som du kan använda i datumbaserade jokertecken finns i artikeln [Översikt över variabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicka på **Spara + Stäng**.

## Ytterligare information

Se även:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Översikt över filtervariabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Skapa eller redigera filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Lägg till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

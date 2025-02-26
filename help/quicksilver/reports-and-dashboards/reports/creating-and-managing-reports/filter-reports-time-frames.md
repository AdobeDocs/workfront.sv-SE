---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrera rapporter efter tidsramar
description: Du kan filtrera en rapport efter tidsramen för ett datum som finns i ett objekt. Du kan t.ex. filtrera en timrapport för en viss tidsram när timmarna angavs.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# Filtrera rapporter efter tidsramar

<!-- Audited: 11/2024 -->

Du kan filtrera en rapport efter tidsramen för ett datum som finns i ett objekt. Du kan t.ex. filtrera en timrapport för en viss tidsram när timmarna angavs.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
      <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Rapporten måste skapas innan du kan filtrera resultaten.

Mer information om hur du skapar rapporter finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrera en rapport efter tidsramen för ett datum {#filter-a-report-by-the-time-frame-of-a-date}

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) och klicka sedan på **Rapportering**.

1. Klicka på **Ny rapport** och välj sedan önskad rapporttyp.\
   Välj till exempel **Timrapport**.

1. Välj fliken **Filter**.
1. Klicka på **Lägg till en filterregel** och välj sedan **Timinmatningsdatum**.\
   ![Filtrerar timrapport efter tidsram](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Välj något av följande alternativ i den nedrullningsbara menyn:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Likvärdigt (skiftlägeskänsligt)</td> 
      <td>När du har valt den här modifieraren anger du datumet då timmarna angavs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inte lika med (skiftlägeskänslig)</td> 
      <td>När du har valt den här modifieraren anger du datumet när timmarna angavs, så att det datumet inte tas med i rapporten. Rapporten visar timmar som loggats in på alla datum, förväntat för det datum du angav.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Välj den här modifieraren om du bara vill visa timmar där transaktionsdatumet saknas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inte null</td> 
      <td>Välj den här modifieraren om du bara vill visa timmar där bokföringsdatumet har ett värde.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mellan</td> 
      <td>När du har valt den här modifieraren anger du ett datumintervall när timmarna angavs. Rapporten visar antal timmar som angetts mellan de angivna datumen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mindre än</td> 
      <td>När du har valt den här modifieraren anger du ett datum före vilket timmarna angavs. I rapporten visas timmar som angetts före det angivna datumet och inte det angivna datumet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mindre än lika med</td> 
      <td>När du har valt den här modifieraren anger du ett datum före vilket timmarna angavs. Rapporten visar timmar som angetts före det angivna datumet, inklusive det angivna datumet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Större än</td> 
      <td>När du har valt den här modifieraren anger du ett datum efter vilket timmarna angavs. I rapporten visas timmar som angetts efter det angivna datumet och inte det angivna datumet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Större än lika</td> 
      <td> <p>När du har valt den här modifieraren anger du ett datum efter vilket timmarna angavs. Rapporten visar timmar som angetts efter det angivna datumet, inklusive det angivna datumet.</p> <p>Välj någon av de inbyggda modifieringarna för tidsbildrutor, vilket beskrivs i <a href="#built-in-time-frame-modifiers" class="MCXref xref">Inbyggda modifierare för tidsbildrutor</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dessa modifierare är tillgängliga för alla datumfält i ett filter eller en uppmaning i en rapport.
1. Klicka på **Spara + Stäng**.

## Inbyggda modifierare för tidsramar {#built-in-time-frame-modifiers}

Adobe Workfront har inbyggda modifierare för tidsramar som du kan använda utan att definiera ett visst datum.

Dessa modifierare är tillgängliga för alla datumfält i ett filter eller en uppmaning i en rapport.

Mer information om hur du filtrerar en rapport efter en tidsram som är associerad med ett datum finns i avsnittet ovan [Filtrera en rapport efter tidsramen för ett datum](#filter-a-report-by-the-time-frame-of-a-date).

Om du till exempel skapar en timrapport och vill visa timmar som anges i en viss tidsram kan du välja bland följande inbyggda alternativ för tidsramsfilter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Idag</td> 
   <td>Visar timmar där anmälningsdatumet är idag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Den här veckan</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i den aktuella veckan, där veckan börjar på en söndag och slutar på en lördag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nästa vecka</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i veckan efter den aktuella veckan, där veckan börjar på en söndag och slutar på en lördag. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Förra veckan</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i veckan före den aktuella veckan, där veckan börjar på en söndag och slutar på en lördag. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Den här månaden</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i den aktuella månaden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nästa månad</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i månaden efter den aktuella månaden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Förra månaden</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i månaden före den aktuella månaden</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Detta kvartal</td> 
   <td> <p>Visar timmar där anmälningsdatumet är ett datum i det aktuella kvartalet, där kvartal definieras som:</p> 
    <ul> 
     <li>Första kvartalet: 1 januari - 30 mars</li> 
     <li>Andra kvartalet: 1 april - 30 juni</li> 
     <li>Tredje kvartalet: 1 juli - 30 september</li> 
     <li>Fjärde kvartalet: 1 oktober - 31 december</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nästa kvartal</td> 
   <td>Visar timmar där transaktionsdatumet är ett datum i kvartalet efter det aktuella kvartalet, där kvartal definieras ovan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sista kvartalet</td> 
   <td> <p>Visar timmar där anmälningsdatumet är ett datum under det kvartal som föregår det aktuella kvartalet, där kvartal definieras ovan.</p> <p>Obs! Om din Workfront-administratör har aktiverat och definierat anpassade kvartal för ditt system, ersätts de inbyggda filtren för kvartal med din anpassade kvartalsinformation. Mer information om att aktivera anpassade kvartal finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Aktivera anpassade kvartal för projekt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Detta år</td> 
   <td>Visar timmar där anmälningsdatumet är ett datum i det aktuella året, där det aktuella året börjar den 1 januari och slutar den 31 december.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Senaste året</td> 
   <td>Visar timmar där transaktionsdatumet är ett datum under det föregående året, där det föregående året börjar 12 månader före det aktuella datumet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Förra året</td> 
   <td> <p>Visar timmar där anmälningsdatumet är ett datum i det sista året, där det sista året börjar den 1 januari och slutar den 31 december året före det aktuella året.</p> <p>Obs! Det finns ingen inbyggd tidsperiod för räkenskapsåret. Du kan skapa en rapport och filtrera informationen efter datum med en anpassad modifierare för räkenskapsårets datumintervall, så som det definieras i din organisation. Om du vill välja en tidsram för ett räkenskapsår på plats bör du använda en uppmaning i stället för ett filter. </p> </td> 
  </tr> 
 </tbody> 
</table>

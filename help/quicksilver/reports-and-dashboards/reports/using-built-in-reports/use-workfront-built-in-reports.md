---
product-area: reporting
navigation-topic: using-built-in-reports
title: Använd inbyggda rapporter från Adobe Workfront
description: Adobe Workfront har en omfattande lista över inbyggda rapporter som är klara att användas. Workfront-administratörer kan dölja inbyggda rapporter så att användare inte har tillgång till dem.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '2964'
ht-degree: 0%

---

# Använd inbyggda rapporter från Adobe Workfront

<!--Audited: 11/2024-->

Adobe Workfront har en omfattande lista med inbyggda rapporter som du kan använda.

Workfront-administratörer kan dölja inbyggda rapporter så att användare inte har tillgång till dem.

Mer information om hur du döljer inbyggda rapporter finns i [Dölj inbyggda rapporter](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Medarbetare eller högre</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Begäran eller senare</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Visa eller öka åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport för att lägga till eller redigera ett filter i en rapport</p> <p>Hantera behörigheter för ett filter för att redigera det i en lista</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över inbyggda rapporter {#overview-of-built-in-reports}

Du kan anpassa en inbyggd rapport och spara den som en ny rapport. Mer information om hur du anpassar inbyggda rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Följande rapporter innehåller Workfront-paketet. Rapporterna är tillgängliga för alla användare som har minst behörighet att visa inbyggda rapporter på åtkomstnivå.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Rapportnamn</strong> </th> 
   <th><strong>Rapportbeskrivning</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Faktisk kostnad per program för Portfolio</td> 
   <td>En projektrapport som visar projektens planerade kostnad och faktiska kostnad. Rapporten grupperas efter programnamn, visas med Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktisk Portfolio kostnad per projekt</td> 
   <td>En projektrapport som visar projektens planerade kostnad och faktiska kostnad. Rapporten grupperas efter projektnamn, visas med namnet på Portfolio och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktisk omsättning för Portfolio per program</td> 
   <td>En projektrapport som visar projektens planerade intäkter och faktiska intäkter. Rapporten grupperas efter programnamn, visas med Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktisk omsättning för Portfolio per projekt</td> 
   <td>En projektrapport som visar projektens planerade intäkter och faktiska intäkter. Rapporten grupperas efter projektnamn, visas med namnet på Portfolio och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktisk intäkt per företag</td> 
   <td>En projektrapport som visar projektens faktiska inkomster och företag. Rapporten grupperas efter företagsnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktisk intäkt per grupp</td> 
   <td>En projektrapport som visar Faktisk omsättning och Grupp för projekten. Rapporten grupperas efter gruppnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Alla öppna tidrapporter</td> 
   <td>En tidrapportrapport som visar öppna tidrapporter. Rapporten innehåller följande fält: Datumintervall, Ägarnamn, Totalt antal timmar, Övertid, Godkännarens namn och Status för tidrapporterna.</td> 
  </tr> 
  <tr> 
   <td>Tidrapporter för godkännande (visas)</td> 
   <td>En tidrapportrapport som visar skickade eller avvisade tidrapporter med godkännare. Rapporten innehåller följande fält: Datumintervall, Ägare, Totalt antal timmar, Övertid, Godkännarens namn och Status för tidrapporterna. Rapporten visas av: Startdatum för tidrapport, Slutdatum för tidrapport, Godkännarnamn för tidrapport och Användarnamn.</td> 
  </tr> 
  <tr> 
   <td>Riskprojekt</td> 
   <td>En projektrapport som visar aktuella projekt och planeringsprojekt med ett villkor för risk eller i problem. Rapporten innehåller följande fält: Beskrivning, Planerat slutförandedatum, Planerat slutförandedatum, Procent slutfört, Status och Prioritet för projekten. Rapporten grupperas efter Portfolio Name.</td> 
  </tr> 
  <tr> 
   <td>Faktureringsintäkt per företag</td> 
   <td>En projektrapport som visar projektets företags- och faktureringsintäkter. Rapporten grupperas efter företagsnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktureringsintäkt per grupp</td> 
   <td>En projektrapport som visar Faktureringsintäkter och Grupp för projekten. Rapporten grupperas efter gruppnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Faktureringsintäkt per månad</td> 
   <td>En faktureringspostrapport som visar projektnamn, projektfaktureringsintäkt och faktureringsdatum för faktureringsposterna. Rapporten grupperas efter månaden för faktureringsdatumet för faktureringsposterna och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Slutförda problem per vecka</td> 
   <td>En problemrapport som visar det faktiska slutförandedatumet för problemen. Rapporten grupperas efter veckan för det faktiska slutförandedatumet för problemen och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Slutförda problem per vecka och användare</td> 
   <td>En problemrapport som visar det faktiska slutförandedatumet och tilldelningarna för problemen. Rapporten grupperas efter den primära tilldelaren och efter veckan för det faktiska slutförandedatumet för problemen, och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Aktuella projekt</td> 
   <td>En projektrapport som visar alla aktuella projekt. Rapporten innehåller följande fält: Beskrivning, Planerat slutförandedatum, Planerat slutförandedatum, Procent slutfört, Status och Prioritet för projekten.</td> 
  </tr> 
  <tr> 
   <td>Timkostnader per användare per månad</td> 
   <td>En matristimrapport som visar antalet loggade timmar och deras faktiska kostnad. Rapporten grupperas efter ägarnamn och månaden för anmälningsdatumet för timmarna.</td> 
  </tr> 
  <tr> 
   <td>Timmar efter användare</td> 
   <td>En timrapport som visar antalet loggade timmar. Rapporten grupperas efter ägarnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Timmar efter användare per vecka</td> 
   <td>En matristimrapport som visar antalet loggade timmar de senaste fyra veckorna och anmälningsdatumet för timmarna. Rapporten får ett meddelande om timmens anmälningsdatum och grupperas efter ägarnamn och månaden för anmälningsdatumet för timmarna.</td> 
  </tr> 
  <tr> 
   <td>Problem efter status</td> 
   <td>En problemrapport som visar status för problem. Rapporten grupperas efter status för utgåvorna och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Problem efter status och projekt</td> 
   <td>En matrisproblemrapport som visar status för problem i aktuella projekt och projektnamnet. Rapporten grupperas efter projektnamn och status för problemen.</td> 
  </tr> 
  <tr> 
   <td>Arbete kontra utgift per Portfolio</td> 
   <td>En projektrapport som visar projektens Planerad arbetskostnad, Faktisk arbetskostnad, Planerad utgiftskostnad och Faktisk utgiftskostnad. Rapporten grupperas efter Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Arbete kontra kostnader per program</td> 
   <td>En projektrapport som visar projektens Planerad arbetskostnad, Faktisk arbetskostnad, Planerad utgiftskostnad och Faktisk utgiftskostnad. Rapporten är grupperad efter namn på Portfolio och programnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Månadskostnad Portfolio jämfört med Faktisk per projekt</td> 
   <td>En matrisprojektrapport (ekonomiska data) som visar datum för allokering, total planerad kostnad, total faktisk kostnad och total kostnadsvariation för projekten. Rapporten grupperas efter projektnamn, kvartal och månad för allokeringsdatumet.</td> 
  </tr> 
  <tr> 
   <td>Planerade intäkter per månad Portfolio kontra faktiska intäkter per projekt</td> 
   <td>En matrisprojektrapport (ekonomiska data) som visar projektens fördelningsdatum, totala planerade intäkter, totala faktiska intäkter och totala intäktsvariation. Rapporten grupperas efter projektnamn, kvartal och månad för allokeringsdatumet.</td> 
  </tr> 
  <tr> 
   <td>Månadsplanerade projektkostnader kontra faktiska</td> 
   <td>En matrisprojektrapport (ekonomiska data) som visar datum för allokering, total planerad kostnad, total faktisk kostnad och total kostnadsvariation för projekten. Rapporten grupperas efter projektnamn, kvartal och månad för allokeringsdatumet och visas efter Projektnamn.</td> 
  </tr> 
  <tr> 
   <td>Planerade månadsintäkter för projekt kontra faktiska</td> 
   <td>En matrisprojektrapport (ekonomiska data) som visar projektens fördelningsdatum, totala planerade intäkter, totala faktiska intäkter och totala intäktsvariation. Rapporten grupperas efter projektnamn, kvartal och månad för allokeringsdatumet och visas efter Projektnamn.</td> 
  </tr> 
  <tr> 
   <td>Mina dokument</td> 
   <td>En dokumentrapport som visar dokument som överförts av den inloggade användaren. Rapporten innehåller följande fält: Ägarnamn, Ändringsdatum, Storlek, Antal versioner, Source och Dokumenttyp.</td> 
  </tr> 
  <tr> 
   <td>Mina favoriter</td> 
   <td>En Favoritrapport som visar en lista över objekt som den inloggade användaren har markerat som favoriter. Rapporten innehåller följande fält: Objekttyp och Namn på favoriter.</td> 
  </tr> 
  <tr> 
   <td>Mina problem</td> 
   <td>En problemrapport som visar ofullständiga problem som tilldelats den användare som är inloggad. Rapporten innehåller följande fält: Source-namn, Ärendetyp, Primär tilldelad, Införseldatum, Status och Prioritet för problemen.</td> 
  </tr> 
  <tr> 
   <td>Min Portfolio</td> 
   <td>En Portfolio-rapport som visar aktiv Portfolio där den inloggade användaren är Portfolio Manager.</td> 
  </tr> 
  <tr> 
   <td>Mina program</td> 
   <td>En programrapport som visar Program och deras beskrivning, där den inloggade användaren är Programhanteraren.</td> 
  </tr> 
  <tr> 
   <td>Mina öppna projektproblem</td> 
   <td>En problemrapport som visar ofullständiga problem i projekt vars projektgrupp innehåller den inloggade användaren. Rapporten innehåller följande fält: Source-namn, Ärendetyp, Primär tilldelad, Införseldatum, Status och Prioritet för problemen.</td> 
  </tr> 
  <tr> 
   <td>Mina projekt</td> 
   <td>En projektrapport som visar Aktuella projekt vars projektgrupp innehåller den inloggade användaren. Rapporten innehåller följande fält: Beskrivning, Planerat slutförandedatum, Planerat slutförandedatum, Procent slutfört, Status och Prioritet för projekten.</td> 
  </tr> 
  <tr> 
   <td>Mina skickade problem</td> 
   <td>En problemrapport som visar problem som har skickats av den inloggade användaren och som har stängts under de senaste tre månaderna eller som är öppna. Rapporten innehåller följande fält: Source-namn, problemtyp, anmälningsdatum, status och prioritet för problemen.</td> 
  </tr> 
  <tr> 
   <td>Mina uppgifter</td> 
   <td>En aktivitetsrapport som visar ofullständiga uppgifter i Aktuella projekt som tilldelats den inloggade användaren. I rapporten visas följande fält: Planerad varaktighet, Projektnamn, primär tilldelad, Planerad start, Planerad slutförande, Procent slutfört och Prioritet för aktiviteterna.</td> 
  </tr> 
  <tr> 
   <td>Mina tidrapporter</td> 
   <td>En tidrapportrapport som visar alla tidrapporter för den inloggade användaren. Rapporten innehåller följande fält: Datumintervall, Ägarnamn, Totalt antal timmar, Övertid, Godkännarens namn och Status för tidrapporterna.</td> 
  </tr> 
  <tr> 
   <td>Mina otilldelade ärenden</td> 
   <td>En problemrapport som visar öppna ärenden som tilldelats någon av den inloggade användarens jobbroller och som inte tilldelats användaren. Rapporten innehåller följande fält: Source-namn, problemtyp, anmälningsdatum, status och prioritet för problemen.</td> 
  </tr> 
  <tr> 
   <td>Mina otilldelade uppgifter</td> 
   <td>En aktivitetsrapport som visar ofullständiga uppgifter som tilldelats någon av jobbrollerna för den inloggade användaren och som inte tilldelats användaren. I rapporten visas följande fält: Planerad varaktighet, Projektnamn, primär tilldelad, Planerat startdatum, Planerat slutförandedatum, Procent slutfört och Prioritet för aktiviteterna.</td> 
  </tr> 
  <tr> 
   <td>Mina kommande uppgifter</td> 
   <td>En aktivitetsrapport som visar ofullständiga uppgifter som ska starta de kommande två veckorna, finns i Aktuella projekt och tilldelas den inloggade användaren. Rapporten innehåller följande fält: Projektnamn, Planerat slutförandedatum, Planerat slutförandedatum, Procent slutfört och Status för aktiviteterna.</td> 
  </tr> 
  <tr> 
   <td>Öppna tidrapporter (visas)</td> 
   <td>En tidrapportrapport som visar öppna tidrapporter. Rapporten innehåller följande fält: Datumintervall, Ägare, Totalt antal timmar, Övertid, Godkännarens namn, Status för tidrapporterna. Rapporten visas av: Startdatum för tidrapport, Slutdatum för tidrapport, Godkännarnamn för tidrapport och Användarnamn.</td> 
  </tr> 
  <tr> 
   <td>Över budgetprojekt per Portfolio</td> 
   <td>En projektrapport som visar projektens planerade kostnad och faktiska kostnad. Rapporten grupperas efter Portfolio Name.</td> 
  </tr> 
  <tr> 
   <td>Planerad kostnad per program för Portfolio</td> 
   <td>En projektrapport som visar projektens planerade kostnad och faktiska kostnad. Rapporten visas av Portfolio Name, grupperad efter Program Name, och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerad kostnad för Portfolio per projekt</td> 
   <td>En projektrapport som visar projektens planerade kostnad och faktiska kostnad. Rapporten visas av Portfolio Name, grupperad efter projektnamn, och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerade Portfolio-intäkter per program</td> 
   <td>En projektrapport som visar projektens planerade intäkter och faktiska intäkter. Rapporten visas av Portfolio Name, grupperad efter Program Name, och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerade intäkter för Portfolio per projekt</td> 
   <td>En projektrapport som visar projektens planerade intäkter och faktiska intäkter. Rapporten visas av Portfolio Name, grupperad efter projektnamn, och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerade kontra faktiska kostnader per Portfolio</td> 
   <td>En projektrapport som visar planerad kostnad och faktisk kostnad för projekten per Portfolio. Rapporten grupperas efter Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerade kontra faktiska kostnader per program</td> 
   <td>En projektrapport som visar planerad kostnad och faktisk kostnad för projekten per program. Rapporten grupperas efter Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerad kontra faktisk intäkt per Portfolio</td> 
   <td>En projektrapport som visar projektens planerade intäkter och faktiska intäkter. Rapporten grupperas efter Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Planerad kontra faktisk intäkt per program</td> 
   <td>En projektrapport som visar projektens planerade intäkter och faktiska intäkter. Rapporten grupperas efter programnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Portfolio kostnad grupperade efter program och månad</td> 
   <td>En matrisprojektrapport som visar projektens Planerad kostnad, Budgeterad kostnad och Faktisk kostnad. Rapporten grupperas efter Portfolio namn, programnamn och månad för det planerade startdatumet för projekten.</td> 
  </tr> 
  <tr> 
   <td>Portfolio-projekt efter status grupperade efter program</td> 
   <td>En projektrapport som visar status för projekten. Rapporten grupperas efter programnamn och projektstatus och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Portfolio-projekt grupperade efter status och Portfolio</td> 
   <td>En projektrapport som visar Portfolio namn och status för projekten. Rapporten grupperas efter Portfolio namn och status för projekten och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Inkomster från Portfolio per program</td> 
   <td>En projektrapport som visar Portfolio namn, programnamn, planerade intäkter och faktiska intäkter för projekten. Rapporten grupperas efter namn på Portfolio och programnamn och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Portfolio Inkomster grupperade efter program och månad</td> 
   <td>En matrisprojektrapport som visar Planerad intäkt, Faktisk intäkt, Namn på Portfolio och Programnamn. Rapporten grupperas efter Portfolio namn, programnamn och månad för det planerade startdatumet för projekten.</td> 
  </tr> 
  <tr> 
   <td>Projektkostnader och intäkter per aktivitetsstatus</td> 
   <td>En matrisaktivitetsrapport som visar aktiviteternas Planerad kostnad, Faktisk kostnad, Planerad intäkt, Faktisk intäkt och Projektnamn. Rapporten grupperas efter projektnamn och status för aktiviteterna.</td> 
  </tr> 
  <tr> 
   <td>Projektkostnader kontra intäkter per Portfolio</td> 
   <td>En projektrapport som visar Portfolio namn, faktisk kostnad och faktisk intäkt för projekten. Rapporten grupperas efter Portfolio Name och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Projektutgifter per månad och kvartal</td> 
   <td>En matrisutgiftsrapport som visar bokföringsdatum, Planerat belopp, Faktiskt belopp och Projekt för utgifterna. Rapporten grupperas efter projektnamn, kvartal och månad för bokföringsdatumet för utgifterna.</td> 
  </tr> 
  <tr> 
   <td>Projekttimkostnad per timtyp per månad</td> 
   <td>En matristimrapport som visar följande fält: Timmar, Ingångsdatum, Faktisk kostnad för projekten, Timtyp, Projektnamn. Rapporten grupperas efter projektnamn, månad på anmälningsdatumet för timmarna och timtyp.</td> 
  </tr> 
  <tr> 
   <td>Projektkostnader för arbete och utgifter per månad och kvartal</td> 
   <td>En matrisprojektrapport som visar projektens Planerad arbetskostnad, Faktisk arbetskostnad, Planerad utgiftskostnad och Faktisk utgiftskostnad. Rapporten grupperas efter projektnamn och kvartal och månad för projektets faktiska startdatum.</td> 
  </tr> 
  <tr> 
   <td>Projektprestanda</td> 
   <td>En projektrapport som visar följande fält i aktuella projekt: förfallodatum, CPI, SPI, CSI, planerad kostnad, budget, EAC och utgifter för projekten.</td> 
  </tr> 
  <tr> 
   <td>Projektförfrågningar</td> 
   <td>En projektrapport som visar begärda projekt. Rapporten innehåller följande fält: Beskrivning, Planerat slutförandedatum, Planerat slutförandedatum, Procent slutfört, Status och Prioritet för projekten.</td> 
  </tr> 
  <tr> 
   <td>Projekt efter villkor</td> 
   <td>En projektrapport som visar projektens villkor. Rapporten grupperas efter villkor och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Projekt efter villkor efter grupp</td> 
   <td>En projektrapport som visar status och grupp för projekten. Rapporten grupperas efter gruppnamn och förloppsstatus och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Projekt efter prioritet</td> 
   <td>En projektrapport som visar prioritet för projekt. Rapporten grupperas efter prioritet och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Status för projekt efter förlopp</td> 
   <td>En projektrapport som visar projektets förloppsstatus. Rapporten grupperas efter förloppsstatus och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Status för aktiviteter efter förlopp</td> 
   <td>En aktivitetsrapport som visar förloppsstatusen för alla aktiviteter i aktuella projekt. Rapporten grupperas efter förloppsstatus och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Aktiviteter efter status</td> 
   <td>En aktivitetsrapport som visar status för alla uppgifter. Rapporten grupperas efter status och innehåller ett diagram.</td> 
  </tr> 
  <tr> 
   <td>Tidrapporter att granska</td> 
   <td>En tidrapportrapport som visar tidrapporter som skickats och avvisats och vars godkännare är inloggad användare. Rapporten innehåller följande fält: Datumintervall, Ägare, Totalt antal timmar, Övertid, Godkännarens namn och Status för tidrapporterna.</td> 
  </tr> 
  <tr> 
   <td>Felaktiga uppgifter</td> 
   <td>En aktivitetsrapport som visar ofullständiga uppgifter med statusvärdet Försenad eller Efter, ett leveransdatum som är tidigare än i morgon och där den inloggade användaren är en del av projektgruppen för det projekt som aktiviteterna är aktiverade. Rapporten innehåller följande fält: Planerad varaktighet, Projektnamn, primär tilldelad, Planerad start, Planerad slutförande, Procent slutfört och Prioritet för aktiviteterna.</td> 
  </tr> 
  <tr> 
   <td>Användarinloggningar</td> 
   <td>En användarrapport som visar följande fält: unikt ID, antal inloggningar (det antal gånger som användaren har loggat in sedan Workfront startades), användarens senaste inloggningsdatum. Rapporten grupperas efter användarnas åtkomstnivå.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Få tillgång till inbyggda rapporter

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Klicka på **Rapporter**.
1. Klicka på **Alla rapporter**.
1. Expandera listrutan **Filter** och välj **Nytt filter**.

1. Klicka på **Lägg till en filterregel**.
1. Börja skriva **Global ID** i fältet **Börja skriva fältnamn**.

1. Välj **Global ID** under objektet **Rapport**.

1. Välj **Är inte tom** i listrutan för filtermodifieraren.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Klicka på **Spara filter**.\
   I rapportlistan visas endast inbyggda rapporter.\
   Mer information om vilka inbyggda rapporter som är tillgängliga finns i avsnittet [Översikt över inbyggda rapporter](#overview-of-built-in-reports) i den här artikeln.

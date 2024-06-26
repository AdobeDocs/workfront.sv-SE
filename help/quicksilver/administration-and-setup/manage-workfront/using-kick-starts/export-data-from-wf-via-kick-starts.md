---
user-type: administrator
product-area: system-administration
keywords: kickstart,sparkstart,kickstarter,sparkstarter
navigation-topic: use-kick-starts
title: Exportera data från Adobe Workfront via Quick-Starts
description: Som Adobe Workfront-administratör kan du använda dataexporteraren Quick-Starts för att exportera data från Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 8e076e9c89ad208aa94ddefead4b8c6105992542
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Exportera data från Adobe Workfront via Quick-Starts

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Som Adobe Workfront-administratör kan du använda dataexporteraren Quick-Starts för att exportera data från Workfront. Du kan använda den i andra program när du har exporterat den.

Att exportera data via snabbstart är också praktiskt när du vill veta vilka fält som är kopplade till varje objekt, hur dessa fält kodas samt hur värdena för dessa fält formateras i databasen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fördelar och nackdelar med att använda&quot;kom igång&quot; för att exportera data

Det finns två sätt att exportera data inom Workfront:

* Exportera data från en rapport eller en lista

  Mer information om hur du exporterar data från en rapport eller en lista finns i [Exportera data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exportera data via snabbstart

I följande tabell visas fördelar och nackdelar med varje metod:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Exporterade data innehåller objekt- och fältvärden</p> </th> 
   <th> <p>Möjlighet att exportera data runt flera objekttyper samtidigt</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportera data från en listvy</strong> </p> <p>Mer information om att exportera data från en lista finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportera data</a></p> </td> 
   <td> <p>Ja</p> <p>Både inbyggda Workfront-fält och anpassade fält som är kopplade till objekten exporteras.</p> </td> 
   <td> <p>Nej</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exportera data via snabbstart</strong> </p> </td> 
   <td> <p>Ja (begränsad)</p> <p>De flesta inbyggda Workfront-fält som är associerade med objekt exporteras, men andra exporteras inte. Du kan till exempel inte exportera fälten Schema, Projektägare eller Projektsponsorer via en projektstartexport.</p> <p>I ett projekt som har ett anpassat formulär bifogat exporteras inga data som har angetts i fälten i formuläret.</p> <p>Men du kan exportera ett anpassat formulär. Den resulterande filen visar de fält som har konfigurerats i formuläret, t.ex. textrutor och alternativknappar.</p> </td> 
   <td> <p>Ja</p> <p>Om du använder Kickstart för att exportera Workfront-data kan du exportera data som relateras till flera objekttyper i en och samma export. Du kan till exempel inkludera uppgifter, problem och projekt i en enda export.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Exportbegränsningar

Följande begränsningar gäller vid export av data via direktstart (data exporteras i ett Excel-filformat):

* **50 000 rader:** Antalet rader som tillåts i filen.
* **65 530 hyperlänkar:** Det här är en gräns som gäller för dokument som innehåller fler än 65 530 hyperlänkar. Dessa dokument kan inte öppnas när de har exporterats. Observera att ett Excel-dokument kanske bara innehåller 200 rader med data, men att dokumentet inte öppnas om det finns fler än 65 530 länkar i dokumentet.

## Exportera data via snabbstart

{{step-1-to-setup}}

1. Klicka **System** > **Sparka igång,** klicka sedan på **Exportera data.**

1. Markera det objekt som du vill exportera. Som standard visas följande objekt under **Vad du ska ta med**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objekt</strong> </p> </th> 
      <th> <p><strong>Exporterade blad i Excel-filen</strong> </p> </th> 
      <th> <p> <strong>Exportformat</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Kontrollpanel</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteralternativ<br>Parametergrupp<br>Kategoriparameter<br>Kategori<br>Rapport<br>Portal Tab Section<br>Kontrollpanel<br>Inställningar</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapport</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parameter<br>Parameteralternativ<br>Parametergrupp<br>Kategoriparameter<br>Kategori<br>Rapport<br>Inställningar</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Godkännande</p> </td> 
      <td scope="col" valign="top"> <p>Steggodkännare<br>Godkännandesteg<br>Godkännande<br>Godkännandeprocess<br>Inställningar</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Anpassade data</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteralternativ<br>Parametergrupp<br>Kategoriparameter<br>Kategori<br>Inställningar</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Utgiftstyp</p> </td> 
      <td valign="top"> <p>Utgiftstyp<br>Inställningar</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Timtyp</p> </td> 
      <td valign="top"> <p>Timtyp<br>Inställningar</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Teammedlem<br>Team<br>Inställningar </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Användare</p> </td> 
      <td valign="top"> <p>Användare<br>Inställningar</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Fler alternativ** om du vill se en fullständig lista över objekt.

   Alla objekt som listas här kan även användas för att importera data till Workfront.

   Det enda undantaget är **Åtkomstnivåer** -objekt. Det datablad för åtkomstnivåer som ingår i en export tillhandahålls endast i referenssyfte. Det gör att du kan tilldela en åtkomstnivå till ett nytt användarkonto via ID.

   Mer information om hur du importerar data till Workfront via direktstarter finns i [Importera data till Adobe Workfront med en snabbstartsmall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Nedan följer en lista över alla objekt som kan exporteras via snabbstarter:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objekt</p> </th> 
      <th> <p>Exporterade blad i Excel-filen</p> </th> 
      <th> <p>Exportformat</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Åtkomstnivå</td> 
      <td scope="col" valign="top">Åtkomstnivå<br>Inställningar</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Tilldelning</td> 
      <td scope="col" valign="top">Tilldelning<br>Inställningar</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Företag</td> 
      <td scope="col" valign="top"> Företag<br>Inställningar </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">E-postmall</td> 
      <td scope="col" valign="top"> E-postmall<br>Inställningar </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Utgift</td> 
      <td valign="top"> Utgift<br>Inställningar </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Extern sida</td> 
      <td valign="top"> Extern sida<br>Inställningar </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filter</td> 
      <td valign="top"> Filter<br>Inställningar </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Grupp</td> 
      <td valign="top"> Grupp<br>Inställningar  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppering</td> 
      <td valign="top"> Gruppering<br>Inställningar </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Timme</td> 
      <td valign="top"> Timme<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problem</td> 
      <td valign="top"> Problem<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Jobbroll</td> 
      <td valign="top"> Jobbroll<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Sökväg för milstolpe</td> 
      <td valign="top"> Milstolpe<br>Sökväg för milstolpe<br>Inställningar </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Anteckning</td> 
      <td valign="top"> Anteckning<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Inställningar  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projekt</td> 
      <td valign="top"> Kö<br>Projekt<br>Cirkulationsregel<br>Köämne<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Resursberäkning</td> 
      <td valign="top"> Resursberäkning<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Resurspool</td> 
      <td valign="top"> Resurspool<br>Inställningar </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">risk</td> 
      <td valign="top"> risk<br>Inställningar  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risktyp</td> 
      <td valign="top"> Risktyp<br>Inställningar  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Styrkort</td> 
      <td valign="top">Styrkortfrågor<br>Styrkortsalternativ<br>Styrkort<br>Inställningar </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Uppgift</td> 
      <td valign="top"> Uppgift<br>Inställningar </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Mall</td> 
      <td valign="top"> Kö<br>Mall<br>Cirkulationsregel<br>Köämne<br>Inställningar </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Malltilldelning</td> 
      <td valign="top"> Malltilldelning<br>Inställningar </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Malluppgift</td> 
      <td valign="top"> Malluppgift<br>Inställningar </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tidrapport</td> 
      <td valign="top"> Tidrapportprofil<br>Tidrapport<br>Inställningar </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Visa </td> 
      <td valign="top"> Visa<br>Inställningar  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Hämta.**

   Den exporterade startfilen hämtas till datorn antingen som en Excel-fil eller en . zip-fil som innehåller flera Excel- och egenskapsfiler. Varje Excel-fil är en samling blad, där varje blad representerar ett fält som är associerat med det markerade objektet. Det finns en **Egenskaper** blad som är associerade med varje export.

   The **Kontrollpanel** och **Rapport** Med kan du välja särskilda instrumentpaneler och rapporter som ska inkluderas i hämtningen. Du kan bara exportera kontrollpaneler som är delade i hela systemet.

   Du kan inte exportera matrisrapporter. Mer information om matrisrapporter finns i [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Quick-Starts stöder inte textlägesfilter. Rapporteringsfiltren måste växlas till standardläge för att exporten ska lyckas.

   Du kan välja upp till 100 instrumentpaneler och 100 rapporter i en enda export.

   ![](assets/kickstart-export-350x381.png)

   Du kan exportera flera objekt samtidigt.

1. (Rekommenderas) Analysera exporterade data för att kontrollera att all information som du förväntar dig har exporterats.

   För stora exporter arbetar Workfront i bakgrunden för att skapa Excel-filen och ger dig ett varningsmeddelande om fördröjningen. Snabbstartfilen skickas med e-post till dig när nedladdningen är klar.

   ![](assets/large-kick-start-file-warning-350x65.png)

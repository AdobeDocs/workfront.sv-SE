---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Rapport: Budgeterad timme'
description: 'Rapport: Budgeterad timme'
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Rapport: Budgeterad timme

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

När du vill dela information om budgeterad timme med andra användare som inte har tillgång till resursplaneraren kan du göra det genom att skapa en rapport om budgeterad timme. Du kan sedan dela rapporten med dem.

>[!IMPORTANT]
>
>Budgeterade timmar uppdateras normalt varje timme (det kan ta max tre timmar) i Adobe Workfront-databasen. Om du uppdaterar rapporten uppdateras inte timinformationen i den. Du kan visa den tid som gått sedan den senaste uppdateringen i det övre högra hörnet i varje rapport för budgeterad timme. När du uppdaterar rapporten uppdateras bara informationen i den när det har gått mer än en timme sedan den senaste uppdateringen.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)

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
   <ul><li><p>Medarbetare som ändrar ett filter </p></li>
   <li><p>Standard för att ändra en rapport</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Begäran om att ändra ett filter </p></li>
   <li><p>Planera att ändra en rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bygg en budgeterad timrapport

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet eller på ikonen **Huvudmeny** ![](assets/lines-main-menu.png) i det övre vänstra hörnet, om den är tillgänglig, och klicka sedan på **Rapporter** .

1. Klicka på **Ny rapport** > **Mer** > **Budgeterad timme**.

   Standardvyn används för rapporten.

1. (Valfritt) Klicka på **Bud om du vill göra rapporten enklare att läsa. Timmar**, **Växla till textläge** och klicka sedan på **Redigera textläge**.
1. Ändra raden `valuefield` till `valueexpreesion` och ange avrundningsuttrycket.

   Detta avrundar antalet budgeterade timmar till ett antal decimaler som du anger.

   Mer information om hur du rundar av ett tal i Workfront finns i artikeln [Översikt över beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Klicka på **Klar**.
1. (Valfritt) Klicka på **Lägg till kolumn** om du vill lägga till fler kolumner.
1. (Valfritt) För att rapporten ska bli lättare att läsa rekommenderar vi att du lägger till en gruppering i den. Vi föreslår följande gruppering:

   Klicka på fliken **Grupperingar** och gör sedan något eller flera av följande:

   * Klicka på **Lägg till gruppering** och börja skriva &quot;Projektnamn&quot;. Markera sedan grupperingen när den visas i listan.
   * Klicka på **Lägg till gruppering** och börja skriva &quot;Jobbrollnamn&quot;. Markera sedan grupperingen när den visas i listan.
   * Klicka på **Lägg till gruppering** och börja skriva Allokeringsdatum. Markera grupperingen när den visas i listan och välj sedan den tidsram som du vill gruppera i fältet **Gruppdatum efter**.

1. (Valfritt) Klicka på **Filter** om du vill lägga till filter i rapporten.
1. (Valfritt) Klicka på **Diagram** om du vill lägga till ett diagram i rapporten.
1. Klicka på **Spara + Stäng**.

## Granska rapporten om budgeterad timme

Följande information finns som standard i rapporten Budgeterad timma:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projekt </td> 
   <td>Det här är namnet på projektet som är associerat med budgeterad timme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Jobbroll</p> </td> 
   <td>Det här är namnet på den jobbroll som är associerad med budgeterad timme. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Användare</td> 
   <td>Det här är namnet på användaren som är associerad med budgeterad timme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fördela. Datum</td> 
   <td> <p>Detta är fördelningsdatumet. Det är den första dagen (en söndag) i veckan som du budgeterade timmarna för.</p> <p>Tips:  <p>Om en vecka sträcker sig över två månader genereras två rader i rapporten: en som motsvarar den första dagen i veckan (söndagen i veckan som infaller under den första månaden) och en andra som motsvarar den första dagen i den andra månaden (och som kan vara vilken dag som helst i veckan).</p> <p>Om du till exempel budgeterar 8 timmar för en användare för veckan 30 juni (söndag) - 6 juli (lördag), visar de två raderna ett allokeringsdatum 30 juni och 1 juli.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bud. Timmar</td> 
   <td>Detta är de budgeterade timmar som tilldelats användaren i resursplaneraren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Plan. Bud. Timmar</td> 
   <td>Detta är de budgeterade timmar som tilldelats jobbrollen eller projektet i resursplaneraren.</td> 
  </tr> 
 </tbody> 
</table>

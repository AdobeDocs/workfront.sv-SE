---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Använda valutafält på arbetsytans kontrollpaneler
description: Du kan använda valutafälten på en Canvas-kontrollpanel.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Använda valutafält på arbetsytans kontrollpaneler

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
   <p>Visa åtkomst till finansiella data</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td><p>Hantera behörigheter för kontrollpanelen</p>
  </td> 
  </tr> 
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Förutsättningar

1. Du måste ha flera valutatyper konfigurerade i din Workfront-instans för att kunna använda de funktioner som beskrivs i den här artikeln. Mer information finns i [Konfigurera valutakurser](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >Funktionen som beskrivs i den här artikeln gäller endast för fält med inbyggd valuta. Stöd för anpassade valutafält kommer snart.


## Ange standardvaluta för en Canvas-instrumentpanel

När du skapar en Canvas-kontrollpanel kan du ange en standardvaluta för kontrollpanelen. Den här valutan används för att visa alla fält för ursprunglig valuta i rapporter på kontrollpanelen, såvida inte valutafältet är låst på rapportnivån.

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel**

1. Ange följande:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Namn</strong></td>
      <td><p>Ange ett namn för instrumentpanelen. Vi rekommenderar att du endast använder UTF-8-tecken för att undvika kompatibilitetsproblem.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beskrivning (valfritt)</strong></td>
      <td>Ange en beskrivning av instrumentpanelen.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Valuta</strong></td>
      <td>Välj standardvalutatypen för instrumentpanelen. <br>
      <br> Användare kan växla mellan olika valutatyper när de filtrerar kontrollpanelen.</td>
     </tr>
    </tbody>
   </table>


## Växla mellan valutor på en arbetsytans kontrollpanel

Du kan växla mellan olika valutatyper på kontrollpanelsnivå. Rapporter som innehåller valutafält uppdateras för att återspegla den valda valutatypen.

Valutafält kan låsas på rapportnivå. Om ett valutafält är låst ändras inte valutatypen för den rapporten när du ändrar valutatypen för instrumentpanelen.

Om du vill ändra valutatypen för instrumentpanelen

1. Klicka på listrutan för valuta i det övre högra hörnet på sidan med information om instrumentpanelen.
1. Välj önskad valutatyp i listan.

   ![listrutan Ändra valuta](assets/filter-by-currency.png)


## Begränsningar

Följande tabell anger begränsningar när valutor definieras i området Valutakurser i Inställningar.

<table> 
<tr>
<td></td>
<td>Användarna kan</td>
<td>Användarna kan inte</td>
</tr>
<tr> 
<td>En valuta är definierad</td>
<td>
<ul>
<li>Använd fält för inbyggda valutor i Canvas-diagram, KPI och tabellrapporter</li>
<li>Använd anpassade valutafält i Canvas-diagram, KPI och diagramrapporter</li>
</ul>
</td>
<td>
<ul>
<li>Tilldela en standardvaluta till kontrollpanelen (när den skapas eller när kontrollpanelen redigeras)</li>
<li>Visa och använd växlingsknappen för valutan på instrumentpanelsnivå</li>
<li>Lås en viss valuta för visning i ett arbetsytans diagram, KPI eller tabellrapport</li>
<li>Använd fält för planeringsvaluta i ett arbetsytans diagram, KPI och tabellrapporter</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Flera valutor har definierats</td>
<td>
<ul>
  <li>Använd fält för inbyggda valutor i Canvas-diagram, KPI och tabellrapporter</li>
  <li>Ange standardvaluta för instrumentpanelen (när den skapas eller när instrumentpanelen redigeras)</li>
  <li>Visa och använd växlingsknappen för valutan på instrumentpanelsnivå</li>
  <li>Lås en viss valuta för visning i ett arbetsytans diagram, KPI eller tabellrapport för att ignorera inställningen för växling mellan instrumentpanelsvaluta</li>
</ul>
</td>
<td><ul>
  <li>Använd anpassade datavalutefält i Canvas-diagram, KPI och tabellrapporter</li>
  <li>Använd fält för planeringsvaluta i ett arbetsytans diagram, KPI och tabellrapporter</li>
</ul>
</td>
</tr></table>






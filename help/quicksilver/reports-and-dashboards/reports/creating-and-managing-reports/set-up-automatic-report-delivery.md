---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Schemalägg automatisk rapportleverans
description: Schemalägg automatisk rapportleverans
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1293'
ht-degree: 0%

---

# Schemalägg automatisk rapportleverans

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Du kan schemalägga rapporter som ska skickas automatiskt till användare enligt ett angivet schema, eller så kan du skicka rapporter manuellt på en engångs basis. När du skickar en rapport från Adobe Workfront får användaren ett e-postmeddelande med Workfront-rapporten i en separat bifogad fil.

Mer information, inklusive storleksbegränsningar som kan påverka rapportleveransen finns i [Översikt över rapportleveransen](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
   <p>Redigera åtkomst till filter, vyer, grupperingar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
     <td> <p>Hantera behörigheter i en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar måste du skapa en rapport. Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Boka en rapportleverans


Så här schemalägger du en rapport för automatisk leverans: &#x200B;

{{step1-to-reports}}

>[!NOTE]
>
>Rapportleveranser innehåller inga uppmaningar. Om du vill begränsa datamängden i en rapport rekommenderar vi att du tillämpar filter på rapporten som du vill skicka.

1. Välj en rapport på sidan **Rapporter**.
1. Klicka på **Rapportåtgärder** överst på skärmen och sedan på **Skicka rapport** i listrutan som visas. Dialogrutan **Skicka rapport** visas.

   >[!TIP]
   >
   >Om du vill skicka en rapport manuellt vid en viss tidpunkt går du till rapporten och klickar sedan på **Rapportåtgärder** > **Skicka rapport** > **Skicka nu**.

1. Välj fliken **Upprepade leveranser**.
1. (Villkorligt) Om du vill ändra en befintlig upprepande rapportleverans markerar du rapportleveransen i avsnittet **Upprepade leveranser** till höger i dialogrutan.
1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Skicka till</p> </td> 
      <td> <p>Börja skriva namnet på den användare, grupp, team eller roll som du vill skicka rapporten till och klicka sedan på namnet när det visas i listrutan.</p> <p>eller</p> <p>Ange e-postadressen till en person utanför Workfront som du vill ska ha åtkomst till rapporten.</p> <p>Upprepa den här processen om du vill skicka rapporten till flera användare, grupper, team eller roller.</p> <p>Obs!  <p>Tänk på följande när du lägger till rapportleveransmottagare:</p> 
        <ul> 
         <li><p>Om din organisation begränsar Workfront-meddelanden till specifika e-postdomäner kanske du bara kan skicka rapporter till e-postadresser som listas i e-posttillåtelselista.</p> <p>Om en användare till exempel är inställd som rapportmottagare och har en e-postadress som tidigare var tillåten och tillåtelselista uppdateras för att inte längre leverera e-post till den domänen, får användaren inte längre några levererade rapporter.</p><p>Information om hur en Workfront-administratör uppdaterar e-postmeddelandet tillåtelselista finns i avsnittet <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Konfigurera e-posttillåtelselista</a>.</p></li> 
         <li> <p>Om du lägger till ett stort antal användare som mottagare kan leveransen misslyckas. Om leveransfel uppstår kan du schemalägga flera rapportleveranser med mindre grupper av användare.</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-postämne</p> </td> 
      <td> <p>Ange ett ämne för e-postmeddelandet.</p> <p>Som standard är e-postmeddelandets ämne:</p> <p><em>Workfront-rapport: [rapportens namn] [Datum]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-postmeddelande</p> </td> 
      <td> <p>Ange ett meddelande som ska inkluderas i e-postmeddelandet.</p> <p>Som standard är e-postmeddelandet:</p> <p><em>Bifogad är rapporten [rapportfrekvens] [rapportens namn] som genererades av Workfront den [datum].</em> </p> <p>Obs! För rapporter som levereras endast som en Excel-fil läggs även följande meddelande till i e-postmeddelandet:"Observera att det finns en gräns (65 530) för hur många hyperlänkar dessa filtyper har. Om du överskrider dessa gränser öppnas inte filen och du bör skicka den igen utan hyperlänkarna. Gå tillbaka till rapportschemaläggaren för att ta bort hyperlänkar och skicka rapporten igen." frasen"gå tillbaka till rapportschemaläggaren" är en länk tillbaka till rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Leverera den här rapporten med åtkomsträttigheter för</p> </td> 
      <td> <p>Börja skriva namnet på en användare som har åtkomst till rapporten och klicka sedan på namnet när det visas i listrutan. Användare som tar emot rapporten får samma åtkomstnivå till rapporten som den användare du anger här.<br> Mer information finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Kör och leverera en rapport med åtkomsträttigheter för en annan användare</a>.</p> <p>Obs! Det här fältet stöder inte jokertecken. Om du till exempel använder jokertecknet <em>$$User.ID</em> körs inte rapporten med åtkomsträttigheterna för den användare som tar emot rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Välj det format som du vill ha för den levererade rapporten:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Om du väljer PDF kan du formatera utdata med de ytterligare alternativen <strong>Pappersstorlek</strong> och <strong>Orientering</strong> som visas.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inkludera länkar</p> </td> 
      <td> <p>Det här alternativet är bara tillgängligt när <strong>MS Excel</strong> har valts i listrutan <strong>Format</strong>. När det här alternativet är aktiverat inkluderas alla hyperlänkar i det exporterade Excel-dokumentet.</p> <p>Det går inte att öppna dokument som innehåller fler än 65 530 länkar. Om det exporterade dokumentet innehåller fler än 65 530 länkar avmarkerar du det här alternativet.</p> <p>Det här alternativet är aktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Sammanfattning</p> </td> 
      <td> <p>Visar en sammanfattning av när leveransen upprepas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Upprepningar</p> </td> 
      <td> <p>Ange om rapporten ska levereras varje dag, vecka, månad eller år.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Upprepa var</p> </td> 
      <td> <p>Välj den frekvens med vilken du vill att leveransen ska upprepas. Värdet som du väljer för det här alternativet baseras på det alternativ som har valts i listrutan <strong>Upprepningar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tid</p> </td> 
      <td> <p>Välj den tid på dagen då leveransen ska skickas.</p> <p>Tips! Eftersom systeminläsningen kan påverka leveranstiderna för rapporter kan det uppstå en fördröjning på upp till 24 timmar mellan den schemalagda tiden och den faktiska leveranstiden. Om du behöver en rapport som levereras vid en viss tidpunkt rekommenderar vi att leveransen schemaläggs före den tidpunkt då den behövs. Vanligtvis rekommenderar vi att leveransen schemaläggs minst en dag före det datum då den behövs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Upprepningar på</p> </td> 
      <td> <p>Det här alternativet är tillgängligt när alternativet <strong>Upprepningar</strong> är inställt på antingen <strong>Veckovis</strong> eller <strong>Månadsvis</strong>:</p> 
       <ul> 
        <li> <p>När alternativet <strong>Upprepningar</strong> är inställt på <strong>Veckovis</strong>: Välj de veckodagar som leveransen skickas.</p> </li> 
        <li> <p>När alternativet <strong>Upprepningar</strong> är inställt på <strong>Månadsvis</strong>: Välj om leveransen ska skickas på dagen i månaden, veckodagen eller den sista dagen i månaden (de här alternativen utnyttjar det datum som du har valt i fältet <strong>Börjar på</strong>).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Börjar på</p> </td> 
      <td>Välj det datum då den schemalagda leveransen ska börja.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Slutar på</p> </td> 
      <td>Välj ett datum för den schemalagda leveransen till slutet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Aldrig</p> </td> 
      <td>Välj <strong>Aldrig</strong> om du vill att den schemalagda leveransen ska hålla i oändlighet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara** för att spara rapportleveransen. Rapporten visas i avsnittet **Upprepade leveranser** i dialogrutan **Skicka rapport** och skickas vid den schemalagda tidpunkten.

   Mer information om storleksbegränsningar som kan påverka rapportleveransen finns i avsnitten [Rapportleveransbegränsningar](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) och [Exportbegränsningar](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Schemalagda rapporter omfattas av en intern tidsgräns när de bearbetas för leverans. Om en rapport tar längre tid än gränsen som ska skickas får du ett meddelande och rapporten levereras inte längre oavsett eventuella återstående schemalagda leveranser. Om du vill fortsätta skicka rapporten försöker du först att minska rapportens storlek med hjälp av filter och vyer och sedan skapa en ny schemalagd leverans.
>
>Om du använder en schemalagd rapportleverans för att analysera Workfront-data via ett BI-verktyg rekommenderar vi att du använder Workfront Data Connect istället. Mer information finns i [Workfront Data Connect - översikt](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

## Ta bort en schemalagd rapportleverans

Så här tar du bort en schemalagd rapportleverans: &#x200B;

{{step1-to-reports}}

1. Välj en rapport på sidan **Rapporter**.

1. Klicka på **Rapportåtgärder** överst på skärmen och sedan på **Skicka rapport** i listrutan som visas. Dialogrutan **Skicka rapport** visas.

1. Välj fliken **Upprepade leveranser**.
1. Klicka på den schemalagda leveransen som du vill ta bort i avsnittet **Upprepade leveranser** till höger i dialogrutan.
1. Klicka på **Ta bort** i detaljavsnittet **Upprepade leveranser**.

1. Bekräfta genom att klicka på **Ta bort**.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->

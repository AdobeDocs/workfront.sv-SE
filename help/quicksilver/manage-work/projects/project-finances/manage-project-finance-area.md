---
product-area: projects
navigation-topic: financials
title: Hantera information i projektfinansieringsdelen
description: Hantera information i projektfinansieringsdelen
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# Hantera information i projektfinansieringsdelen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Du kan visa eller redigera den ekonomiska informationen för ett projekt genom att gå till området Ekonomi i avsnittet Projektinformation. Det finns ett begränsat antal fält som du kan visa eller redigera i det här området. Mer information om hur du redigerar all information för ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

## Åtkomstkrav

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
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomst till projekt och finansiella data</p> <p>Redigera åtkomst till projekt och finansiella data för att redigera finansiell information om projektet</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till ett projekt eller högre som innehåller Visa finansiella behörigheter</p> <p>Hantera behörigheter till projektet som innehåller Hantera finans för att redigera finansiell information för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Översikt över finanssektorn

Tänk på följande när du visar eller redigerar information på finansområdet:

* Den finansiella information som du hittar under Ekonomi Projektdetaljer representerar värden som går upp till projektnivå från aktiviteter, samt information som anges direkt i projektet. Viss ekonomisk information kan hanteras på både projektnivå och aktivitetsnivå.
* Du måste ha behörigheten Visa för projektet samt åtkomst till finansiella data från din åtkomstnivå för att kunna visa finansieringsdelen i ett projekt.
* Du måste ha behörigheten Hantera för projektet samt åtkomst till finansiella data från din åtkomstnivå för att kunna redigera informationen på finanssidan. Vi rekommenderar dock att endast projektägaren ska redigera informationen i det här området.

## Visa finansieringsinformation för ett projekt

1. Gå till ett projekt.
1. Klicka **Projektinformation** i den vänstra panelen.
1. Klicka på **Redigera** icon ![](assets/edit-icon.png) i det övre högra hörnet av detaljavsnittet och klicka sedan på **Ekonomi**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör har konfigurerat layoutmallen kanske inte översiktsavsnittet visas först, och då komprimeras det. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Visa följande fält i projektets finanssektor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Resultatindexmetod</td> 
      <td> Styr den metod som Workfront använder för att beräkna värden för upparbetat värde. Det kan vara timbaserat eller kostnadsbaserat. <br>Mer information om PIM finns i artikeln <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Ange PIM (Performance Index Method)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>Detta är projektresultatvärden som visar hur projektet fungerar vid en viss tidpunkt. Deras värden beräknas utifrån prestandaindexmetoden.<br>Mer information finns i följande artiklar: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Beräkna index för kostnadsprestanda (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Beräkna SPI (Schedule Performance Index) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Beräkna prestanda för kostnadsschema (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppskattning vid slutförande</td> 
      <td> Prognostiserad total kostnad för ditt projekt, i timmar om PIM (Performance Index Method) är timbaserad och den representeras i ett valutavärde om PIM (Performance Index Method) är kostnadsbaserad.<br>Mer information om hur du beräknar offerten vid slutförande finns i artikeln <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Beräkna uppskattning vid slutförande</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Det här är budgetuppsättningen för projektet. Detta anges manuellt av projektägaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fast kostnad</td> 
      <td>Detta är de fasta kostnaderna för projektet, oberoende av annan verksamhet i projektet. De anges manuellt av projektägaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerad kostnad</td> 
      <td>Den uppskattade kostnaden för projektet, baserat på Planerade timmar och hastigheterna som är associerade med uppgiftstilldelningarna (jobbroller eller användare).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktisk kostnad</td> 
      <td>Alla projektets kostnader. Faktisk kostnad är summan av alla faktiska kostnader: arbetskostnad (baserat på faktiska timmar och de taxor som är kopplade till jobbrollerna eller användarna som loggar dem), utgifter och fasta kostnader, som kan kopplas till ett projekt eller en uppgift.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fast intäkt</td> 
      <td>Ange förväntade intäkter baserat på projekttidsplanen. Fast intäkt anges manuellt av projektägaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerad intäkt</td> 
      <td>Beräknad inkomst förväntas baserat på de planerade timmarna och de taxor som är associerade med uppgiftstilldelningarna (jobbroller eller användare).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktisk intäkt</td> 
      <td>Faktisk inkomst från projektet baserat på faktiska timmar och hastigheter associerade med uppgiftstilldelningarna (jobbroller eller användare).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fakturerad intäkt</td> 
      <td> <p>Inkomster som faktureras kunder eller andra parter och som anges i Faktureringsregister. Mer information om faktureringsposter finns i artikeln <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Skapa faktureringsposter</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Redigera ekonomisk information i ett projekt

Som projektägare kan du redigera informationen på underfliken Ekonomi i ett projekt.

Så här redigerar du information på underfliken Projektfinansiering:

1. Gå till ett projekt som du är ägare till.

   >[!NOTE]
   >
   >Du måste ha behörigheten Hantera för projektet för att kunna utföra följande steg. Vi rekommenderar också att endast projektägaren ska göra ändringar på projektets finansunderflik.

1. Klicka **Projektinformation** i den vänstra panelen.
1. Klicka på **Redigera** icon ![](assets/edit-icon.png) i det övre högra hörnet av detaljavsnittet och klicka sedan på **Ekonomi** . Då öppnas finansdelen för redigering.
1. Redigera alla fält som är tillgängliga för redigering genom att klicka en gång på fältet eller klicka **+Lägg till** om du vill lägga till information i ett tomt fält.

   >[!TIP]
   >
   >Fält är inte tillgängliga för redigering om de beräknas automatiskt av Workfront eller om du inte har redigeringsbehörighet för dem.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Uppdatera något av fälten nedan.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör konfigurerar vår layoutmall kan fälten i avsnittet Projektinformation vara olika i din miljö. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Resultatindexmetod</td> 
      <td> <p>Styr den metod som Workfront använder för att beräkna projektresultatmått. Detta konfigureras på systemnivå av administratören, men du kan även redigera det på projektnivå. Välj något av följande alternativ:</p> 
       <ul> 
        <li><strong>Timbaserad:</strong>Workfront använder de planerade timmarna för att beräkna projektets CPI och EAC, och projektets EAC visas som ett tal i timmar. </li> 
        <li><strong>Kostnadsbaserad:</strong>Workfront använder den planerade arbetskostnaden vid beräkning av projektets CPI och EAC och EAC visas som ett valutavärde. När du väljer det här alternativet kontrollerar du att dina uppgiftstilldelningar (jobbroller eller användare) är kopplade till kostnadstariffer.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppskattning vid slutförande</td> 
      <td> <p>Representerar den beräknade totala kostnaden för ditt projekt eller din uppgift när den har slutförts. Detta konfigureras på systemnivå av administratören, men du kan även redigera det på projektnivå. Välj något av följande alternativ:</p> 
       <ul> 
        <li><strong>Beräkna på projektnivå</strong>: EAC för den överordnade uppgiften och projektet bestäms genom att de faktiska timmarna/den faktiska arbetskostnaden anges i EAC-formlerna. Beräkningen inkluderar Faktiska timmar/kostnader och utgifter som lagts till direkt i den överordnade uppgiften eller projektet.</li> 
        <li><strong>Samla upp från aktiviteter/underaktiviteter</strong>: EAC för den överordnade uppgiften och projektet bestäms genom att sammanfatta EAC för varje underordnad uppgift. Den här beräkningen exkluderar faktiska timmar/kostnader och utgifter som läggs till direkt i den överordnade aktiviteten eller projektet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Ange budgeten för det här projektet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fast kostnad</td> 
      <td>Ange den fasta kostnaden för det här projektet. Detta ska inte omfatta arbets- eller utgiftskostnader.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fast intäkt</td> 
      <td> <p>Ange fasta intäkter för det här projektet. Detta ska inte omfatta intäkter från faktureringsposter som faktureras partner eller tredje part.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projektvaluta</td> 
      <td> <p>Ange en valuta för det här projektet, om den skiljer sig från standardvalutan i systemet. Standardvalutan i ditt system definieras av din Workfront-administratör. Mer information om hur du ställer in valutakurser i Workfront finns i artikeln <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Ställ in valutakurser</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Klicka **Spara ändringar**.

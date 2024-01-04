---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Skapa rapporter om finansiella data med unika valutakurser
description: Om flera valutakurser har konfigurerats i Adobe Workfront kan du ange ekonomiska värden i rapporter och listor som ska visas i en annan valuta än standardvalutan.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Skapa rapporter om finansiella data med unika valutakurser

Om flera valutakurser har konfigurerats i Adobe Workfront kan du ange ekonomiska värden i rapporter och listor som ska visas i en annan valuta än standardvalutan.

>[!IMPORTANT]
>
>Om du väljer en annan valuta än standardvalutan i en vy visas inte längre länkarna **Lägg till fler aktiviteter** och **Lägg till fler problem** längst ned i en projektlista.

Mer information om hur du ändrar standardvalutan för ett visst projekt finns i [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md).

Om det finns projekt med en enda valuta i rapporten visas summorna i grupperingar också i systemets standardvaluta.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du kan visa alternativa valutor enligt beskrivningen i det här avsnittet måste Workfront-administratören först aktivera och konfigurera flera valutor under Konfigurera i Workfront. Mer information finns i [Ställ in valutakurser](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Tillämpa ekonomiska värden på en rapport {#apply-financial-values-to-a-report}

Så här konverterar du ekonomiska värden mellan valutor när du arbetar med rapporter:

1. Gå till rapporten där du vill konvertera ekonomiska värden till en annan valuta.
1. Klicka på **Visa** listruta, klicka **Ändra valuta** väljer du sedan någon av följande valutor som du vill visa ekonomiska värden i:

   * Projektets ursprungliga valuta
   * Valfri annan valuta

     >[!TIP]
     >
     >Du kan bara välja valutor som tidigare har valts i Inställningar.

   Med det här alternativet kan du snabbt konvertera ekonomiska värden i en rapport mellan olika tariffvärden.

   ![Ändra valuta](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## Visa standardvalutan i flera projekt med olika valutor

När du anpassar valutan på projektnivå och vill visa information från alla projekt i samma rapport finns följande scenarier:

* Om du skapar en rapport som samlar in ekonomisk information från två eller flera projekt som har olika valutor, återspeglar grupperingssammanfattningen som standard systemets standardvaluta som valts av Workfront-administratören.
* Om du skapar en rapport för två eller flera projekt som har samma valuta, men som skiljer sig från systemets standardvaluta, visas summorna i grupperingarna med systemets standardvaluta.
* Om du skapar en rapport för två eller flera projekt som har jobbrolltilldelningar associerade med en valutaåsidosättning, konverterar Workfront den ekonomiska informationen från jobbrollens åsidosatta valutakurser till antingen projektets valuta (när du väljer projektets ursprungliga valuta i vyn) eller till en annan valuta som du väljer när du visar rapporten. Mer information om hur du åsidosätter valutan för en jobbroll finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Så här visar du två projekt med anpassade valutor i en rapport:

1. Skapa två projekt med olika valutor.

   ![](assets/qs-currency-350x217.png)

1. Logga timmar i båda projekten.

   Mer information om loggningstid finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)och sedan klicka **Rapportering**.
1. Klicka **Ny rapport** sedan **Projektrapport**.
1. I **Kolumner (vy)** flik, lägga till **Faktisk kostnad** kolumn och sammanfatta det med **Summa**.

   Mer information om hur du skapar en kolumn finns i [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. I **Grupperingar** -flik, använda en **Planerat slutförandedatum** gruppering.

   Mer information om hur du skapar en gruppering finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. I **Filter** flik, lägga till ett filter för **Projektnamn** och välja de två projekten med olika valutor.

   Mer information om hur du skapar ett filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Spara + Stäng**.

   Summan av **Faktisk kostnad** visas i grupperingen med hjälp av systemets standardvaluta, oavsett vilken valuta projekten i rapporten har.

   ![Valuta som visas i gruppering](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   Om de två projekten har olika valutor, visas systemets standardvaluta även i rapportens gruppering.

## Visa projektvalutan i en rapport på projektnivå

Om en gruppering används för en uppgift eller timlista i ett projekt visas summorna i grupperingen i projektets valuta.

1. Skapa ett projekt med en annan anpassad valuta än systemets standardvaluta.
1. Gå till projektet och kontrollera att det innehåller timmar som har loggats för uppgifter.

   Mer information om loggningstid finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Uppgifterna ska tilldelas användare eller jobbroller med priset per timkostnad.

1. Klicka **Uppgifter**.
1. Expandera **Visa** nedrullningsbar meny och välj **Ny vy**.
1. Lägg till **Faktisk kostnad** i den nya vyn som en ny kolumn och sammanfatta den med **Summa**.
1. Klicka **Klar** och sedan klicka **Spara vy**.
1. Expandera **Gruppering** nedrullningsbar meny och välj **Ny gruppering**.
1. Lägg till **Faktiskt slutförandedatum** i den nya grupperingen som ett nytt fält och klicka sedan på **Spara gruppering**.

   The **Faktisk kostnad** kolumner sammanfattas i den nya grupperingen och visar summan i projektets valuta.

## Redigera rapporter med unika valutor

De ekonomiska fälten i en rapport kan inte redigeras förrän du ändrar rapportinställningen så att den ursprungliga valutan för projekt visas.

Så här redigerar du ett ekonomiskt fält i en rapport:

1. Navigera till en rapport.

   >[!NOTE]
   >
   >Om standardvalutan inte visas för en lista i något annat område kan du redigera vyn så att standardvalutan visas.\
   >Mer information om hur du ändrar valutan i en vy finns i avsnittet i den här artikeln [Tillämpa ekonomiska värden på en rapport](#apply-financial-values-to-a-report).

1. Klicka **Rapportåtgärder** väljer **Redigera**.
1. Klicka **Rapportinställningar**.
1. Klicka på **Standardvaluta** nedrullningsbar meny och välj **Projektets ursprungliga valuta**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Klicka **Klar**.

---
product-area: reporting
navigation-topic: report-usage
title: Visa rapportanvändning
description: Visa rapportanvändning
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Visa rapportanvändning

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

För att förstå hur omfattande rapporterna används i ditt system kan du visa följande information i en lista över rapporter:

* De 10 senaste användarna som visade rapporten
* Visa antal inom en angiven tidsram

   >[!NOTE]
   >
   >Adobe Workfront räknar en vy per användare och dag. Om du öppnar samma rapport flera gånger om dagen räknas detta som en vy för rapporten åt dig. Om en annan användare får åtkomst till samma rapport samma dag räknas detta som en ny vy för den andra användaren.

* Senast visat den
* Senast visad av användare
* En lista över kontrollpaneler som innehåller rapporten\
   Mer information om hur du visar namnet på kontrollpanelerna som rapporter kan läggas till i finns i artikeln [Förstå hur du organiserar rapporter på en kontrollpanel](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Du kan skapa en vy för en lista med rapporter där du kan visa den här informationen.\
Du kan filtrera en lista med rapporter efter några av dessa fält.\
Mer information om vilka fält du kan filtrera en rapport efter finns i artikeln [Filtrera en rapportlista efter användningsinformation](#filter-a-report-list-by-usage-information).

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

## Visa användningsinformation för rapporter i Visa en rapportlista

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.

1. Klicka på knappen **Visa** nedrullningsbar meny.
1. (Valfritt) Välj **Rapportanvändning** för att visa den vanligaste rapportanvändningsinformationen.\
   eller

1. Klicka **Ny vy** för att skapa en anpassad vy.
1. Klicka **Lägg till kolumn**.
1. Börja skriva något av följande fält och markera dem när de visas i listan under **Rapport** objekt som ska läggas till i en ny kolumn:

   * **De senaste 10 användarna**: Visar namnen på de 10 senaste användarna som visade rapporten.
   * **Vyer**: Visar antalet vyer inom någon av följande tidsramar:

      * **Den här månaden, kvartal, år**
      * **Förra månaden, kvartal, år**
      * **Alla vyer**: Visar ett totalt antal för alla vyer i rapporten
   * **Senast visad av**: Visar information om användaren som senast visade rapporten
   * **Senast visat den**: Visar datumet då rapporten senast visades


1. Klicka **Spara vy**.\
   Användningsinformationen om rapporten visas i de kolumner som du har lagt till i vyn.\
   Du kan också skapa en rapport för rapportobjektet och använda den här vyn i rapporten.\
   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Du måste ha behörighet att redigera rapporter på åtkomstnivån för att kunna skapa en rapport.\
   Mer information om åtkomst till rapporter finns i artikeln [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrera en rapportlista efter användningsinformation {#filter-a-report-list-by-usage-information}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.
1. Klicka på knappen **Filter** nedrullningsbar meny.
1. Klicka **Nytt filter** och sedan klicka **Lägg till en filterregel**.
1. Börja skriva något av följande fält och markera dem när de visas i listan under **Rapport** objekt som ska läggas till som en ny filterregel:

   * **Vyer**: Visar antalet vyer inom någon av följande tidsramar:

      * **Den här månaden, kvartal, år**
      * **Förra månaden, kvartal, år**
      * **Alla vyer**
   * **Senast visad av**: Visar information om användaren som senast visade rapporten
   * **Senast visat den**: Visar datumet då rapporten senast visades


1. Välj en modifierare för fältet och ange sedan ett värde när du uppmanas till det.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Klicka **Spara filter**.\
   Här visas en lista med rapporter som uppfyller användningsinformationen som du har definierat.\
   Du kan också skapa en rapport för rapportobjektet och använda det här filtret i rapporten.\
   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Du måste ha behörighet att redigera rapporter på åtkomstnivån för att kunna skapa en rapport.\
   Mer information om åtkomst till rapporter finns i artikeln [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Undantag vid visning av användningsinformation för rapporter

>[!IMPORTANT]
>
>Rapportanvändningsinformationen har samlats in sedan mars 2018. Information som infaller före detta datum är inte tillgänglig.

Följande är några undantag som du bör vara medveten om när du arbetar med rapportanvändningsinformation:

* Varje gång en rapport visas på en kontrollpanel eller en anpassad flik räknas den som en vy. Den användare som visar rapporten på sin kontrollpanel visas som Senaste vy av: Namnge användaren och det datum då instrumentpanelen visades visas som datumet Senast visad den.
* Workfront samlar inte in användningsinformation för inbyggda rapporter.\
   Mer information om inbyggda rapporter från Workfront finns i artikeln [Använd inbyggda rapporter från Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront samlar inte in användningsinformation om levererade rapporter. En levererad rapport räknas inte som en vy.\
   Mer information om levererade rapporter finns i artikeln [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* När en system- eller gruppadministratör loggar in som en annan användare räknas vyerna och kopplas till system- eller gruppadministratören.
* Workfront samlar inte in användningsinformation för rapporter från anpassade kvartal. Det finns bara referenser till de inbyggda standardkvarteren i rapportanvändningsfälten.
* Workfront samlar inte in användningsinformation för rapporter som delas och visas offentligt. När en offentlig rapport visas av någon utan att logga in på Workfront räknas inte rapportvyerna.\
   Mer information om att dela rapporter finns i artikeln [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

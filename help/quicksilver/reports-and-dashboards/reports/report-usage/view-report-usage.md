---
product-area: reporting
navigation-topic: report-usage
title: Visa rapportanvändning
description: Visa rapportanvändning
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '960'
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
  Mer information om hur du visar namnet på de instrumentpaneler som rapporter kan läggas till på i en lista med rapporter finns i artikeln [Förstå hur du organiserar rapporter på en instrumentpanel](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Du kan skapa en vy för en lista med rapporter där du kan visa den här informationen.\
Du kan filtrera en lista med rapporter efter några av dessa fält.\
Mer information om vilka fält du kan filtrera en rapport efter finns i artikeln [Filtrera en rapportlista efter användningsinformation](#filter-a-report-list-by-usage-information).

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
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa användningsinformation för rapporter i Visa en rapportlista

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.

1. Klicka på listrutan **Visa** i listan med rapporter.
1. (Valfritt) Markera vyn **Rapportanvändning** om du vill visa den vanligaste informationen om rapportanvändning.\
   eller

1. Klicka på **Ny vy** om du vill skapa en anpassad vy.
1. Klicka på **Lägg till kolumn**.
1. Börja skriva något av följande fält och markera dem när de visas i listan under objektet **Rapport** för att lägga till dem i en ny kolumn:

   * **De 10 senaste användarna**: Visar namnen på de 10 senaste användarna som visade rapporten.
   * **Vyer**: Visar antalet vyer inom någon av följande tidsramar:

      * **Den här månaden, kvartal, år**
      * **Senaste månaden, kvartal, år**
      * **Alla vyer**: Visar ett totalt antal för alla vyer i rapporten

   * **Senast visad av**: Visar information om användaren som senast visade rapporten
   * **Senast visat den**: Visar datumet då rapporten senast visades

1. Klicka på **Spara vy**.\
   Användningsinformationen om rapporten visas i de kolumner som du har lagt till i vyn.\
   Du kan också skapa en rapport för rapportobjektet och använda den här vyn i rapporten.\
   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Du måste ha behörighet att redigera rapporter på åtkomstnivån för att kunna skapa en rapport.\
   Mer information om åtkomst till rapporter finns i artikeln [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrera en rapportlista efter användningsinformation {#filter-a-report-list-by-usage-information}

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.
1. Klicka på listrutan **Filter** i rapportlistan.
1. Klicka på **Nytt filter** och sedan på **Lägg till en filterregel**.
1. Börja skriva något av följande fält och markera dem när de visas i listan under objektet **Rapport** för att lägga till dem som en ny filterregel:

   * **Vyer**: Visar antalet vyer inom någon av följande tidsramar:

      * **Den här månaden, kvartal, år**
      * **Senaste månaden, kvartal, år**
      * **Alla vyer**

   * **Senast visad av**: Visar information om användaren som senast visade rapporten
   * **Senast visat den**: Visar datumet då rapporten senast visades

1. Välj en modifierare för fältet och ange sedan ett värde när du uppmanas till det.\
   ![Rapportera användningsfilterstatistik](assets/qs-report-usage-filter-statistics-350x150.png)

1. Klicka på **Spara filter**.\
   Här visas en lista med rapporter som uppfyller användningsinformationen som du har definierat.\
   Du kan också skapa en rapport för rapportobjektet och använda det här filtret i rapporten.\
   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Du måste ha behörighet att redigera rapporter på åtkomstnivån för att kunna skapa en rapport.\
   Mer information om åtkomst till rapporter finns i artikeln [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Undantag vid visning av användningsinformation för rapporter

>[!IMPORTANT]
>
>Rapportanvändningsinformationen har samlats in sedan mars 2018. Information som infaller före detta datum är inte tillgänglig.

Följande är några undantag som du bör vara medveten om när du arbetar med användningsinformation för rapporter:

* Varje gång en rapport visas på en kontrollpanel eller en anpassad flik räknas den som en vy. Den användare som visar rapporten på sin kontrollpanel visas som Senaste vy efter: Namn-användare, och det datum då instrumentpanelen visades visas som Senast visad den-datum.
* Workfront samlar inte in användningsinformation för inbyggda rapporter.\
  Mer information om inbyggda rapporter från Workfront finns i artikeln [Använd inbyggda rapporter från Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront samlar inte in användningsinformation om levererade rapporter. En levererad rapport räknas inte som en vy.\
  Mer information om levererade rapporter finns i artikeln [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* När en system- eller gruppadministratör loggar in som en annan användare räknas vyerna och kopplas till system- eller gruppadministratören.
* Workfront samlar inte in användningsinformation för rapporter från anpassade kvartal. Det finns bara referenser till de inbyggda standardkvarteren i rapportanvändningsfälten.
* Workfront samlar inte in användningsinformation för rapporter som delas och visas offentligt. När en offentlig rapport visas av någon utan att logga in på Workfront räknas inte rapportvyerna.\
  Mer information om att dela rapporter finns i artikeln [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

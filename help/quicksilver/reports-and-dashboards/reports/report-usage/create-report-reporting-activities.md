---
product-area: reporting
keywords: ändring,ägare,delad,rapport,resurs,körning,användare,åtkomst,rättigheter,införd,senast,visade,datum,rapportering,aktiviteter
navigation-topic: report-usage
title: Skapa en rapport om rapporteringsaktiviteter
description: När du skapar en rapport om rapporter kan du identifiera specifik rapportinformation, som kan inkludera om rapporter tilldelas till inaktiverade användare, om rapporter är inställda på att köras med åtkomsträttigheter för en inaktiverad användare, om användare öppnar en rapport som du planerar att ta bort o.s.v.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Skapa en rapport om rapporteringsaktiviteter

När du skapar en rapport om rapporter kan du identifiera specifik rapportinformation, som kan inkludera om rapporter tilldelas till inaktiverade användare, om rapporter är inställda på att köras med åtkomsträttigheter för en inaktiverad användare, om användare öppnar en rapport som du planerar att ta bort o.s.v.

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

## Skapa rapporten om befintliga rapporter {#create-the-report-about-existing-reports}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.
1. Klicka **Rapporter** sedan **Ny rapport**.
1. I **Ny rapport** nedrullningsbara menyer, välj **Rapport** för att skapa en rapport om befintliga rapporter.

1. I **Kolumner (vy)** lägger du till de kolumner du vill ha i rapporten.\
   Några av följande fält kan vara användbara:

   | Fält | Beskrivning |
   |---|---|
   | **Kör som användare: Namn** | Detta är den användare som anges i **Kör den här rapporten med åtkomsträttigheterna för:** i rapporten. Om den här användaren inaktiveras visas ingen rapport för någon som rapporten delas med. |
   | **Delas med** | Detta är alla entiteter som rapporten delas med. |
   | **Anges av** | Detta är rapportens ägare. |
   | **Senast visat den** | Detta är det datum och den tidpunkt då rapporten senast visades av en användare. |

   {style=&quot;table-layout:auto&quot;}

1. (Valfritt) Om du vill begränsa din lista över rapporter till specifika inaktiverade användare:

   1. Välj **Filter** tabbtangenten och sedan klicka **Lägg till en filterregel**.

   1. Lägg till filtret **Användar-ID för Kör som** > **Jämn**.

   1. Skriv namnet på den inaktiverade användare som du vill lägga till i filtret och klicka sedan på namnet när det visas i listan.
   1. Upprepa steg C tills du har valt alla inaktiverade användare som du vill ta med i rapporten.

1. (Valfritt) Om du vill begränsa din lista över rapporter till schemalagda rapporter:

   1. Välj **Filter** tabbtangenten och sedan klicka **Lägg till en filterregel**.

   1. Lägg till filtret **Schemalagt rapport-ID** > **Är inte tom**.

1. Klicka **Spara + Stäng**, skriver ett namn för rapporten och klickar på **Spara rapport**.

   Din rapportinformation visas.

1. (Valfritt) Exportera den här rapporten till Excel och spara den på datorn.\
   Mer information om hur du exporterar en rapport finns i [Exportera data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Uppdatera information om en rapport

När du har skapat rapporten kan du uppdatera dina rapporter efter behov.

1. Gå till rapporten som du vill uppdatera.
1. Beroende på vilken åtgärd du vill utföra gör du något av följande:

   * Uppdatera **Kör den här rapporten med åtkomsträttigheterna för:** till en aktiv användare: Mer information finns i [Kör och leverera en rapport med åtkomsträttigheter för en annan användare](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Skapa en kopia av rapporten: Mer information finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Ta bort en rapport: Mer information finns i [Skapa en exakt kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) artikelns avsnitt [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Dela en rapport: Mer information finns i [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Villkorligt) Om du kopierar originalrapporterna ska du använda informationen från rapporten som du skapade i [Skapa rapporten om befintliga rapporter](#create-the-report-about-existing-reports) att dela de nya kopiorna med samma enheter som de ursprungliga rapporterna.

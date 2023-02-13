---
product-area: reporting;user-management
keywords: spara,ny,rapport,kopiera
navigation-topic: create-and-manage-reports
title: Skapa en kopia av en rapport
description: Du kan skapa en kopia av alla rapporter som du har tillgång till. Du kan antingen skapa en exakt kopia av en anpassad rapport eller spara en ny version av en standardrapport. När du har kopierat en rapport blir du ägare till den kopierade rapporten och den visas i delen Mina rapporter.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Skapa en kopia av en rapport

Du kan skapa en kopia av alla rapporter som du har tillgång till. Du kan antingen skapa en exakt kopia av en anpassad rapport eller spara en ny version av en standardrapport. När du har kopierat en rapport blir du ägare till den kopierade rapporten och den visas i delen Mina rapporter.

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
   <td> <p>Visa behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en exakt kopia av en rapport

Om du vill skapa en kopia av en rapport som du är ägare av gör du följande:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Rapporter** sedan **Alla rapporter**.
1. Öppna en rapport.
1. Klicka **Rapportåtgärder** sedan **Kopiera**.

   >[!TIP]
   >
   >Om rapporten är en standardrapport visas inte alternativet Kopiera på menyn Rapporteringsåtgärder.\
   >Mer information om hur du skapar en kopia av en standardrapport finns i [Skapa en ny version av en rapport](#create-a-new-version-of-a-report).

   ![Kopiera rapport](assets/nwe-fulllistofreportactions-2022.png)

   En kopia av den ursprungliga rapporten skapas med standardnamnet *Kopia av [Namn på den ursprungliga rapporten]*. Rapporten&quot;Slutförda uppgifter i Q4&quot; skulle till exempel ha&quot;Kopia av slutförda uppgifter i Q4&quot; som namn.

1. (Valfritt) Om du vill byta namn på rapporten börjar du skriva ett nytt namn.

   >[!TIP]
   >
   >Om du avmarkerar titeln innan du skriver det nya namnet markerar du rapportrubriken, tar bort namnet och anger det nya namnet.

1. (Valfritt) Om du vill dela den nya versionen av rapporten med andra användare klickar du på **Rapportåtgärder** sedan **Delning**.

   >[!NOTE]
   >
   >Delningsinformationen överförs inte till den kopierade rapporten från den ursprungliga versionen.\
   >Mer information om vem den föregående rapporten delades med finns i [Skapa en rapport om rapporteringsaktiviteter](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Valfritt) Om du har behörigheten Hantera för den ursprungliga rapporten och den ursprungliga rapporten inte längre behövs, kan du ta bort den för att ta bort onödiga dubblettrapporter i Workfront.

   Så här tar du bort den ursprungliga rapporten:

   1. Navigera till rapporten.
   1. Klicka **Rapportåtgärder** sedan **Ta bort**.

   1. Klicka **Ja, ta bort den** för att bekräfta att du vill ta bort rapporten.

## Skapa en ny version av en rapport {#create-a-new-version-of-a-report}

Om du vill skapa en kopia av en standardrapport gör du följande:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Rapporter** sedan **Alla rapporter**.
1. Klicka på namnet på en standardrapport för att öppna den.
1. Klicka **Rapportåtgärder** sedan **Redigera**.

   ![Redigera rapport](assets/nwe-reportactionsfordefaultreport-2022.png)

1. Gör de ändringar du behöver på följande flikar i rapporten:

   * **Kolumner (vy)**: Mer information om hur du anpassar vyer finns i artikeln [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Grupperingar**: Mer information om hur du anpassar grupperingar finns i artikeln [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filter**: Mer information om hur du anpassar filter finns i artikeln [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Diagram**: Mer information om hur du anpassar ett rapportdiagram finns i artikeln [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Klicka på i det övre högra hörnet **Rapportinställningar**.
1. I **Rapporttitel** ger du rapporten ett nytt namn.
1. Klicka **Klar**.
1. Klicka **Spara som ny rapport**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Valfritt) Om du vill dela den nya versionen av rapporten med andra användare klickar du på **Rapportåtgärder** sedan **Delning**.

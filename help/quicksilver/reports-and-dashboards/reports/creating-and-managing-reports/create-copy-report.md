---
product-area: reporting;user-management
keywords: spara,ny,rapport,kopiera
navigation-topic: create-and-manage-reports
title: Skapa en kopia av en rapport
description: Du kan skapa en kopia av alla rapporter som du har tillgång till. Du kan antingen skapa en exakt kopia av en anpassad rapport eller spara en ny version av en standardrapport. När du har kopierat en rapport blir du ägare till den kopierade rapporten och den visas i delen Mina rapporter.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Skapa en kopia av en rapport

<!-- Audited: 11/2024 -->

Du kan skapa en kopia av alla rapporter som du har tillgång till. Du kan antingen skapa en exakt kopia av en anpassad rapport eller spara en ny version av en standardrapport. När du har kopierat en rapport blir du ägare till den kopierade rapporten och den visas i delen Mina rapporter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter*</td> 
   <td><p>Visa behörigheter till en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en exakt kopia av en rapport

Om du vill skapa en kopia av en anpassad rapport gör du följande:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Reports]**.

1. Klicka på **Alla rapporter** och öppna sedan en rapport.

1. Klicka på **Rapportera åtgärder** och sedan på **Kopiera**.

   >[!TIP]
   >
   >Om rapporten är en standardrapport visas inte alternativet Kopiera på menyn Rapporteringsåtgärder.\
   >Mer information om hur du skapar en kopia av en standardrapport finns i [Skapa en ny version av en rapport](#create-a-new-version-of-a-report).

   ![Kopiera rapport](assets/unshimmed-report-actions-copy.png)

   En kopia av den ursprungliga rapporten skapas med standardnamnet _[Namnet på den ursprungliga rapporten] (kopia)_. En kopia av rapporten&quot;Kvarvarande aktiviteter under det fjärde kvartalet&quot; får till exempel namnet&quot;Kvarvarande aktiviteter under det fjärde kvartalet (kopia)&quot;.

1. (Valfritt) Om du vill byta namn på rapporten klickar du på **Rapportåtgärder** och sedan på **Redigera**. Skriv ett nytt namn i textrutan i det övre vänstra hörnet och klicka sedan på **Spara + stäng** när du är klar.

1. (Valfritt) Om du vill dela den nya versionen av rapporten med andra användare klickar du på **Rapportera åtgärder** och sedan på **Dela**.

   >[!NOTE]
   >
   >Delningsinformationen överförs inte till den kopierade rapporten från den ursprungliga versionen.\
   >Mer information om hur du ser vem den föregående rapporten delades med finns i [Skapa en rapport om rapportaktiviteter](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Valfritt) Om du har behörigheten Hantera för den ursprungliga rapporten och den ursprungliga rapporten inte längre behövs, kan du ta bort den för att ta bort onödiga dubblettrapporter i Workfront.

   Så här tar du bort den ursprungliga rapporten:

   1. Navigera till rapporten.

   1. Klicka på **Rapportera åtgärder** och sedan på **Ta bort**.

   1. Klicka på **Ja, ta bort den** för att bekräfta att du vill ta bort rapporten.

## Skapa en ny version av en rapport {#create-a-new-version-of-a-report}

Om du vill skapa en kopia av en inbyggd rapport gör du följande:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Rapporter** och sedan på **Alla rapporter**.
1. Klicka på namnet på en inbyggd rapport för att öppna den.
1. Klicka på **Rapportera åtgärder** och sedan på **Redigera**.

   ![Redigera rapport](assets/unshimmed-report-actions-default-report.png)

1. Gör de ändringar du behöver på följande flikar i rapporten:

   * **Kolumner (Visa)**: Mer information om hur du anpassar vyer finns i artikeln [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Grupperingar**: Mer information om hur du anpassar grupperingar finns i artikeln [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filter**: Mer information om hur du anpassar filter finns i artikeln [Filteröversikt](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Diagram**: Mer information om hur du anpassar ett rapportdiagram finns i artikeln [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Klicka på **Rapportinställningar** i det övre högra hörnet.
1. I fältet **Rapporttitel** ger du rapporten ett nytt namn.
1. Klicka på **Klar**.
1. Klicka på **Spara som ny rapport**.

   ![Spara som ny rapport](assets/unshimmed-save-as-new-report.png)

1. (Valfritt) Om du vill dela den nya versionen av rapporten med andra användare klickar du på **Rapportera åtgärder** och sedan på **Dela**.

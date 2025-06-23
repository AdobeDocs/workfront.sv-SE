---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visa alla uppdateringar i en anteckningsrapport
description: Om du vill se alla uppdateringar som någon av användarna har angett för ett objekt kan du skapa en anteckningsrapport som visar alla uppdateringar.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Visa alla uppdateringar i en anteckningsrapport

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Under Uppdateringar för ett objekt visas maximalt 200 uppdateringar som standard. Om du vill se alla uppdateringar som någon av användarna har angett för ett objekt kan du skapa en anteckningsrapport som visar alla uppdateringar.

>[!NOTE]
>
>Du kan skapa en rapport för att visa uppdateringar av objekt i Förhandsgranska med journalpostrapporten. Mer information finns i [Rapport om uppdateringsområdet med en journalpostrapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard </p>
   <p>Aktuell: Planera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa</p>
    <p>Obs! Om du inte har behörigheten Visa eller högre för ett objekt visas inte information för det objektet i rapporten.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Skapa en anteckningsrapport

Att skapa en rapport för anteckningar för ett objekt är identiskt, oavsett objektet.

Om du till exempel vill skapa en anteckningsrapport för alla anteckningar i ett projekt:

{{step1-to-reports}}

1. Klicka på **Ny rapport** i det övre vänstra hörnet på sidan och välj sedan **Obs!**.

1. (Valfritt) Klicka på **(Kolumner) Visa** och sedan på **Lägg till kolumn** för att lägga till **namnet** för **projektet** i rapportvyn. 

1. (Valfritt) Om du rapporterar flera projekt samtidigt klickar du på **Grupperingar** och sedan på **Lägg till gruppering** för att gruppera efter **namnet** för **projektet**. Detta gör att anteckningarna grupperas efter deras respektive projekt, vilket gör rapporten lättare att läsa. 

1. (Valfritt) Klicka på **Filter** och sedan på **Lägg till en filterregel**.
1. Lägg till ett filter för **Obs!** > **Anteckningstext** > **Är inte tom**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Om ett projektfält uppdaterades men ingen anteckning lades till vid tidpunkten för uppdateringen, visas **anteckningstexten** för uppdateringen som **(Ingen text har lagts till för uppdatering)**.


1. (Valfritt) Lägg till ett annat filter för **Projekt** > **Namn** > **Lika med** och lägg till ett eller flera projektnamn som du vill visa anteckningar för.
1. Klicka på **Spara + Stäng**. Alla uppdateringar som har angetts i projektet av alla användare med behörighet att visa projektet visas i rapporten.

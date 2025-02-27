---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visa alla uppdateringar i en anteckningsrapport
description: Visa alla uppdateringar i en anteckningsrapport
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Visa alla uppdateringar i en anteckningsrapport

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
   <td role="rowheader"><strong>Adobe Workfront</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Nytt: Standard </p>
   <p>Aktuell: Planera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa</p> <p><b>ANMÄRKNING</b></p>
   <p>Om du inte har behörigheten Visa eller högre för ett objekt visas inte information för det objektet i rapporten.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Skapa en anteckningsrapport

Att skapa en rapport för anteckningar för ett objekt är identiskt, oavsett objektet.

Om du till exempel vill skapa en anteckningsrapport för alla anteckningar i ett projekt:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Obs!**.

1. (Valfritt) Klicka på **Vyer** och sedan på **Lägg till kolumn** för att lägga till **namnet** för **projektet** i rapportvyn. 

1. (Valfritt) Klicka på **Grupperingar** och sedan på **Lägg till gruppering** i gruppen med **Projektnamn** om du rapporterar flera projekt samtidigt.\
   Detta gör att anteckningarna grupperas efter deras respektive projekt, vilket gör rapporten lättare att läsa. 

1. (Valfritt) Klicka på **Filter,** och sedan **Lägg till en filterregel**.
1. Lägg till ett filter för **Obs!** > **Anteckningstext** > **Är inte tom**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Om ett projektfält uppdaterades men ingen anteckning lades till vid tidpunkten för uppdateringen, visas **anteckningstexten** för uppdateringen som **(Ingen text har lagts till för uppdatering)**.


1. (Valfritt) Lägg till ett annat filter för **Projekt** > **Namn** > **Lika med** och lägg till ett eller flera projektnamn som du vill visa anteckningar för.
1. Klicka på **Spara + Stäng**.\
   Alla uppdateringar som har angetts i projektet av alla användare med behörighet att åtminstone visa projektet visas i rapporten.

---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visa alla uppdateringar i en anteckningsrapport
description: Visa alla uppdateringar i en anteckningsrapport
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Visa alla uppdateringar i en anteckningsrapport

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Under Uppdateringar för ett objekt visas maximalt 200 uppdateringar som standard. Om du vill se alla uppdateringar som någon av användarna har angett för ett objekt kan du skapa en anteckningsrapport som visar alla uppdateringar.

>[!NOTE]
>
>Du kan skapa en rapport för att visa uppdateringar av objekt i Förhandsgranska med journalpostrapporten. Mer information finns i [Rapport om uppdateringsområdet](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå.<br>Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa</p> <p>Obs! Om du inte har behörigheten Visa eller högre för ett objekt visas inte information för det objektet i rapporten.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en anteckningsrapport

Att skapa en rapport för anteckningar för ett objekt är identiskt, oavsett objektet.

Om du till exempel vill skapa en anteckningsrapport för alla anteckningar i ett projekt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Rapporter**.
1. Klicka **Ny rapport** väljer du **Anteckning**.

1. (Valfritt) Klicka på **Vyer** sedan **Lägg till kolumn** för att lägga till **Namn** i **Projekt** i rapportens vy. 

1. (Valfritt) Klicka på **Grupperingar** sedan **Lägg till gruppering** att gruppera efter **Projektnamn**, om du rapporterar om flera projekt samtidigt.\
   Detta gör att anteckningarna grupperas efter deras respektive projekt, vilket gör rapporten lättare att läsa. 

1. (Valfritt) Klicka på **Filter,** sedan **Lägg till en filterregel** för att filtrera efter endast ett projekt eller specifika projekt.

1. (Villkorligt och valfritt) Ange **Projektnamn** as **Jämn** till projektnamnet för det projekt som du vill visa uppdateringar för.  

1. Klicka **Spara + Stäng**.\
   Alla uppdateringar som har angetts i projektet av alla användare med behörighet att åtminstone visa projektet visas i rapporten.

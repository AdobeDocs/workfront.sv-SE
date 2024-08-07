---
navigation-topic: business-case-and-scorecards
title: Tillämpa ett styrkort på ett projekt och generera ett justeringsresultat
description: Du kan använda ett styrkort för att mäta hur väl ett projekt anpassar sig till de villkor som tidigare fastställts för en portfölj. Ett styrkort avspeglar ofta en organisations uppdrag, värderingar och strategiska mål.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Tillämpa ett styrkort på ett projekt och generera ett justeringsresultat

<!-- Audited: 02/2024 -->

Du kan använda ett styrkort för att mäta hur väl ett projekt anpassar sig till de villkor som tidigare fastställts för en portfölj. Ett styrkort avspeglar ofta en organisations uppdrag, värderingar och strategiska mål.

Mer information om styrkort och hur du kan skapa ett finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>
   <p>Nytt: Prime eller senare</p>
   <p>eller</p>
   <p>Aktuell: Business eller högre</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Visa eller ge senare åtkomst till Portfolio</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td><p>Hantera behörigheter för ett projekt</p> <p>Visa eller högre behörigheter för en portfölj</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Projektstyrkort {#project-scorecards}

* [Översikt över styrkort](#scorecards-overview)
* [Tillämpa ett styrkort på ett projekt](#apply-a-scorecard-to-a-project)

### Översikt över styrkort {#scorecards-overview}

Vanligtvis slutför en projektledare styrkortsinformationen för att skapa ett justeringsvärde mellan 0 och 100 för projektet. Värdet som skapas används senare när portföljförvaltaren granskar projekten i portföljoptimeraren för att jämföra dem.

Mer information om portföljoptimering finns i [Översikt över Portfolio-optimering](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Tillämpa ett styrkort på ett projekt

Som användare med en Standard- eller Plan-licens och Hantera-behörighet för ett projekt kan du bifoga ett styrkort till projektet.

Mer information om projektbehörigheter finns i [Dela ett projekt i Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Du kan lägga till styrkort i ett projekt som en del av arbetet med att skapa ett affärsärende för projektet.

Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Adobe Workfront-administratören eller gruppadministratören måste aktivera styrkortsavsnittet i projektdelen innan du kan komma åt styrkort från affärsärendet. Mer information om hur du ställer in projektinställningar och aktiverar områden i affärsärendet finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Så här använder du ett styrkort för ett projekt:

1. Gå till ett projekt som du vill tillämpa ett styrkort på.
1. Klicka på **Affärsfall** i den vänstra panelen.
1. Hitta avsnittet **Styrkort** i affärsärendet.\
   Du måste skapa ett styrkort innan avsnittet **Styrkort** visas i affärsärendet.

   Mer information om hur du skapar ett styrkort finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Välj ett styrkort i listrutan.

   ![Nytt styrkort](assets/new-scorecard.png)

1. Ange ett svar på alla frågor i styrkortet.

   Workfront poängsätter varje fråga och beräknar ett totalt projektresultat baserat på poängen i varje fråga.

   Mer information om generering av projektets övergripande justeringspoäng finns i [Generera en justeringspoäng för ett projekt](#generate-an-alignment-score-for-a-project).

1. Klicka på **Spara** för att spara styrkortet och poängsätta projektet.

   Styrkortet är nu kopplat till projektet och projektet poängsätts.

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## Generera en justeringspoäng

* [Skapa en justeringspoäng för ett projekt](#generate-an-alignment-score-for-a-project)
* [Generera en justeringspoäng för en portfölj](#generate-an-alignment-score-for-a-portfolio)

### Generera en justeringspoäng för ett projekt {#generate-an-alignment-score-for-a-project}

Justeringspoängen är det värde som skapas när styrkortet har slutförts.

Styrkort innehåller frågor med svarsalternativ som har tilldelats numeriska värden, så kallade justeringspunkter. Dessa punkter används för att avgöra hur väl projektet passar in i din organisation. Justeringspunkterna för varje fråga innehåller ett tal mellan 0 och 100.

När styrkortet är klart beräknar Workfront justeringspoängen för projektet i procent med hjälp av följande formel:

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

Mer information finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generera en justeringspoäng för en portfölj {#generate-an-alignment-score-for-a-portfolio}

Portföljens justeringspoäng är ett genomsnitt av justeringspoängen för alla projekt i portföljen.

När poängen för projekten är klara använder Workfront dessa värden för att beräkna portföljens justeringspoäng i procent med hjälp av följande formel:

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Om ett projekt inte har något associerat styrkort och därför inte har någon justeringspoäng, anses det att portföljen har en justering på 0 %. Projektet beaktas i antalet projekt i portföljen.

## Visa justeringspoäng

Du kan visa justeringspoängen för ett projekt på projektnivå eller i Portfolio-optimering.

* [Visa justeringsresultat för ett projekt](#view-the-alignment-score-on-a-project)
* [Visa justeringspoängen för projektet och för portföljen i optimeringsverktyget för Portfolio](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Visa justeringspoäng i ett projekt

Du kan visa justeringspoängen för ett projekt på projektnivå om du har Contribute-behörighet till projektet.

1. Gå till det projekt vars justeringspoäng du vill visa.
1. Klicka på **Affärsfall** i den vänstra panelen.
1. Gå till **Översikt över affärsärenden** till höger på skärmen.

   Justeringspoängen finns i affärsärendesammanfattningen i värdet **Justerad**.

   ![Justeringspoäng i ett projekt](assets/alignment-score-on-a-project.png)

### Visa justeringspoängen för projektet och för portföljen i optimeringsverktyget för Portfolio

Du kan visa justeringspoängen för ett projekt eller för en portfölj i Optimera för Portfolio om du har Hantera-åtkomst till portföljen.

Mer information om vilken information som visas i Portfolio-optimering finns i [Översikt över Portfolio-optimering](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Leta reda på projektets justeringspoäng i Optimering för Portfolio](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Leta reda på portföljens justeringspoäng i optimeraren för Portfolio](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![Justeringspoäng i Portfolio-optimering](assets/alignment-score-in-portfolio-optimizer.png)

#### Leta reda på projektets justeringspoäng i Optimering för Portfolio {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Klicka på namnet på en portfölj.
1. Klicka på **Optimering av Portfolio** på den vänstra panelen.

   Optimeraren för Portfolio visas.

   Justeringspoängen för ett projekt visas som ett procenttal i kolumnen **Justering** i optimeraren för Portfolio.

   Detta är projektets justeringspoäng baserat på det styrkort som är associerat med projektet.

#### Leta reda på portföljens justeringspoäng i optimeraren för Portfolio  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Klicka på namnet på en portfölj.
1. Klicka på **Optimering av Portfolio** på den vänstra panelen.
1. Överst i optimeringsprogrammet för Portfolio hittar du värdet **Justerad** samt måttet **Justering** som anger portföljens justeringspoäng.

   Detta är portföljens justeringspoäng.

   Mer information om hur justeringspoängen för en portfölj genereras finns i [Skapa en justeringspoäng för en portfölj](#generate-an-alignment-score-for-a-portfolio).

## Översikt över Portfolio Optimizer-poängen

Det finns en skillnad mellan justeringspoängen och portföljoptimeringspoängen för ett projekt.

Justeringspoängen för ett projekt beräknas utifrån de poäng som erhålls när styrkortet har fyllts i. Poängen används sedan för att fastställa poängen för portföljjusteringen. Justeringspoängen visas i procent.

Justeringspoängen för ett projekt visas i kolumnen **Justering** i optimeraren för Portfolio.

Poängen för portföljoptimering är en rankning som automatiskt beräknas i optimeringsfunktionen för Portfolio som projekt kan prioriteras efter. Poängen för portföljoptimering visas som en indikatorikon tillsammans med ett tal och visas i kolumnen **Poäng** i optimeraren för Portfolio. Poängen Portfolio Optimizer genereras endast när alla avsnitt i affärsärendet är slutförda, utom för mål.

Mer information om hur du skapar ett affärsärende för ett projekt finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Mer information om hur du beräknar portföljoptimeringspoängen för ett projekt finns i [Översikt över Portfolio Optimizer-poängen](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

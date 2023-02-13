---
navigation-topic: business-case-and-scorecards
title: Tillämpa ett styrkort på ett projekt och generera ett justeringsresultat
description: Du kan använda ett styrkort för att mäta hur väl ett projekt anpassar sig till de villkor som tidigare fastställts för en portfölj. Ett styrkort avspeglar ofta en organisations uppdrag, värderingar och strategiska mål.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# Tillämpa ett styrkort på ett projekt och generera ett justeringsresultat

Du kan använda ett styrkort för att mäta hur väl ett projekt anpassar sig till de villkor som tidigare fastställts för en portfölj. Ett styrkort avspeglar ofta en organisations uppdrag, värderingar och strategiska mål.

Mer information om styrkort och hur du kan skapa ett finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Visa eller ge senare åtkomst till Portfolio</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p> <p>Visa eller högre behörigheter för en portfölj </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Projektstyrkort {#project-scorecards}

* [Översikt över styrkort](#scorecards-overview)
* [Projektstyrkort](#project-scorecards)

### Översikt över styrkort {#scorecards-overview}

Vanligtvis slutför en projektledare styrkortsinformationen för att skapa ett justeringsvärde mellan 0 och 100 för projektet. Värdet som skapas används senare när portföljförvaltaren granskar projekten i portföljoptimeraren för att jämföra dem.

Mer information om portföljoptimering finns i artikeln [Portfolio Optimizer - översikt](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Tillämpa ett styrkort på ett projekt

Som användare med en planlicens och behörigheten Hantera för ett projekt kan du bifoga ett styrkort till projektet.

Mer information om projektbehörigheter finns i [Dela ett projekt i Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Du kan lägga till styrkort i ett projekt som en del av arbetet med att skapa ett affärsärende för projektet.

Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Adobe Workfront-administratören eller gruppadministratören måste aktivera styrkortsavsnittet i projektdelen innan du kan komma åt styrkort från affärsärendet. Mer information om hur du ställer in projektinställningar och aktiverar områden i affärsärendet finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Så här använder du ett styrkort för ett projekt:

1. Gå till ett projekt som du vill tillämpa ett styrkort på.
1. Klicka **Affärsärende** i den vänstra panelen.
1. Hitta **Styrkort** i affärsärendet.\
   Du måste skapa ett styrkort före **Styrkort** visas i affärsärendet.

   Mer information om hur du skapar ett styrkort finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Välj ett styrkort i listrutan.

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. Ange ett svar på alla frågor i styrkortet.

   Workfront poängsätter varje fråga och beräknar ett totalt projektresultat baserat på poängen i varje fråga.

   Mer information om generering av projektets övergripande justeringspoäng finns i [Generera en justeringspoäng för ett projekt](#generate-an-alignment-score-for-a-project).

1. Klicka **Spara** för att spara styrkortet och poängsätta projektet.

   Styrkortet är nu kopplat till projektet och projektet poängsätts.

## Generera en justeringspoäng

* [Generera en justeringspoäng för ett projekt](#generate-an-alignment-score-for-a-project)
* [Generera en justeringspoäng för en portfölj](#generate-an-alignment-score-for-a-portfolio)

### Generera en justeringspoäng för ett projekt {#generate-an-alignment-score-for-a-project}

Justeringspoängen är det värde som skapas när styrkortet har fyllts i.

Styrkort innehåller frågor med svarsalternativ som har tilldelats numeriska värden, så kallade justeringspunkter. Dessa punkter används för att avgöra hur väl projektet passar in i din organisation. Justeringspunkterna för varje fråga innehåller ett tal mellan 0 och 100.

När styrkortet är klart beräknar Workfront justeringspoängen för projektet i procent med hjälp av följande formel:

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

Mer information finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generera en justeringspoäng för en portfölj {#generate-an-alignment-score-for-a-portfolio}

Portföljens justeringspoäng är ett genomsnitt av justeringspoängen för alla projekt i portföljen.

När poängen för projekten är klara använder Workfront dessa värden för att beräkna portföljens justeringspoäng i procent med hjälp av följande formel:

Justeringspoäng för Portfolio = Summan av procentsatserna för projektjusteringspoängen/ Antal projekt i portföljen

>[!NOTE]
>
>Om ett projekt inte har något associerat styrkort och därför inte har någon justeringspoäng, anses portföljen ha en justering på 0 %. Projektet beaktas i antalet projekt i portföljen.

## Visa justeringspoäng

Du kan visa justeringspoängen för ett projekt på projektnivå eller i Portfolio-optimering.

* [Visa justeringspoäng i ett projekt](#View%20the)
* [Visa justeringspoängen för projektet och för portföljen i optimeringsverktyget för Portfolio](#View%20the2)

### Visa justeringspoäng i ett projekt

Du kan visa justeringspoängen för ett projekt på projektnivå om du har Contribute-behörighet till projektet.

1. Gå till det projekt vars justeringspoäng du vill visa.
1. Klicka **Affärsärende** i den vänstra panelen.
1. Gå till **Översikt över affärsärenden** till höger på skärmen.

   Justeringspoängen finns i Översikt över affärsfall i **Justerad** värde.

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### Visa justeringspoängen för projektet och för portföljen i optimeringsverktyget för Portfolio

Du kan visa justeringspoängen för ett projekt eller för en portfölj i Optimera för Portfolio om du har Hantera-åtkomst till portföljen.

Mer information om vilken information som visas i Portfolio-optimering finns i [Portfolio Optimizer - översikt](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Leta reda på projektets justeringspoäng i Optimering för Portfolio](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Leta reda på portföljens justeringspoäng i optimeraren för Portfolio](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### Leta reda på projektets justeringspoäng i Optimering för Portfolio {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)sedan **Portfolio**.

1. Klicka på namnet på en Portfolio.
1. Klicka **Optimering för Portfolio** i den vänstra panelen.

   Portfolio Optimizer visas.

1. Justeringspoängen för ett projekt visas i procent i **Justering** i Portfolio Optimizer.

   Detta är projektets justeringspoäng baserat på det styrkort som är associerat med projektet.

#### Leta reda på portföljens justeringspoäng i optimeraren för Portfolio  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. Gå till **Projekt** i fältet Global navigering.
1. Välj **Portfolio** -fliken.
1. Klicka på namnet på en Portfolio.
1. Välj **Optimering för Portfolio** -fliken.
1. Överst i Portfolio Optimizer finns **Justerad** och **Justering** En mätare som anger portföljens justeringspoäng.

   Detta är portföljens justeringspoäng.

   Mer information om hur justeringspoängen för en portfölj genereras finns i [Generera en justeringspoäng för en portfölj](#generate-an-alignment-score-for-a-portfolio).

## Översikt över Portfolio Optimizer-poängen

Det finns en skillnad mellan justeringspoängen och portföljoptimeringspoängen för ett projekt.

Justeringspoängen för ett projekt beräknas utifrån de poäng som erhålls när styrkortet har fyllts i. Poängen används sedan för att fastställa poängen för portföljjusteringen. Justeringspoängen visas i procent.

Justeringspoängen för ett projekt visas i **Justering** i Portfolio Optimizer.

Poängen för portföljoptimering är en rankning som automatiskt beräknas i optimeringsfunktionen för Portfolio som projekt kan prioriteras efter. Poängen för portföljoptimering visas som en indikatorikon tillsammans med ett tal och visas i **Poäng** i Portfolio Optimizer. Poängen Portfolio Optimizer genereras endast när alla avsnitt i affärsärendet är slutförda, utom för mål.

Mer information om hur du skapar ett affärsärende för ett projekt finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Mer information om hur du beräknar portföljoptimeringspoängen för ett projekt finns i [Översikt över Portfolio Optimizer-poängen](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

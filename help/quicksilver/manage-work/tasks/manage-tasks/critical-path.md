---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Översikt över projektets kritiska sökväg
description: Att fastställa den kritiska vägen för ett projekt är ett automatiskt sätt för Adobe Workfront att flagga en sekvens av uppgifter i ett projekt som kan påverka tidslinjen i projektet. Uppgifter som kan påverka tidslinjen i projektet flaggas som uppgifter för kritisk sökväg.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Översikt över projektets kritiska sökväg

Att fastställa den kritiska vägen för ett projekt är ett automatiskt sätt för Adobe Workfront att flagga en sekvens av uppgifter i ett projekt som kan påverka tidslinjen i projektet. Uppgifter som kan påverka tidslinjen i projektet flaggas som uppgifter för kritisk sökväg.

Följande funktioner kan påverka projektets kritiska väg:

* Projektets arbetsstruktur.

   Mer information om arbetsstruktur finns i [Bestämma struktur för arbetsfördelning i ett projekt](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* Den tid (varaktighet) som varje aktivitet tar att slutföra.
* Beroenden mellan aktiviteterna.

   Tänk på följande:

   * När en uppgift på den kritiska sökvägen har en föregående relation, är dess föregångare och efterföljare också på den kritiska vägen om datumändringarna för föregående eller efterföljande aktiviteter direkt påverkar deras underordnade.

      >[!TIP]
      >
      >När datumet för en efterföljande uppgift inte direkt påverkar datumet för deras beroende uppgifter och det inte påverkar datumen för projektet, ligger den efterföljande uppgiften inte på den kritiska sökvägen.
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * När en underaktivitet identifieras som en kritisk sökvägsuppgift identifieras även den överordnade aktiviteten som en kritisk sökvägsuppgift, om det planerade startdatumet och starttiden för den överordnade aktiviteten är samma som för underaktiviteten.

Med dessa funktioner i åtanke beräknar systemet den kritiska sökvägen genom att använda den längsta vägen mellan den tidigaste uppgiften och den uppgift som bestämmer projektets slut. Vid beräkning av kritisk sökväg beaktas den tidigaste och senaste gången som varje uppgift kan starta och slutföras utan att projektet blir längre. Den här processen avgör vilka uppgifter som är&quot;kritiska&quot; (och tillhör den längsta banan) och vilka som har&quot;totalt flytande&quot; (kan fördröjas utan att projektet blir längre).

Eventuella förseningar i en uppgiftsaktivitet på den kritiska vägen påverkar direkt projektets planerade slutförandedatum (det finns inget flytande på den kritiska vägen).

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för en uppgift </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa den kritiska sökvägen

Du kan visa de uppgifter som hör till den kritiska sökvägen i följande områden i Workfront-programmet:

* [Visa den kritiska sökvägen i Gantt-diagrammet](#view-the-critical-path-in-the-gantt-chart)
* [Visa den kritiska sökvägen i en uppgiftslista eller rapport](#view-the-critical-path-in-a-task-list-or-report)

### Visa den kritiska sökvägen i Gantt-diagrammet {#view-the-critical-path-in-the-gantt-chart}

Så här visar du uppgifter på den kritiska sökvägen i Gantt-schemat:

1. Gå till ett projekt som du vill visa den kritiska sökvägen för.
1. Klicka **Uppgifter** i den vänstra panelen.
1. Klicka på **Gantt-schema** i det övre högra hörnet av uppgiftslistan.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. Expandera **Alternativ** aktiverar du **Kritisk sökväg** alternativ.

   De uppgifter som finns på den kritiska sökvägen har en röd linje ovanför tidslinjen i Gantt-diagrammet.

   ![crtitical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Visa den kritiska sökvägen i en uppgiftslista eller rapport {#view-the-critical-path-in-a-task-list-or-report}

Så här visar du vilka uppgifter som finns på den kritiska sökvägen i en lista över uppgifter:

1. Gå till ett projekt som du vill visa den kritiska sökvägen för.
1. Klicka **Uppgifter** i den vänstra panelen.
1. Från **Visa** nedrullningsbar meny, välja **Status**.

   De uppgifter som finns på den kritiska banan har en **Kritisk sökväg** flagga i **Flaggor** -kolumn i listan.

   Du kan använda samma vy för en uppgiftsrapport.

   Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   eller

   Från **Filter** nedrullningsbar meny, välja **Nytt filter**.

1. Klicka **Lägg till filterregel** och börja skriva **Är kritisk** i **Visa bara uppgifter där ...** fält.

1. Markera den när den visas i listan.
1. Klicka **Spara filter**.

   Listan ska endast visa uppgifter som finns på den kritiska sökvägen.

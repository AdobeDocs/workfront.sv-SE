---
product-area: reporting
navigation-topic: reporting-elements
title: Använda vyn Milstolpe
description: Du kan använda vyn Milstolpe på en projektlista eller rapport. Du kan använda vyn Milstolpe för att visa alla milstolpar som är kopplade till uppgifter i de projekt som du visar.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# Använda vyn Milstolpe

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<div class="preview">

Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Samma funktioner är också tillgängliga i produktionsmiljön för alla kunder från och med en vecka från förhandsversionen.

Mer information finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Du kan använda vyn Milstolpe på en projektlista eller rapport. Du kan använda vyn Milstolpe för att visa alla milstolpar som är kopplade till uppgifter i de projekt som du visar.

Innan du kan använda milstolpevyn måste följande element finnas:

* Sökvägar för milstolpar har konfigurerats. Mer information finns i [Skapa en milstolpe-sökväg](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* Milstolpesökvägar som behövs läggs till i projekt. Mer information finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).
* Milstolpar är associerade med uppgifter. Mer information finns i [Associera milstolpar med uppgifter](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

Vyn Milstolpe är tillgänglig när du visar en projektlista eller en projektrapport. I följande avsnitt beskrivs hur du visar och använder milstolpevyn.

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
   <td role="rowheader">Adobe Workfront-licens</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Arbeta eller högre</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomst till rapporter, instrumentpaneler och kalendrar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
    <td> <p>Visa behörigheter för en projektrapport om du vill använda milstolpevyn på en rapport</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Växla till vyn Milstolpe {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Klicka på listrutan **Visa** och sedan på **Milstolpe**.

   Listan eller rapporten visas i en milstolpe-vy.

   Mer information om milstolpevyn finns i avsnittet [Översikt över milstolpevyn](#milestone-view-overview) i den här artikeln.

## Översikt över milstolpe {#milestone-view-overview}

<div class="preview">

Vyn Milstolpe är tillgänglig i projektlistor och projektrapporter. Du kan snabbt visa alla milstolpar som är kopplade till uppgifter i de projekt du visar.

![Projekt med milstolpe-vy](assets/project-with-milestone-view-with-complete.png)

</div>

>[!NOTE]
>
>Vyn Milstolpe är inte tillgänglig i följande områden:
>
>* Tidrapporter, i projektlistan när du lägger till ett projekt.

Mer information om hur du växlar till vyn Milstolpe finns i avsnittet [Växla till vyn Milstolpe](#switch-to-the-milestone-view) i den här artikeln.


### Vyavsnitt för milstolpe

När du använder vyn Milstolpe på en lista med projekt visas projekten i följande avsnitt:

* De projekt som är associerade med en milstolpbana visas först, listade under namnet på deras respektive milstolpbanor.

  Workfront sorterar projekten i det första avsnittet efter följande kriterier, i denna ordning:

   1. Sökväg-ID för milstolpe. Du kan visa ID för milstolpe-sökväg i en rapport för milstolpe-sökväg.

   2. Det fält som valts som det första sorteringsfältet för projektlistan i den vy som tidigare använts på projektlistan, innan du valde vyn Milstolpe.

* De projekt som inte är associerade med en Milestobe Path visas därefter i avsnittet Ej tilldelad. Workfront sorterar projekten i avsnittet Ej tilldelad efter det fält som valts som det första sorteringsfältet för projektlistan i den vy som tidigare använts på projektlistan, innan du valde vyn Milstolpe.

### Projektinformation i milstolpevyn

När du visar en projektlista eller en projektrapport i vyn Milstolpe är följande information tillgänglig:

* **Planerade datum eller planerade datum:** Ange om du vill visa planerade datum eller planerade datum i milstolpsvyn.\
  Datum visas för start- och slutförandedatum för projektet, samt för slutförande av varje milstolpeuppgift i milstolpebanan.

  Om du visar Projicerade datum kan datumen inte redigeras. Planerade datum beräknas av Workfront och kan inte ändras manuellt.

  Om du visar Planerade datum och även har Hantera-åtkomst till projektet kan du redigera följande datum direkt från milstolpevyn:

   * **Projektets startdatum:** Om ett projekt har schemalagts från startdatumet kan du ändra projektets planerade startdatum manuellt, och sedan beräknas det planerade slutförandedatumet.
   * **Datum för projektslutförande:** Om ett projekt har schemalagts från det planerade slutförandedatumet kan du ändra projektets planerade slutförandedatum manuellt, och det planerade startdatumet beräknas sedan.
   * **Datum för slutförande av aktivitet:** Du kan uppdatera det planerade slutförandedatumet manuellt för aktiviteter direkt från milstolpe-vyn.

* **Procent färdigt:** Visar slutförandeprocenten för varje aktivitet och projekt.

  Du kan inaktivera att procentandelen slutförande visas, vilket beskrivs i avsnittet [Konfigurera vilken information som ska visas i vyn Milstolpe](#configure-what-information-displays-in-the-milestone-view) i den här artikeln.

  Du kan justera procentandelen för slutförande direkt från vyn Milstolpe, vilket beskrivs i avsnittet [Justera procent färdigt för aktiviteter i vyn Milstolpe](#adjust-percent-complete-for-tasks-in-the-milestone-view) i den här artikeln.

* **Statusikoner för aktivitetens förlopp:** Beroende på vilken miljö du använder för att visa milstolpevyn visas följande ikoner som anger aktivitetens förloppsstatus:

   * I produktionsmiljön visas följande statusikoner bredvid varje projekt och uppgift i vyn Milstolpe:

      * I tid\
        ![Ikon i tid](assets/gantt-ontime.png)

      * Bakom\
        ![Bakom-ikon](assets/gantt-behind.png)

      * Risk\
        ![Riskikon](assets/gantt-atrisk.png)

      * Sena\
        ![Sena ikonen](assets/gantt-late.png)

     <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <div class="preview">

   * I förhandsgranskningsmiljön visas följande färgade cirklar bredvid varje projekt och uppgift i vyn Milstolpe:

      * I tid - grön
      * Bakom - gul
      * Risk - blå
      * Sena - röda

  </div>

  Du kan inaktivera att dessa statusikoner visas, vilket beskrivs i avsnittet [Konfigurera vilken information som ska visas i vyn Milstolpe](#configure-what-information-displays-in-the-milestone-view) i den här artikeln.

  Mer information om respektive statustyp finns i artikeln [Översikt över status för aktivitetsstatus](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Skuggning av aktivitetsstatus för slutförda aktiviteter**: När en aktivitet har markerats som Slutförd skuggas bakgrunden för aktiviteten i milstolpe-vyn för att ange om aktiviteten slutfördes i tid eller sent:

   * **Röd skuggning för aktivitetskolumnen**: Bakgrunden till en aktivitet är röd när förloppsstatusen är **Sent**.

   * **Grön skuggning för aktivitetskolumnen**: Bakgrunden till en aktivitet är grön när förloppsstatusen är **Vid tid**.

* **Projektstatusskuggning för kolumnerna Start och Slutförd för projekt**:

   * **Projektets startkolumn**: Bakgrunden för projektets startkolumn är röd eller grön endast när det faktiska startdatumet har fyllts i:

      * **Röd skuggning för projektstartkolumn**: Bakgrunden i projektstartkolumn är röd när projektets förloppsstatus är **Sent**.

      * **Grön skuggning för projektstartkolumn**: Bakgrunden i projektstartkolumnen är grön när projektets förloppsstatus är **Vid tid**.

     >[!TIP]
     >
     >Du måste gå till sidan Projektinformation för att visa projektets faktiska startdatum.

   * **Kolumn för projektslutförande**: Bakgrunden i kolumnen Projektslutförande är röd eller grön endast när Faktiskt slutförandedatum har fyllts i:

      * **Röd skuggning för projektslutförandekolumn**: Bakgrunden i kolumnen Projektslutförande är röd när projektets förloppsstatus är **Sent**.

      * **Grön skuggning för kolumnen Projektslutförande**: Bakgrunden i kolumnen Projektslutförande är grön när projektets förloppsstatus är **Vid tid**.

     >[!TIP]
     >
     >Du måste gå till sidan Projektinformation för att visa projektets faktiska slutförandedatum.

   * Ingen färgskuggning tilldelas till kolumnerna Start och Slutförd när aktiviteterna har statusvärdet Vid risk eller Efter.

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![Vyn Milstolpe med skuggning](assets/milestone-view-with-shading.png)

* **Projektnamn**: Projektnamnet visas med en länk till projektet.
* **Ikon för projektvillkor**: Beroende på vilken miljö du använder vyn Milstolpe från följande indikatorer visar projektvillkoret:

   * I produktionsmiljön visas en ikon bredvid projektnamnet som anger projektets villkor. Projektets villkor kan vara något av följande:

      * På mål
      * Risk
      * I problem

  <div class="preview">

   * I förhandsvisningsmiljön visas en villkorsikon i form av en färgad cirkel bredvid varje projekt. Möjliga projektvillkor och cirkelfärger är:

      * On Target - green
      * Risk - gul
      * I problem - röd

     </div>


## Konfigurera vilken information som ska visas i vyn Milstolpe {#configure-what-information-displays-in-the-milestone-view}

Du kan konfigurera om följande element ska visas i vyn Milstolpe:

* Statusikoner för förlopp
* Procent färdigt med projekt och uppgifter

Som standard visas förloppsikoner och procent färdigt projekt och uppgifter.

De ändringar du gör i dessa alternativ gäller bara dig. Övriga användare påverkas inte. De ändringar du gör behålls nästa gång du loggar in på Workfront.

Så här konfigurerar du om projektstatusikoner och procent slutförda projekt ska visas:

{{step1-to-projects}}

1. Klicka på listrutan **Visa** och sedan på **Milstolpe**.

1. I produktionsmiljön klickar du på **Alternativ** i det övre högra hörnet av vyn Milstolpe och väljer sedan bland alternativen i nästa steg.

   ![millestone_view_options.png](assets/milestone-view-options-350x141.png)

   <div class="preview">I förhandsgranskningsmiljön väljer du bland alternativen i nästa steg i det övre högra hörnet av vyn Milstolpe.</div>

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->


1. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status för förlopp</td> 
      <td> <p>Välj det här alternativet om du vill visa förloppsikoner bredvid varje projekt och uppgift.</p> <p>Det här alternativet är aktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procent färdigt</td> 
      <td> <p>Välj det här alternativet om du vill visa procentandelen för slutförande bredvid varje projekt och uppgift.</p> <p>Det här alternativet är aktiverat som standard.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Justera procent färdigt för uppgifter i vyn Milstolpe {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Du kan justera Procent färdigt för uppgifter i vyn Milstolpe. Du kan inte justera Procent färdigt för en överordnad aktivitet (en aktivitet som innehåller underaktiviteter) eller för ett projekt.

Så här justerar du procentandelen färdigt för en aktivitet i vyn Milstolpe:

{{step1-to-projects}}

1. Klicka på listrutan **Visa** och sedan på **Milstolpe**.

1. (Villkorligt) Om procentsatser för slutförande inte visas för närvarande i vyn Milstolpe aktiverar du visningen av uppgifter och projekt för Procent färdigt enligt beskrivningen i avsnittet [Konfigurera vilken information som ska visas i vyn Milstolpe](#configure-what-information-displays-in-the-milestone-view) i den här artikeln.

1. I produktionsmiljön klickar du på procentsatsen för slutförande under en uppgift, anger en ny procentsats och trycker sedan på Retur.

   <div class="preview">I förhandsvisningsmiljön flyttar du reglaget Procent färdigt till det nya Procent färdigt för att uppdatera det. </div>

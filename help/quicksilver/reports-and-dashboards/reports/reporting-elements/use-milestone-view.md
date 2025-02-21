---
product-area: reporting
navigation-topic: reporting-elements
title: Använda vyn Milstolpe
description: Du kan använda vyn Milstolpe på en projektlista eller rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 0%

---

# Använda vyn Milstolpe

<!-- Audited: 11/2024 -->

Du kan använda vyn Milstolpe på en projektlista eller rapport.

Innan du kan använda milstolpevyn måste milstolpar konfigureras, milstolpbanor måste läggas till i projekt och milstolpar måste kopplas till aktiviteter, vilket beskrivs i artiklarna [Skapa en milstolpssökväg](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) och [Koppla milstolpar till aktiviteter](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

Vyn Milstolpe är tillgänglig när du visar en projektlista eller en projektrapport. I följande avsnitt beskrivs hur du visar och använder milstolpevyn.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Arbeta eller högre</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Visa eller öka åtkomst till rapporter, instrumentpaneler och kalendrar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa behörigheter för en projektrapport om du vill använda milstolpevyn på en rapport</p> </td> 
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

Vyn Milstolpe är tillgänglig i projektlistor och projektrapporter. I den här vyn kan du snabbt visa alla milstolpar som är kopplade till uppgifter i projekt som du visar.


>[!NOTE]
>
>Vyn Milstolpe är inte tillgänglig i följande områden:
>
>* Tidrapporter, i projektlistan när du lägger till ett projekt.


Mer information om hur du växlar till vyn Milstolpe finns i avsnittet [Växla till vyn Milstolpe](#switch-to-the-milestone-view) i den här artikeln.

![Projekt med milstolpe-vy](assets/project-with-milestone-view-with-complete.png)

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
  Datum visas för Start och Slutförande samt för varje milstolpe i milstolpen.\
  Om du visar Planerade datum och även har Hantera-åtkomst till projektet kan du redigera följande datum direkt från vyn Milstolpe: (Om du visar Projicerade datum kan datumen inte redigeras eftersom Projicerade datum beräknas och inte kan ändras manuellt.)

   * **Projektets startdatum:** Om ett projekt har schemalagts från startdatumet kan du ändra startdatumet för projektet manuellt och sedan beräkna slutförandedatumet.
   * **Datum för projektslutförande:** Om ett projekt har schemalagts från slutförandedatumet kan du ändra projektets slutförandedatum manuellt och sedan beräkna startdatumet.
   * **Datum för slutförande av aktivitet:** Du kan uppdatera slutförande manuellt för aktiviteter direkt från milstolpe-vyn.

* **Procent färdigt:** Visar slutförandeprocenten för varje aktivitet och projekt.\
  Du kan inaktivera att procentandelen slutförande visas, vilket beskrivs i avsnittet [Konfigurera vilken information som ska visas i vyn Milstolpe](#configure-what-information-displays-in-the-milestone-view) i den här artikeln.\
  Du kan justera procentandelen för slutförande direkt från vyn Milstolpe, vilket beskrivs i avsnittet [Justera procent färdigt för aktiviteter i vyn Milstolpe](#adjust-percent-complete-for-tasks-in-the-milestone-view) i den här artikeln.

* **Ikoner för aktivitetsstatus:** En statusikon visas bredvid varje projekt och uppgift i vyn Milstolpe.

   * I tid\
     ![Ikon i tid](assets/gantt-ontime.png)

   * Bakom\
     ![Bakom-ikon](assets/gantt-behind.png)

   * Risk\
     ![Riskikon](assets/gantt-atrisk.png)

   * Sena\
     ![Sena ikonen](assets/gantt-late.png)

  Du kan inaktivera att dessa statusikoner visas, vilket beskrivs i avsnittet [Konfigurera vilken information som ska visas i vyn Milstolpe](#configure-what-information-displays-in-the-milestone-view) i den här artikeln.\
  Mer information om respektive statustyp finns i artikeln [Översikt över status för aktivitetsstatus](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Skuggning av aktivitetsstatus för slutförda aktiviteter**: När en aktivitet har markerats som Slutförd skuggas bakgrunden för aktiviteten i milstolpe-vyn för att ange om aktiviteten slutfördes i tid eller sent:

   * **Röd skuggning för aktivitetskolumnen**: Bakgrunden till en aktivitet är röd när förloppsstatusen är **Sent**.

   * **Grön skuggning för aktivitetskolumnen**: Bakgrunden till en aktivitet är grön när förloppsstatusen är **Vid tid**.

* **Projektstatusskuggning för kolumnerna Start och Slutförd för projekt**:

   * **Projektets startkolumn**: Bakgrunden för projektets startkolumn är röd eller grön endast när det faktiska startdatumet har fyllts i:

      * **Röd skuggning för projektstartkolumn**: Bakgrunden i projektstartkolumn är röd när projektets förloppsstatus är **Sent**.

      * **Grön skuggning för projektstartkolumn**: Bakgrunden i projektstartkolumnen är grön när projektets förloppsstatus är **Vid tid**.

   * **Kolumn för projektslutförande**: Bakgrunden i kolumnen Projektslutförande är röd eller grön endast när Faktiskt slutförandedatum har fyllts i:

      * **Röd skuggning för projektslutförandekolumn**: Bakgrunden i kolumnen Projektslutförande är röd när projektets förloppsstatus är **Sent**.

      * **Grön skuggning för kolumnen Projektslutförande**: Bakgrunden i kolumnen Projektslutförande är grön när projektets förloppsstatus är **Vid tid**.

   * Ingen färgskuggning tilldelas till kolumnerna Start och Slutförd när aktiviteterna har statusvärdet Vid risk eller Efter.

  ![Vyn Milstolpe med skuggning](assets/milestone-view-with-shading.png)

* **Projektnamn**: Projektnamnet visas med en länk till projektet.
* **Ikon för projektvillkor**: En ikon visas bredvid projektnamnet som anger projektets villkor.

## Konfigurera vilken information som ska visas i vyn Milstolpe {#configure-what-information-displays-in-the-milestone-view}

Du kan konfigurera om följande element ska visas i vyn Milstolpe:

* Statusikoner för förlopp
* Procent färdigt med projekt och uppgifter

Som standard visas projektstatusikoner och procent färdigt projekt.

De ändringar du gör i dessa alternativ gäller bara dig. Övriga användare påverkas inte. De ändringar du gör behålls nästa gång du loggar in på Adobe Workfront.

Så här konfigurerar du om projektstatusikoner och procent slutförda projekt ska visas:

{{step1-to-projects}}

1. Klicka på listrutan **Visa** och sedan på **Milstolpe**.\
   Om du visar en lista med projekt i en Portfolio eller ett program väljer du underfliken **Milstolpe**.

1. Klicka på **Alternativ** i det övre högra hörnet i vyn Milstolpe.\
   ![millestone_view_options.png](assets/milestone-view-options-350x141.png)

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

Du kan justera Procent färdigt för uppgifter i vyn Milstolpe. Du kan inte justera Procent färdigt för en överordnad aktivitet (en aktivitet som innehåller underaktiviteter).

Så här justerar du procentandelen färdigt för en aktivitet i vyn Milstolpe:

{{step1-to-projects}}

1. Klicka på listrutan **Visa** och sedan på **Milstolpe**.

1. (Villkorligt) Om procentsatser för slutförande inte visas i vyn Milstolpe klickar du på **Alternativ** i det övre högra hörnet i vyn Milstolpe och kontrollerar sedan att **Procent färdigt** är aktiverat.

1. Klicka på procentsatsen för slutförande under en uppgift, ange en ny procentsats och tryck sedan på Retur.

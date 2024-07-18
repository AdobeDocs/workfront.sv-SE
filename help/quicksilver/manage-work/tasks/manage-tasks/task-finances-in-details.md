---
product-area: projects
navigation-topic: manage-tasks
title: Hantera aktivitetsfinanser i avsnittet Uppgiftsinformation
description: Hantera aktivitetsfinanser i avsnittet Uppgiftsinformation
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---

# Hantera aktivitetsfinanser i avsnittet Uppgiftsinformation

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Du kan visa eller redigera den ekonomiska informationen för en uppgift genom att gå till området Översikt i avsnittet Uppgiftsinformation. Det finns ett begränsat antal fält som du kan visa eller redigera i det här området. Mer information om hur du redigerar all ekonomisk information för en uppgift finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Redigera åtkomst till projekt och uppgifter</p> <p>Visa åtkomst till finansiella data eller högre</p> <p>Du måste ha Redigera åtkomst till ekonomiska data för att kunna redigera ekonomisk information om aktiviteter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för aktiviteten som innehåller View Finance eller senare</p> <p>Du måste ha behörigheten Hantera för den uppgift som innehåller Redigera ekonomi för att kunna redigera ekonomisk information om uppgifter</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Redigera aktivitetsfinanser i avsnittet Uppgiftsinformation

1. Gå till ett projekt där du vill visa en uppgift.

   >[!NOTE]
   >
   >Om du vill söka efter en uppgift kan du också söka efter den och klicka på namnet för att få åtkomst till uppgiften. Mer information om hur du söker efter objekt i Workfront finns i [Sök i Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Klicka på **Åtgärder** i den vänstra panelen.
1. Klicka på namnet på en uppgift som du vill visa.
1. Klicka på **Aktivitetsinformation**.
1. (Valfritt) Klicka på ikonen **Komprimera alla** längst upp till höger på sidan Uppgiftsinformation.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör eller gruppadministratör konfigurerar vår layoutmall kan fälten i avsnittet Uppgiftsinformation ordnas om eller inte visas. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klicka på **Ekonomi** om du vill expandera och visa den ekonomiska informationen för aktiviteten.

   Klicka på ikonen **Redigera** ![](assets/edit-icon.png) i det övre högra hörnet av informationsavsnittet och klicka sedan på **Ekonomi**.

1. Redigera alla fält som är tillgängliga för redigering genom att klicka en gång på fältet eller klicka på **+Lägg till** för att lägga till information i ett tomt fält.
1. Granska eller redigera följande information i området **Ekonomi** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostnadstyp</td> 
      <td> <p>Ange uppgiftens kostnadstyp. Detta avgör hur kostnaden för uppgiften beräknas, baserat på antalet timmar för uppgifterna. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
        <li> <p>Ingen kostnad</p> </li> 
        <li> <p>Fast en timme </p> </li> 
        <li> <p> Användare per timme </p> </li> 
        <li> <p> Roll timvis</p> </li> 
       </ul> <p>Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a> . Workfront-administratören eller en gruppadministratör väljer standardinställningen för kostnadstyp för uppgifterna i ditt system eller din grupp. Mer information om hur du anger standardinställningar för projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intäktstyp</td> 
      <td> <p>Ange uppgiftens intäktstyp. Det här avgör hur Intäkten för uppgiften beräknas, baserat på antalet timmar för uppgifterna. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
        <li> <p> Ej fakturerbar </p> </li> 
        <li> <p>Användare per timme </p> </li> 
        <li> <p>Roll timvis </p> </li> 
        <li> <p>Fast en timme </p> </li> 
        <li> <p>Användartimme med versaler </p> </li> 
        <li> <p>Roll timvis med ändpunkt </p> </li> 
        <li> <p>Användarens timma plus fast </p> </li> 
        <li> <p>Roll timvis plus fast </p> </li> 
        <li> <p>Fast intäkt </p> </li> 
       </ul> <p>Mer information om att spåra intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a> . </p> <p>Din Workfront-administratör eller gruppadministratör väljer standardinställningen för Intäktstyp för uppgifterna i ditt system eller din grupp. Mer information om hur du anger standardinställningar för projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerad kostnad</td> 
      <td> <p>Detta är en beräkning som visar kostnaden för aktiviteten baserat på planerade timmar, kostnadstyp och timpriset för användare eller jobbroller. Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktisk kostnad</td> 
      <td> <p> Detta är en beräkning som visar kostnaden för uppgiften baserat på faktiska timmar, kostnadstyp och timpriset för användare eller jobbroller. Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerad intäkt</td> 
      <td> <p>Det här är en beräkning som visar de intäkter som är associerade med aktiviteten baserat på de planerade timmarna, intäktstypen och timpriset för användare eller jobbroller. Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktisk intäkt</td> 
      <td> <p>Detta är en beräkning som visar de intäkter som är associerade med uppgiften baserat på de faktiska timmarna, intäktstypen och timpriset för användare eller jobbroller. Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI/SPI/CSI</strong> </td> 
      <td> <p>Det här är aktivitetsprestandamätningar som visar hur din uppgift fungerar vid en given tidpunkt. Deras värden beräknas utifrån projektets prestandaindexmetod.<br>Mer information finns i följande artiklar:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Beräkna index för kostnadsprestanda (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Beräkna SPI (Schedule Performance Index) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Beräkna prestanda för kostnadsschema (CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppskattning vid slutförande</td> 
      <td> <p>Det här är en beräkning som visar den totala kostnaden för uppgiften när den är slutförd. Mer information om beräkning vid slutförande finns i <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Beräkna beräkning vid slutförande (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du redigerar fälten i avsnittet Ekonomi klickar du på **Spara***Ändringar**.

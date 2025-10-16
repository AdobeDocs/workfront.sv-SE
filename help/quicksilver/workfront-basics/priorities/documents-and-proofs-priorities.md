---
navigation-topic: get-started-with-workfront
title: Ladda upp dokument och skapa korrektur i prioriteter
description: Dokument
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 63aa5e45-e51d-4049-a5d9-18dfaaa79647
source-git-commit: 985f1aa11ad1d5efc8d043907d60ad5f5c1bba13
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Ladda upp dokument och skapa korrektur i prioriteter

Du kan överföra dokument och skapa korrektur i prioriteter.

Prioriteter visar arbetsuppgifter som tilldelats dig. Du kan inte se arbetsobjekt som tilldelats ditt team.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> 
   <p>Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller senare för att ladda upp dokument; Standard för att skapa korrektur</p>
   <p>Begär eller högre för att ladda upp dokument; Arbeta eller högre för att skapa korrektur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överföra ett dokument till en arbetsuppgift

Du kan överföra ett dokument till en arbetsuppgift från sidan med arbetslistan eller Information om arbetsuppgift.

### Sammanfattningspanel för Worklist


{{step1-to-priorities}}

1. Håll markören över arbetsnamnet i arbetslistan och klicka sedan på ikonen **Sammanfattning** ![öppna sammanfattningsikonen](assets/summary-icon.png).
1. Kontrollera att du är på fliken **Aktivitet** eller **Problem** på sammanfattningspanelen.
1. Klicka på ikonen **Överför fil** ![Överför fil ](assets/upload-file-icon.png) .
1. Dra och släpp filen eller Cmd/Ctrl + V för att klistra in från Urklipp
eller
Klicka på **Lägg till filer** om du vill bläddra bland filer eller importera filer från en Document Cloud-leverantör.
   ![Lägg till filer](assets/add-files.png)
1. (Valfritt) Lägg till en kommentar.
1. (Valfritt) Lägg till fler filer.

   >[!NOTE]
   >
   >Ytterligare filer överförs som separata dokument.
1. Klicka på **Överför**.

### Information om arbetsuppgift

{{step1-to-priorities}}

1. Klicka på arbetsobjektets namn i arbetslistan.
1. Klicka på fliken **Dokument** högst upp på skärmen.
1. Klicka på **Överför dokument** i det övre högra hörnet och välj sedan **Dokument**.
1. Dra och släpp filen eller Cmd/Ctrl + V för att klistra in från Urklipp
eller
Klicka på **Lägg till filer** om du vill bläddra bland filer eller importera filer från en Document Cloud-leverantör.
   ![Lägg till filer](assets/add-files.png)
1. (Valfritt) Lägg till en kommentar.
1. (Valfritt) Lägg till fler filer.

   >[!NOTE]
   >
   >Ytterligare filer överförs som separata dokument.
1. Klicka på **Överför**.


## Skapa ett enkelt eller avancerat korrektur

Du kan skapa ett korrektur av ett dokument från arbetslistan eller på sidan Information om arbetsobjekt.

### Sammanfattningspanel för Worklist


{{step1-to-priorities}}

1. Håll markören över arbetsnamnet i arbetslistan och klicka sedan på ikonen **Sammanfattning** ![öppna sammanfattningsikonen](assets/summary-icon.png).
1. Kontrollera att du är på fliken **Aktivitet** eller **Problem** på sammanfattningspanelen.
1. Klicka på ikonen **Dokument** ![Dokument](assets/show-document-icon.png) i den högra listen.
1. Klicka på ikonen **Överför fil** ![Överför fil](assets/upload-file-icon.png) och välj sedan filen.

   >[!NOTE]
   >
   >Du måste överföra dokumentet innan du kan skapa korrekturet.


1. När filen har överförts markerar du den i avsnittet **Dokument**.
1. Klicka på **Skapa korrektur** i det övre högra hörnet av rutan Filinformation.
1. Välj något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>Enkelt korrektur</b></td> 
      <td>Med det här alternativet skapas ett korrektur utan ett kopplat arbetsflöde och standardinställningarna för korrektur används. Du kan uppdatera standardkorrekturinställningarna eller lägga till ett arbetsflöde när du har skapat korrekturet. Mer information om korrekturinställningar finns i <a href="/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Redigera korrekturinställningar</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Avancerat korrektur</b></td> 
      <td> <p>Med det här alternativet kan du konfigurera ett grundläggande eller avancerat arbetsflöde och ändra korrekturinställningarna för det korrektur du skapar. Mer information finns i </p> 
       <ul> 
        <li><p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Skapa ett avancerat korrektur med ett grundläggande arbetsflöde</a> </p> </li> 
        <li> <p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Skapa ett avancerat korrektur med ett automatiserat arbetsflöde</a></p></li> 
       </ul>
        </td> 
     </tr> 
    </tbody> 
   </table>

### Information om arbetsuppgift

{{step1-to-priorities}}

1. Klicka på arbetsobjektets namn i arbetslistan.
1. Klicka på fliken **Dokument** högst upp på skärmen.
1. Klicka på **Överför dokument** i det övre högra hörnet och välj sedan **Korrektur**.
1. Skapa ett korrektur enligt beskrivningen i
   [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

<!--

## Open a proof



## Edit a document

Edit name

Add description

manage

Add new version, open proof, edit, download, move, share, remove
-->

## Filter och sortering

Du kan ordna dokumentet med hjälp av filter och sorteringsalternativ.

### Filter

Du kan filtrera dokument efter

* Tillagd av
* Filtyp

### Sortera

Du kan sortera dokument efter

* Datum tillagt
* Filtyp

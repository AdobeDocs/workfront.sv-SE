---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Översikt över korrektur och status
description: Du kan visa information om hur ett korrektur fortskrider genom granskningsprocessen och se en övergripande sammanfattning av bevisets beslutsstatus i området Dokument.
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Översikt över korrektur och status

Du kan visa information om hur ett korrektur fortskrider genom granskningsprocessen och se en övergripande sammanfattning av bevisets beslutsstatus i området Dokument.

## Översikt över korrekturstatus

Förloppet för korrektur anger det arbete som utförts med ett korrektur från det att du skickar beviset till mottagarna till den tidpunkt då de fattar ett beslut om beviset. Förloppsikonerna, S, O, C och D, visas bredvid korrekturnamnet och ger information om korrekturets förlopp.

![](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Förloppsikon</strong> </p> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>Skickat</strong> </p> </td> 
   <td> <p>Beviset har skickats till tilldelade mottagare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Öppnad</strong> </p> </td> 
   <td> <p>Alla tilldelade mottagare öppnar sidan med korrektur- eller korrekturinformation.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Kommentarer gjorda</strong> </p> </td> 
   <td> <p>Alla tilldelade mottagare gör minst en kommentar på korrekturet.</p> <p>Om det inte finns någon granskare tilldelad korrekturet visas <strong>C</strong> visas inte i förloppsindikatorn.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>Beslut</strong> </p> </td> 
   <td> <p>Alla tilldelade godkännare fattar ett beslut om beviset. Alla tilldelade godkännare fattar ett beslut om beviset, såvida inte den som skapat beviset bara anger ett beslut.</p> <p>Om inga godkännare (beslutsfattare) har utsetts för bevisupptagningen ska <strong>D</strong> visas inte i förloppsindikatorn. </p> </td> 
  </tr> 
 </tbody> 
</table>

Förloppsikonerna kan visas i följande färger för att visa viss information om korrekturets förlopp:

* **Grön**: Slutförd.
* **Vit**: Inte fullständigt.
* **Orange**: Inte fullständigt och deadline är mindre än 24 timmar.
* **Röd**: Inte komplett och förbi deadline.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## Översikt över korrekturstatus

Korrekturstatusen visar statusen för de beslut som krävs för beviset. Bevisets status styrs av deltagaren i det värsta fallet. Anta till exempel att det finns tre beslut om beviset: två har statusen **Accepterad** och en har statusen **Avvisad**. Det värsta fallet **Avvisad** överstyr de andra besluten och bevisets övergripande status visas som **Avvisad**. 

![](assets/proof-edit-existing-progress-350x62.png)

Standardstatusalternativen är följande:

* Väntande
* Godkänd
* Godkänd med ändringar
* Ändringar krävs
* Inte relevant

Om anpassade beslut har konfigurerats i ditt konto återspeglar statusalternativen dina anpassade beslutsinställningar.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->

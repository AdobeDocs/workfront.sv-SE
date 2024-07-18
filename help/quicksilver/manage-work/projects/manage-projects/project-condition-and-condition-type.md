---
title: Översikt över projektvillkor och villkorstyp
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Projektvillkoret är en visuell representation av hur projektet fortskrider. Det är en variabel som kan rapporteras och som bestäms av förhållandet mellan projektets planerade, planerade och beräknade datum.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Översikt över projektvillkor och villkorstyp

<!-- Audited: 12/2023 -->

Projektvillkoret är en visuell representation av hur projektet fortskrider. Det är en variabel som kan rapporteras och som bestäms av förhållandet mellan projektets planerade, planerade och beräknade datum.

## Översikt över projektvillkor

Tänk på följande när du är insatt i ett projekts villkor:

* Som projektägare kan du bestämma om villkoret för ett projekt ska anges manuellt eller automatiskt. Ett projekts villkor kan anges på följande sätt:

   * Manuellt av användare som har åtkomst till Hantera projektet och när villkorstypen för projektet är inställd på Manuell.
   * Automatiskt av Adobe Workfront när villkorstypen för projektet är inställd på Status. Projektets förloppsstatus bestäms av förloppet för aktiviteterna i projektet. Mer information om projektets förloppsstatus finns i [Översikt över projektets förloppsstatus](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Mer information om hur du uppdaterar villkorstypen för projektet finns i [Ange villkorstypen för ett projekt](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* När du tillåter att Workfront automatiskt beräknar projektvillkoren rekommenderar vi att du använder föregående aktiviteter för dina uppgifter så att aktivitetens förlopp återspeglar projektets aktuella förlopp och förloppsstatus.
* Som projektägare kan du ändra projektet till att använda en manuell villkorstyp i stället för att använda förloppsstatusen genom att ändra villkorstypen från förloppsstatus till Manuell.

  >[!NOTE]
  >
  >Projekt som har någon av följande statusvärden markeras alltid som På mål, oavsett datum för aktiviteterna och förloppet:
  >
  >* Idea
  >* Begärd
  >* Godkänd
  >* Avvisad

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Så här uppdaterar Workfront projektvillkor baserat på förloppsstatus

När villkorstypen för projektet är inställd på Manuell kan du bestämma vilket villkor för projektet som är oberoende av projektets förloppsstatus.

Vi rekommenderar dock att du ställer in villkorstypen för projektet på Status så att du tydligt kan se vilket förlopp projektet har, baserat på förloppet för dina uppgifter. Information om hur Workfront beräknar förloppsstatus för projekt finns i [Översikt över projektförloppsstatus](../../../manage-work/projects/planning-a-project/project-progress-status.md).

I det här fallet kan värdena för Projektvillkor vara:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Projektvillkor</strong></td> 
   <td><strong>Status för projektförlopp</strong></td> 
   <td><strong>Workfront villkorsindikator</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>På mål</td> 
   <td>När statusen för projektet är I tid är villkoret för projektet <strong>På mål</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td>När projektets förloppsstatus är <strong>Bakom</strong> eller <strong>Vid risk</strong> är villkoret för projektet <strong>Vid risk</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>I problem</td> 
   <td>När projektets förloppsstatus är <strong>SENT</strong> är projektets villkor <strong>I problem</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Villkoren kan anpassas efter din miljö, så du kan hitta fler än tre alternativ för Villkor i din miljö. Namnen på villkoren kan skilja sig från namnen ovan. Mer information om hur du anpassar villkor i finns i artikeln [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Rapport om projektvillkor, uppdatering av projektvillkor och sista villkorsanteckning

I vyn för en projektrapport kan du visa följande fält som är relaterade till projektets villkor:

* **Projektvillkor:** Visar projektets aktuella villkor.
* **Projektvillkorsuppdatering**: Visar den senaste uppdateringen som projektägaren har tillhandahållit i projektets uppdateringsström, tillsammans med det nya villkoret.\
  Kommentarer som gjorts för villkorsuppdateringar visas inte i kolumnen **Villkorsuppdatering**. Endast huvuduppdateringen visas.

* **Senaste villkorsanteckning**: Visar den uppdatering som objektets ägare senast angav för ett objekt. Det här fältet är användbart för att visa ägarens senaste aktivitet eller interaktion för ett objekt.\
  Kolumnen **Sista villkorsanteckning** är tom om anteckningstexten för den sista anteckningen i ett objekt har tagits bort. När en ny anteckning läggs in på objektet blir den sista anteckningen och visas igen i kolumnen.

Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

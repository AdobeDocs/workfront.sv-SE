---
title: Avpublicera ett begärandeformulär i Adobe Workfront Planning
description: Du kan avpublicera ett begärandeformulär om det inte längre behövs eller är relevant. Genom att avpublicera tar du bort allas behörigheter för att komma åt formuläret.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Avpublicera ett begärandeformulär i Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan avpublicera ett begärandeformulär om det inte längre behövs eller är relevant. Genom att avpublicera tar du bort allas behörigheter för att komma åt formuläret.

Du kan också ändra de enheter som du delar ett begärandeformulär med, om du vill att det ska vara tillgängligt för en mindre grupp personer.

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
<tr>
<td>
   <p> Produkter</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td>
   <td>
<p>Något av följande Workfront-planer:</p>
<ul><li>Välj</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td>
   <td>
<p>Alla </p>  
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <ul>
   <li><p>Hantera behörigheter till en arbetsyta</p></li>
    <li><p>Systemadministratörer kan hantera arbetsytor som de inte skapade. </p></li>
    </ul>
   <p>Information om delningsbehörigheter för Workfront Planning-objekt finns i  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändra delning av ett begärandeformulär

Om du delar en begäran för allmänheten med alla, inklusive användare utanför organisationen, kan du överväga att begränsa åtkomsten till vissa användare som antingen visar eller hanterar arbetsytan som formuläret är kopplat till.

Så här ändrar du delningen av ett begärandeformulär:

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn i sidhuvudet och klicka sedan på **Uppdatera begärandeformuläret**.
1. Klicka på **Dela** i skärmens övre högra hörn och uppdatera delningsalternativen. Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Valfritt) Klicka på **Kopiera länk** om du har ändrat delningen av begärandeformuläret och vill dela det med den nya gruppen med personer med en ny länk.

## Avpublicera ett begärandeformulär för en posttyp

När ett begärandeformulär blir irrelevant och du inte längre vill att någon ska få åtkomst till det, kan du avpublicera det.

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn i sidhuvudet och klicka sedan på **Uppdatera begärandeformuläret**.
1. Klicka på **Avpublicera** i det övre högra hörnet.

   ![](assets/unpublish-button-highlighted.png)

   En bekräftelse visas längst ned på skärmen som meddelar att formuläret har avpublicerats.

   Knappen **Avpublicera** ändras till **Publish**.

1. Klicka på **Spara**.

   Det går inte längre att komma åt formuläret från länken <!--or from the request queue in the Requests area of Workfront-->.

   Alla poster som tidigare lagts till med hjälp av frågeformuläret finns kvar på posttypssidan.

   Alla tidigare tillagda begäranden finns kvar i området Begäranden i Workfront på fliken Planering.

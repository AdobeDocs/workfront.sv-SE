---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: 2019.4 andra förbättringar
description: Den här sidan beskriver olika förbättringar som gjorts i version 2019.4. Den kommer att göras tillgänglig i produktionsmiljön den 11 november 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: e1bf5fbc7dc25bf8ce472b21b9a0906530f82cf0
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# 2019.4 andra förbättringar

Den här sidan beskriver olika förbättringar som gjorts i version 2019.4. Den kommer att göras tillgänglig i produktionsmiljön den 11 november 2019.

En lista över alla ändringar som gjorts under 2019.4 finns på [Översikt över version 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Starta ett automatiskt korrekturarbetsflöde från ett Adobe CC-dokument</strong> <p>Utan att lämna Adobe CC kan du starta ett automatiskt korrekturarbetsflöde för ett Adobe CC-dokument som du har skapat. Mer information finns i avsnittet <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Generera ett korrektur från Illustrator eller InDesign</a> i artikeln <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Använda Workfront-tillägget för Illustrator och InDesign</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Förhindra dubblerade e-postadresser</strong> <p>Du kan inte längre använda samma e-postadress när du skapar flera användare i Workfront, även om e-postadresserna varierar beroende på fall. Du kan till exempel inte skapa en användare med e-postadressen JohnDoe@example.com och en annan användare med e-postadressen johndoe@example.com. </p> <p>Före den här ändringen stöddes skapande av användare med matchande e-postadresser som endast skiljer sig åt från fall till fall. </p> <p>Obs! Befintliga användare med matchande e-postadresser som bara skiljer sig åt från fall till fall måste uppdateras vid ett framtida datum. Om du har användare i en Workfront-instans med matchande e-postadresser som bara skiljer sig åt från fall till fall, kommer Workfront att kontakta dig med ytterligare information och en tidslinje när dessa behöver uppdateras.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Ytterligare objekttyper är tillgängliga för Typeahead-fält i ett anpassat formulär</strong> 
     <p>När du nu skapar ett anpassat fält av typen Typeahead kan du koppla följande objekttyper till fältet: Användare, Företag, Grupp, Jobbroll, Portfolio, Program, Projekt och Mall.</p> 
     <p>Tidigare kunde du bara koppla objekttypen User till ett anpassat typsnittsfält.</p> 
     <p>Mer information finns i avsnittet <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Skapa eller redigera ett anpassat formulär</a> i artikeln <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Skapa eller redigera ett anpassat formulär</a>.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Filnamn på den senaste versionen av ett dokument som visas</strong> <p>När du överför en dokumentversion med ett annat filnamn än den befintliga versionen visas nu det nya filnamnet i Workfront.</p> <p>När du tidigare lade till en ny version med ett annat filnamn fortsatte filnamnet för den tidigare versionen att visas i Workfront.</p> <p>Mer information finns i <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Överföra en ny version av ett dokument</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Lägga till ett filter i ett Typhead-fält i ett anpassat formulär</strong> <p>När du lägger till ett texthuvudsfält i ett anpassat formulär kan du nu lägga till ett filter som begränsar vilka objekt som är tillgängliga när någon använder fältet. Du kan till exempel begränsa fältet så att användaren bara kan välja medlemmar i marknadsförings- och säljteamen i organisationen.</p> <p>Mer information finns i avsnittet Skapa och lägga till ett nytt fält i artikeln Skapa anpassad Forms.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Ändra visningstypen för ett fält i ett anpassat formulär</strong> 
     <p>Nu kan du ändra visningstypen för ett fält i ett anpassat formulär.</p> 
     <p>Om du t.ex. har skapat ett kryssrutefält kan du ändra det till ett nedrullningsbart fält eller ett alternativknappsfält. Dessa tre fälttyper är utbytbara.</p> 
     <p>Om du har skapat ett textfält med en rad kan du ändra det till ett textfält med en rad. Dessa två fälttyper är utbytbara.</p> 
     <p>Tidigare var du tvungen att skapa ett nytt fält och ta bort det gamla för att ändra visningstypen för ett anpassat fält. Detta krävde överföring av data, som ofta var tidskrävande.</p> 
     <p>Mer information finns i <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Skapa eller redigera ett anpassat formulär</a> i artikeln <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Skapa eller redigera ett anpassat formulär</a></p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Skapa tid för kalendrar och rapporter</strong> 
     <p>Nu kan du se användarens ledig tid för bättre planering och körning. Du kan också lägga till ny tid med rapporter och kalendrar på kontrollpanelerna för att få en realtidsbild av användarnas tillgänglighet.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

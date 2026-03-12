---
product-area: documents
navigation-topic: approvals
title: Överför en ny dokumentversion och begär godkännande
description: Du kan överföra en ny dokumentversion och begära godkännande från andra användare i Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 0%

---

# Överför en ny dokumentversion och begär godkännande

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Om ett dokument är markerat som&quot;Behöver arbete&quot; i en tidigare granskning kan du överföra en ny version till originaldokumentet och starta en ny godkännandeomgång. När du har överfört en ny version av dokumentet är de tidigare versionerna låsta.

Om den nya versionens filnamn skiljer sig från den tidigare versionens filnamn visas dokumentet med det nya filnamnet i Workfront.

När en ny version läggs till i ett dokument med enastående godkännanden visas godkännandet för den föregående versionen som&quot;Återkallad&quot;. Den föregående godkännandeprocessen avslutas, även om vissa deltagare ännu inte har fattat något beslut.

Om den senaste dokumentversionen tas bort förblir de tidigare versionerna låsta. Om du behöver redigera en tidigare version måste du låsa upp den manuellt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser</td> 
   <td> <p>Begäran eller senare</p>
   <p>Medarbetare eller högre</p>
   <p>Om du använder Frame.io-integreringen måste du ha en standardlicens för att skapa arbetsflöden för godkännande.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till objektet som är associerat med dokumentet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Använd dra-och-släpp för att lägga till en ny version i produktionsmiljön

>[!NOTE]
>
>Det går inte att dra och släppa i Internet Explorer.


Om du behöver en ny granskningsrunda och ett godkännande av ett dokument kan du skapa en ny dokumentversion i Workfront.

Du kan lägga till föregående deltagare, nya deltagare eller en blandning av båda. Du kan visa information om tidigare versioner och deltagare på sidan Dokumentinformation.

Lägga till en ny version:

1. Navigera till dokumentet i Workfront.
1. Dra och släpp den nya filen ovanpå det föregående dokumentet. En ny version skapas automatiskt.

1. När dokumentet har överförts markerar du dokumentet och klickar sedan på **Dokumentinformation**.
   ![Öppna dokumentinformationssidan](assets/open-doc-details.png)


1. Klicka på **Godkännanden** i den vänstra panelen och klicka sedan på **Lägg till**.

1. Om du vill lägga till alla tidigare deltagare klickar du på **Lägg till alla**. Du kan också lägga till nya deltagare eller ta bort tidigare deltagare efter behov.


1. Om du vill lägga till en befintlig godkännandemall klickar du på knappen Mall och börjar skriva in ett mallnamn.

   >[!TIP]
   >
   >   Användare med en standardlicens kan skapa återanvändbara godkännandemallar under Konfigurera. Mer information finns i [Skapa en arbetsflödesmall för godkännande för dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Valfritt) Ange en tidsgräns för godkännandet. Användare och team meddelas via e-post 72 timmar, sedan 24 timmar före den angivna tidsgränsen.

1. När du har lagt till alla granskare och godkännare klickar du på **Skicka begäran**. Deltagare meddelas via e-post.

   ![skicka ny version för godkännande](assets/add-previous-participants.png)





<div class="preview">

## Använd dra-och-släpp för att lägga till en ny version i förhandsvisningsmiljön i det äldre dokumentområdet

Om ditt företag använder Workfront-lagring visas det äldre dokumentområdet när du öppnar dokument i Workfront. Mer information om Workfront-lagring finns i [Workfront-lagring jämfört med Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

>[!NOTE]
>
>Det går inte att dra och släppa i Internet Explorer.


Om du behöver en ny granskningsrunda och ett godkännande av ett dokument kan du skapa en ny dokumentversion i Workfront.

Du kan lägga till föregående deltagare, nya deltagare eller en blandning av båda. Du kan visa information om tidigare versioner och deltagare på sidan Dokumentinformation.

Lägga till en ny version:

1. Navigera till dokumentet i Workfront.
1. Dra och släpp den nya filen ovanpå det föregående dokumentet. En ny version skapas automatiskt.

1. När dokumentet har överförts markerar du dokumentet för att öppna panelen Dokumentsammanfattning. Här visas versionsnumret längst upp på panelen.
   ![Öppna dokumentinformationssidan](assets/open-doc-details.png)


1. Bläddra ned till avsnittet **Godkännanden**.

1. Klicka på **Skapa arbetsflöde** och fyll sedan i följande information:

   <table>
   <tr>
   <td><strong>Scennamn</strong></td>
   <td>Lägg till ett scennamn. Du kan ändra namnet till något mer beskrivande, till exempel <em>Inledande granskning</em> eller <em>Slutligt godkännande</em>.</td>
   </tr>
   <tr>
   <td><strong>Lägg till namn eller e-post</strong></td>
   <td>Börja skriva ett användar- eller teamnamn som ska läggas till som godkännare eller granskare. Om du bara har granskare meddelas de och har möjlighet att slutföra granskningen, men inget beslut krävs eller fattas.</td>
   </tr>
   <tr>
   <td><strong>Ett beslut krävs (valfritt)</strong></td>
   <td>Den första personen som fattar ett beslut slutför steget.</td>
   </tr>
   <tr>
   <td><strong>Förfallodatum (valfritt)</strong></td>
   <td>Ange ett förfallodatum för godkännandet. Användare och team meddelas via e-post 72 timmar och sedan 24 timmar före det angivna förfallodatumet.</td>
   </tr>
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till ytterligare steg.

   >[!NOTE]
   >
   >Om du lägger till flera faser fortsätter arbetsflödet för godkännande i den ordning som faserna listas. När alla nödvändiga beslut fattas börjar nästa steg och den föregående fasen låses.



1. (Valfritt) Om du vill lägga till en befintlig godkännandemall väljer du en mall till vänster i dialogrutan.

   >[!TIP]
   >
   >   Användare med en standardlicens kan skapa återanvändbara godkännandemallar under Konfigurera. Mer information finns i [Skapa en arbetsflödesmall för godkännande för dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. När du har lagt till alla faser och deltagare som du behöver klickar du på **Begär godkännande**.

   Godkännandearbetsflödet startar och godkännarna får ett meddelande om att deras godkännande krävs för den nya dokumentversionen. Den tidigare dokumentversionen är låst och alla utestående godkännanden i den tidigare versionen tas bort.

   ![begär godkännande](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->



</div>


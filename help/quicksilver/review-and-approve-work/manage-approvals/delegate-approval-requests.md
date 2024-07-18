---
product-area: projects
navigation-topic: approvals
title: Delegera godkännandebegäran
description: Genom att delegera godkännandebegäranden kan du tilldela en annan användare behörighet att godkänna dina begäranden under en tidsperiod, till exempel om du inte kommer att vara på semester.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 0%

---

# Delegera godkännandebegäran

Du kan tillfälligt delegera det arbete du är tilldelad när du inte är på kontoret. Du kan delegera uppgifter och utleveranser eller delegera godkännandebegäranden. I den här artikeln beskrivs hur du delegerar godkännandebegäranden. Mer information om delegering av uppgifter och ärenden finns i [Hantera uppgifter och utfärda delegering](../../manage-work/delegate-work/how-to-delegate-work.md).

Du kan delegera följande typer av godkännanden, oavsett hur du tilldelades godkännandet (oavsett om det tilldelats direkt till dig, till ett team som du är medlem i eller till din jobbroll):

* Projektgodkännanden
* Uppgiftsgodkännanden
* Utfärda godkännanden

Du kan inte delegera tidrapport-, dokument- eller korrekturgodkännanden.

>[!NOTE]
>
>För att säkerställa att inga inkonsekvenser inträffar med de datum som du schemalägger för dina godkännanden som ska delegeras, rekommenderar vi att användarprofilens tidszon matchar tidszonen i ditt schema. Mer information finns i följande artiklar:
>
>* [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

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
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan eller licenstyp du har.

+++

## Förstå användaråtkomst för delegerade godkännanden

Under den angivna godkännandeperioden har användaren som du delegerar en godkännandebegäran följande funktioner:

* Kan godkänna eller avvisa befintliga godkännandebegäranden när inget beslut har fattats
* Kan godkänna och avvisa nya godkännandebegäranden som tas emot under en angiven tidsperiod
* Har beviljats Visa-åtkomst till objekt som väntar på godkännande

  >[!NOTE]
  >
  > Adobe Workfront-administratören kan hindra användare från att komma åt vissa objekttyper. När en användare inte har åtkomst till en objekttyp och ett godkännande av den typen delegeras till användaren, har användaren inte åtkomst till objektet via Visa. Användaren kan dock fortfarande godkänna eller avvisa begäranden om godkännande från sidan **Hem**, enligt beskrivningen i [Godkänna arbete](../../review-and-approve-work/manage-approvals/approving-work.md).\
  >Användare A tillhör till exempel grupp A. Workfront-administratören har begränsat åtkomsträttigheterna för grupp A så att användare i den här gruppen inte kan visa uppgifter i Workfront. Om en begäran om aktivitetsgodkännande delegeras till Användare A kan Användare A inte visa den uppgift som godkännandet är kopplat till. Användare A kan dock godkänna eller avvisa godkännandebegäran från hemsidan.

  Information om hur Workfront-administratören kan begränsa åtkomst till objekttyper i installationsprogrammet finns i  [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

När delegeringen av godkännande har stoppats eller avbrutits har användaren utsetts till godkännare:

* Har inte längre åtkomst till att godkänna arbete för artiklar som kräver godkännande
* Fortsätter ha Visa-åtkomst till arbetsobjekt\
  Användare som har beviljats Visa åtkomst till objekt via en godkännandedelegering behåller den visningsåtkomsten även när godkännandedelegeringen stoppats eller återkallats. Om du vill ta bort Visa-åtkomst till objekt som användaren hade åtkomst till under tiden som godkännandena delegerades, måste du gå till objektet och ta bort åtkomsträttigheter direkt från objektet.

## Delegera godkännandebegäranden i hemområdet

Du kan delegera godkännandebegäranden från Hem-området.

### Delegera dina godkännanden till en annan användare {#delegate-your-approvals-to-another-user}

Du kan delegera följande typer av godkännanden, oavsett hur du tilldelades godkännandet (oavsett om det tilldelats direkt till dig, till ett team som du är medlem i eller till din jobbroll):

* Projektgodkännanden
* Uppgiftsgodkännanden
* Utfärda godkännanden

Du kan inte delegera tidrapport-, dokument- eller korrekturgodkännanden.

Tänk på följande när du delegerar godkännanden:

* När du delegerar godkännanden delegeras alla dina godkännanden. Du kan inte delegera enskilda godkännandebegäranden.
* Du kan delegera godkännanden till endast en användare. Du kan inte delegera godkännanden till flera användare samtidigt.\
  Alla godkännanden för alla projekt, uppgifter och ärenden delegeras till den användare som du utser.
* Högst fem användare kan delegera godkännanden till samma användare samtidigt. En enskild användare kan med andra ord inte utses till tillfällig godkännare för mer än fem användare samtidigt.
* Aktivitet för godkännanden visas på fliken Uppdateringar. Visa systemuppdateringar måste vara aktiverat. Både den användare som delegerar godkännandet och den användare till vilken godkännandena delegeras får ett e-postmeddelande om godkännandeaktiviteten.

Så här delegerar du godkännanden till en annan användare:

1. Klicka på ikonen **Hem** ![](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmenyn** ![](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

   eller

   Klicka på ikonen **Huvudmeny** > **ditt namn** > **Stäng av** i den vänstra panelen.

1. (Valfritt och villkorligt) I området Hem klickar du på listrutan **Filter** och sedan på **Godkännanden**.

1. (Villkorligt) Klicka på **Delegera mina godkännanden**

   eller

   Om din system- eller gruppadministratör har aktiverat aktiviteten och utfärdat delegering klickar du på **Delegera** och sedan på **Delegera godkännanden**.

   ![](assets/delegate-approvals-nwe.png)

1. Ange följande information i avsnittet Delegera mina godkännanden:

   * **Namn**: Börja skriva namnet på den användare som du vill delegera godkännanden till och klicka sedan på namnet när det visas i listrutan.
   * **Startdatum**: Välj det datum då godkännanden ska vidarebefordras. Vidarebefordran börjar kl. 12.00 på det datum du väljer.\
     Startdatumet måste vara det aktuella datumet eller ett framtida datum.
   * **Slutdatum**:Gör något av följande:

      * Välj det datum då godkännanden inte längre ska vidarebefordras. Vidarebefordran upphör kl. 23.59 på det datum du väljer.
      * Välj **Inget slutdatum** om du vill konfigurera Workfront att delegera godkännanden på obestämd tid.

1. Klicka på **Spara**.

### Uppdatera eller stoppa en godkännandedelegering {#update-or-stop-an-approval-delegation}

1. Klicka på ikonen **Hem** ![](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmenyn** ![](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Klicka på listrutan **Filter** och sedan på **Godkännanden**.

1. (Villkor) Klicka på **Redigera delegering**

   eller

   Om aktiviteten och delegeringen har aktiverats av systemadministratören eller gruppadministratören klickar du på **Redigera delegering** och sedan på **Delegera godkännanden**.

1. (Villkorligt) Gör något av följande:

   * Så här uppdaterar du den befintliga godkännandedelegeringen: Ändra den information som visas och klicka sedan på **Spara**.

   * Så här stoppar du den befintliga delegeringen: Klicka på **Stoppa delegering** och sedan på **Stoppa delegering** för att bekräfta.

     ![](assets/stop-delegation-nwe.png)

### Visa delegerade godkännanden {#view-delegated-approvals}

Du kan bara visa följande typer av godkännandedelegeringar i arbetslistan:

* Projektgodkännanden
* Uppgiftsgodkännanden
* Utfärda godkännanden

Så här visar du delegerade godkännanden:

1. Klicka på ikonen **Hem** ![](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmenyn** ![](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Klicka på listrutan **Filter** och sedan på **Godkännanden**.\
   Alla godkännanden visas som standard i listan, inklusive godkännanden som tilldelats dig och godkännanden som delegerats till dig.

   ![](assets/delegated-to-me-nwe-350x93.png)

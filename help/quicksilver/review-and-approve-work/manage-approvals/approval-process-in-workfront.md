---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Översikt över godkännandeprocessen
description: Du kan skapa en godkännandeprocess och bifoga den till ett objekt för att se till att angivna användare granskar vissa ändringar innan objektet bearbetas.
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Översikt över godkännandeprocessen

Du kan skapa en godkännandeprocess och bifoga den till ett objekt för att se till att angivna användare granskar vissa ändringar innan objektet bearbetas.

Detta är tillgängligt för följande typer av objekt i Adobe Workfront:

* Arbetsuppgift (projekt, uppgift eller utgåva, mall, malluppgift)
* Dokument
* Korrektur

Instruktioner om hur du skapar en godkännandeprocess finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Den här artikeln innehåller allmän information om godkännandeprocesser som är kopplade till arbetsobjekt.

## Typ av godkännandeprocesser

Om du är Adobe Workfront-administratör, eller en användare med administrativ åtkomst till godkännandeprocesser, kan du skapa följande godkännandeprocesser för projekt, uppgifter och ärenden:

* **En global godkännandeprocess på systemnivå**: Användare kan bifoga dessa till något av följande:

   * Ett projekt, en uppgift eller en utgåva i avsnittet Godkännanden
   * I rutan Redigera projekt visas området Standardprocess för godkännande av uppgift
   * Under Standardgodkännandeprocess i avsnittet Köinformation eller Köämne i ett projekt. Projektet måste aktiveras som en begärandekö.

* **En global godkännandeprocess på gruppnivå**: Användarna kan bifoga dessa till följande:

   * Ett projekt, en uppgift eller en utgåva som tillhör gruppen som är associerad med godkännandeprocessen i avsnittet Godkännanden
   * I rutan Redigera projekt, området Standardprocess för godkännande av uppgift för ett projekt som tillhör gruppen som är associerad med godkännandeprocessen
   * Under Standardgodkännandeprocess i avsnittet Köinformation eller Köämne i ett projekt. Projektet måste aktiveras som en begärandekö och måste tillhöra gruppen som är associerad med godkännandeprocessen.

   Mer information om hur du skapar godkännandeprocesser på system- eller gruppnivå finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **En godkännandeprocess för enstaka användning**: För användning med ett enda projekt, en uppgift, en utgåva, en mall eller en malluppgift. Den här typen av godkännandeprocess påverkar bara det objekt som är associerat med det och som inte är tillgängligt för att kopplas till några andra objekt.

   Mer information om hur du skapar en godkännandeprocess för enstaka användning finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>I den här artikeln används termen&quot;global godkännandeprocess&quot; för att skilja sig från&quot;godkännandeprocess för enstaka användning&quot;. En global godkännandeprocess kan användas upprepade gånger.
>
>Termen global godkännandeprocess på gruppnivå avser en godkännandeprocess som kan användas upprepade gånger för artiklar och med statusvärden som bara är kopplade till en viss grupp.

Mer information om hur du skapar en godkännandeprocess på systemnivå eller en godkännandeprocess på gruppnivå finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Överväganden om godkännandeprocesser

* Du måste skapa projektet, uppgiften, utgåvan, mallen eller malluppgiften innan godkännandeprocessen kan kopplas till dem.
* En godkännandeprocess är alltid kopplad till två viktiga saker:

   * Varje godkännandeprocess motsvarar en viss arbetsartikelstatus i Workfront-systemet. När du ändrar status för en arbetsuppgift, kräver ett bifogat godkännande för den statusen att statusändringen ska bekräftas innan den nya statusen kan tilldelas artikeln.

      >[!TIP]
      >
      >
      >   
      >   
      >   * Du kan koppla ett godkännande på gruppnivå till en global status eller en gruppnivåstatus.
      >   * Du kan inte ändra status för en artikel med en godkännandeprocess till en annan status än den som är associerad med godkännandeprocessen.

         >   
         >   
         >     Om du till exempel har ett uppgiftsgodkännande som är associerat med statusen Pågår, ändrar aktiviteten automatiskt status till Pågår när godkännandet beviljas. Det kan inte automatiskt ändra sin status till Slutförd eller någon annan status som inte är associerad med godkännandet.


   * Enheterna som är kopplade till en godkännandeprocess kan vara användare, jobbroller eller team. Användarna ansvarar själva för att godkänna eller avvisa godkännandet. Du kan tilldela godkännanden till användare som fyller i en viss roll i projektet. Du kan till exempel tilldela ett godkännande till en projektägare eller Sponsorn. Mer information finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      Följande scenarier finns:

      * När du tilldelar ett godkännande till jobbroller kan alla användare i projektgruppen som är associerade med jobbrollen fatta ett beslut om godkännandet. Rollen som är associerad med godkännandet kan vara deras primära roll eller andra roller.

         Mer information om projektteamet finns i [Översikt över projektteamet](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * När du tilldelar ett godkännande till ett team kan alla medlemmar i det teamet fatta ett beslut om godkännandet. Teamet som är associerat med godkännandet kan antingen vara deras hemteam eller något av deras andra team.

         Mer information om en användares roller och team finns i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* När du skapar en arbetsuppgift bifogas ingen godkännandeprocess automatiskt. Du måste bifoga en manuellt om du vill använda en. Mer information om hur du bifogar en godkännandeprocess till ett objekt finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront-administratören eller en användare med administrativ åtkomst till godkännandeprocesser kan skapa globala godkännandeprocesser på systemnivå som kan användas i hela systemet. En gruppadministratör med administrativ åtkomst till godkännandeprocesser kan skapa en global godkännandeprocess på gruppnivå som bara kan användas av en viss grupp som de hanterar.
* Om du inte vill använda en fördefinierad global godkännandeprocess på system- eller gruppnivå för en arbetsuppgift, kan du skapa och bifoga en godkännandeprocess för den när du har behörigheten Hantera för det objekt som du vill bifoga godkännandeprocessen för.

   >[!NOTE]
   Du kan bara använda en godkännandeprocess en gång för det specifika objekt som det skapades för. Du kan associera globala statusvärden och gruppnivåstatusar för engångsgodkännandeprocesser för projekt, uppgifter, utgåvor, mallar och malluppgifter.

* När du kopplar en godkännandeprocess på gruppnivå till ett objekt med anpassade statusvärden på gruppnivå, kan en konflikt skapas mellan godkännandestatusarna för den föregående gruppen och de som finns på systemnivå om du ändrar projektgruppen. Överväg att ta bort godkännandeprocesserna på gruppnivå för projektet eller dess uppgifter eller problem innan gruppen uppdateras. Mer information om hur du skapar godkännandeprocesser på gruppnivå finns i [Godkännandeprocesser på gruppnivå](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Mer information om hur du skapar anpassade gruppstatusar finns i [Skapa eller redigera en gruppstatus](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Mer information om hur du uppdaterar gruppen med ett projekt finns i [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

## Arbetsflödet för godkännandeprocess

I det här avsnittet förklaras följande om hur du godkänner arbetsobjekt:

* [Hur godkännandeprocesser bygger på status](#how-approval-processes-rely-on-statuses)
* [Så här använder ett typiskt arbetsflöde en godkännandeprocess](#how-a-typical-workflow-uses-an-approval-process)

### Hur godkännandeprocesser bygger på status {#how-approval-processes-rely-on-statuses}

Genom att bifoga en status till en godkännandeprocess försäkrar du dig om att artikeln rör sig mellan avdelningarna i rätt ordning.

**Exempel:** Du kan bifoga en godkännandeprocess till statusen för marknadsföringsavdelningen som kräver godkännande av finansavdelningen. När någon sedan ändrar status för en arbetsuppgift till&quot;Marknadsföringsavdelning&quot; kan artikeln inte flyttas till den avdelningen förrän finansavdelningen signerar den.

Mer information om status för arbetsobjekt finns i följande artiklar:

* [Öppna listan över status för systemprojekt](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Åtkomst till listan över status för systemaktivitet](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Åtkomst till listan över status för systemproblem](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Så här använder ett typiskt arbetsflöde en godkännandeprocess {#how-a-typical-workflow-uses-an-approval-process}

Följande scenario visar hur en godkännandeprocess hjälper användare att godkänna arbetet när ett Workfront-objekt går igenom ett arbetsflöde med flera steg i den här ordningen:

1. Workfront-administratören eller en användare med administrativ åtkomst till godkännandeprocesser skapar en godkännandeprocess för ett projekt, en uppgift eller ett problem.

   >[!NOTE]
   Du kan koppla projektgodkännandeprocesser till en mall och uppgiftsgodkännandeprocesser till en malluppgift. När du har gjort det blir godkännandeprocessen ett projekt eller en process för godkännande av en uppgift när någon använder mallen för att skapa ett projekt. En godkännandeprocess som är kopplad till en mall- eller malluppgift är fortfarande en engångsprocess för projekt och uppgifter.

1. En användare med behörigheten Hantera för projektet, uppgiften eller utgåvan kopplar godkännandeprocessen till objektet, eller skapar ett engångsgodkännande för objektet.
1. En användare som är tilldelad arbetsuppgiften ändrar sin status till den status som initierar godkännandeprocessen och godkännandeprocessen börjar. (Den person som skapade godkännandeprocessen definierade relationen mellan statusen och godkännandeprocessen.)
1. De utsedda godkännarna får ett meddelande om den väntande godkännandeprocessen och de granskar arbetsuppgiften.
1. Godkännandeprocessen avslutas när de utsedda godkännarna har godkänt alla steg i processen. Om de avvisar ett steg återställs statusen till en fördefinierad status eller så skapas ett problem. (Den person som skapade godkännandeprocessen definierade vilka av dessa automatiska steg som ska utföras efter ett avvisande.)

**Exempel:** Ett reklamteam har skapat statusen Ready for Printing och en godkännandeprocess som kallas Designer/Copywriter Signoff, som är kopplad till den här statusen. Godkännandeprocessen är konfigurerad till:

* Kräv godkännande av teamets designer och copywriter
* Starta när någon ändrar en arbetsuppgifts status till Klar för utskrift

En ägare av ett broschyrprojekt kopplar godkännandeprocessen för Designer/Copywriter till broschyrprojektet.

När någon i projektet ändrar status till Klart för utskrift får copywriter och designern meddelanden om att de ska godkänna eller avvisa det. Under godkännandeprocessen, när de överväger om de ska godkänna det eller inte, visas statusen för projekten som Klar för utskrift - väntar på godkännande.

När de båda har godkänt broschyren i Workfront ändras projektstatusen till Klar för utskrift.

## Dokumentgodkännandeprocesser

Dokumentgodkännanden används för ett mer allmänt godkännande. Synpunkter hämtas i chattformat på fliken Uppdateringar. Du kan använda godkännandeknapparna för att godkänna, avvisa eller godkänna med ändringar.

Information om hur du lägger till godkännare i ett dokument när det har överförts till Workfront finns i [Begär dokumentgodkännanden](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Bevis på godkännandeprocesser

Bevisgodkännanden används för en djupare granskning och innehåller vanligtvis mer komplicerade arbetsflöden. Feedback spelas in med markeringsverktyg i korrekturläsaren. Du kan använda godkännandeknapparna för att godkänna, avvisa eller godkänna med ändringar.

Information om hur du lägger till ett automatiskt arbetsflöde i ett dokumentkorrektur och anger vissa användare i arbetsflödet som godkännare av korrekturet finns i [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Konfigurera inställningar för arbetsartikelgodkännandeprocesser

Som Workfront-administratör kan du konfigurera globala inställningar för arbetsartikelgodkännandeprocesser i ditt system. De här inställningarna avgör olika regler för godkännandeprocesser, som hur länge ett godkännandebeslut ska vara öppet eller hur du hanterar delegering av godkännande i systemet. Mer information om inställningar för godkännandeprocess finns i [Konfigurera globala inställningar för godkännande](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

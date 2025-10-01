---
product-area: documents
navigation-topic: approvals
title: Kom igång med Frame.io-integrering
description: Kom igång med Frame.io-integreringen.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: 9825f095a7be7debb5150ca4bd50f7cf6fd12295
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Kom igång med Frame.io-integrering

Integreringen mellan Workfront och Frame.io gör att kreatörer, marknadsförare och intressenter kan arbeta i ett smidigt arbetsflöde. Få tillgång till uppdateringar i realtid, undvik dubbelarbete och se till att materialet godkänns före start.

Mer information om Frame.io finns i [Komma igång med Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Arbetsplanering i Workfront

Projektsamordnare kan skapa projekt och planera arbetet i Workfront. Projekt som skapas i en instans med Frame.io-integreringen aktiverad använder Adobe Enterprise Storage, som gör att resurser kan lagras och hanteras i Adobe ekosystem.

Om din organisation har en Frame.io Enterprise-licens visas även projekt som skapats i Workfront i Frame.io, vilket gör att användare kan interagera och överföra resurser i båda produkterna.

Mer information om Adobe Enterprise Storage och projekt i Frame.io finns i

* [Workspace - översikt: Projekt](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Adobe Enterprise Storage - översikt](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Granska och godkänn resurser

När en mediefil är klar kan projektsamordnaren initiera den formella gransknings- och godkännandeprocessen i Workfront.

När arbetsflödet för godkännande har skapats kan granskare och godkännare använda Frame.io-visningsprogrammet för att lägga till kommentarer och markera resursen. De kan också fatta beslut om godkännande i Frame.io-visningsprogrammet.

Mer information om hur du konfigurerar projekt finns i

* [Skapa ett projekt](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
* [Bildruta.io - integreringsöversikt](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)

### Starta formella granskningar och godkännanden i Workfront

Projektsamordnare kan skapa engångs- och godkännandemallar eller återanvändbara mallar för godkännande. De kan tilldela granskare, godkännare eller en blandning av båda:

* **Granskare** kan lägga till kommentarer och kommentera resurser. När de är klara kan de markera granskningen som slutförd. Att markera granskningen som slutförd krävs inte för att resursen ska gå framåt i godkännandeprocessen.
* **Godkännare** kan lägga till kommentarer och kommentera resurser. De måste fatta beslut om att flytta godkännandeprocessen framåt.

#### Skapa ett arbetsflöde för granskning och godkännande

Granskare och godkännare kan läggas till i ett arbetsflöde för engångsgodkännande eller i en återanvändbar godkännandemall:

* **Engångsgodkännanden**: I det projekt eller den uppgift där resursen finns kan projektkoordinatorn tilldela granskare och godkännare och ange en sluttid. Granskare och godkännare får påminnelser via e-post 72 timmar före ansökningsdeadline, 24 timmar före ansökningsdeadline och sedan efter själva deadline.

  Mer information finns i [Skapa en begäran om dokumentgranskning eller godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

* **Godkännandemallar**: Under Konfigurera i Workfront kan projektkoordinatorer skapa återanvändbara godkännandemallar. I en mall kan användare lägga till granskare och godkännare och ange en tidsram för slutförande. När godkännandemallen används för en resurs beräknas tidsgränsen från den angivna tidsramen.

  När en mall har skapats kan den tillämpas på en mediefil för att starta den formella gransknings- och godkännandeprocessen i Workfront.

  Mer information finns i [Skapa en godkännandemall](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


  ![Tilldela mall](assets/assign-template.png)

### Granska och godkänn resurser i Frame.io-visningsprogrammet

När arbetsflödet för granskning och godkännande har startats i Workfront kan granskare och godkännare öppna Frame.io-visningsprogrammet för att lägga till kommentarer, kommentera resursen och fatta ett beslut.

Mer information finns i [Granska och godkänn med Frame.io-visningsprogrammet](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

#### Öppna Frame.io-visningsprogrammet

Användarna kan öppna Frame.io-visningsprogrammet på följande sätt:

* Workfront e-postmeddelanden
* The My approval widget in the Workfront Home area

>[!NOTE]
>
>Externa Workfront-användare meddelas via e-post och uppmanas att skapa en Frame.io-inloggning för att granska och godkänna mediefiler.

![öppna bildrutevisningsprogrammet från startsidan](assets/open-fio-viewwer.png)

#### Lägga till kommentarer och markera resurser

Kommentarer och resursmarkeringar visas i Frame.io-visningsprogrammet. Mer information om hur du använder Frame.io-visningsprogrammet finns i [Kommentera på dina media](https://help.frame.io/en/articles/9105251-commenting-on-your-media).

#### Fatta ett beslut

När all granskningsaktivitet är klar måste godkännarna fatta något av följande beslut:

* **Godkänn**: Resursen behöver inte ändras och är klar att användas.
* **Behöver arbete**: Resursen behöver ändras och är inte klar att användas. När de angivna ändringarna har gjorts måste resursen överföras som en ny version och gå igenom en ny godkännandeomgång. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Granskarna kan markera sin granskning som slutförd i Workfront, men detta krävs inte för att resursen ska gå vidare i godkännandeprocessen.

Mer information om beslut i Workfront finns i [Översikt över dokumentets beslutsstatus](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Bildrutevisningsprogram och -beslut](assets/decision-fio.png)


### Spåra gransknings- och godkännandestatistik

Projektsamordnarna kan övervaka förloppet för alla pågående godkännanden i Workfront Home-området eller med anpassade rapporter i Canvas Dashboards:

* **Anpassad kontrollpanel**: Skapa en rapportkontrollpanel i kontrollpanelerna på arbetsytan för att visa både högnivåinformation och detaljerad information om granskningar och godkännanden med funktionen för enhetliga godkännanden. Information om hur du kommer igång finns i [Skapa en rapportinstrumentpanel för granskning och godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Hem-widgeten för dokumentgodkännandemått**: Visar 2 diagram med information om genomsnittlig godkännandetid och beslut samt listvyer över väntande och försenade godkännanden.
  ![Alla godkännanden](assets/all-approvals.png)
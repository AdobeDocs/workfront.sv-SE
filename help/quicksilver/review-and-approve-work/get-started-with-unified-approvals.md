---
product-area: documents
navigation-topic: approvals
title: Kom igång med enhetlig granskning och godkännande
description: Läs mer om enhetlig granskning och godkännande från Workfront och Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 10962d59-284e-4c41-8523-18ea4ed78362
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: c989b5d6a91a4b1f19b044916b4f68a1738f9b16
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 0%

---

# Kom igång med enhetlig granskning och godkännande


Enhetlig granskning och godkännande sammanför Adobe Workfront och Adobe Frame.io till en enda, sammanhängande upplevelse - som överbryggar klyftan mellan hantering av marknadsföring, granskning och innehållsleverans. Projektsamordnarna hanterar arbetet i Workfront medan kreatörer, marknadsförare och intressenter granskar och godkänner resurser i den professionella versionen av Frame.io-visningsprogrammet, utan att behöva flytta filer mellan olika verktyg.

Mer information om Frame.io finns i [Komma igång med Frame.io](https://support.frame.io/en/collections/49298-getting-started).

Du måste ha Workfront- och Frame.io-integreringen konfigurerad i din Workfront-instans. Mer information finns i [Översikt över enhetlig granskning och godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#integration-requirements).

## Videoöversikt

>[!VIDEO](https://video.tv.adobe.com/v/3471078)

## Integrationskrav

* Workfront och Frame.io måste distribueras till samma Identity Management-systemorganisation (IMS).

* Användare kan bara tillhöra en Workfront-instans inom IMS-organisationen.

* Workfront-instansen måste aktiveras för Adobe Unified Experience och Adobe Enterprise-lagring.

## Arbetsplanering i Workfront

Projektsamordnare kan skapa projekt och planera arbetet i Workfront. Projekt som skapas i en instans med Frame.io-integreringen aktiverad använder Adobe Enterprise-lagring, som gör att resurser kan lagras och hanteras i Adobe ekosystem.

Om din organisation har en Frame.io Enterprise-licens visas även projekt som skapats i Workfront i Frame.io, vilket gör att användare kan interagera och överföra resurser i båda produkterna.

Mer information om Adobe Enterprise-lagring eller projekt i Frame.io finns i

* [Workspace - översikt: Projekt](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Adobe Enterprise Storage - översikt](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Granska och godkänn resurser

När en mediefil är klar kan projektsamordnaren initiera den formella gransknings- och godkännandeprocessen i Workfront.

När arbetsflödet för godkännande har skapats kan granskare och godkännare använda Frame.io-visningsprogrammet för att lägga till kommentarer och markera resursen. De kan också fatta beslut om godkännande i Frame.io-visningsprogrammet.

Mer information om hur du konfigurerar projekt finns i

* [Skapa ett projekt](/help/quicksilver/manage-work/projects/create-projects/create-project.md)

### Starta formella granskningar och godkännanden i Workfront

Projektsamordnare kan skapa engångs- och godkännandemallar eller återanvändbara mallar för godkännande. De kan tilldela granskare, godkännare eller en blandning av båda:

* **Granskare** kan lägga till kommentarer och kommentera resurser. När de är klara kan de markera granskningen som slutförd. Att markera granskningen som slutförd krävs inte för att resursen ska gå framåt i godkännandeprocessen.
* **Godkännare** kan lägga till kommentarer och kommentera resurser. De måste fatta beslut om att flytta godkännandeprocessen framåt.

#### Skapa ett arbetsflöde för granskning och godkännande

Granskare och godkännare kan läggas till i ett arbetsflöde för engångsgodkännande eller i en återanvändbar godkännandemall:

* **Engångsgodkännanden**: I det projekt eller den uppgift där resursen finns kan projektkoordinatorn tilldela granskare och godkännare och ange en sluttid. Granskare och godkännare får påminnelser via e-post 72 timmar före ansökningsdeadline, 24 timmar före ansökningsdeadline och sedan efter själva deadline.

  Mer information finns i [Skapa ett arbetsflöde för dokumentgodkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-from-the-summary-panel-in-the-new-document-area).

* **Godkännandemallar**: Under Konfigurera i Workfront kan projektsamordnare skapa återanvändbara godkännandemallar. I en mall kan användare lägga till granskare och godkännare och ange en tidsram för slutförande. När godkännandemallen används för en resurs beräknas tidsgränsen från den angivna tidsramen.

  När en mall har skapats kan den tillämpas på en mediefil för att starta den formella gransknings- och godkännandeprocessen i Workfront.

  Mer information finns i [Skapa en arbetsflödesmall för godkännande för dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

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
* **Godkänd med ändringar**: Resursen är för det mesta slutförd men behöver mindre ändringar innan den kan användas. När de angivna ändringarna har gjorts är resursen klar och behöver inte gå igenom ytterligare en godkännandeomgång.
* **Behöver arbete**: Resursen behöver ändras och är inte klar att användas. När de angivna ändringarna har gjorts måste resursen överföras som en ny version och gå igenom en ny godkännandeomgång. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Granskarna kan markera sin granskning som slutförd i Workfront, men detta krävs inte för att resursen ska gå vidare i godkännandeprocessen.

Mer information om beslut i Workfront finns i [Översikt över dokumentets beslutsstatus](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Bildrutevisningsprogram och -beslut](assets/decision-fio.png)


### Spåra gransknings- och godkännandestatistik

Projektsamordnarna kan övervaka förloppet för alla pågående godkännanden i Workfront Home-området eller med anpassade rapporter i Canvas Dashboards:

* **Anpassad kontrollpanel**: Skapa en rapportkontrollpanel i kontrollpanelerna på arbetsytan för att visa både högnivåinformation och detaljerad information om granskningar och godkännanden med funktionen för enhetliga godkännanden. Information om hur du kommer igång finns i [Skapa en rapportinstrumentpanel för granskning och godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Hem-widgeten för dokumentgodkännandemått**: Visar 2 diagram med information om genomsnittlig godkännandetid och beslut samt listvyer över väntande och försenade godkännanden.
  ![Alla godkännanden](assets/all-approvals.png)

## Skicka färdigt material till Adobe Experience Manager

Du kan använda &#x200B; [!DNL Experience Manager Assets] för att hantera och lagra dina digitala resurser som har gått igenom gransknings- och godkännandecykeln. Tack vare integreringen kan ni utnyttja funktionerna i Adobe Experience Manager, Frame.io och Workfront för att effektivisera innehållshanteringen och samarbetet.

Mer information finns i [Använda Adobe Experience Manager med Frame.io-integrering](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).


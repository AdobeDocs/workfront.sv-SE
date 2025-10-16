---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Kom igång med integrationen mellan GenStudio for Performance Marketing och Workfront Proof
description: Kom igång med integrationen mellan GenStudio for Performance Marketing och Workfront Proof
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Kom igång med integrationen mellan GenStudio for Performance Marketing och Workfront Proof

Tack vare integrationen mellan GenStudio for Performance Marketing och Workfront Proof kan du

* Använd Workfront korrekturmallar för att definiera arbetsflöden för granskning och godkännande

* Granska och godkänn GenStudio for Performance Marketing-utkast i Workfront korrekturläsare

* Visa granskningsbeslut i GenStudio for Performance Marketing för slutligt godkännande och publicering

Mer information om granskning och godkännande i GenStudio for Performance Marketing finns i [Workfront Proof-integrering med GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/proof-integration).


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
   <p>Standard </p> 
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare produkter</td> 
   <td> 
   <p> Du måste ha GenStudio for Performance Marketing, och du måste läggas till i produkten som användare i Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Integrationskrav

* Workfront och GenStudio for Performance Marketing måste driftsättas i samma Identity Management-systemorganisation (IMS).

* Användare kan bara tillhöra en Workfront-instans inom IMS-organisationen.

* Workfront-instansen måste vara aktiverad på Adobe Unified Experience.

* Integrationen måste vara aktiverad i Workfront Setup.


## Aktivera integreringen i Workfront

Du måste vara systemadministratör för att kunna aktivera den här integreringen.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på ikonen **[!UICONTROL Setup]** ![Konfigurera &#x200B;](/help/_includes/assets/gear-icon-setup.png) .
1. Klicka på **Granska och godkänn** > **Adobe GenStudio** i den vänstra panelen.
1. Aktivera **Använd korrekturgodkännanden**.
   ![aktivera korrektur för GenStudio-inställning](assets/enable-proofing-gs.png)

## Använd Workfront korrekturmallar för att definiera arbetsflöden för godkännande

Om ditt företags granskningsprocess ofta upprepas eller granskas av samma personer, kan du använda korrekturmallar för att automatisera gransknings- och godkännandearbetsflödena.

### Skapa en korrekturmall i Workfront

Du kan skapa enkla mallar i ett steg för bara en eller två granskare, eller så kan du skapa automatiska mallar i flera steg för komplexa granskningar med många faser och beroenden.

Mer information om hur du skapar automatiska arbetsflöden och mallar i Workfront finns i

* [Översikt över automatiserat arbetsflöde](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [Skapa och hantera automatiserade arbetsflödesmallar](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

### Välja eller ändra mallen i GenStudio for Performance Marketing

När en användare initierar en granskning i GenStudio for Performance Marketing väljer de bara den mall de behöver. Användarna kan enkelt ändra alla korrekturmallar, lägga till eller ta bort granskare och faser när som helst.

Mer information finns i [Begär granskning och godkännande](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/request-review).

## Granska och godkänn GenStudio for Performance Marketing-utkast i Workfront korrekturläsare

Du kan granska och godkänna utkast direkt i GenStudio for Performance Marketing i Workfront korrekturläsare.

Med korrekturläsaren kan du

* Lämna kommentarer
* Markera utkast för att visa vad som behöver ändras
* Fatta ett beslut

Mer information finns i [Granska och redigera innehåll](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/review-and-edit).


>[!IMPORTANT]
>
>Användare måste installera [Granska interaktivt innehåll med Adobe Workfront granskningsverktyg](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) innan de kan börja granska utkast i GenStudio for Performance Marketing.


## Visa granskningsbeslut i GenStudio for Performance Marketing för slutligt godkännande och publicering

När materialet har granskats och godkänts kan du se granskningsbeslutet och publicera det direkt från GenStudio for Performance Marketing.

Mer information finns i [Publicera godkänt innehåll](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/publish-content).

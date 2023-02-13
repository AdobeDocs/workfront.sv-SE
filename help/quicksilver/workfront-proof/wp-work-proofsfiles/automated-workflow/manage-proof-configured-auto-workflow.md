---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Hantera ett korrektur konfigurerat med ett automatiserat arbetsflöde i [!DNL Workfront Proof]
description: Du kan enkelt spåra förloppet för automatiska korrektur av arbetsflöden i avsnittet Arbetsflöde på sidan Korrekturinformation. Du kan visa det arbete du har utfört på varje scen och ändra, lägga till, starta och låsa stegen i korrekturet.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1d0ad905-f3fb-471a-8766-096b978cdf4e
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Hantera ett korrektur konfigurerat med ett automatiserat arbetsflöde i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan enkelt spåra förloppet för automatiska korrektur av arbetsflöden i avsnittet Arbetsflöde i [!UICONTROL Proof details] sida. Du kan visa det arbete du har utfört på varje scen och ändra, lägga till, starta och låsa stegen i korrekturet.

## Visa ett automatiserat arbetsflöde

Du kan visa ditt automatiserade arbetsflöde på tre sätt:

* [Visa en scen i detalj](#view-a-stage-in-detail)
* [Visa alla faser](#view-all-stages)
* [Visa alla faser i detalj](#view-all-stages-in-detail)

### Visa en scen i detalj {#view-a-stage-in-detail}

1. Klicka på knappen längst upp i avsnittet (1).

   Du kan växla mellan faserna med hjälp av diagrammet. Scenen som du visar markeras med grått (2).

1. Om du vill visa en annan scen markerar du den i diagrammet.

![View_a_stage_in_detail.png](assets/view-a-stage-in-detail-350x249.png)

### Visa alla faser {#view-all-stages}

Så här visar du alla faser i ett automatiserat arbetsflöde:

1. Klicka på knappen längst upp på sidan (3).

   Alla steg i det automatiserade arbetsflödet visas i avsnittet, men informationen är dold.

1. Om du vill visa information om en scen klickar du på plusikonen bredvid namnet på varje scen (4).

![View_all_stage.png](assets/view-all-stages-350x212.png)

### Visa alla faser i detalj {#view-all-stages-in-detail}

Så här visar du alla faser i ditt automatiserade arbetsflöde i detalj:

1. Klicka på knappen längst upp på sidan (5).

   Här visas alla faser i det automatiserade arbetsflödet med information om varje fas utökat.

   Du kan dölja detaljerna för varje scen genom att klicka på minusikonen (6).

![View_all_stage_in_detail.png](assets/view-all-stages-in-detail-350x370.png)

## Använda det automatiska arbetsflödesdiagrammet

Bilden på din automatiska [!UICONTROL Workflow] visas högst upp i avsnittet Arbetsflöde.

Så här döljer du diagrammet

1. Klicka på **[!UICONTROL Hide]** knapp (1).

![Diagram__1_.png](assets/diagram--1--350x217.png)

Stegen i diagrammet markeras enligt följande:

![dot.png](assets/dot.png)- en aktiv fas

![gray_dot.png](assets/grey-dot.png)- en inaktiv fas\
![sbw-key-icon.png](assets/sbw-key-icon.png)  - en privat fas

![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  - en låst scen

Raderna mellan faserna visar beroendena mellan faserna. Linjerna som leder till inaktiva stadier prickas tills scenen aktiveras.

Om du håller pekaren över en scen i diagrammet visas scenens förlopp. Om scenen inte är aktiv och du har redigeringsbehörighet på scenen, kan du starta scenen från popup-fönstret med hjälp av [!UICONTROL Start stage] -knappen. Alternativet Lås en aktiv scen visas också.

Mer information om förloppsindikatorn finns i  [Visa förlopp och status för ett korrektur i [!DNL Workfront] Korrektur](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

![Diagram_-_scensammanfattning.png](assets/diagram---stage-summary-350x214.png)

## Lägg till en ny fas

Du kan lägga till en ny fas i ditt automatiska arbetsflöde från [!UICONTROL Proof details] sida.

1. Klicka på **[!UICONTROL New stage]** knapp (1).

![Adding_a_new_stage_1.png](assets/adding-a-new-stage-1-350x218.png)

I **Ny fas** som visas kan du fylla i information och inställningar för scenen.

![Adding_a_new_stage_2.png](assets/adding-a-new-stage-2-350x332.png)

## Hantera sceninställningar

På sidan kan du ändra inställningarna för varje fas (om du har redigeringsbehörighet):

* Ändra, lägga till eller ta bort deadline för scenen (1)
* Lås scenen (2) - det här alternativet aktiveras om scenen är aktiv. för inaktiva stadier visas alternativet Starta scenen
* Ändra inställningarna genom infogad redigering (3)
* Aktivera eller inaktivera Endast ett beslut krävs på scenen (4)
* Ändra scenens sekretess (5)

![Managing_stage_settings.png](assets/managing-stage-settings-350x93.png)

Du kan också flytta granskarna mellan faserna genom att helt enkelt dra och släppa dem från en scen till en annan. De tillgängliga stadierna markeras med blått och de släppområden som visas för varje scen är tydligt markerade.

![Moving_reviewers_between_stage.png](assets/moving-reviewers-between-stages-350x254.png)

## Scenalternativ

The [!UICONTROL Actions] meny (1) för varje scen har följande alternativ:

* Meddelande alla (2) - du kan skicka en påminnelse via e-post till alla granskare på scenen
* Dela (3) - du kan lägga till nya granskare på scenen
* Ta bort fas (4) - Om korrekturläsaren befinner sig på den scenen blir du ombedd att välja en ny fas för dem

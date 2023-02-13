---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Översikt över automatiska arbetsflödessteg
description: Korrekturfaser är tidssegment där olika användare granskar ett korrektur. När korrekturet flyttas från en fas till nästa underrättar Adobe Workfront granskarna om när det är dags att arbeta med det.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Översikt över automatiska arbetsflödessteg

Korrekturfaser är tidssegment där olika användare granskar ett korrektur. När korrekturet flyttas från en fas till nästa underrättar Adobe Workfront granskarna om när det är dags att arbeta med det.

![stage_chart.png](assets/stages-diagram-350x63.png)

Stegen inträffar i två olika situationer:

* [Skapa ett korrektur med ett automatiserat arbetsflöde](#create-a-proof-with-an-automated-workflow)
* [Tilldela deadlines för olika granskare på ett korrektur](#assign-deadlines-for-different-reviewers-on-a-proof)

## Skapa ett korrektur med ett automatiserat arbetsflöde {#create-a-proof-with-an-automated-workflow}

När du lägger till ett automatiserat arbetsflöde i ett korrektur ställer du in de steg i granskningsarbetet som du vill ska utföras.

När du ställer in faser för ett korrektur med ett automatiskt arbetsflöde:

* Du kan konfigurera scenerna så att de körs i följd eller samtidigt.
* Du kan konfigurera vissa stadier så att de blir aktiva först när en tidigare fas har slutförts.
* Du kan göra vissa faser privata. Detta är användbart för en byrå som granskar ett korrektur innan det delas med en kund och inte vill att de resulterande kommentarerna ska vara synliga för kunden.

Instruktioner om hur du skapar faser för ett korrektur med ett automatiserat arbetsflöde finns i [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Om en användare inte finns med i någon fas men har åtkomst till dokumentet och öppnar korrekturet, skapas en fas med namnet *Workfront*.
>
>Användaren som öppnade korrekturet tilldelas den roll som anges i Inställningar > Granska och godkännade > Roller för icke-mottagare som öppnar ett dokumentkorrektur.

## Tilldela deadlines för olika granskare på ett korrektur {#assign-deadlines-for-different-reviewers-on-a-proof}

När du tilldelar olika korrekturtider till granskare för ett korrektur skapas en fas för varje deadline och grupperar granskarna för varje deadline i motsvarande fas. 

**Exempel:** Om du till exempel skapar ett korrektur med fyra granskare:

* För granskarna Olivia och Tony anger du en deadline för 14:00 om några dagar.
* För Aaron och Amy anger du en deadline för 17:00 några dagar senare.
* Du anger ingen deadline för dig själv.

Systemet skapar en fas för var och en av dessa tre&quot;grupper&quot; av granskare:

![stage.png](assets/stages-350x239.png)

Om du delar korrekturet med en annan granskare, och inte anger någon deadline, lägger Workfront till användaren på scen 3, där det inte finns någon deadline. 

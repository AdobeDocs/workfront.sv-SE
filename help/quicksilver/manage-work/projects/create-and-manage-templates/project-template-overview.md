---
product-area: templates
navigation-topic: templates-navigation-topic
title: Översikt över projektmallen
description: Du kan använda projektmallar för att hämta in de flesta repeterbara processer, information och inställningar som är kopplade till projekten i organisationen.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Översikt över projektmallen

<!-- Audited: 12/2023 -->

Du kan använda projektmallar för att hämta in de flesta repeterbara processer, information och inställningar som är kopplade till projekten i organisationen.

Du kan definiera uppgifter, köämnen, anpassade formulär och bifoga dokument i mallen.

När du har skapat mallar kan du bifoga dem till befintliga projekt eller använda dem för att skapa nya projekt. All information i mallen överförs till de projekt som skapas med den.

## Fördelar med att använda mallar i Adobe Workfront

Nedan följer några av fördelarna med att använda mallar för att skapa projekt:

* Det sparar både tid och kraft när du skapar nya projekt som är repetitiva.
* Ni har enhetlig information i alla projekt som har liknande omfattning.
* Det är användbart när du rapporterar om projekt. Du kan till exempel rapportera om projekt som delar samma mall, jämföra deras förlopp och hitta förbättringar i hur de kan slutföras.
* Förutom att definiera de framtida projektinställningarna kan du lägga till följande information för det framtida projektet i en mall:

   * Uppgifter
   * Dokument
   * Godkännanden
   * Köinformation
   * Köämnen
   * Ämnesgrupper
   * Routningsregler
   * Anpassad Forms
   * Information om företag och grupper

## Bästa tillvägagångssätt för att skapa mallar

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Tänk på följande när du skapar mallar:

* Tilldela inte användare till malluppgifter. Även om du kan lämna uppgifterna otilldelade rekommenderar vi att du tilldelar jobbroller till uppgifter. Då får du en uppfattning om vilka användare som kan tilldelas till uppgifterna när du skapar projektet med hjälp av mallen.
* Ge alltid malluppgifterna ett värde för Varaktighet och Planerade timmar. Alla uppgifter i projektet ska vara kopplade till en varaktighet för hur länge aktiviteten kan vara öppen och till ett värde för planerad timme för hur lång tid det faktiskt tar för uppgiften att slutföras. Uppgifter utan den här informationen kan inte budgeteras korrekt för resurser när resurshanteringsverktyg används i Workfront.

  Mer information om Varaktighet finns i följande artiklar:

   * [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Översikt över projektvaraktighet](../../../manage-work/projects/planning-a-project/project-duration.md)

  Mer information om planerade timmar finns i [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

* Lägg till de föregående relationerna mellan aktiviteterna i själva slutet, när du har en tydlig förståelse för den framtida projektplanen i sin helhet. Att lägga till föregångare till malluppgifter liknar att lägga till föregående aktiviteter till aktiviteter i ett projekt.

  Mer information om hur du lägger till föregående aktiviteter i aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Ange vem mallen ska delas med för framtida bruk och vilka projekt som ska skapas från mallen ska delas med. Mer information om att dela mallar finns i [Dela projektmallar](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Använd globala godkännandeprocesser och lägg till dem i dina mall- och malluppgifter om det går. Detta sparar tid när uppgifter eller det framtida projektet behöver gå igenom samma godkännanden.

  Mer information om hur du skapar godkännanden finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Mer information om hur du associerar en godkännandeprocess till en arbetsuppgift finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Olika sätt att skapa mallar

Du kan skapa en ny mall på följande sätt:

* Från scratch.\
  Mer information om hur du skapar en ny mall från grunden finns i [Skapa en projektmall](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Från befintliga projekt genom att spara ett projekt som en mall.\
  Mer information om hur du skapar mallar från befintliga projekt finns i [Skapa mall från projekt](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Genom att kopiera den från en annan mall.\
  Mer information om hur du kopierar en befintlig mall finns i [Kopiera en projektmall](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Med våra exempelmallar.\
  Mer information om hur du skapar mallar med våra exempelmallar finns i [Skapa projektmallar från exempel](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).

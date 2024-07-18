---
product-area: projects
navigation-topic: approvals
title: Associera en ny eller befintlig godkännandeprocess med arbete
description: I den här artikeln beskrivs hur du kan associera godkännandeprocesser med arbetsobjekt. Mer information om hur du associerar godkännanden med korrektur eller dokument finns i följande artiklar.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 65680d320a06cc96c7434d3efb91eb16e6e86e44
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# Associera en ny eller befintlig godkännandeprocess med arbete

I den här artikeln beskrivs hur du kan associera godkännandeprocesser med arbetsobjekt. Mer information om hur du associerar godkännanden med korrektur eller dokument finns i följande artiklar:

* [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Begär dokumentgodkännanden](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Du kan associera en global eller engångsprocess med en arbetsuppgift i Adobe Workfront. Följande scenarier finns:

* Koppla en befintlig global godkännandeprocess till en projekt-, uppgifts-, utgåva-, mall- eller malluppgift. Vissa globala godkännandeprocesser är tillgängliga för alla grupper i systemet. Globala godkännandeprocesser på gruppnivå är bara tillgängliga för vissa grupper.
* Skapa en godkännandeprocess som kan användas endast en gång och koppla den till en befintlig projekt-, uppgifts-, utgåva-, mall- eller malluppgift.

>[!NOTE]
>
>I den här artikeln används termen&quot;global godkännandeprocess&quot; för att skilja sig från&quot;godkännandeprocess för enstaka användning&quot;. En global godkännandeprocess kan användas upprepade gånger.
>
>Termen global godkännandeprocess på gruppnivå avser en godkännandeprocess som kan användas upprepade gånger för artiklar och med statusvärden som bara är kopplade till en viss grupp.

Mer allmän information om godkännandeprocesser finns i [Översikt över godkännandeprocessen](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Mer information om hur du skapar en global godkännandeprocess finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst eller senare till projekt, uppgifter, problem eller mallar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet, aktiviteten, utgåvan eller mallen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Överväganden om att associera godkännandeprocesser med arbetsobjekt

Förutom de överväganden som beskrivs nedan rekommenderar vi att du går igenom de allmänna övervägandena om godkännandeprocesser i Workfront. Mer information finns i [Översikt över godkännandeprocessen](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* Du måste skapa projektet, uppgiften, utgåvan, mallen eller malluppgiften innan godkännandeprocessen kan kopplas till dem.
* När du kopplar en godkännandeprocess till ett objekt för en status som har passerat och i vilken objektet för närvarande är, kommer godkännandeprocessen inte att aktiveras och inga meddelanden skickas till godkännarna.

  **Exempel:** Om en aktivitet har statusen Fullständig och du bifogar en godkännandeprocess som är associerad med statusen Fullständig, utlöses inte godkännandet.

* När du kopplar en godkännandeprocess till den första statusen för ett objekt (genom att använda en mall för uppgifter och projekt, använda inställningarna för köinställningar för utgåvor eller definiera uppgiftsinställningarna för ett projekt för nya uppgifter), åsidosätts godkännandeprocesserna om det inskickade godkännandet återkallas. I det här fallet får godkännarna inga meddelanden.

  Mer information om hur du återkallar godkännanden finns i [Visa godkännanden](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >Den första statusen för en aktivitet eller ett problem är Ny. Den första statusen för ett projekt är den status som valts av Workfront-administratören i Projektinställningar i systemet. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Associationen mellan godkännandeprocesser och ett objekt registreras inte i objektets uppdateringsområde.
* Du kan inte associera en godkännandeprocess med en överordnad aktivitet.
* När du lägger till en användare, ett team eller en roll som godkännare får de inte automatiskt behörighet till objektet som är kopplat till det godkännandet. De får behörigheter till objektet när godkännandesteget aktiveras. Annars måste objekten delas med dem innan de kan fatta ett beslut om godkännande.

I följande avsnitt beskrivs de olika metoderna för att koppla en godkännandeprocess till ett projekt, en uppgift eller ett problem.

## Associera en global godkännandeprocess med en arbetsuppgift {#associate-a-global-approval-process-with-a-work-item}

Du kan associera en global godkännandeprocess med en arbetsuppgift (projekt, uppgift, utgåva, mall, malluppgift).

Den globala godkännandeprocessen måste vara tillgänglig för den grupp som är associerad med arbetsuppgiften eller för alla grupper i systemet.

>[!NOTE]
>
>Du kan koppla projektgodkännandeprocesser till en mall och uppgiftsgodkännandeprocesser till en malluppgift. När du har gjort det blir godkännandeprocessen ett projekt eller en process för godkännande av en uppgift när någon använder mallen för att skapa ett projekt. En godkännandeprocess som är kopplad till en mall- eller malluppgift är fortfarande en engångsprocess för projekt och uppgifter.

Mer information om hur Workfront-administratörer kan konfigurera en global godkännandeprocess för alla grupper i systemet och hur gruppadministratörer kan skapa godkännanden för en grupp finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>Du kan också ändra en global godkännandeprocess efter dina specifika behov. Mer information finns i avsnittet [Ändra en global godkännandeprocess för ett specifikt objekt](#modify-a-global-approval-process-for-use-on-a-specific-object) i den här artikeln.

Så här associerar du en befintlig global godkännandeprocess med en projekt-, uppgifts-, utgåva-, mall- eller malluppgift:

1. Gå till den arbetsuppgift där du vill associera en godkännandeprocess.
1. Klicka på **Godkännanden** på den vänstra panelen.

   Du kan behöva klicka på **Visa mer** och sedan på **Godkännanden**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Den valda godkännandeprocessen visas.

1. Expandera listrutan **Använd befintlig** och välj en befintlig godkännandeprocess.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Den valda godkännandeprocessen visas.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Klicka på **Spara**.
1. (Valfritt) Klicka på Redigera godkännandeprocess om du vill ändra det befintliga godkännande som du har kopplat till objektet. Detta ändrar den globala godkännandeprocessen till en enda godkännandeprocess. Mer information finns i avsnittet [Ändra en global godkännandeprocess för ett specifikt objekt](#modify-a-global-approval-process-for-use-on-a-specific-object) i den här artikeln.

## Ändra en global godkännandeprocess för användning på ett specifikt objekt {#modify-a-global-approval-process-for-use-on-a-specific-object}

Workfront-administratören eller gruppadministratören skapar globala godkännandeprocesser som du kan använda, vilket beskrivs i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Att ändra en global godkännandeprocess som är kopplad till ett objekt är identiskt med att ändra en godkännandeprocess för enstaka användning.

Du kan ändra en global godkännandeprocess så att den passar alla specifika behov för projektet, uppgiften eller utgåvan som du associerar med den.

>[!IMPORTANT]
>
>När du ändrar en global godkännandeprocess blir den en godkännandeprocess som bara kan användas på det objekt där du ändrade den. Den globala godkännandeprocessen ändras inte.
>
>Tänk på följande begränsningar när du ändrar en global godkännandeprocess:
>
>* Godkännandeprocessen ändras endast för det projekt, den uppgift eller det problem som du associerar godkännandeprocessen med.
>* Eventuella ändringar som en administratör gör i den ursprungliga globala godkännandeprocessen återspeglas inte i den globala godkännandeprocess som du har ändrat.
>

Så här ändrar du en godkännandeprocess som redan är kopplad till ett objekt:

1. Lägg till en global godkännandeprocess för projektet, uppgiften eller utgåvan.

   Instruktioner finns i avsnittet [Koppla en global godkännandeprocess till en arbetsuppgift](#associate-a-global-approval-process-with-a-work-item) i den här artikeln.

   >[!IMPORTANT]
   >
   >Kontrollera att du klickar på **Spara** när du lägger till godkännandet.

1. När den globala godkännandeprocessen har lagts till klickar du på ikonen **Redigera**![](assets/edit-icon.png) i det övre högra hörnet på godkännandesidan. Den här åtgärden omvandlar den globala godkännandeprocessen eller godkännandeprocessen på gruppnivå till en enda godkännandeprocess.
1. Gör eventuella ändringar i den befintliga godkännandeprocessen. Mer information finns i avsnittet [Associera en godkännandeprocess för enstaka användning med en projekt-, uppgifts-, utgåva-, mall- eller malluppgift](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) i den här artikeln.
1. Klicka på **Spara** och klicka sedan på **Spara** igen för att bekräfta att du vill konvertera den globala godkännandeprocessen till en godkännandeprocess som bara är tillgänglig för det här objektet.

## Associera en godkännandeprocess med ett projekt, en uppgift, en utgåva, en mall eller en malluppgift {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Du kan skapa en godkännandeprocess som bara kan användas för ett specifikt projekt, en viss uppgift eller en viss utgåva.

Du kan även koppla en enstaka godkännandeprocess till en mall- eller malluppgift så att den är tillgänglig för projekt och uppgifter som skapas från mallen.

>[!NOTE]
>
>Du kan associera en godkännandeprocess för enstaka användning med status på system- eller gruppnivå för ett projekt, en uppgift, en utgåva, en mall eller en malluppgift. Mer information om Workfront-status finns i [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Om du skapar en godkännandeprocess på det här sättet kan du skapa en anpassad godkännandeprocess som passar dina behov. Godkännandeprocessen kan dock inte kopplas till andra arbetsuppgifter i framtiden.

Du kan också ändra en global godkännandeprocess för ett visst objekt och det blir också en godkännandeprocess för enstaka användning. Mer information finns i avsnittet [Ändra en global godkännandeprocess för ett specifikt objekt](#modify-a-global-approval-process-for-use-on-a-specific-object) i den här artikeln.

Så här skapar du en godkännandeprocess för en enstaka användning:

1. Gå till projektet, uppgiften, utgåvan, mallen eller malluppgiften där du vill koppla en godkännandeprocess.
1. Klicka på **Godkännanden** på den vänstra panelen.

   Du kan behöva klicka på **Visa fler** > **Godkännanden**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klicka på **Skapa för engångsbruk**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Slutför stegen som börjar med steg 6 i avsnittet Skapa en global godkännandeprocess på systemnivå eller gruppnivå för arbetsobjekt i artikeln [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >När du har kopplat godkännandeprocessen för en enstaka användning visas den som `<Custom>` i fältet Godkännandeprocess i rutan Redigera för mallar och malluppgifter. Mer information om hur du redigerar mallar och malluppgifter finns i följande artiklar:
   >
   >* [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [Redigera en malluppgift](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Ta bort en godkännandeprocess från en arbetsuppgift

Du kan ta bort en global godkännandeprocess eller en godkännandeprocess på gruppnivå eller ta bort en enstaka godkännandeprocess från ett projekt, en uppgift eller ett problem som tidigare associerats med den.

Följande scenarier finns: 

* Godkännandet tas inte bort om du tar bort den globala godkännandeprocessen eller godkännandeprocessen på gruppnivå. Godkännandet är fortfarande tillgängligt för framtida bruk.
* Om du tar bort en enanvändares godkännandeprocess tas den bort från Workfront och kan inte återställas.

Så här tar du bort eller tar bort en godkännandeprocess från en arbetsuppgift:

1. Gå till projektet, uppgiften, utgåvan, mallen eller malluppgiften där du vill ta bort en godkännandeprocess som du har lagt till tidigare.
1. Klicka på **Godkännanden** på den vänstra panelen.

   Du kan behöva klicka på **Visa fler** > **Godkännanden**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klicka på en av följande ikoner i det övre högra hörnet av avsnittet Godkännanden, beroende på vilken typ av godkännande som är associerat med objektet:

   * **Ta bort** ikon ![](assets/remove-icon---x-in-circle.png) för globala godkännanden eller godkännanden på gruppnivå.
   * **Ta bort** ikon ![](assets/delete.png) för enanvändargodkännanden.

1. Bekräfta genom att klicka på **Ta bort** eller **Ta bort**.

   Godkännandeprocessen tas bort från arbetsuppgiften.

## Associera en godkännandeprocess automatiskt med arbetsuppgifter

Du kan koppla en godkännandeprocess automatiskt till arbetsobjekt med följande arbetsflöden:

* För projekt och uppgifter kan du associera en godkännandeprocess med en mall. Du kan bifoga en befintlig godkännandeprocess till fliken Mallgodkännanden eller fliken Mallar för uppgiftsgodkännanden. Mer information om hur du associerar ett befintligt godkännande med en arbetsuppgift finns i [Associera en global godkännandeprocess med en arbetsuppgift](#associate-a-global-approval-process-with-a-work-item) i den här artikeln.
* För nya uppgifter i ett befintligt projekt kan du koppla en global godkännandeprocess eller en global godkännandeprocess på gruppnivå i området Uppgiftsinställningar i rutan Redigera projekt. Mer information finns i avsnittet Aktivitetsinställningar i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).
* För problem kan du koppla ett godkännande till varje ny utgåva som läggs till i ett projekt genom att koppla en befintlig godkännandeprocess till en begärandekö. Mer information om hur du konfigurerar begärandeköer finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

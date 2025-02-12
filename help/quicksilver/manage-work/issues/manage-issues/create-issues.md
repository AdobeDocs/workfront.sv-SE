---
product-area: projects
navigation-topic: manage-issues
title: Skapa problem
description: När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en uppgift. Användare med lämplig åtkomst kan visa och övervaka status för problem allt eftersom projektet eller aktiviteten fortskrider till slutförandet, vilket eliminerar behovet av långa e-postkedjor eller statusmöten. Till skillnad från planerade aktiviteter representerar ärenden oplanerade arbetsuppgifter i Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 0%

---

# Skapa problem

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en uppgift. Användare med lämplig åtkomst kan visa och övervaka status för problem allt eftersom projektet eller aktiviteten fortskrider till slutförandet, vilket eliminerar behovet av långa e-postkedjor eller statusmöten. Till skillnad från planerade aktiviteter representerar ärenden oplanerade arbetsuppgifter i Adobe Workfront.

Du kan även lägga till problem i projekt som begäranden. Mer information finns i [Skapa och skicka Adobe Workfront-begäranden](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Problem och förfrågningar används utan åtskillnad i Workfront. Du kan registrera problem i både projekt och uppgifter för att indikera oförutsedda arbeten som behöver åtgärdas. Du kan också skicka in begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller senare om du vill lägga till problem i ett projekt eller en uppgift</p> <p>Begär eller högre för att lägga till problem som begäranden med hjälp av en frågekö.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller öka åtkomsten till projekt och uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till problem på din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Bevilja åtkomst till problem</a>. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter med möjlighet att lägga till problem i den uppgift eller det projekt där du skapade problemet</p> <p> Mer information om att bevilja behörigheter för problem finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett problem </a></p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Begränsningar för att skapa problem

När du har rätt behörighet och behörighet kan du skapa problem i ett projekt eller en uppgift. I följande fall kanske du inte kan skapa problem:

* Din Workfront-administratör eller en gruppadministratör måste aktivera tillägg av problem i ett projekt som har statusen Fullständigt eller Dölj i området Projektinställningar. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Du kan inte lägga till utgåvor i ett projekt som väntar på godkännande.

## Förbered formuläret för nytt problem

Organisationen bör ha en väldefinierad process för när och hur ett problem ska registreras. När du konfigurerar den här processen är det första steget att skapa det formulär som behövs för att skicka in ett ärende. Oavsett om du vill tillåta att utgåvor läggs till direkt i uppgifter och projekt, eller om du har frågeköer där utgåvor skickas, kan du definiera vilka Workfront-fält och vilka anpassade fält som är tillgängliga för användare när de skickar nya utgåvor och måste fyllas i. Formuläret Nytt problem kan innehålla viktig information som kan vara till hjälp när du snabbt vill lösa problemet.

Fälten för de nya problemen i ett projekt definieras i avsnittet Köinformation i projektet där problemen loggas. Mer information om hur du konfigurerar avsnittet Köinformation i projektet finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Mer information om hur du skapar problem genom att skicka dem till en begärandekö finns i avsnittet [Skapa problem genom att ange en ny begäran](#create-issues-by-entering-a-new-request) i den här artikeln.

## Skapa problem i en uppgift eller ett projekt med knappen Nytt problem

När du har definierat fälten för ett nytt utgivningsformulär i ditt projekt kan du börja skapa problem.

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![New issue screen](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

Så här skapar du ett problem för en aktivitet eller ett projekt:

1. Gå till ett projekt där du vill skapa problemet.
1. (Valfritt) Om du vill logga problemet för en aktivitet går du till området **Åtgärder** och klickar sedan på namnet på en aktivitet.
1. Klicka på avsnittet **Problem**.

   Listan med projektproblem visas

1. Klicka på **Nytt problem** högst upp i listan över utgåvor.
Rutan Nytt problem visas.

   ![Ny utgåva](assets/new-issue-box-matches-new-request-ui.png)

1. (Villkorligt) Om den som skapat projektet har skapat köämnen eller ämnesgrupper i projektet läggs de till i det nya utgivningsformuläret. Ange **ämnesgruppen** eller **köämnet** för det nya problemet. Ämnesgrupper och Köämnen har namn som är anpassade efter din miljö.\
   Mer information om hur du skapar ämnesgrupper finns i [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Om det bara finns ett köämne i projektet visas det automatiskt.
   * Om ämnesgruppen inte har några köämnen eller ämnesgrupper under sig är ingenting tillgängligt i listrutan Ämnesgrupp.

1. Lägg till problemnamnet i fältet **Ämne** och lägg sedan till en **Beskrivning**.

1. (Villkorligt) Om den som skapat projektet tillåter att fältet **Typ av begäran** visas i formuläret Nytt problem, väljer du typ av problem bland följande alternativ:

   * Felrapport
   * Ändra ordning
   * Problem
   * Begäran\
     Beroende på hur din Workfront-administratör har konfigurerat dina projektinställningar kan det finnas olika namn på problemtyperna.

   >[!TIP]
   >
   >Begärandetyperna måste vara aktiverade i köinformationen och även när du skapar ett köämne som ska visas som ett val i formuläret Nytt problem. Mer information finns i följande artiklar:
   >* [Skapa en begärandekö](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Skapa köämnen](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Fortsätt att ange fälten som är tillgängliga i formuläret **Ny utgåva**. Mer information om de fält som är tillgängliga när du anger ett nytt problem finns i [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Alla problemrelaterade fält är inte tillgängliga i formuläret Ny utgåva. Den som skapar projektet aktiverar de fält som är tillgängliga när ett problem skapas när de definierar området Köinformation i projektet. Mer information finns i [Skapa en begärandekö](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Villkorligt) Om köämnen är kopplade till ett anpassat formulär visas det anpassade formuläret i formuläret **Nytt problem**.\
   eller\
   Om projektet är kopplat till ett anpassat formulär via området Köinformation, visas formuläret i formuläret **Nytt problem**, efter Workfront standardfält.

   Mer information finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicka på **Skicka**.

   Problem kan tilldelas flera användare, jobbroller eller ett team. Mer information om hur du tilldelar och hanterar begäranden finns i [Hantera arbets- och teamförfrågningar](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Skapa ärenden för en aktivitet eller ett projekt

>[!IMPORTANT]
>
>Projektägaren måste aktivera **Tillåt användare att lägga till interna utgåvor** när de definierar utgåvinställningar för projektet innan du kan lägga till utgåvor i projektet eller aktiviteterna. Mer information om hur du konfigurerar probleminställningar för ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).
>

När du snabbt vill lägga till flera problem kan du skapa problem för en uppgift eller ett projekt genom att lägga till dem i en lista med problem.

>[!NOTE]
>
>När du lägger till fel i dokumentet använder Workfront inte formuläret Nytt problem för de nya utgåvorna. Vi rekommenderar inte att du infogar fel om du vill att användarna ska ange viss information när de anger problem. Detta kan ha en negativ inverkan på problemrapporteringen och senare på möjligheten för användaren som är tilldelad problemet att ha all information som krävs för att lösa problemet.

Så här skapar du interna utgåvor:

1. Gå till ett projekt där du vill skapa problemet.
1. (Valfritt) Om du vill logga problemet för en aktivitet går du till avsnittet **Åtgärder** och klickar sedan på namnet på en aktivitet.
1. Klicka på avsnittet **Problem** i den vänstra panelen.
1. Klicka på **Lägg till fler problem** längst ned i listan med utgåvor.

   En ny rad skapas i listan med problem i avsnittet Problem.

   >[!TIP]
   >
   >Det här alternativet är nedtonat om inställningen Tillåt användare att lägga till interna utgåvor är avmarkerad i rutan Redigera projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Knappen Lägg till fler problem](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Börja skriva namnet på problemet i fältet Namn och fortsätt sedan att lägga till mer information om problemet.

   >[!TIP]
   >
   >De fält som är tillgängliga för redigering online är tillgängliga i den vy du använder i din problemlista. Du kanske inte kan redigera följande typer av fält:
   >   
   >* Fält som tillhör ett annat objekt
   >* Fält som du inte har behörighet att redigera
   >* Fält som är beräkningar och som uppdateras automatiskt av Workfront

1. Klicka på Retur för att slutföra den infogade redigeringen och lägga till problemet i projektet eller uppgiften.

## Skapa problem genom att ange en ny begäran {#create-issues-by-entering-a-new-request}

Du kan ange projekt som mottagare för att ta emot ärenden. Den här typen av projekt kallas frågeköer i Workfront. Du kan öppna Begäranköer via området Förfrågningar på huvudmenyn.

>[!TIP]
>
>Termerna&quot;issue&quot; och&quot;request&quot; är utbytbara i Workfront.

Mer information om hur du konfigurerar projekt som frågeköer för att ta emot problem finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Mer information om hur du skickar begäranden finns i [Skapa och skicka Adobe Workfront-begäranden](../../../manage-work/requests/create-requests/create-submit-requests.md).

---
product-area: projects
navigation-topic: manage-issues
title: Skapa problem
description: När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en uppgift. Användare med lämplig åtkomst kan visa och övervaka status för problem allt eftersom projektet eller aktiviteten fortskrider till slutförandet, vilket eliminerar behovet av långa e-postkedjor eller statusmöten. Till skillnad från planerade aktiviteter representerar ärenden oplanerade arbetsuppgifter i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# Skapa problem

När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en uppgift. Användare med lämplig åtkomst kan visa och övervaka status för problem allt eftersom projektet eller aktiviteten fortskrider till slutförandet, vilket eliminerar behovet av långa e-postkedjor eller statusmöten. Till skillnad från planerade aktiviteter representerar ärenden oplanerade arbetsuppgifter i Adobe Workfront.

Du kan även lägga till problem i projekt som begäranden. Mer information finns i [Skapa och skicka Adobe Workfront-förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Problem och förfrågningar används utan åtskillnad i Workfront. Du kan registrera problem i både projekt och uppgifter för att indikera oförutsedda arbeten som behöver åtgärdas. Du kan också skicka in begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö.

## Åtkomstkrav

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
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller öka åtkomsten till projekt och uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till problem på din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Bevilja åtkomst till utleveranser</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter med möjlighet att lägga till problem i den uppgift eller det projekt där du skapade problemet</p> <p> Information om hur du beviljar behörigheter för problem finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett ärende </a></p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Begränsningar för att skapa problem

När du har rätt behörighet och behörighet kan du skapa problem i ett projekt eller en uppgift. I följande fall kanske du inte kan skapa problem:

* Din Workfront-administratör eller en gruppadministratör måste aktivera tillägg av problem i ett projekt som har statusen Fullständigt eller Dölj i området Projektinställningar. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Du kan inte lägga till utgåvor i ett projekt som väntar på godkännande.

## Förbered formuläret för nytt problem

Organisationen bör ha en väldefinierad process för när och hur ett problem ska registreras. När du konfigurerar den här processen är det första steget att skapa det formulär som behövs för att skicka in ett ärende. Oavsett om du vill tillåta att utgåvor läggs till direkt i uppgifter och projekt, eller om du har frågeköer där utgåvor skickas, kan du definiera vilka Workfront-fält och vilka anpassade fält som är tillgängliga för användare när de skickar nya utgåvor och måste fyllas i. Formuläret Nytt problem kan innehålla viktig information som kan vara till hjälp när du snabbt vill lösa problemet.

Fälten för de nya problemen i ett projekt definieras i avsnittet Köinformation i projektet där problemen loggas. Information om hur du konfigurerar avsnittet Köinformation i projektet finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Information om hur du skapar problem genom att skicka dem till en begärandekö finns i [Skapa problem genom att ange en ny begäran](#create-issues-by-entering-a-new-request) i den här artikeln.

## Skapa problem i en uppgift eller ett projekt med knappen Nytt problem

När du har definierat fälten för ett nytt utgivningsformulär i ditt projekt kan du börja skapa problem.

Så här skapar du ett problem för en aktivitet eller ett projekt:

1. Gå till ett projekt där du vill skapa problemet.
1. (Valfritt) Om du vill logga problemet för en uppgift går du till **Uppgifter** och klicka sedan på namnet på en uppgift.
1. Klicka på **Problem** -avsnitt.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Klicka **Nytt problem**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Villkorligt) Om den som skapat projektet har skapat köämnen eller ämnesgrupper i projektet läggs de till i det nya utgivningsformuläret. Ange **Ämnesgrupp** eller **Köämne** av din nya utgåva. De bör ha namn som är anpassade efter din miljö.\
   Mer information om hur du skapar ämnesgrupper finns i [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Om det bara finns ett köämne i projektet visas det automatiskt.
   * Om ämnesgruppen inte har några köämnen eller ämnesgrupper under sig är ingenting tillgängligt i listrutan Ämnesgrupp.

1. (Villkorligt) Om den som skapat projektet tillåts för **Ärendetyp** fält som ska visas i formuläret Nytt problem, välj typ av problem bland följande alternativ:

   * Felrapport
   * Ändra ordning
   * Problem
   * Begäran\
      Beroende på hur din Workfront-administratör har konfigurerat dina projektinställningar kan det finnas olika namn på problemtyperna.

1. Ange något av fälten som finns i **Nytt problem** formulär. Mer information om hur du definierar fält när du anger ett nytt problem finns i [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md).
1. (Villkorligt) Om köämnen är kopplade till ett anpassat formulär visas det anpassade formuläret i dialogrutan **Nytt problem** formulär.\
   eller\
   Om projektet är kopplat till ett anpassat formulär via området Köinformation, visas formuläret i dialogrutan **Nytt problem** -formulär, under Workfront standardfält.

   Mer information finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicka **Spara nytt problem.**

Problem kan tilldelas flera användare, jobbroller eller ett team. Mer information om hur du tilldelar och hanterar begäranden finns i [Hantera arbets- och teamförfrågningar](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Skapa ärenden för en aktivitet eller ett projekt

>[!IMPORTANT]
>
>Projektägaren måste aktivera **Tillåt användare att lägga till interna utgåvor** när du definierar utgivningsinställningar för projektet innan du kan lägga till utleveranser i projektet eller aktiviteterna. Mer information om hur du konfigurerar probleminställningar för ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

När du snabbt vill lägga till flera problem kan du skapa problem för en uppgift eller ett projekt genom att lägga till dem i en lista med problem.

>[!NOTE]
>
>När du lägger till fel i dokumentet använder Workfront inte formuläret Nytt problem för de nya utgåvorna. Vi rekommenderar inte att du infogar fel om du vill att användarna ska ange viss information när de anger problem. Detta kan ha en negativ inverkan på problemrapporteringen och senare på möjligheten för användaren som är tilldelad problemet att ha all information som krävs för att lösa problemet.

Så här skapar du interna utgåvor:

1. Gå till ett projekt där du vill skapa problemet.
1. (Valfritt) Om du vill logga problemet för en uppgift går du till **Uppgifter** och klicka sedan på namnet på en uppgift.
1. Klicka på **Problem** -avsnitt.
1. Klicka **Lägg till fler problem**.

   En ny rad skapas i listan med problem i avsnittet Problem.

   >[!TIP]
   >
   >Det här alternativet är nedtonat om inställningen Tillåt användare att lägga till interna utgåvor är avmarkerad i rutan Redigera projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

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

Mer information om hur du ställer in projekt som frågeköer för att ta emot problem finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Mer information om hur du skickar begäranden finns i [Skapa och skicka Adobe Workfront-förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).

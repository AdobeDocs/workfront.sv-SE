---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Begär åtkomst till objekt
description: Din synlighet för objekt i Adobe Workfront beror på din åtkomst till den typen av objekt samt dina behörigheter för ett enskilt objekt.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---

# Begär åtkomst till objekt

Din synlighet för objekt i Adobe Workfront beror på din åtkomst till den typen av objekt samt dina behörigheter för ett enskilt objekt.

>[!NOTE]
>
>I den här artikeln beskrivs hur du kan begära behörigheter för alla objekt utom för planer i Adobe Workfront Scenario Planner. Information om hur du begär åtkomst till planer finns i [Begär åtkomst till en plan i scenarioplanen](../../scenario-planner/request-access-to-plan.md). Detta kräver ytterligare en licens.

Din Workfront-administratör konfigurerar din åtkomst till en typ av objekt på din åtkomstnivå. Mer information finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Om du behöver behörighet för specifika objekt i Workfront kan du begära åtkomst till dem. I stället för att skicka e-post till Workfront-administratören eller objektägaren för att förklara dina behov kan du begära ytterligare åtkomst (eller behörigheter) inom Workfront.

Du kan begära inledande åtkomst till objekt om någon delar en länk till objektet med dig eller om du kan begära ytterligare åtkomst till objekt som du åtminstone kan visa.

Du kan till exempel ha behörigheten Visa i ett projekt, men du måste lägga till uppgifter i det projektet. I så fall kan du begära Contribute-behörigheter för projektet.

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Du måste ha följande för att kunna dela objekt:

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
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller högre till objekt som du begär behörighet till</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förstå standarddelningsregler

Följande standarddelningsregler träder i kraft automatiskt när de ställs in som standardalternativ i ditt Workfront-system. 

* Användare som tilldelats en uppgift eller ett problem har Contribute-åtkomst. 
* Projekt-, Portfolio- och programhanterare har behörigheten Hantera för de objekt de äger.
* Användare som ingår i en konversation har åtkomst till Visa på objektet där konversationen sker.
* Användare som tilldelats som godkännare har åtkomst till Visa på det objekt som väntar på godkännande.
* När du delar en kontrollpanel delas även alla rapporter på kontrollpanelen med samma åtkomst till samma användare. 
* Objektägare kan inte utöka åtkomsten till ett objekt utanför sin åtkomst till det objektet enligt administratörens definition.

## Begär åtkomst

Du kan begära inledande åtkomst till objekt som du för närvarande inte har åtkomst till eller begära ytterligare åtkomst till objekt som du bara har begränsad åtkomst till.

* [Begär initial åtkomst](#request-initial-access)
* [Begär ytterligare åtkomst](#request-additional-access)

### Begär initial åtkomst  {#request-initial-access}

Om du inte redan har åtkomst till ett objekt och navigerar till det objektet från en länk, visas en skärm som talar om att du inte har tillgång till informationen.  

Så här begär du inledande åtkomst till ett objekt:

1. Klicka **Begär åtkomst**.\
   The **Begär åtkomst** visas.

1. (Villkorligt) Om fler än en användare har behörighet att ge dig ytterligare åtkomst visas en nedrullningspil bredvid användarens namn. 
1. Välj den användare i listrutan som du vill ska få din åtkomstbegäran.\
   Endast 10 användare visas i listrutan. Listan sorteras i bokstavsordning.\
   Mer information om ordningen för användarna i den här listrutan finns i  [Hierarki för de nedrullningsbara menyerna Begär åtkomst och Begär mer åtkomst](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Välj den typ av åtkomst du begär i listrutan.
1. (Valfritt) I dialogrutan **P.S.** anger du en anteckning till användaren om varför du behöver ytterligare åtkomst.

   ![](assets/request-access-dialog-350x314.png)

Om du inte har åtkomstnivåbehörighet för ett objekt och du försöker få åtkomst till det från en länk, visas en skärm som talar om för dig att du ska kontakta Workfront-administratören. 

Om du t.ex. inte har portföljåtkomst, men fått en länk till en portfölj, visas följande meddelande:\
![](assets/permission-request-initial2-350x96.png)

### Begär ytterligare åtkomst {#request-additional-access}

Så här begär du ytterligare åtkomst till ett objekt som du redan har begränsad åtkomst till:

1. Gå till objektet som du vill begära ytterligare åtkomst för.

1. Klicka på **Mer** inline with the project name, then click **Begär mer åtkomst**.\
   ![](assets/request-access-in-project-350x201.png)

1. (Villkorligt) Om fler än en användare har behörighet att ge dig ytterligare åtkomst visas en nedrullningspil bredvid användarens namn.
1. Välj den användare i listrutan som du vill ska få din åtkomstbegäran.\
   Endast 10 användare visas i listrutan. Listan sorteras i bokstavsordning.\
   Mer information om ordningen för användarna i den här listrutan finns i  [Hierarki för de nedrullningsbara menyerna Begär åtkomst och Begär mer åtkomst](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Välj den åtkomstnivå du begär i listrutan.
1. (Valfritt) I dialogrutan **P.S.** anger du en anteckning om varför du behöver ytterligare åtkomst.
1. Klicka **Begär åtkomst**.\
   ![](assets/request-access-dialog-350x314.png)

## Hierarki för de nedrullningsbara menyerna Begär åtkomst och Begär mer åtkomst {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Förstå hierarkin för användare som listas i listrutorna Begär åtkomst och Begär mer åtkomst](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Förstå objektets ägare](#understand-the-owner-of-an-object)

### Förstå hierarkin för användare som listas i listrutorna Begär åtkomst och Begär mer åtkomst {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

När du fyller i listorna Begär åtkomst eller Begär mer åtkomst på objekt, väljer Workfront en lista med upp till tio användare som uppfyller olika roller vid delning av objektet enligt beskrivningen nedan. Dessa användare kan ge åtkomst till objektet till den användare som begär det.\
Resultatlistan sorteras sedan efter namn i stigande alfabetisk ordning.\
Workfront visar upp till 10 användare i listorna Begär åtkomst och Begär mer åtkomst. 

Användarnas ordning i listrutorna Begär åtkomst eller Begär mer åtkomst bestäms av följande regler: 

* Den första användaren i listan är objektet &quot;owner&quot;, vilket beskrivs i [Förstå objektets ägare](#understand-the-owner-of-an-object). 
* Därefter fylls listan i med användare som objektet delas individuellt med. De visas i alfabetisk ordning.
* Listan fylls sedan i ytterligare med användare som får den åtkomst de behöver genom att dela med sina team, grupper eller företag. De visas i alfabetisk ordning.
* Om listan är tom läggs Workfront-administratörerna till så att det alltid finns någon att begära åtkomst från. De visas i alfabetisk ordning. 
* Var och en av användarna i listan måste ha den begärda åtkomsten till objektet och åtkomsten för att kunna dela objektet. 

### Förstå objektets ägare {#understand-the-owner-of-an-object}

Ägaren till ett objekt definieras så här:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objekt</strong> </th> 
   <th><strong>Definition av objektets ägare</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt</td> 
   <td>Ägaren är projektägaren eller, om den saknas eller inte har nödvändig åtkomst, ägaren till den överordnade portföljen. <p>De är kanske inte samma person som den som skapat projektet. </p></td> 
  </tr> 
  <tr> 
   <td>Uppgifter</td> 
   <td>Ägaren är den primära uppdragstagaren eller, om den saknas eller inte har nödvändig åtkomst, ägaren av det projekt där aktiviteten finns, enligt definitionen ovan. <p>De är kanske inte samma person som den som har skapat uppgiften. </p></td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td> <p>Ägaren är den primära kontakten för problemet eller, om det saknas eller om de inte har nödvändig åtkomst, ägaren till det projekt där problemet finns, enligt definitionen ovan. </p> <p>De är kanske inte samma person som den som skapade utgåvan. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Ägaren är Portfolio-ägaren. <p>De är kanske inte samma person som den som har skapat portföljen. </p></td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td>Ägaren är ägaren till dokumentet (den användare som överförde dokumentet) eller, om det saknas eller om de inte har nödvändig åtkomst, ägaren till det objekt som dokumentet finns på.</td> 
  </tr> 
  <tr> 
   <td>Rapporter och kontrollpaneler</td> 
   <td>Ägaren är skaparen, rapporten eller kontrollpanelen. </td> 
  </tr> 
  <tr> 
   <td>Kalendrar</td> 
   <td>Ägaren är den som har skapat kalendern. Alla användare har som standard en kalender tilldelad dem. De betraktas som ägare av den kalendern. </td> 
  </tr> 
  <tr> 
   <td>Filter, vyer och grupperingar</td> 
   <td>Ägaren till ett filter, en vy eller en gruppering är skaparen. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Planer</span> </td> 
   <td> <p><span>Ägaren är planens skapare.</span> </p> <p>Detta kräver ytterligare en licens. </p> <p><span>Mer information om Workfront Scenario Planner finns i</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Översikt över scenarioplanen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Mål</td> 
   <td> <p>Ägaren är den användare som anges som ägare. De kanske inte är samma person som målskaparen. </p> <p>Detta kräver ytterligare en licens. </p> <p>Mer information om Workfront-mål finns på <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Översikt över Adobe Workfront-mål</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

 

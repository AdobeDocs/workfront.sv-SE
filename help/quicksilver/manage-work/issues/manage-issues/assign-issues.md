---
product-area: projects
navigation-topic: manage-issues
title: Tilldela ärenden
description: Du kan tilldela utgåvor till användare, roller och team för att ange vem som ansvarar för att slutföra utgåvorna. Allmän information om hur du tilldelar problem finns i Ändra problemtilldelningar - översikt.
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 0%

---

# Tilldela ärenden

<!--keep the rate card job role information always in yellow till it releases to production - check with Lisa - this might not apply to issues?! -->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba versioner finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Mer information om den aktuella versionen finns i [Översikt över utgåvan för tredje kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Du kan tilldela utgåvor till användare, roller och team för att ange vem som ansvarar för att slutföra utgåvorna. Allmän information om hur du tilldelar problem finns i [Översikt över ändring av utgivningstilldelningar](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
>
>Om en användare, en jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
>
>* Tilldela om arbetsuppgiften till aktiva resurser.
>* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.

Utöver den här artikeln rekommenderar vi att du läser följande artiklar för mer information om hur du tilldelar problem:

* [Översikt över ändring av utgivningstilldelningar](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Ändra användartilldelningar för flera utgåvor i en lista](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Skapa avancerade uppdrag](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Gör smarta uppdrag](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Översikt över tilldelning av arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Du kan tilldela en utgåva till en eller flera resurser på en enskild utgåva eller tilldela flera resurser till flera utgåvor samtidigt.

Att tilldela ärenden och uppgifter är detsamma som i Adobe Workfront. Allmän information om hur du tilldelar uppgifter finns i [Översikt över ändring av uppgiftstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller öka åtkomsten till projekt och uppgifter</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till problem på din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Bevilja åtkomst till utleveranser</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p>Contribute-behörigheter för det objekt där du kopierar problemet med möjlighet att lägga till problem.</p> <p> Information om hur du beviljar behörigheter för problem finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett ärende </a></p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Bevilja åtkomst för användare</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Överväganden för flera tilldelningar till jobbroller, team och användare

Tänk på följande när du tilldelar flera resurser till en arbetsuppgift:

* Användare kan ha mer än en jobbroll kopplad till sin profil. Mer information om hur du associerar användare med jobbroller finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Uppgifter eller ärenden tilldelas vanligtvis först till en eller flera jobbroller eller team. När projekten är klara att starta kan de behöva tilldelas användare.

  Om en uppgift eller ett ärende tilldelas till en eller flera roller och du sedan även tilldelar en användare, bestämmer Adobe Workfront vilken jobbroll som ska associeras med den andra användaren (om någon) enligt följande regler:

   * Om det bara finns en tilldelad jobbroll och den matchar användarens primära roll, tilldelas uppgiften eller utgåvan endast den användare som fyller sin primära roll.
   * Om det finns flera roller tilldelade och minst en av rollerna matchar användarens sekundära roller, tilldelas uppgiften eller utgåvan till användaren som uppfyller en av deras övriga roller - som Workfront väljer slumpmässigt om det finns flera matchningar - samt eventuella ytterligare roller som tilldelas.
   * Om det finns en eller flera jobbroller tilldelade och det inte finns några matchningar mot användarens roller, tilldelas uppgiften eller utgåvan till både rollen eller rollerna och till användaren.

* Om en uppgift eller ett problem har tilldelats ett team och du även tilldelar en användare, förblir uppgiften eller utgåvan tilldelad till både teamet och användaren.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Tilldela en utgåva

1. Gå till ett ärende som du vill tilldela.
1. Klicka **Tilldela till** i det övre högra hörnet av utgåvans rubrik, i **Uppdrag** area

   eller

   Klicka på namnet på de aktuella tilldelningarna, om utgåvan redan har tilldelats.

   ![Knappen Tilldela till](assets/assign-to-button-in-header.png)

1. Gör något av följande:

   * Börja skriva namnet på en användare, roll eller team som du vill tilldela och klicka sedan på den när den visas i listan.

     Exempelbild i produktionsmiljön:
     ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

     <span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
     <span class="preview">![Uppdragssökning](assets/smart-assignments-issue-header.png)</span>

   * (Villkorligt) Klicka på ett av namnen, rollerna eller teamen i de tillgängliga listorna
   * Klicka **Tilldela mig** tilldela den till dig själv
   * Klicka **Avancerat**.

     Att skapa avancerade uppdrag fungerar ungefär på samma sätt för uppgifter och ärenden. Mer information om avancerade uppdrag finns i [Skapa avancerade uppdrag](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn.
     >
     >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
     >
     >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- not sure if this applies to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Klicka **Spara** för att slutföra tilldelningen av problemet.
1. (Valfritt) Klicka på **X-ikon** bredvid namnet på tilldelningarna i uppdragsområdet i huvudet på utgåvan för att ta bort en tilldelning.

## Tilldela en utgåva i en lista

Du kan tilldela utgåvor i en lista eller en rapport när något av uppdragsfälten visas i listvyn. Det här är ett snabbare sätt att tilldela ärenden.

Beroende på vilket fält som visas i vyn kan du tilldela följande enheter till utgåvan:

| Alternativ | Enheter tilldelade |
|---|---|
| **Tilldela till** | Tilldela en användare |
| **Tilldelad** | Tilldela en användare |
| **Uppdrag** | Tilldela användare, jobbroller eller team. |

Så här tilldelar du utgåvor i en lista:

1. Gå till en lista med problem som har fälten Tilldelad, Tilldelad eller Uppdrag i vyn.
1. Gör något av följande om du vill tilldela problem:

   * Klicka inuti **Tilldelad till** eller **Tilldelad** fält och börja skriva namnet på en aktiv användare som du vill tilldela utgåvan och klicka sedan på den när den visas i listan.

     ![](assets/assigned-to-field-task-list-nwe.png)

   * Klicka inuti **Uppdrag** och börja skriva namnet på en aktiv användare, jobbroll eller aktivt team som du vill tilldela till utgåvan och klicka sedan på det när det visas i listan.

     Exempelbild i produktionsmiljön:
     ![](assets/assignments-field-task-list-nwe.png)

     <span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
     ![Uppdragsfält](assets/assignments-field-task-list-0424.png)

   >[!TIP]
   >
   >När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn.
   >
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
   >
   >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. (Villkorligt) Klicka på knappen **Ikonen Personer** ![](assets/teams.png) i det övre högra hörnet av uppdragsrutan för att öppna rutan Avancerade uppdrag och skapa avancerade uppdrag. Mer information finns i [Skapa avancerade uppdrag](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Du kan inte göra avancerade uppdrag från fälten Tilldelad till eller Tilldelad.

1. När du har lagt till dina tilldelningar till problemet trycker du på Enter eller klickar någonstans på sidan för att spara ändringarna.

## Tilldela flera utgåvor samtidigt

1. Gå till en lista över problem som du vill tilldela gruppvis.
1. Markera flera problem i listan.
1. Klicka på **Ikonen Redigera** ![](assets/qs-edit-icon.png).

   The **Redigera problem** öppnas.

1. I **Uppdrag** markerar du **Tilldelad** börjar du sedan skriva namnet på en användare, en jobbroll eller ett team som du vill tilldela till alla utgåvor.

   >[!IMPORTANT]
   >
   >Om något av problemen redan har tilldelats läggs de resurser du anger här till i problemen i stället för att ersätta de befintliga resurserna i problemen.

1. (Valfritt) Markera alternativknappen i dialogrutan **Ärendeägare** kolumn som anger vilken resurs som är den primära tilldelaren eller ägaren av utgåvan när du tilldelar mer än en resurs till utgåvan. Detta är inte tillgängligt för team.
1. (Valfritt) Välj en roll som användaren ska fylla i problemet från **Välj en roll** nedrullningsbar meny i **Uppdragarens roll** när du tilldelar användare till utgåvor. Om du inte väljer någon roll väljs automatiskt användarens primära roll.

1. (Valfritt) Om du vill ta bort befintliga tilldelningar från alla utgåvor gör du något av följande:

   1. Börja skriva namnet på en användare, roll eller team som du vill ta bort från utgåvan, markera det när det visas i listan och klicka på **Ta bort tilldelad** om du vill lägga till ytterligare tilldelningar som ska tas bort.
   1. Klicka **Ta bort alla befintliga tilldelningar** om du vill ta bort alla tilldelningar från alla markerade utgåvor.

1. Klicka **Spara ändringar**.
1. (Valfritt och villkorligt) När fälten Tilldelad till eller Uppdrag visas i listan med utgåvor klickar du i en av dessa kolumner för ett problem och klickar sedan på **X-ikon** bredvid namnet på en tilldelad som ska ta bort den från utgåvan.

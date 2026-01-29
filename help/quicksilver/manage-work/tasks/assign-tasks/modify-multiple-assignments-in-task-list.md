---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Ändra flera användartilldelningar i en uppgiftslista
description: När du hanterar uppgiftstilldelningar kan du ändra dem samtidigt för flera uppgifter samtidigt genom att använda gruppredigeringsfunktionen i en lista med uppgifter.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4167910f36921e04351190f722ea1e7fac9641c7
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# Ändra flera användartilldelningar i en uppgiftslista

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

När du hanterar uppgiftstilldelningar kan du ändra dem samtidigt för flera uppgifter samtidigt genom att använda gruppredigeringsfunktionen i en lista med uppgifter.

Den här artikeln handlar om att ändra flera användartilldelningar för flera uppgifter i en uppgiftslista. Se även följande artiklar för att ändra uppdrag för flera uppgifter i andra områden:

* Mer information om hur du tilldelar uppgifter med hjälp av belastningsutjämnaren finns i [Översikt över hur du tilldelar arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Mer information om hur du tilldelar en aktivitet till en resurs i en lista finns i [Tilldela uppgifter](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och uppgifter</p> <p>Visa eller ge användare högre åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td>
   <td>Contribute eller högre behörigheter för åtgärderna</td>
  </tr>
 </tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Ändra tilldelningar för flera uppgifter

1. Gå till listan som innehåller de uppgifter där du vill ändra tilldelningar.
1. (Valfritt) Skapa ett filter som endast visar uppgifter som tilldelats den tilldelade personen och som du vill ändra.

   Om ditt projekt till exempel innehåller en viss roll som standardtilldelare för flera uppgifter kan du skapa ett filter som bara visar uppgifter med den rollen som tilldelad. Sedan kan du ersätta rollen med en viss användare.

   Mer information om hur du skapar ett filter finns i [Skapa eller redigera filter](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Om du vill filtrera efter en roll väljer du **Tilldelningsroller** och klickar sedan på **ID**.

   >[!TIP]
   >
   >Använd inte fältet **Tilldelad till**. Detta söker bara efter den primära ägaren för uppgiften i stället för någon av rollerna som kan tilldelas dem.

   eller

   Om du vill filtrera efter en användare väljer du **Tilldelningsanvändare** och klickar sedan på **ID.**

   >[!TIP]
   >
   >Använd inte fältet **Tilldelad till**. Detta söker bara efter den primära ägaren för uppgiften i stället för de användare som kan tilldelas till dem.

1. Markera de uppgifter som du vill ändra uppdrag för och klicka sedan på ikonen **Redigera** ![](assets/edit-icon.png) .

   Redigering av uppdrag i uppgifter varierar beroende på vilken miljö du väljer.

1. (Villkorligt) Om du använder produktionsmiljön för att tilldela uppgifter öppnas rutan **Redigera uppgifter** i den nya versionen. Gör följande i produktionsmiljön:

   1. Gör något av följande om du vill lägga till eller ta bort tilldelningar:

      * Om du vill lägga till tilldelningar börjar du skriva namnet på en tilldelad i fältet **Sök efter personer, roller eller team** och markerar dem sedan när de visas i listan.
      * Klicka på ikonen **x** till höger om namnet om du vill ta bort tilldelningar. Endast tilldelningar som är gemensamma för alla uppgifter visas i listan.
      * Klicka på Tilldela mig om du vill tilldela de markerade uppgifterna till dig själv.

   1. (Villkorligt) Klicka på **Spara** när du använder den nya versionen.

   1. (Valfritt) Klicka på **Byt till gammal upplevelse** längst ned i rutan **Redigera uppgifter**.

      Rutan **Redigera uppgifter** öppnas i den gamla versionen.

   1. (Villkorligt) Gör följande i den gamla versionen för att ändra tilldelningarna:

      1. Gå till avsnittet **Uppdrag**.

         >[!IMPORTANT]
         >
         >Om du tar bort tilldelningar kan detta påverka aktivitetstimmar och allokeringsprocenttal. Mer information finns i avsnittet [Hur borttagning av tilldelningar påverkar aktivitetstimmar och procentsatser för allokering](#how-removing-assignees-affects-task-hours-and-allocation-percentages) i den här artikeln.

      1. Gör något av följande för att lägga till eller ta bort tilldelningar:

         * Så här lägger du till en ny tilldelad:

            1. Välj **Tilldelad** i avsnittet **Uppdrag**.

               Information som är vanlig för alla markerade uppgifter visas. Om samma användare till exempel har tilldelats alla uppgifter visas den användaren i kolumnen **Tilldelning**. Om information inte är vanlig för de markerade aktiviteterna visas ingen information.

            1. Börja skriva namnet på en användare, roll eller team och markera det sedan när det visas i listan. Uppdraget läggs till och ersätter inte de aktuella tilldelningarna för de markerade aktiviteterna.

           >[!TIP]
           >
           > * Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
           >   
           > * När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem. Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
           > 
           >   Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
           >   
           >     * Tilldela om arbetsuppgiften till aktiva resurser.
           >     * Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.


         * Så här tar du bort enskilda tilldelningar:

            1. Klicka på **X-ikonen** bredvid namnet på den tilldelade personen som du vill ta bort om den tilldelade personen visas i uppdragslistan.

               eller

               (Villkorligt) Om den tilldelade personen som du vill ta bort inte visas i avsnittet Uppdrag eftersom den tilldelade personen endast är tilldelad till vissa av de uppgifter som du har markerat, klickar du på **Ta bort tilldelad** och börjar skriva namnet på den tilldelade personen som du vill ta bort. Klicka sedan på namnet när det visas i listrutan.

         * Så här tar du bort alla befintliga tilldelningar:

            1. Klicka på **Ta bort alla befintliga tilldelningar** och sedan på **Ja, Ta bort alla tilldelningar**.

               Detta tar inte bara bort vanliga tilldelningar (tilldelningar som visas i redigeringsdialogrutan), utan även alla tilldelningar för alla markerade uppgifter.

           Om du tar bort användare från uppgifter kan detta påverka aktivitetstimmar och allokeringsprocentsatser.

           Mer information finns i [Översikt över att ändra aktivitetstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Valfritt) Ändra något av följande alternativ för tilldelningar:

         * (Villkorligt) **Allokering % eller Timmar**: Ange en ny allokeringsprocent eller timmar.

         >[!NOTE]
         >
         >Det här alternativet kan bara ändras om varaktighetstypen är densamma för alla åtgärder som redigeras. När varaktighetstypen är Beräknad arbets- eller insatsstyrd kan du uppdatera allokeringen %. När varaktighetstypen är Enkel kan du uppdatera timarna. Mer information om varaktighetstyp finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >Om fältet är tomt innebär det att värdet är olika för olika åtgärder, men du kan fortfarande ändra det.

         * **Aktivitetsägare**: Välj det här alternativet om du vill att den som tilldelats ska vara ägare av uppgiften för alla åtgärder som redigeras.
         * **Tilldelningens roll**: Välj en roll i listrutan. Om alternativet inte är markerat väljs automatiskt användarens primära roll.

      1. Klicka på **Spara ändringar.**



   1. <span class="preview">(Villkorligt) Om du använder förhandsvisningsmiljön för att tilldela uppgifter öppnas rutan **Redigera uppgifter** . Gör följande i förhandsvisningsmiljön: </span>

      <div class="preview">

      1. Gör något av följande om du vill lägga till eller ta bort tilldelningar:

         * Om du vill lägga till tilldelningar börjar du skriva namnet på en tilldelad i fältet **Sök efter personer, roller eller team** och markerar dem sedan när de visas i listan.

           Den nya tilldelaren läggs till i de befintliga för de valda uppgifterna.
         * Om du vill ta bort tilldelningar klickar du på namnet på en tilldelad i rutan **Ta bort tilldelad**

           eller

           Klicka på **Ta bort alla befintliga tilldelningar**.

           Tilldelningar tas bort från alla markerade uppgifter.

           Om du tar bort användare från uppgifter kan detta påverka aktivitetstimmar och allokeringsprocentsatser.

           Mer information finns i [Översikt över att ändra aktivitetstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).


           >[!TIP]
           >
           >* Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
           >   
           >* När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem. Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
           > 
           >   Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
           >   
           >* Tilldela om arbetsuppgiften till aktiva resurser.
           >* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.


      1. (Valfritt) Ändra något av följande alternativ för tilldelningar:

         * (Villkorligt) **Allokering % eller Timmar**: Ange en ny allokeringsprocent eller timmar.

         >[!NOTE]
         >
         >Det här alternativet kan bara ändras om varaktighetstypen är densamma för alla åtgärder som redigeras. När varaktighetstypen är Beräknad arbets- eller insatsstyrd kan du uppdatera allokeringen %. När varaktighetstypen är Enkel kan du uppdatera timarna. Mer information om varaktighetstyp finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >Om fältet är tomt innebär det att värdet är olika för olika åtgärder, men du kan fortfarande ändra det.

         * **Gör primär**: Håll markören över de markerade aktiviteterna och välj det här alternativet om du vill att den som tilldelats ska vara ägare till uppgiften för alla aktiviteter som redigeras.
         * **Tilldelningens roll**: Välj en roll i listrutan. Om alternativet inte är markerat väljs automatiskt användarens primära roll.
         * **Varaktighetstyp**
         * **Varaktighet**
         * **Planerade timmar**

      1. Klicka på **Spara**.

         </div>






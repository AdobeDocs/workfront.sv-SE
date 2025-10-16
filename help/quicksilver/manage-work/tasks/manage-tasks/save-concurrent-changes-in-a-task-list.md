---
product-area: projects
navigation-topic: manage-tasks
title: Översikt över Spara samtidiga ändringar i en uppgiftslista
description: När du redigerar uppgifter i en lista kan du använda separata inställningar för att ange om du vill att ändringarna ska sparas automatiskt när du redigerar uppgifter i en lista manuellt.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Översikt över att spara samtidiga ändringar i en uppgiftslista

När du redigerar uppgifter i en lista kan du använda separata inställningar för att ange om du vill att ändringarna ska sparas automatiskt när du redigerar uppgifter i en lista manuellt.

Mer information om hur du redigerar uppgifter i en uppgiftslista finns i artikeln [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Ibland kan konflikter uppstå om två användare gör ändringar för samma uppgifter.

Tänk på följande när du redigerar uppgifter i en uppgiftslista:

* Adobe Workfront sparar ändringarna direkt när du väljer att spara ändringarna automatiskt om projektets uppdateringstyp är Automatisk eller Automatisk eller Vid ändring. Mer information om projektets uppdateringstyp finns i [Välj projekttyp](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront uppdaterar informationen i listan som du arbetar med varje minut med ändringar som andra användare kan göra var som helst i systemet. På så sätt får du alltid den senaste informationen om uppgifterna.

Följande scenarier gäller när flera användare redigerar samma uppgifter:

* **En användare sparar ändringarna i en uppgiftslista automatiskt och en annan manuellt**: Om en användare (Användare A) sparar ändringarna manuellt medan Användare B redigerar samma uppgifter, men de sparar sina ändringar automatiskt, uppdateras de ändringar som görs av Användare B i listan för Användare A varje minut. Om det finns konflikter mellan de ändringar som gjorts av de två användarna visas ett varningsmeddelande när användaren sparar manuellt (Användare A) innan ändringarna kan sparas. Varningsmeddelandet visar de objekt som har ändringskonflikter. Användaren A kan nu välja om han eller hon vill behålla sina ändringar (som skriver över de ändringar som gjorts av Användare B) eller ignorera dem (vilket gör att Användare B behåller ändringarna)

>[!NOTE]
>
>När du väljer att ignorera de ändringar du har gjort gäller detta alla ändringar och inte bara de som står i konflikt med en annan användares redigeringar.

* **Flera användare sparar ändringarna i en uppgiftslista manuellt**: Om flera användare gör ändringar i uppgifter i en lista manuellt samtidigt, sparar Workfront ändringarna som gjorts av den användare som sparar först. Inga konflikter uppstår när du sparar dessa ändringar. I Workfront jämförs de ändringar som gjorts av alla andra användare med den information som redan har sparats, och en varning om vilka ändringar som är i konflikt visas för de andra användarna innan de kan spara sin information.

>[!IMPORTANT]
>
>När du väljer att behålla ändringarna för alla andra ändringar sparas alla ändringar, såvida inte de uppgifter du har gjort har tagits bort av en annan användare. I det här fallet visas ett varningsmeddelande om att de ändringar du har gjort i de borttagna uppgifterna går förlorade.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->

---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Översikt över ändring av uppgiftstilldelningar
description: Du kan tilldela uppgifter till eller ta bort tilldelning från användare, team eller jobbroller. Du kan tilldela flera resurser samtidigt, eller bara en resurs. Du kan tilldela en uppgift åt gången eller flera uppgifter samtidigt.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Översikt över ändring av uppgiftstilldelningar

Du kan tilldela uppgifter till eller ta bort tilldelning från användare, team eller jobbroller. Du kan tilldela flera resurser samtidigt, eller bara en resurs. Du kan tilldela en uppgift åt gången eller flera uppgifter samtidigt.

>[!TIP]
>
>Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
>
>Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
>
>* Tilldela om arbetsuppgiften till aktiva resurser.
>* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.
>


Den här artikeln innehåller allmän information om effekten av att ändra uppgiftstilldelningar. Mer information om hur du tilldelar uppgifter finns i följande artiklar:

* Mer information om hur du tilldelar uppgifter finns i [Tilldela uppgifter](../../../manage-work/tasks/assign-tasks/assign-tasks.md) och [Ändra flera användartilldelningar i en uppgiftslista](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Mer information om hur du ändrar tilldelningar för flera aktiviteter i schemaläggningsområdet finns i&quot;Ändra flera användartilldelningar för aktiviteter i schemaläggningsområdena&quot;.
* Mer information om hur du tilldelar uppgifter med hjälp av belastningsutjämnaren finns i [Översikt över tilldelning av arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Viss information i den här artikeln gäller även för uppdrag i ärenden. Mer information om hur du tilldelar problem och andra överväganden finns i [Ändra översikt över utleveranstilldelningar](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## När användartilldelningar ska ändras för uppgifter

Du kan ändra användartilldelningarna för uppgifter av olika anledningar, bland annat följande:

* Användarna går med eller lämnar teamet
* En användare tar en semester som sträcker sig längre än förfallodatum för uppgifter

   >[!NOTE]
   >
   >När du tilldelar användare arbetsuppgifterna påverkar tillgängligheten enligt deras scheman de planerade och planerade datumen för uppgifterna. Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* En specifik roll eller användare anges som tilldelad för flera uppgifter och du vill snabbt ändra alla objekt som ska tilldelas till en annan användare eller roll

## Överväganden för flera tilldelningar till jobbroller, team och användare

Tänk på följande när du tilldelar flera resurser till en arbetsuppgift:

* Användare kan ha mer än en jobbroll kopplad till sin profil. Mer information om hur du associerar användare med jobbroller finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Uppgifter eller ärenden tilldelas vanligtvis först till en eller flera jobbroller eller till ett team. När projekten är klara att starta kan de behöva tilldelas användare.\
   Om en uppgift eller ett ärende tilldelas till en eller flera roller och du sedan även tilldelar en användare, bestämmer Adobe Workfront vilken jobbroll som ska associeras med den andra användaren (om någon) enligt följande regler:

   * Om det bara finns en tilldelad jobbroll och den matchar användarens primära roll, tilldelas uppgiften eller utgåvan endast den användare som fyller sin primära roll.
   * Om det finns flera roller tilldelade och minst en av rollerna matchar användarens sekundära roller, tilldelas uppgiften eller utgåvan till användaren som uppfyller en av deras övriga roller - som Workfront väljer slumpmässigt om det finns flera matchningar - samt eventuella ytterligare roller som tilldelas.
   * Om det finns en eller flera jobbroller tilldelade och det inte finns några matchningar mot användarens roller, tilldelas uppgiften eller utgåvan till både rollen eller rollerna och till användaren.

* Om en uppgift eller ett problem har tilldelats ett team och du även tilldelar en användare, förblir uppgiften eller utgåvan tilldelad till både teamet och användaren.

## Hur borttagning av tilldelningar påverkar aktivitetstimmar och allokeringsprocent

Borttagning av användare kan påverka aktivitetstimmar och allokeringsprocentsatser. Vilken effekt en användare har på aktiviteten beror på vilken typ av varaktighet som har valts för uppgiften. Mer information om varaktighetstyp finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

När du tar bort en användare från en uppgift med följande varaktighetstyper:

* **Enkelt:** De planerade timmar som tilldelats den användaren subtraheras från aktivitetens totala planerade timmar.

   >[!IMPORTANT]
   >
   >Detta kan påverka projektplanen negativt eftersom det ändrar det totala antalet planerade timmar för aktiviteten och projektet.

* **Ansträngningsstyrd:** Allokeringsprocenten ändras inte för andra användare.
* **Beräknad tilldelning:** Allokeringsprocenten för andra användare justeras så att summan motsvarar 100 %.
* **Beräknat arbete:** Allokeringsprocenten ändras inte för andra användare.

## Att tänka på när du frigör tilldelningar av uppgifter

Du kan ta bort uppdrag från en uppgift i taget eller ta bort uppdrag från flera uppgifter samtidigt.

Mer information om hur du tar bort uppdrag från gruppaktiviteter finns i [Ändra flera användartilldelningar i en uppgiftslista](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Tänk på följande när du tar bort tilldelningar från uppgifter:

* När du tar bort tilldelningen för en användare från en uppgift förblir uppgiften tilldelad till den jobbroll som användaren utförde i uppgiften.
* När du tar bort tilldelningen för en jobbroll eller ett team från en uppgift, förblir uppgiften inte tilldelad om den inte har tilldelats till några andra resurser.

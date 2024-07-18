---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Översikt över projektägare och sponsorer
description: Du kan ange en projektägare och en projektsponsorer för ett projekt.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 111c776af19fbc2982c14cc9d3b3778d37bc0be3
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Översikt över projektägare och sponsorer

<!-- Audited: 1/2024 -->

Du kan ange en projektägare och en projektsponsorer för ett projekt.

Projektägaren är den person som ansvarar för att projektet slutförs i tid och i budget.

Projektsponsorn är en viktig intressent för det projekt som har resurser som investerats i projektet. Projektets slutförande är vanligtvis till nytta för projektsponsorn.

Mer information om hur du uppdaterar projektägaren eller sponsorn för ett projekt finns i [Uppdatera projektägare och sponsorer](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Projektägare

Du kan utse projektledare genom att ange en projektägare för ett projekt eller en mall.

Du kan bara definiera en projektägare för ett projekt.

Du kan använda fältet Projektägare till följande:

* Du kan bara ange en användare som projektägare.
* Du kan ange Projektägare som timmergodkännare för projektet.
* Du kan ange projektägaren som en allmän godkännare när du definierar projekt-, uppgifts- eller godkännandeprocesser. Mer information om godkännanden finns i [Redigera en godkännandeprocess](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >När du tilldelar projektägaren ett godkännande och ingen utses till projektägare tilldelas godkännandet till Workfront huvudadministratör enligt anvisningarna i avsnittet Kundinformation i inställningsområdet. Mer information finns i [Konfigurera grundläggande information för systemet](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >


* Du kan aktivera vissa meddelanden som bara skickas till projektägaren.

  Mer information om e-postmeddelanden finns i avsnittet [Konfigurera händelsemeddelanden för alla i systemet](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) i artikeln [Konfigurera händelsemeddelanden för alla i systemet](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Du kan visa fältet Projektägare i en rapport eller lista.

  Du kan även visa fältet Projektägare i en vy, gruppering eller fråga.

  Du kan till exempel kopiera följande textlägesuttryck till ett filter för att visa projekt som ägs av den inloggade användaren: 

  ```
  ownerID=$$USER.ID
  ```

Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Projektsponsorer

Du kan utse valfri användare i systemet till projektsponsor. Projektsponsorn är vanligtvis en chef, en chef eller en berörd part som behöver veta vad som händer med projektet.

Tänk på följande när du tilldelar en projektsponsor:

* Projektsponsorn får ingen ytterligare åtkomst till projektet, men läggs till i e-postmeddelandena för projektet. Mer information om meddelanden finns i artikeln [Konfigurera händelsemeddelanden för alla i systemet](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Du kan bara utse en projektsponsorer.
* Du kan ange projektsponsorn som en allmän godkännare när du definierar projekt-, uppgifts- eller godkännandeprocesser. Mer information om godkännanden finns i [Redigera en godkännandeprocess](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >När du tilldelar ett godkännande till projektsponsorn och ingen utses till projektledare tilldelas godkännandet till projektägaren. Om ingen har utsetts till projektägare tilldelas Workfront-administratören godkännandet.

* Du kan visa fältet Projektsponsorer i en rapport eller lista.

  Du kan även visa fältet Projektsponsorer i en vy, gruppering eller en fråga.

  Du kan till exempel kopiera följande textlägesuttryck till ett filter för att visa projekt som sponsras av den inloggade användaren:

  ```
  sponsorID=$$USER.ID
  ```

   

  Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

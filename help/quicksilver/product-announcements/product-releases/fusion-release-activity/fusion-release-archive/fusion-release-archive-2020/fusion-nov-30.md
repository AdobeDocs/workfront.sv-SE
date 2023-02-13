---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: fusion
navigation-topic: fusion-release-activity
title: '''Workfront Fusion-lanseringsaktivitet: Vecka 30 november 2020"'
description: Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 30 november 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Versionsaktivitet för Workfront Fusion: 30 november 2020

Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 30 november 2020.

En lista med alla senaste ändringar finns på [Versionsaktivitet för Adobe Workfront Fusion](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

En lista med de senaste felkorrigeringarna i Workfront Fusion finns i [Workfront Maintenance Updates](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) och sök efter uppdateringar som heter Workfront Fusion Maintenance Update.

## Hastighetsgräns för Workfront Fusion 2.0-webbhooks.

Vi har introducerat ett nytt prestandaresäkerhetsskydd för Workfront Fusion 2.0. Nu har webhooks en hastighetsbegränsning på 100 förfrågningar per sekund. När denna gräns har nåtts skickar Workfront Fusion 2.0 en 429-status (för många begäranden).

Tidigare var webkrok-begäranden inte begränsade.

Mer information finns i [Adobe Workfront Fusion - prestandaräknare](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Lägga till ett anpassat formulär i ett Workfront-objekt i Workfront Fusion 2.0

För att du ska kunna lägga till anpassade formulär till objekt är Workfront Fusion 2.0, har vi lagt till en AssignCategories-åtgärd i Workfront > Misc. Åtgärdsmodul.

Tidigare var det inte möjligt att använda en Workfront Fusion 2.0-modul för att lägga till ett anpassat formulär i ett objekt i Workfront.

Mer information om Workfront > Div. Åtgärdsmodul, se [Adobe Workfront-moduler](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->

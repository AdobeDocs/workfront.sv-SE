---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Konfigurera begärandetyper
description: När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en viss uppgift. Du kan också skicka begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö. Problem och förfrågningar anses vara utbytbara i Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Konfigurera begärandetyper

När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en viss uppgift. Du kan också skicka begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö. Problem och förfrågningar anses vara utbytbara i Adobe Workfront.

Mer information om hur du skapar problem i [!DNL Workfront], se [Skapa problem](../../../manage-work/issues/manage-issues/create-issues.md). Mer information om hur du skapar begäranden i [!DNL Workfront], se [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md). Mer information om hur du associerar frågetyper med projekt finns i [Definiera frågetyper för ett projekt](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Anpassa namnen på förfrågningstyperna

Som [!DNL Workfront] kan du konfigurera namnen på förfrågningstyperna i systemet. De nya namnen visas i alla områden i [!DNL Workfront] där **[!UICONTROL Issue Type]** eller **[!UICONTROL Request Type]** visas fält:

* I **[!UICONTROL Queue Details]** del av ett projekt som ska ta emot utleveranser eller förfrågningar.
* Om mer än en frågetyp har valts för en frågekö går du till **[!UICONTROL New Issue]Formulär** i **[!UICONTROL Issue Type]** när du skapar ett nytt problem eller skickar en ny begäran.

   Mer information om hur du skapar problem i [!DNL Workfront], se  [Skapa problem](../../../manage-work/issues/manage-issues/create-issues.md)

   Mer information om hur du skapar begäranden i [!DNL Workfront], se  [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).

* På **[!UICONTROL Queue Topic Detail]** när du konfigurerar köämne.\
   Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Så här anpassar du namnen på begärandetyperna:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]**.

1. Klicka på **[!UICONTROL Issues]** -fliken.
1. Överst på **[!UICONTROL Issues]** hovra över namnet på en frågetyp och klicka sedan på **[!UICONTROL Edit]** -ikon som visas.

   ![](assets/edit-request-type-name-nwe.png)

1. Skriv ett nytt namn i rutan som visas och tryck sedan på **[!UICONTROL Enter]**.

## Konfigurera utgivningsstatus i olika typer av förfrågningar

Du kan associera varje begärandetyp med olika utgivningsstatus. Du kan också ändra i vilken ordning statusvärdena visas för ett problem, beroende på vilken typ av problem det är.

Mer information om hur du ändrar standardordningen för utgivningsstatus och konfigurerar utgivningsstatus finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) avsnitt i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

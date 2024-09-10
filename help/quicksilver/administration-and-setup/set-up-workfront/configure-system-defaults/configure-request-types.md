---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Konfigurera frågetyper
description: När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en viss uppgift. Du kan också skicka begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö. Problem och förfrågningar anses vara utbytbara i Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Konfigurera begärandetyper

När du arbetar med ett projekt kanske du upptäcker att oväntade händelser inträffar. Du kan logga oväntade händelser som problem för ett visst projekt eller en viss uppgift. Du kan också skicka begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö. Problem och förfrågningar anses vara utbytbara i Adobe Workfront.

Mer information om hur du skapar problem i [!DNL Workfront] finns i [Skapa problem](../../../manage-work/issues/manage-issues/create-issues.md). Mer information om hur du skapar begäranden i [!DNL Workfront] finns i [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md). Mer information om hur du associerar frågetyper med projekt finns i [Definiera frågetyper för ett projekt](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

Som [!DNL Workfront]-administratör kan du konfigurera namnen på förfrågningstyperna i systemet. De nya namnen visas i alla områden i [!DNL Workfront] där fälten **[!UICONTROL Issue Type]** eller **[!UICONTROL Request Type]** visas:

* I området **[!UICONTROL Queue Details]** i ett projekt som ska ta emot problemen eller förfrågningarna.
* Om du har valt mer än en frågetyp för en frågekö, i **[!UICONTROL New Issue]Formulär** i fältet **[!UICONTROL Issue Type]**, när du skapar ett nytt problem eller skickar en ny begäran.

  Mer information om hur du skapar problem i [!DNL Workfront] finns i [Skapa problem](../../../manage-work/issues/manage-issues/create-issues.md)

  Mer information om hur du skapar begäranden i [!DNL Workfront] finns i [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).

* När du konfigurerar köämnet i formuläret **[!UICONTROL Queue Topic Detail]**.\
   Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Så här anpassar du namnen på begärandetyperna:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]**.

1. Klicka på fliken **[!UICONTROL Issues]**.
1. Överst på fliken **[!UICONTROL Issues]** håller du muspekaren över namnet på en frågetyp och klickar sedan på ikonen **[!UICONTROL Edit]** som visas.

   ![](assets/edit-request-type-name-nwe.png)

1. Skriv ett nytt namn i rutan som visas och tryck sedan på **[!UICONTROL Enter]**.

## Konfigurera utgivningsstatus i olika typer av förfrågningar

Du kan associera varje begärandetyp med olika utgivningsstatus. Du kan också ändra i vilken ordning statusvärdena visas för ett problem, beroende på vilken typ av problem det är.

Mer information om hur du ändrar standardordningen för utgivningsstatus och konfigurerar utgivningsstatus finns i avsnittet [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

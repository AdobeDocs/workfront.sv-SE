---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Lägga till en användare i en organisation i Adobe Workfront Fusion
description: Du kan lägga till användare i organisationer i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 447ab70566d5f9de3bc368933c9efdb94d2b9e7e
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Lägga till en användare i en organisation i Adobe Workfront Fusion

>[!IMPORTANT]
>
>Den procedur som beskrivs på den här sidan gäller endast för organisationer som ännu inte har anslutit till [!DNL Adobe Admin Console]. Om din organisation har anslutit sig till [!DNL Adobe Admin Console] måste du utföra den här åtgärden via [!DNL Adobe Admin Console].
>
>Instruktioner om hur du lägger till en användare i [!DNL  Adobe Admin Console] finns i avsnittet Redigera användarinformation i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) eller kontakta [!UICONTROL Adobe Admin Console]-administratören.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> 
     <p>Du måste vara administratör för [!DNL Workfront Fusion] för din organisation.</p>
     <p>Du måste vara administratör för [!DNL Workfront Fusion] för ditt team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Lägga till användare i en organisation


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

Om du vill lägga till användare i organisationen måste du vara administratör för den organisation som du vill lägga till användare i. Mer information om roller finns i [Organisationsroller i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Så här lägger du till en användare i organisationen:

1. Navigera till **[!UICONTROL Organizations]** på menyn och markera den organisation du vill lägga till en användare i.
1. Öppna fliken **[!UICONTROL Users]** i din instrumentpanel.
1. Klicka på **[!UICONTROL Invite a new user]**, fyll i formuläret (E-post, Meddelande, Roll) och skicka inbjudan genom att klicka på **[!UICONTROL Send]**.

>[!NOTE]
>
>   
>Om du inte ser knappen [!UICONTROL Invite a new user] har din organisation anslutit till [!DNL Adobe Business Platform.]
>
>  Instruktioner om hur du lägger till en användare i en organisation som har anslutit till [!DNL Adobe Business Platform] finns i [Lägg till användare i [!DNL Adobe Workfront Fusion] via  [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

Användaren får ett e-postmeddelande med en inbjudan där han/hon kan acceptera inbjudan.

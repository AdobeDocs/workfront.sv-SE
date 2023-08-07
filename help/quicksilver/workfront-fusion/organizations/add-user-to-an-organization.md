---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Lägga till en användare i en organisation i Adobe Workfront Fusion
description: Du kan lägga till användare i organisationer i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2884f709ef9ea89f275ff88db41ddde725dbd781
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Lägga till en användare i en organisation i Adobe Workfront Fusion

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till [!DNL Adobe Admin Console]. Om din organisation har anslutit sig till [!DNL Adobe Admin Console]måste du utföra den här åtgärden via [!DNL Adobe Admin Console].
>
>Instruktioner om hur du lägger till en användare i[!DNL  Adobe Admin Console]finns i avsnittet Redigera användarinformation i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) eller kontakta [!UICONTROL Adobe Admin Console] Administratör.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> 
     <p>Du måste vara en [!DNL Workfront Fusion] administratör för din organisation.</p>
     <p>Du måste vara en [!DNL Workfront Fusion] administratör för ditt team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Lägga till användare i en organisation

<p>Hur du lägger till en användare i din Fusion-organisation skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Lägg till en användare i en organisation som har anslutit sig till Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Lägg till en användare i en organisation som inte har anslutit till Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Lägg till en användare i en organisation som har anslutit sig till Adobe Business Platform</strong></p>
<p>Om din organisation har anslutit sig till Adobe Business Platform måste du utföra den här åtgärden via Adobe Admin Console.</p>
<p>Instruktioner om hur du lägger till en användare i Adobe Admin Console:</p>
<ul>
<li> <p>Se <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Skapa användare i Workfront med Adobe Admin Console</a></p> </li>
<li> <p>Se avsnittet"Lägg till användare" i artikeln <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Hantera användare individuellt</a></p> </li>
<li> <p>Kontakta Adobe Admin Console-administratören.</p> </li>
</ul>
<p>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform finns på <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Lägg till en användare i en organisation som inte har anslutit till Adobe Business Console</strong></p>

Om du vill lägga till användare i organisationen måste du vara administratör för den organisation som du vill lägga till användare i. Mer information om roller finns i [Organisationsroller i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Så här lägger du till en användare i organisationen:

1. Navigera till **[!UICONTROL Organizations]** på menyn och välj den organisation som du vill lägga till en användare i.
1. Öppna **[!UICONTROL Users]** i Dashboard.
1. Klicka **[!UICONTROL Invite a new user]** fylla i formuläret (E-post, Meddelande, Roll) och skicka inbjudan genom att klicka på **[!UICONTROL Send]**.

>[!NOTE]
>
>   
><p>Om du inte ser [!UICONTROL Invite a new user] har din organisation gått med på [!DNL Adobe Business Platform.] </p>
>
>   <p>Instruktioner om hur du lägger till en användare i en organisation som har anslutit till [!DNL Adobe Business Platform], se <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Lägg till en användare i en organisation som har anslutit sig till [!DNL Adobe Business Platform]</a></p>

Användaren får ett e-postmeddelande med en inbjudan där han/hon kan acceptera inbjudan.

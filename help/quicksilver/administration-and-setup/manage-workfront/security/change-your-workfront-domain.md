---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Ändra din Adobe Workfront-domän
description: Som Adobe Workfront-administratör och behörig Workfront Support-kontakt kan du begära hjälp från Workfront Support-team för att ändra din organisations Workfront-domän.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Ändra din Adobe Workfront-domän

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om din organisation har anslutit sig till Adobe Admin Console går det inte att ändra din Workfront-domän.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Som Adobe Workfront-administratör och behörig Workfront Support-kontakt kan du begära hjälp från Workfront Support-team för att ändra din organisations Workfront-domän.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begär en domänändring

1. Börja skapa en supportanmälan på Experience League.
1. I rutan **Beskrivning** tar du med den nya domänen som du vill ha samt tidsramen när du vill att den nya domänen ska vara aktiv.
1. Fyll i rutorna för supportärendet och klicka sedan på **Skicka**.

Du kan även ringa Workfront Support och få hjälp med att ändra din domän.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->

---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)
description: Om din organisation har anslutit sig till Adobe Business Platform använder dina användare Adobe Business Platform för att få tillgång till Adobe Workfront. Detta innebär att användarhantering i stor utsträckning sker via Adobe Admin Console och att enkel inloggning (SSO) hanteras via Adobe Business Platform i stället för via Workfront. Som Adobe Workfront-administratör skiljer sig dina administrativa ansvar och procedurer åt beroende på om din organisation har anslutit sig till Adobe Business Platform eller inte. I den här artikeln listas de procedurer som måste hanteras på olika sätt, samt länkar till instruktioner för både Workfront och Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>Alla Workfront-organisationer har nu anslutit sig till Adobe Admin Console.
>
>Den här artikeln kommer att tas bort inom den närmaste framtiden.

Som Adobe Workfront-administratör kan ditt administrationsansvar och dina administrationsprocedurer skilja sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform. I den här artikeln listas de procedurer som hanteras på olika sätt och länkar till instruktioner för både Workfront och Adobe Admin Console.

Om din organisation har anslutit sig till Adobe Business Platform använder dina användare Adobe Business Platform för att få tillgång till Adobe Workfront. Detta innebär att

* Systemadministratörer skapas via Adobe Admin Console
* Att förnya ett SAML-certifikat hanteras via Adobe Admin Console.
* enkel inloggning (SSO) hanteras via Adobe Business Platform i stället för via Workfront

## Skapa Workfront systemadministratörer i Adobe Admin Console

>[!NOTE]
>
>Vi rekommenderar att du lägger till användare som inte är systemadministratörer direkt i Workfront. Det går att lägga till användare i Adobe Admin Console, men om du lägger till dem i Workfront kan du ange åtkomstnivå när du skapar dem, vilket sparar tid.

Mer information om hur du skapar systemadministratörer för Workfront finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/se/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/se/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/se/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## Förnya SAML-certifikatet

Instruktioner om hur du förnyar SAML-certifikatet på Adobe Admin Console finns i avsnittet&quot;Den digitala signaturen i SAML-svaret validerades inte ...&quot; i [Felsökning av Federated ID](https://helpx.adobe.com/se/enterprise/kb/tshoot-fed-id.html).

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/se/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## enkel inloggning (enkel inloggning)

Eftersom Adobe Business Platform styr enkel inloggning (SSO) för användare hanteras följande åtgärder och funktioner automatiskt via Adobe Business Platform. Om din organisation ännu inte har anslutit sig till Adobe Business Platform måste du utföra dessa åtgärder i Workfront.


* [Konfigurera Adobe Workfront med SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Konfigurera Adobe Workfront med SAML 2.0 med ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Inaktivera enkel inloggning i Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Uppdatera SAML 2.0-metadata i identitetsleverantören](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Uppdatera användare för enkel inloggning](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Konfigurera lösenordsprinciper för autentisering](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Konfigurera systemsäkerhetsinställningar](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)

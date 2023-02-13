---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)
description: Om din organisation har anslutit sig till Adobe Business Platform använder dina användare Adobe Business Platform för att få tillgång till Adobe Workfront. Detta innebär att användarhantering i stor utsträckning sker via Adobe Admin Console och att enkel inloggning (SSO) hanteras via Adobe Business Platform i stället för via Workfront. Som Adobe Workfront-administratör skiljer sig dina administrativa ansvar och procedurer åt beroende på om din organisation har anslutit sig till Adobe Business Platform eller inte. I den här artikeln listas de procedurer som måste hanteras på olika sätt, samt länkar till instruktioner för både Workfront och Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)

Om din organisation har anslutit sig till Adobe Business Platform använder dina användare Adobe Business Platform för att få tillgång till Adobe Workfront. Detta innebär att

* Användarhantering sker i stor utsträckning via Adobe Admin Console
* enkel inloggning (SSO) hanteras via Adobe Business Platform i stället för via Workfront

Som Adobe Workfront-administratör skiljer sig dina administrativa ansvar och procedurer åt beroende på om din organisation har anslutit sig till Adobe Business Platform eller inte. I den här artikeln listas de procedurer som måste hanteras på olika sätt, samt länkar till instruktioner för både Workfront och Adobe Admin Console.

## Användare

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtgärd</th> 
   <th>Instruktioner i Workfront finns i</th> 
   <th>Instruktioner i Admin Console i Adobe finns i</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Ge en användare administratörsåtkomst</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet Redigera användarinformation i <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Hantera användare individuellt</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lägga till en användare i Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Lägg till användare</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Hantera användare i Adobe Admin Console</a> </p> </li> 
     <li> <p>Avsnittet"Lägg till användare" i <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Hantera användare individuellt</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Inaktivera en användare</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet"Ta bort användare" i <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Hantera användare individuellt</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ta bort en användare</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Ta bort användare</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet"Ta bort användare permanent" i <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Hantera kataloganvändare</a>
     </p><p>Obs! Ta bort en användare från [!DNL Adobe Admin Console] inaktiverar användaren i [!DNL Workfront], men tar inte bort dem från [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Redigera en användarprofil</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet"Redigera användarinformation" i <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Hantera användare individuellt</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Redigera användarprofiler gruppvis</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Redigera användarprofiler gruppvis</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet Redigera användarinformation i <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Massöverföring av CSV</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importera användare </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importera användare</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet"Lägg till användare" i <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Massöverföring av CSV</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Logga in som en annan användare</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Logga in som en annan användare</a> </p> </li> 
    </ul> </td> 
   <td>Inte tillgängligt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Förnya SAML-certifikat</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Förnya Adobe Workfront SAML 2.0-metadatacertifikatet</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Avsnittet"Den digitala signaturen i SAML-svaret validerade inte...". in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Federated ID Felsökning</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## enkel inloggning (enkel inloggning)

Eftersom Adobe Business Platform styr enkel inloggning (SSO) för användare hanteras följande åtgärder och funktioner automatiskt via Adobe Business Platform. Om din organisation ännu inte har anslutit sig till Adobe Business Platform måste du utföra dessa åtgärder i Workfront.


* [Konfigurera Adobe Workfront med SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Konfigurera Adobe Workfront med SAML 2.0 med ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Inaktivera enkel inloggning i Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Uppdatera SAML 2.0-metadata hos identitetsleverantören](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Uppdatera användare för enkel inloggning](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Konfigurera lösenordsprinciper för autentisering](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Konfigurera säkerhetsinställningar för system](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)

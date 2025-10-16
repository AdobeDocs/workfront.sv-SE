---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: SAML 2.0-autentiseringen misslyckades: Användaridentifieraren hittades inte'
description: När du använder SAML 2.0 innebär felet"SAML 2.0 Authentication Failed-User Identifier Not found" att inget UID- eller NAME-ID skickas från ADFS Claim-reglerna.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Felmeddelande: SAML 2.0-autentiseringen misslyckades: Användaridentifieraren hittades inte

## Problem

Jag får det här felet när jag använder SAML 2.0: &quot;SAML 2.0-autentiseringen misslyckades: Det gick inte att hitta användaridentifieraren.&quot;

## Orsak

Detta inträffar när ett **UID** eller **NAME ID** inte skickas från **ADFS-anspråksreglerna**.

I ADFS måste **förlitande part-förtroende** ha en **anspråksregel** som skickar antingen ett **UID**- eller ett **NAME ID**-värde. När du kör en **[!DNL Workfront]Test Connection** bör den visa detta om den lyckas.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösning

1. När du redigerar **[!UICONTROL ADFS INFO]** går du till **[!UICONTROL Relying Party Trusts]** > Markera objekt >**[!UICONTROL Edit Claim Rules]**.

1. **[!UICONTROL LDAP Attribute]** (vänster kolumn) ska ha **[!UICONTROL E-Mail Addresses]** (eller en unik identifierare).

1. **[!UICONTROL Outgoing Claim Type]** (höger kolumn) ska vara **[!UICONTROL Name ID]**.

   >[!NOTE]
   >
   >Den behöver inte ha LDAP-attributets e-postadresser. Alla unika identifierare som identifierar användaren kan användas, men den måste skickas till [!DNL Adobe Workfront] som **NAME-ID**.

---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: SAML 2.0-autentiseringen misslyckades: Det gick inte att hitta användaridentifieraren'
description: När du använder SAML 2.0 innebär felet"SAML 2.0 Authentication Failed-User Identifier Not found" att inget UID eller NAME ID skickas från ADFS Claim-reglerna. I ADFS måste förlitande part-förtroende ha en anspråksregel som skickar antingen ett UID- eller ett NAME ID-värde. När du kör en  [!DNL Workfront] Test Connection bör den visa detta om den lyckas.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Felmeddelande: SAML 2.0-autentiseringen misslyckades: Användaridentifieraren hittades inte

## Problem

Jag får det här felet när jag använder SAML 2.0: &quot;SAML 2.0-autentiseringen misslyckades: Det gick inte att hitta användaridentifieraren.&quot;

## Orsak

Detta inträffar när ett **UID** eller **NAME ID** inte skickas från **ADFS-anspråksreglerna**.

I ADFS måste **förlitande part-förtroende** ha en **anspråksregel** som skickar antingen ett **UID** eller ett **NAME ID**-värde. När du kör en **[!DNL Workfront]Test Connection** bör den visa detta om den lyckas.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösning

1. När du redigerar **[!UICONTROL ADFS INFO]** går du till **[!UICONTROL Relying Party Trusts]** > Markera objekt >**[!UICONTROL Edit Claim Rules]**.

1. **[!UICONTROL LDAP Attribute]** (vänster kolumn) ska ha **[!UICONTROL E-Mail Addresses]** (eller en unik identifierare).

1. **[!UICONTROL Outgoing Claim Type]** (höger kolumn) ska vara **[!UICONTROL Name ID]**.

   >[!NOTE]
   >
   >Den behöver inte ha LDAP-attributets e-postadresser. Alla unika identifierare som identifierar användaren kan användas, men den måste skickas till [!DNL Adobe Workfront] som **NAME-ID**.

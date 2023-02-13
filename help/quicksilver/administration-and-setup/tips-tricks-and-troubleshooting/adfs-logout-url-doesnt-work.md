---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Utloggnings-URL för ADFS fungerar inte
description: Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Utloggnings-URL för ADFS fungerar inte

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till [!UICONTROL Adobe Admin Console].
>
>Om din organisation har anslutit sig till [!UICONTROL Adobe Admin Console], se [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problem

När du använder ADFS-utloggnings-URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) får du en meddelandesida med felet: &quot;Det gick inte att komma åt webbplatsen. Försök att gå till webbplatsen igen.&quot;

Om problemet kvarstår kontaktar du administratören för den här webbplatsen och anger följande referensnummer för att identifiera problemet: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösning

1. Gå till ADFS-hanterarservern **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** > `<your party trust>` egenskaper.

1. Under **[!UICONTROL Endpoints]** flik, klicka **[!UICONTROL Add]**.

1. **[!UICONTROL Endpoint Type]** = SAML-utloggning, bindning = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Du kan ange en svars-URL om du vill att den ska dirigeras om till en annan sida. Men vi rekommenderar ADFS-webbplatsen eftersom den varnar om att du är utloggad, men du bör ändå stänga webbläsaren.

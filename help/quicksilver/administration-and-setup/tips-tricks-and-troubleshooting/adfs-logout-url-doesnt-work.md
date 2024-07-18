---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Utloggnings-URL för ADFS fungerar inte
description: Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Utloggnings-URL för ADFS fungerar inte

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Den procedur som beskrivs på den här sidan gäller endast för organisationer som ännu inte har anslutit till [!UICONTROL Adobe Admin Console].
>
>Om din organisation har anslutit sig till [!UICONTROL Adobe Admin Console], se [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problem

När du använder ADFS-utloggnings-URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) får du en meddelandesida med följande fel:&quot;Det gick inte att komma åt webbplatsen. Försök att gå till webbplatsen igen.&quot;

Om problemet kvarstår kontaktar du webbplatsens administratör och anger följande referensnummer för att identifiera problemet: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td role="rowheader">Adobe [!DNL Workfront]-licens</td> 
   <td> 
   <p>Nytt: Standard</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösning

1. Gå till **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** > `<your party trust>` egenskaper på ADFS-hanterarservern.

1. Klicka på **[!UICONTROL Add]** på fliken **[!UICONTROL Endpoints]**.

1. **[!UICONTROL Endpoint Type]** = SAML-utloggning, bindning = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Du kan ange en svars-URL om du vill att den ska dirigeras om till en annan sida. Men vi rekommenderar ADFS-webbplatsen eftersom den varnar om att du är utloggad, men du bör ändå stänga webbläsaren.

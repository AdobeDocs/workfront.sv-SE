---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: '"Felmeddelande på [!DNL Adobe Workfront] Mobilapp: "Ditt konto är inte API-aktiverat."'
description: '"Felmeddelande på [!DNL Adobe Workfront] Mobilapp: "Ditt konto är inte API-aktiverat."'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---

# Felmeddelande på [!DNL Adobe Workfront] Mobilapp: &quot;[!UICONTROL Your account is not API enabled.]&quot;

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licens</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL System administrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

När du försöker logga in på [!DNL Adobe Workfront] mobilappen får du följande fel: *[!UICONTROL Your account is not API enabled. Let your system admin know and they'll get you set up. Sorry about that.]*

## Orsak

Dina [!DNL Workfront] administratören har inte aktiverat [!DNL Workfront] miljö som ska nås från en mobil enhet.

## Lösning

1. Logga in på [!DNL Workfront] webbprogram som [!DNL Workfront] Administratör.
1. Gå till **[!UICONTROL Setup]** område.
1. Expandera **[!UICONTROL System]** menyn och klicka sedan på **[!UICONTROL Preferences]**.

1. Under **[!UICONTROL Security]** väljer du **[!UICONTROL Let people use [!DNL Workfront]'s mobile applications and the [!DNL Workfront Outlook] Add-In]** för att aktivera det.

1. Klicka på **[!UICONTROL Save]**.\
   Alla användare i systemet har nu åtkomst [!DNL Workfront] från mobilapparna och från [!DNL Outlook].

---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Redigera användarens övriga grupper gruppvis
description: Vid gruppredigering försökte jag lägga till en enda annan grupp till flera användare. När ändringarna har sparats togs alla befintliga andra grupper bort och endast den nya gruppen blev kvar.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Redigera användarens övriga grupper gruppvis

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

## Problem:

Vid gruppredigering försökte jag lägga till en enda annan grupp till flera användare.
När ändringarna har sparats togs alla befintliga andra grupper bort och endast den nya gruppen blev kvar.

## Svar:

Det beteende som blir resultatet beror på det aktuella gruppmedlemskapet för de valda användarna:

* Om alla de valda användarna har andra gruppmedlemskap som matchar exakt.. När du har valt användare och valt [!UICONTROL edit], [!UICONTROL Other Groups] visas en fullständig lista över alla grupper som användarna tillhör.

* Om de valda användarna har andra andra gruppmedlemskap.. När du har valt användare och klickat [!UICONTROL Edit], [!UICONTROL Other Groups] fältet kommer att vara tomt.

När du klickar **[!UICONTROL Save Changes]**, sparas det som visas i fältet Andra grupper.

Föregående innehåll i fältet skrivs över.

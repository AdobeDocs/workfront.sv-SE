---
product-area: projects
navigation-topic: approvals
title: Återkalla inskickade godkännanden
description: Du kan återkalla följande objekt som skickats in för godkännande.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
exl-id: 33df75f0-47d0-4848-8d9a-203f40d8831c
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 0%

---

# Återkalla inskickade godkännanden

Du kan återkalla följande objekt som skickats in för godkännande:

* Projekt
* Uppgifter
* Problem
* Tidrapporter
* Dokument
* Åtkomstbegäranden

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, tidrapporter, dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller ge högre åtkomst till objektet som är associerat med godkännandet </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Projekt

När du återkallar ett projektgodkännande återgår projektet till den status det hade innan godkännandeprocessen startades.

Om du återkallar ett godkännande som är associerat med projektets inledande status, kringgås godkännandeprocessen och projektet behåller sin startstatus.

>[!NOTE]
>
>Du kan koppla den första statusen för ett projekt eller en uppgift till en godkännandeprocess med hjälp av en mall. Mer information om hur du lägger till godkännanden i en mall finns i  [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Så här återkallar du ett projektgodkännande som du har skickat:

1. Klicka på **Startsida** icon ![](assets/home-icon-30x29.png) i Adobe Workfront övre vänstra hörn.

   >[!NOTE]
   >
   Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   * Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   * Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmeny** ![](assets/main-menu-icon.png) i sidans övre högra hörn och klicka sedan på **Startsida**.

1. I **Arbetslista** område, navigera till **Godkännanden som jag har skickat** gruppering.

1. Klicka på en **Projekt** godkännande i arbetslistan.

   Då öppnas projektet till höger om arbetslistan.

   ![](assets/project-pending-approval-phome-nwe-350x106.png)

1. Klicka **Återkalla** i det övre högra hörnet av den högra panelen.

## Uppgifter

När du återkallar ett uppgiftsgodkännande återgår uppgiften till den status den hade innan godkännandeprocessen startades.

Om du återkallar ett godkännande som är associerat med aktivitetens inledande status, kringgås godkännandeprocessen och aktiviteten behåller sin startstatus.

>[!NOTE]
>
Du kan koppla den första statusen för ett projekt eller en uppgift till en godkännandeprocess med hjälp av en mall. Mer information om hur du lägger till godkännanden i en mall finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Så här återkallar du ett aktivitetsgodkännande som du har skickat:

1. Klicka på **Startsida** icon ![](assets/home-icon-30x29.png) i Adobe Workfront övre vänstra hörn.

   >[!NOTE]
   >
   Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   * Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   * Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmeny** ![](assets/main-menu-icon.png) i sidans övre högra hörn och klicka sedan på **Startsida**.

1. I **Arbetslista** område, navigera till **Godkännanden som jag har skickat** gruppering.

1. Klicka på en **Uppgift** godkännande i arbetslistan.

   Då öppnas uppgiften till höger om arbetslistan.

   ![](assets/task-pending-approval-home-nwe-350x97.png)

1. Klicka **Återkalla** i det övre högra hörnet av den högra panelen.

## Problem

När du återkallar ett godkännande av en utgåva återgår utgåvan till den status den hade innan godkännandeprocessen startades.

Om du återkallar ett godkännande som är associerat med den inledande statusen för utgåvan, kommer godkännandeprocessen att ignoreras och utgåvan kommer att fortsätta att vara i den inledande statusen.

>[!NOTE]
>
Du kan koppla den första statusen för en utgåva till en godkännandeprocess med hjälp av en mall. Mer information om hur du skapar en frågekö finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicka på **Startsida** icon ![](assets/home-icon-30x29.png) i Adobe Workfront övre vänstra hörn.

   >[!NOTE]
   >
   Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   * Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   * Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmeny** ![](assets/main-menu-icon.png) i sidans övre högra hörn och klicka sedan på **Startsida**.

1. I **Arbetslista** område, navigera till **Godkännanden som jag har skickat** gruppering.

1. Klicka på en **Problem** godkännande i arbetslistan.

   Detta öppnar problemet till höger om arbetslistan.

   ![](assets/issue-pending-approval-home-nwe-350x103.png)

1. Klicka **Återkalla** i det övre högra hörnet av den högra panelen.

## Tidrapporter

När du återkallar ett tidrapportgodkännande återgår tidrapporten till den status den hade innan den skickades för godkännande.

1. Klicka på **Startsida** icon ![](assets/home-icon-30x29.png) i Adobe Workfront övre vänstra hörn.

   >[!NOTE]
   >
   Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   * Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   * Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmeny** ![](assets/main-menu-icon.png) i sidans övre högra hörn och klicka sedan på **Startsida**.

1. I **Arbetslista** område, navigera till **Godkännanden som jag har skickat** gruppering.

1. Klicka på en **Tidrapport** godkännande i arbetslistan.

   Då öppnas tidrapporten till höger om arbetslistan.

   ![](assets/timesheet-pending-approval-home-nwe-350x157.png)

1. Klicka **Återkalla** i det övre högra hörnet av den högra panelen.

## Dokument

Om du vill återkalla ett dokumentgodkännande måste du ta bort en eller alla användare från godkännandet manuellt.

1. Klicka på **Startsida** icon ![](assets/home-icon-30x29.png) i Adobe Workfront övre vänstra hörn.

   >[!NOTE]
   >
   Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   * Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   * Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmeny** ![](assets/main-menu-icon.png) i sidans övre högra hörn och klicka sedan på **Startsida**.

1. I **Arbetslista** område, navigera till **Godkännanden som jag har skickat** gruppering.

1. Klicka på en **Dokument** godkännande i arbetslistan.

   Då öppnas dokumentet till höger om arbetslistan.

   ![Document.png](assets/document-350x232.png)

1. Klicka **Hantera godkännanden** i det övre högra hörnet av den högra panelen. Då öppnas rutan Hantera godkännanden.
1. Klicka på **Ta bort** -ikonen är infogad med namnet på en användare i rutan Hantera godkännanden. Ta bort alla användare för att helt återkalla dokumentgodkännandet.

   ![Remove_User.png](assets/remove-user-350x41.png)

## Åtkomstbegäranden

1. Klicka på **Startsida** icon ![](assets/home-icon-30x29.png) i Adobe Workfront övre vänstra hörn.

   >[!NOTE]
   >
   Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   * Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   * Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmeny** ![](assets/main-menu-icon.png) i sidans övre högra hörn och klicka sedan på **Startsida**.

1. I **Arbetslista** område, navigera till **Godkännanden som jag har skickat** gruppering.

1. Klicka på en **Åtkomstbegäran** godkännande i arbetslistan.

   Då öppnas åtkomstbegäran till höger om arbetslistan.

   ![](assets/access-request-pending-approval-nwe-350x104.png)

1. Klicka **Återkalla** i det övre högra hörnet av den högra panelen.

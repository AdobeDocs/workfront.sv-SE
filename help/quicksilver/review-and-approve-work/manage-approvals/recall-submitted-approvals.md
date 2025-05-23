---
product-area: projects
navigation-topic: approvals
title: Återkalla inskickade godkännanden
description: Du kan återkalla följande objekt som skickats in för godkännande.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
exl-id: 33df75f0-47d0-4848-8d9a-203f40d8831c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1251'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, tidrapporter, dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller ge högre åtkomst till objektet som är associerat med godkännandet </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Projekt

När du återkallar ett projektgodkännande återgår projektet till den status det hade innan godkännandeprocessen startades.

Om du återkallar ett godkännande som är associerat med projektets inledande status, kringgås godkännandeprocessen och projektet behåller sin startstatus.

>[!NOTE]
>
>Du kan koppla den första statusen för ett projekt eller en uppgift till en godkännandeprocess med hjälp av en mall. Mer information om hur du lägger till godkännanden i en mall finns i  [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Så här återkallar du ett projektgodkännande som du har skickat:

1. Klicka på ikonen **Hem** ![Hem](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gå till grupperingen **Godkännanden som jag har skickat** i området **Arbetslista**.

1. Klicka på ett **projektgodkännande** i arbetslistan.

   Då öppnas projektet till höger om arbetslistan.

   ![Projektet väntar på godkännande](assets/project-pending-approval-phome-nwe-350x106.png)

1. Klicka på **Återkalla** i det övre högra hörnet av den högra panelen.

## Uppgifter

När du återkallar ett uppgiftsgodkännande återgår uppgiften till den status den hade innan godkännandeprocessen startades.

Om du återkallar ett godkännande som är associerat med aktivitetens inledande status, kringgås godkännandeprocessen och aktiviteten behåller sin startstatus.

>[!NOTE]
>
>Du kan koppla den första statusen för ett projekt eller en uppgift till en godkännandeprocess med hjälp av en mall. Mer information om hur du lägger till godkännanden i en mall finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Så här återkallar du ett aktivitetsgodkännande som du har skickat:

1. Klicka på ikonen **Hem** ![Hem](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gå till grupperingen **Godkännanden som jag har skickat** i området **Arbetslista**.

1. Klicka på ett **Task**-godkännande i arbetslistan.

   Då öppnas uppgiften till höger om arbetslistan.

   ![Aktivitet väntar på godkännande](assets/task-pending-approval-home-nwe-350x97.png)

1. Klicka på **Återkalla** i det övre högra hörnet av den högra panelen.

## Problem

När du återkallar ett godkännande av en utgåva återgår utgåvan till den status den hade innan godkännandeprocessen startades.

Om du återkallar ett godkännande som är associerat med den inledande statusen för utgåvan, kommer godkännandeprocessen att ignoreras och utgåvan kommer att fortsätta att vara i den inledande statusen.

>[!NOTE]
>
>Du kan koppla den första statusen för en utgåva till en godkännandeprocess med hjälp av en mall. Mer information om hur du skapar en begärandekö finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicka på ikonen **Hem** ![Hem](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gå till grupperingen **Godkännanden som jag har skickat** i området **Arbetslista**.

1. Klicka på ett **ärende**-godkännande i arbetslistan.

   Detta öppnar problemet till höger om arbetslistan.

   ![Utfärdar väntande godkännande](assets/issue-pending-approval-home-nwe-350x103.png)

1. Klicka på **Återkalla** i det övre högra hörnet av den högra panelen.

## Tidrapporter

När du återkallar ett tidrapportgodkännande återgår tidrapporten till den status den hade innan den skickades för godkännande.

1. Klicka på ikonen **Hem** ![Hem](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gå till grupperingen **Godkännanden som jag har skickat** i området **Arbetslista**.

1. Klicka på ett **tidrapportgodkännande** i arbetslistan.

   Då öppnas tidrapporten till höger om arbetslistan.

   ![Tidrapport väntar på godkännande](assets/timesheet-pending-approval-home-nwe-350x157.png)

1. Klicka på **Återkalla** i det övre högra hörnet av den högra panelen.

## Dokument

Om du vill återkalla ett dokumentgodkännande måste du ta bort en eller alla användare från godkännandet manuellt.

1. Klicka på ikonen **Hem** ![Hem](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gå till grupperingen **Godkännanden som jag har skickat** i området **Arbetslista**.

1. Klicka på ett **dokument**-godkännande i arbetslistan.

   Då öppnas dokumentet till höger om arbetslistan.

   ![Document.png](assets/document-350x232.png)

1. Klicka på **Hantera godkännanden** i det övre högra hörnet av den högra panelen. Då öppnas rutan Hantera godkännanden.
1. Klicka på ikonen **Ta bort** bredvid namnet på en användare i rutan Hantera godkännanden. Ta bort alla användare för att helt återkalla dokumentgodkännandet.

   ![Remove_User.png](assets/remove-user-350x41.png)

## Åtkomstbegäranden

1. Klicka på ikonen **Hem** ![Hem](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gå till grupperingen **Godkännanden som jag har skickat** i området **Arbetslista**.

1. Klicka på ett **åtkomstbegäran**-godkännande i arbetslistan.

   Då öppnas åtkomstbegäran till höger om arbetslistan.

   ![Begäran om åtkomst väntar på godkännande](assets/access-request-pending-approval-nwe-350x104.png)

1. Klicka på **Återkalla** i det övre högra hörnet av den högra panelen.

---
content-type: overview
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Översikt över kalenderrapporter
description: En kalenderrapport är egentligen en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan visa datuminformation i en kalenderrapport för följande objekt - REDIGERA ME.
author: Lisa
feature: Reports and Dashboards
exl-id: c65cf8ab-e37f-42a4-9a81-70962629e9ba
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Översikt över kalenderrapporter

En kalenderrapport är egentligen en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan visa datuminformation i en kalenderrapport för följande objekt:

* Uppgifter
* Problem
* Projekt

Din möjlighet att få åtkomst till kalenderrapporter i [!DNL Adobe Workfront] bestäms av [!DNL Workfront] genom din åtkomstnivå. Mer information om åtkomstnivån som behövs för att visa kalenderrapporter finns i [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Skapa egna kalendrar

[!UICONTROL Workfront] skapar automatiskt en egen standardkalender när:

* En nyskapad användare som inte har tillgång till några andra kalendrar besöker kalenderrapportsidan för första gången\
   ELLER
* En användare tar bort alla kalendrar manuellt och har inte åtkomst till några andra kalendrar

>[!NOTE]
>
>Den personliga kalendern skapas inte om användaren har åtkomst till andra kalendrar, till exempel en systemomfattande delad kalender eller kalendrar som delas specifikt med användaren.

Dessutom kan användare skapa kalendrar och komma åt kalendrar som delas med dem av andra användare. Det finns ingen gräns för hur många kalendrar som en användare har tillgång till i Workfront.

>[!NOTE]
>
>Du måste ha [!UICONTROL Edit] behörighet till [!UICONTROL Reports], [!UICONTROL Dashboards]och [!UICONTROL Calendars] på din åtkomstnivå för att skapa en kalenderrapport. Kontakta [!DNL Workfront] administratör.

## Gruppera artiklar efter datum

I varje kalenderrapport kan du skapa grupper med objekt som gör att du kan begränsa kalenderns fokus. Du kan t.ex. ha en kalendergrupp som visar datum för alla uppgifter i ett visst projekt, de medlemmar i marknadsföringsteamet som för närvarande arbetar med projektet och de försenade ärenden som tilldelats projektteamet. Mer information finns i följande artiklar:

* [Använd [!UICONTROL Planned Dates] i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
* [Använd [!UICONTROL Projected Dates] i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
* [Använd anpassade datumfält i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)

>[!NOTE]
>
>Om 504-fel visas när du kör en kalenderrapport har du förmodligen för många filter i rapporten. Om du minskar antalet filter kan rapporten köras.

## Lägga till dina kalendrar på en instrumentpanel

Du kan få snabb åtkomst till dina kalenderrapporter genom att visa dem på en kontrollpanel. Mer information om hur du lägger till en kalender på en kontrollpanel finns i [Redigera en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).

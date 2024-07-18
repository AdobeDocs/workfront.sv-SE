---
content-type: reference
navigation-topic: search
title: Använd referensnumret för objekt
description: I  [!DNL Adobe Workfront] identifieras objekt som objekt. Objekten motsvarar databasen och används för att korrelera data med ett objekt. Referensnummer är användbara när du ska skilja mellan två i övrigt liknande objekt (till exempel uppgifter med samma namn). Du kan söka efter referensnummer och inkludera dem i rapporter.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Använd referensnumret för objekt

I [!DNL Adobe Workfront] identifieras objekt som objekt. Objekten motsvarar databasen och används för att korrelera data med ett objekt.

Workfront tilldelar automatiskt följande objekt ett unikt referensnummer när objektet skapas:

* Projekt
* Uppgifter
* Problem
* Dokument

Referensnummer är användbara när du ska skilja mellan två i övrigt liknande objekt (till exempel uppgifter med samma namn). Du kan söka efter referensnummer och inkludera dem i rapporter.

>[!IMPORTANT]
>
>* [!DNL Workfront] tilldelar referensnummer kontinuerligt till alla kunder och alla objekt. När du till exempel skapar en uppgift kan [!DNL Workfront] tilldela den ett referensnummer på 0005. Om en annan kund skapar ett projekt nästa gång kan hans/hennes projekt få nästa tillgängliga referensnummer, till exempel 00006. Om du skapar ett problem härnäst kan din utgåva få referensnumret 0007 och så vidare.
>* Du kan inte styra sekvensen med referensnummer för objekt i [!DNL Workfront]. Sekvensen styrs alltid av vår databas.
>



## Visa ett objekts referensnummer

Referensnummer visas som standard för uppgifter och ärenden. Du kan också enkelt konfigurera [!DNL Workfront] så att referensnummer visas för andra typer av objekt.

* [Visa referensnummer för uppgifter och ärenden](#view-reference-numbers-for-tasks-and-issues)
* [Visa referensnummer för andra objekt](#view-reference-numbers-for-other-objects)
* [Visa referensnummer i rapporter](#view-reference-numbers-in-reports)

### Visa referensnummer för uppgifter och ärenden

Referensnummer visas som standard när du visar en uppgift eller ett problem.  Om du vill visa referensnumret klickar du på **[!UICONTROL Task Details]** eller **[!UICONTROL Issue Details]** i den vänstra panelen och letar sedan upp avsnittet **[!UICONTROL Basic Information]** i översikten.

![](assets/reference-number-nwe-350x184.png)

### Visa referensnummer för andra objekt

Om du vill visa referensnummer för objekt kan du skapa en anpassad vy eller ändra en befintlig vy och lägga till fältet [!UICONTROL Reference Number] i en kolumn i vyn. Du kan till exempel ändra vyn [!UICONTROL Projects] så att referensnumret för alla dina projekt visas.

Mer information om hur du skapar eller ändrar en vy finns i [Vyöversikt i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Visa referensnummer i rapporter

Du kan visa referensnumret för objekt i rapporter genom att lägga till kolumnen [!UICONTROL Reference Number] i rapporten.

Mer information om hur du lägger till en kolumn i en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Söka efter ett objekt efter referensnummer

Med [!DNL Workfront] kan du söka efter ett objekt efter referensnummer.

Skriv ett objekts referensnummer i fältet **[!UICONTROL Search]** och tryck sedan på **[!UICONTROL Enter]**.

Mer information om hur du söker i Workfront finns i [Sök [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

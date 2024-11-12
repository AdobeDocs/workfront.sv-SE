---
title: Skapa Workfront-objekt med Workfront Planning Record Automations
description: Du kan konfigurera automatisering i Workfront Planning som, när den aktiveras, skapar objekt i Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: cfaacc4137ebfa7f2ed057522d43bd82715011df
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---


# Skapa objekt med automatisering av Workfront Planning Record

Du kan konfigurera automatisering i Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller Workfront Planning.

Du aktiverar automatiseringen i poster. Objektet som skapas är anslutet till Planning-posten där du aktiverade automatiseringen.

Du kan till exempel skapa en automatisering som tar en Workfront Planning-kampanj och skapar ett projekt i Workfront för att spåra kampanjens utveckling. Projektet skulle kopplas till Workfront Planning Campaign.

Mer information om anslutna poster finns i [Översikt över anslutna poster](/help/quicksilver/planning/records/connected-records-overview.md).


## Konfigurera automatisering i Workfront Planning

Du måste konfigurera en automatisering i Workfront Planning innan du kan använda den för att skapa objekt.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) och välj **Automationer**.

   En lista över tillgängliga automatiseringar öppnas.

1. Klicka på **Skapa ny automatisering** i skärmens övre högra hörn.
1. I fältet **Knapptext** anger du texten som du vill ska visas på knappen. Användare klickar på den här knappen när de använder automatiseringen för att skapa ett Workfront-objekt.
1. (Valfritt) Om du vill lägga till en ikon till knappen väljer du en ikon bland de tillgängliga alternativen.
1. I fältet **Skapa en typ av** markerar du det objekt som du vill att automatiseringen ska skapa.

   Tillgängliga objekt är:

   * Projekt
   * Portfolio
   * Program
   * Grupp

1. Välj ett postfält i fältet **Markera det fält som ska användas i projektnamnet**. Det nya objektet får fältets innehåll som namn.
1. I fältet **Markera fältet för att länka tillbaka det skapade projektet** markerar du ett postfält. Det nya objektet visas i det här fältet när du visar posten i Workfront Planning.
1. Välj andra alternativ som är tillgängliga för den typ av objekt som du skapar.
1. Klicka på **Skapa**

Automatiseringen visas i listan över automatiseringar och finns tillgänglig för arkivering.

## Skapa ett objekt med en Workfront Planning Automation

1. Öppna den posttypssida som innehåller de poster du vill använda för att skapa Workfront-objekt i Workfront Planning.
1. Markera en eller flera poster.
1. Klicka på knappen för automatisering i skärmens nedre högra hörn.

   I det här exemplet är det knappen Skapa projekt.

   ![Automatiseringsknappen](assets/automation-custom-button.png)

>[!NOTE]
>
>Vi rekommenderar att du kontrollerar att objektet har skapats och anslutits som förväntat.


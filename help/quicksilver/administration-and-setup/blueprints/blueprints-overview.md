---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Översikt över utkast
description: Med utkast får du grundläggande byggstenar som hjälper dig att skapa ett arbetsstyrningssystem som växer med dig.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 006df3f8c391596cd0c769df5d7eb843949b4e01
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Översikt över utkast

Med utkast får du grundläggande byggstenar som hjälper dig att skapa ett arbetsstyrningssystem som växer med dig. Systemadministratörer kan bläddra i katalogen med utkast och installera färdiga projektmallar, instrumentpaneler och organisationsstrukturer. Andra användare kan bläddra i katalogen och begära installation av en plan. Mer information finns i [Bläddra i katalogen med ritningar och begär installation av ritningar](../../administration-and-setup/blueprints/browse-catalog.md).

Varje plan är avsedd för en avdelning och en viss mognadsnivå, vilket gör att du snabbare kan implementera beprövade metoder i ditt system. De mognadsnivåer som anges nedan anges på prenumerationskortet för trycksakskatalogen och detaljerna.

**[!UICONTROL Managed]:** Hanterade projektmallar gör det lättare att anta en ny affärsprocess innan aktiviteter och slutprodukter accepteras som standardprocedurer. De innehåller uppgifter för att säkerställa att varje steg i den nya processen följs.

**[!UICONTROL Integrated]:** Integrerade projektmallar förutsätter att affärsfunktionerna stöds genom en standardiserad procedur. Deltagare i processen vet vilka steg och uppgifter de behöver för att slutföra processen. Projektmallarna som stöder den här processen innehåller färre uppgifter för att bara spåra milstolpar och andra viktiga slutprodukter som behövs för rapportering.

## Hitta rätt ritning

Du kan bläddra bland skisser efter användningsfall, mognadsnivå, installationsstatus och typ med filtren till höger om katalogen. När du har hittat en plan som intresserar dig kan du visa information på informationssidan.

### Typ av blåtryck

Den blå typen visar vad som ingår i ritningen. Typen visas längst ned på kortet i katalogen. Observera att en rityta kan ha mer än en typ.

Följande typer av ritningar finns:

* Projektmallar: Inkluderar standardobjekt som är kopplade till en projektmall (uppgifter, ärenden, roller och team) och vissa inställningar som är relaterade till dessa objekt. Mer information finns i [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).
* Organisationsstrukturer: Inkluderar objekt som är kopplade till en organisations struktur (företag, grupper, roller och team). Mer information finns i [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).
* Kontrollpaneler: Inkluderar en eller flera instrumentpaneler för ett visst användningsfall, t.ex. implementeringstjänster.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Om du vill granska de aktuella ritningarna kan du läsa [Lista över tillgängliga ritningar](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Visa detaljer

Varje plan innehåller en informationssida. Från den här sidan kan du:

* Visa en sammanfattning av arbetsflödets innehåll
* Läs en kort sammanfattning av planen
* Visa installationshistorik (klicka **[!UICONTROL See Details]** om du vill se en fullständig lista över objekt som har installerats med en plan)
* Se beskrivningar av roller, team, företag och grupper
* Se ett visuellt exempel på en viss plan, t.ex. en projektmall (du kan förhandsvisa hela bilden i webbläsaren eller hämta den)

![[!UICONTROL Blueprint Details] page](assets/blueprint-details-page-2022.png)

## Installera en plan

Systemadministratören kan installera direkt i produktionsmiljön eller i sandlådemiljöer. Mer information finns på [Installera en plan](../../administration-and-setup/blueprints/blueprints-install.md) eller [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).

Efter installationen kan du vara osäker på vilka åtgärder som ska vidtas. Mer information finns i [Åtgärder som ska vidtas efter installation av en plan](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Ytterligare information om ritningar och mallar

Ritningar ersätter inte projektmallarnas funktion i [!DNL Adobe Workfront]. Med utkast kan du skapa nya mallar snabbare och ordna mer av ditt arbete i [!DNL Workfront].

Du kan inte kopiera eller redigera en plan. När du har installerat lösningen från en plan kan du dock ändra projektmallen, jobbrollerna eller teamen som skapas utifrån planen på samma sätt som du vanligtvis uppdaterar posterna i [!DNL Workfront] gränssnitt. När du installerar en plan sparas mallen i [!UICONTROL Templates] område på [!DNL Workfront] och originalritningen finns kvar i [!UICONTROL Blueprints] område. Du behöver inte göra en kopia av mallen innan du börjar anpassa den efter dina behov.

Utskriftsbilder tar inte bort eller ersätter ingenting som är konfigurerat i din miljö. Om du tänker ersätta en befintlig mall genom att installera en plan som skapar en ny mall, rekommenderar vi att du inaktiverar den tidigare versionen för att undvika förvirring hos de planerare som skapar projekt från mallar.

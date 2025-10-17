---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Översikt över utkast
description: Utkast är uppsättningar av Workfront-objekt som hanterar vanliga användningsområden i Workfront. Du kan hämta och installera en plan och sedan konfigurera objekten för ditt specifika användningsfall.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Översikt över utkast

<!--Audited: 01/2024-->

Utkast är uppsättningar av Workfront-objekt som hanterar vanliga användningsområden i Workfront. Du kan hämta och installera en plan och sedan konfigurera objekten för ditt specifika användningsfall.

![Huvudsidan för utkast](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>Exempel:
>
>* **Organisationsinställningar för personaladministration**
>
>   Den här planen innehåller konfigurationen av organisationsstrukturer som ska utökas till en personalavdelning.
>
>* **Lägg till IT-checklista för ny anställd**
>
>   Den här planen innehåller en mall för att organisera nya anställdas introduktionsaktiviteter. Genom att använda den här mallen kan IT-avdelningen arbeta effektivt, vilket ger en positiv ny medarbetarupplevelse och ger snabbare produktivitet.
>
>* **Grunderna för ärvda instanser | Checklista**
>
>    Den här planen innehåller en projektmall (eller checklista) som du kan granska med en kort lista över frågor, resurser och länkar för att få en tydlig förståelse för hur din Workfront-instans har konfigurerats. Använd detta när du nyligen har ärvt en Workfront-instans och behöver hjälp med var du ska börja.
>
>Information om hur du granskar aktuella ritningar finns i [Lista över tillgängliga ritningar](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


Med utkast får du grundläggande byggstenar som hjälper dig att skapa ett arbetsstyrningssystem som växer med dig. Systemadministratörer kan bläddra i katalogen med utkast och installera färdiga projektmallar, instrumentpaneler och organisationsstrukturer. Andra användare kan bläddra i katalogen och begära installation av en plan. Mer information finns i [Bläddra i katalogen med utkast och begära installation av utkast](../../administration-and-setup/blueprints/browse-catalog.md).

Varje plan är avsedd för en avdelning och en viss mognadsnivå, vilket gör att du snabbare kan implementera beprövade metoder i ditt system. De mognadsnivåer som anges nedan anges på prenumerationskortet för trycksakskatalogen och detaljerna.

* **[!UICONTROL Managed]:** Hanterade projektmallar hjälper till att anta en ny affärsprocess innan aktiviteter och slutprodukter accepteras som en standardprocedur. De innehåller uppgifter för att säkerställa att varje steg i den nya processen följs.

* **[!UICONTROL Integrated]:** Integrerade projektmallar förutsätter att affärsfunktioner stöds via en standardprocedur. Deltagare i processen vet vilka steg och uppgifter de behöver för att slutföra processen. Projektmallarna som stöder den här processen innehåller färre uppgifter för att bara spåra milstolpar och andra viktiga slutprodukter som behövs för rapportering.

## Hitta rätt ritning

Du kan bläddra bland skisser efter användningsfall, mognadsnivå, installationsstatus och typ med filtren till höger om katalogen. När du har hittat en plan som intresserar dig kan du visa information på informationssidan.

### Typ av blåtryck

Den blå typen visar vad som ingår i ritningen. Typen visas längst ned på kortet i katalogen. Observera att en rityta kan ha mer än en typ.

Följande typer av ritningar finns:

* **Projektmallar**: Innehåller standardobjekt som är kopplade till en projektmall (uppgifter, ärenden, roller och team) och vissa inställningar som är relaterade till dessa objekt. Mer information finns i [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).
* **Organisationsstrukturer**: Inkluderar objekt som är kopplade till en organisations struktur (företag, grupper, roller och team). Mer information finns i [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).
* **Instrumentpaneler**: Inkluderar en eller flera instrumentpaneler för ett visst användningsfall, till exempel implementeringstjänster.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Information om hur du granskar aktuella ritningar finns i [Lista över tillgängliga ritningar](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Visa detaljer

Varje plan innehåller en informationssida. Från den här sidan kan du:

* Visa en sammanfattning av arbetsflödets innehåll
* Läs en kort sammanfattning av planen
* Visa installationshistorik (klicka på **[!UICONTROL See Details]** om du vill visa en fullständig lista över objekt som har installerats med planen)
* Se beskrivningar av roller, team, företag och grupper
* Se ett visuellt exempel på en viss plan, t.ex. en projektmall (du kan förhandsvisa hela bilden i webbläsaren eller hämta den)

![[!UICONTROL Blueprint Details] sida &#x200B;](assets/blueprint-details-page-2022.png)

## Installera en plan

En Workfront-administratör kan installera en plan direkt i alla miljöer (i produktions-, förhandsgransknings- eller sandlådemiljöer). Mer information finns i [Installera en plan](../../administration-and-setup/blueprints/blueprints-install.md) eller [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).

Efter installationen kan du vara osäker på vilka åtgärder som ska vidtas. Mer information finns i [Åtgärder som ska vidtas efter att en plan har installerats](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Ytterligare information om ritningar och mallar

Det går inte att ersätta projektmallsfunktionerna i [!DNL Adobe Workfront] med utkast. Med utkast kan du skapa nya mallar snabbare för att ordna mer av ditt arbete i [!DNL Workfront].

Du kan inte kopiera eller redigera en plan. När du har installerat lösningen från en plan kan du dock ändra projektmallen, jobbrollerna eller teamen som skapas utifrån planen på samma sätt som du vanligtvis uppdaterar posterna i [!DNL Workfront]-gränssnittet. När du installerar en plan sparas mallen i [!UICONTROL Templates]-området för [!DNL Workfront] och den ursprungliga planen behålls i [!UICONTROL Blueprints]-området. Du behöver inte göra en kopia av mallen innan du börjar anpassa den efter dina behov.

Utskriftsbilder tar inte bort eller ersätter ingenting som är konfigurerat i din miljö. Om du tänker ersätta en befintlig mall genom att installera en plan som skapar en ny mall, rekommenderar vi att du inaktiverar den tidigare versionen för att undvika förvirring hos de planerare som skapar projekt från mallar.

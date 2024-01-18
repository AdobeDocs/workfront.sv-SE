---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatering,release
navigation-topic: 2021-2-release-activity
title: 21.2 Andra förbättringar
description: Den här sidan beskriver alla andra förbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i versionsöversikt 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 21.2 Andra förbättringar

Den här sidan beskriver alla andra förbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i [21.2 Versionsöversikt](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vi är nu officiellt Adobe Workfront

Workfront har gett sitt varumärke till Adobe Workfront.

De mest framträdande områdena inom Adobe Workfront och våra kundtillvända webbplatser uppdateras nu. Övriga områden kommer snart att uppdateras.

**Uppdaterade områden**

* Inloggningsskärm, övre navigering, korrektur
* Layoutmallsgränssnitt, huvudmeny, anpassad Forms-export (endast tillgängligt i den nya Adobe Workfront-upplevelsen)
* Mobilappen Workfront (iOS och Android)

Områden uppdateras snart

* Språkprogram för datorer och mobila enheter
* Export från PDF till listor och rapporter
* Favicon icon in the browser tab

**Områden som uppdateras senare**

* E-postaviseringar

## E-postvalidering av tillåtelselista

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Om du använder e-postadressen tillåtelselista valideras nu nya och uppdaterade e-postadresser mot tillåtelselista. När du lägger till en ny användare eller redigerar en befintlig användare och anger en e-postdomän som inte finns på tillåtelselista visas ett meddelande om att användaren inte kommer att få e-postmeddelanden. Du kan fortfarande spara användarprofilen, men du bör lägga till domänen i tillåtelselista så att användaren får e-post.

Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nytt utseende och ny känsla för objektrubriker

>[!NOTE]
>
>Den här funktionen släpptes till produktionsmiljön den 10 mars 2020.
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

För att ytterligare förstärka informationshierarkin och hjälpa användarna att förstå vilken sida de är på, har nu varje objektrubrik:

* Färgstarka, modernare ikoner för varje objekttyp
* Objekttypen som anges ovanför objektets namn
* En uppdaterad teckensnittsstil och textstorlek
* Andra mindre formatändringar

Tidigare fanns det ingen ikon och ett märke med objektnamnet visades till höger om objekttiteln.

Sidhuvudena för områden i den nya Workfront-upplevelsen - som Förbättrad analys, Resurshantering och andra - har också den här uppdaterade utseendet och känslan.

Mer information om objektrubrikerna i den nya Workfront-upplevelsen finns i [Nya objektrubriker](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Uppdateringar av söksvar för objektstatus

Workfront lagrar nu objektstatusar på ett nytt sätt.

De här ändringarna påverkar inte hur statussökningar utförs. API-begäranden som innehåller en objektstatussökning returnerar dock en ofullständig lista över gruppstatus.

Mer information finns i [Centrala API-ändringar: statussöksvar](../../../wf-api/api/api-changes-search.md) .

## Nyttolaster för händelseprenumerationer har uppdaterats för att inkludera alla fält som slutar i ID

Alla händelseabonnemangsnyttolaster innehåller nu alla fält som slutar med ID.

Observera att varje objekt har en egen unik uppsättning associerade fält, som innehåller en unik uppsättning associerade fält som slutar i ID. Detta innebär att medan varje nyttolast innehåller alla objektets associerade fält som slutar i ID, har varje objekt olika fältuppsättningar som slutar i ID.

## Betaversionen av utkast är nu tillgänglig i förhandsvisning

>[!NOTE]
>
>Den här funktionen kommer inte att vara allmänt tillgänglig i produktionsmiljön förrän i version 21.3, senare i år. Finns endast i nya Adobe Workfront.

Med utkast får du grundläggande byggstenar som hjälper dig att skapa ett arbetsstyrningssystem som växer med dig. Systemadministratörer kan bläddra i katalogen med utkast och installera färdiga projektmallar.

Mer information finns i [Blueprints](../../../administration-and-setup/blueprints/blueprints.md).

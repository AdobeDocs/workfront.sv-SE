---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Förbättringar av 2019.1-språkkontroll
description: Den här sidan beskriver alla korrekturförbättringar som ingår i version 2019.1. Funktionerna är nu tillgängliga i produktionsmiljön.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Förbättringar av 2019.1-språkkontroll

Den här sidan beskriver alla korrekturförbättringar som ingår i version 2019.1. Funktionerna är nu tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2019.1 finns i [Översikt över versionsaktivitet för 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## För administratörer

* [Konfigurera standardroll för korrektur för icke-mottagare som öppnar ett korrektur](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## För alla användare

* [Korrektur för interaktivt innehåll i Web Proofing Viewer](#proof-interactive-content-in-the-web-proofing-viewer)
* [Standardsorteringsordning för kommentarer i korrekturläsaren är nu äldsta till senaste](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Förbättrad granskning för kommentarer i korrekturläsaren som är kopplad till ett videointervall](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Länka till dokumentinformation från ett korrekturmeddelande eller korrekturläsaren](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Ändra dina e-postmeddelanden i korrekturläsaren](#change-your-email-notifications-in-the-proofing-viewer)
* [Ändra bakgrundsfärg i Desktop Proofing Viewer](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Rensa cachelagrade webbläsardata från ett korrektur i Desktop Proofing Viewer](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Konfigurera standardroll för korrektur för icke-mottagare som öppnar ett korrektur {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront-administratörer kan nu konfigurera standardrollen för korrektur för användare som inte är angivna mottagare i korrekturets arbetsflöde, men som har åtkomst till korrekturet via sitt Workfront-objekt (till exempel projekt, uppgift eller utgåva).

När användare och gäster hade åtkomst till ett korrektur utan att ha lagts till i arbetsflödet var deras standardroll för korrektur granskare.

Den här funktionen gäller endast korrektur som skapats i Workfront, inte i Workfront Proof.

## Korrektur för interaktivt innehåll i Web Proofing Viewer {#proof-interactive-content-in-the-web-proofing-viewer}

Om din organisations säkerhetsprofiler inte tillåter användning av den fristående visningsprogramappen för korrektur för skrivbord kan din Workfront-administratör nu aktivera interaktivt innehåll i Web Proofing Viewer. Innehållet måste paketeras i en ZIP-fil innan du skapar korrekturet.

Mer information finns i artikeln.

VIDEO

## Standardsorteringsordning för kommentarer i korrekturläsaren är nu äldsta till senaste  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

I korrekturläsaren är standardsorteringsordningen för kommentarer i ett korrektur nu Äldst till Senaste, som i en verbal konversation.

Tidigare var standardsorteringsordningen Senaste till Äldst.

Du kan välja ett annat sorteringsalternativ och det sparas för alla andra korrektur som du öppnar.

Mer information finns i avsnittet i artikeln.

## Förbättrad granskning för kommentarer i korrekturläsaren som är kopplad till ett videointervall {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

När du granskar en kommentar som är associerad med ett videomaterial i korrekturläsaren kan du nu klicka på Spela upp för att visa hela filmomfånget. Uppspelningen pausas när den når slutet av intervallet. Kommentaren förblir öppen så att du inte tappar bort kontrollen över var du är.

När du tidigare öppnade en kommentar för ett intervall med videotagningar var du tvungen att leta reda på början av intervallet manuellt genom att titta på bildrutenumren som visades i kommentaren innan du klickade på Spela upp. I annat fall påbörjade korrekturläsaren uppspelningen när du senast klickade på videons tidslinje och den inte pausade i slutet av intervallet. Kommentaren komprimerades också när du klickade på Spela upp, så det var inte längre tydligt vilken kommentar du granskade.

Mer information om hur du granskar videokorrektur finns i .

VIDEO

## Länka till dokumentinformation från ett korrekturmeddelande eller korrekturläsaren {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

När du får ett e-postmeddelande med en inbjudan om att granska ett korrektur eller när du granskar ett korrektur i korrekturläsaren, kan du nu snabbt komma åt sidan Dokumentinformation för korrekturet. På den här sidan kan du se det Workfront-objekt (till exempel en uppgift, ett projekt eller ett problem) som är kopplat till korrekturet. Detta ger en kontext som hjälper dig att förstå vad du behöver göra med beviset.

Den här funktionen fungerar kanske bara för nya användare som du lägger till i systemet. Problemet är tillfälligt.

Mer information finns i artikeln .

VIDEO

## Ändra dina e-postmeddelanden i korrekturläsaren {#change-your-email-notifications-in-the-proofing-viewer}

Nu kan alla granskare ange vilka korrekturmeddelanden de vill få för korrektur. Detta är särskilt viktigt vid samarbete med externa intressenter.

Tidigare var det bara korrekturläsaren eller trafikchefen som kunde konfigurera korrekturens e-postaviseringar för granskarna som de lade till i korrekturet. Externa medarbetare kunde inte kontrollera vilka e-postaviseringar de fick om beviset eftersom de inte hade den åtkomst till Workfront som krävdes eller rätt behörighetsnivå.

Dessa inställningar skiljer sig från de e-postaviseringsinställningar som du kan konfigurera i Workfront.

Mer information finns i [Hantera meddelanden om korrekturkommentarer och beslut](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDEO

## Ändra bakgrundsfärg i Desktop Proofing Viewer {#change-the-background-color-in-the-desktop-proofing-viewer}

Nu kan du ändra bakgrundsfärgen i Desktop Proofing Viewer från standardfärgen nära svart till vitt. Det gör det enklare att se korrekturgranska innehåll med genomskinlig bakgrund.

Mer information finns i [Konfigurera inställningar för korrekturläsare](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO

## Rensa cachelagrade webbläsardata från ett korrektur i Desktop Proofing Viewer {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

När webbläsarens inställningar för cookie och cache är inställda på att blockera innehåll som popup-fönster, kan detta blockeringsbeteende även inträffa i Desktop Proofing Viewer, vilket gör det omöjligt för granskarna att se och kommentera popup-innehållet i korrekturet.

Nu kan du rensa webbläsarens cachedata som kan sparas med ett korrektur så att allt innehåll visas i Desktop Proofing Viewer och granskarna kan se och kommentera det.

Mer information finns i [Konfigurera inställningar för korrekturläsare](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO

---
title: 2.1 Förbättrade begäranden
description: 2.1 Förbättrade begäranden
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 2.1 Förbättrade begäranden

Den här sidan beskriver alla begäranden som gjorts i version 2.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

veckan 17 januari 2022.

En lista över alla ändringar som är tillgängliga i version 2.1 finns i [2.1 Versionsöversikt](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Gränssnittsförbättring för användare som inte har behörighet att skapa begäranden

För att förbättra användarnas upplevelse när de arbetar med förfrågningar har vi infört en förbättring av gränssnittet som anger för den inloggade användaren att de inte har tillgång till att skapa förfrågningar. I och med den här förbättringen är knappen Ny begäran nedtonad för användare som inte har åtkomst till att skapa problem. När du hovrar över den nedtonade knappen visas ett verktygstips som förklarar att Workfront-administratören har begränsat den aktuella användarens åtkomst för att skapa begäranden.

Före den här förbättringen visades inte knappen Ny begäran i området Begäranden för dessa användare. Kopiering och inlämning av en begäran som ny är också begränsad.

Mer information om hur du skapar begäranden finns i [Skapa och skicka Adobe Workfront-förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Kopiera och skicka begäranden

För att optimera processen för att skicka in begäranden introducerar vi nya funktioner som gör att du kan kopiera en befintlig begäran och skicka den som en ny begäran. Detta är praktiskt när du ofta skickar in liknande förfrågningar. I det här fallet kan du återanvända en befintlig begäran, göra några ändringar och sedan skicka den som en ny begäran.

Med den här ändringen kan användare som kan visa förfrågningar som andra har skickat även kopiera dessa förfrågningar och skicka dem som nya. Du kan förhindra detta genom att uppdatera följande inställning i begärandeköprojektet: Personer från samma företag ärver samma behörigheter för alla begäranden.

>[!NOTE]
>
>Du kan inte kopiera och skicka om utgåvor som har skickats till en begärandekö utan ett köämne innan den här funktionen släpptes.

Mer information finns i [Kopiera och skicka begäranden](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Uppdaterad sammanfattning i avsnittet Skickat i området Begäranden

>[!NOTE]
>
>Den här funktionen togs tillfälligt bort från förhandsvisningsmiljön den 12 november 2021. Den kommer att läggas till på nytt vid ett senare tillfälle.

För att förbättra synligheten och interaktionen med panelen Sammanfattning har vi lagt till en etikett till ikonen Öppna sammanfattning i avsnittet Skickat i området Begäranden. Etiketten är nu dynamisk och uppdateras beroende på om panelen är öppen eller stängd.

När du öppnar panelen Sammanfattning utan att först markera en begäran visas nu en mer användarvänlig bild som tydligt instruerar användaren att markera ett objekt innan panelen öppnas. Mer information finns i [Sök efter skickade begäranden](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Den här ändringen innebär att panelen Sammanfattning för uppgifter, utgåvor och dokument också har uppdaterats. Mer information om panelen Sammanfattning finns i [Sammanfattning](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

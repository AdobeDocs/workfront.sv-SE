---
title: Adobe Workfront Planning AI Assistant - översikt
description: Du kan använda AI-assistenten för att generera, uppdatera eller ta bort poster baserat på den aktuella sidkontexten och poststrukturen. Användarens kommandon och AI:ns körning av dessa kommandon fungerar tillsammans för att se till att ändringar som görs av AI återspeglas korrekt i din miljö.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 57e0fe65180cec3fab5cb10b3afbc0ac0a1dbb55
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Adobe Workfront Planning AI Assistant - översikt

<!-- update metadata above at GA-->

>[!IMPORTANT]
>
><span class="preview">Workfront AI Assistant har tagits bort tillfälligt och är tillgänglig vid ett senare datum.</span>
>Informationen i den här artikeln gäller Adobe Workfront Planning och Workfront AI Assistant (beta), som är nya erbjudanden från Adobe Workfront.
>
>För närvarande är Workfront Planning i ett tidigt skede och Workfront AI Assistant är i en betafas.
>
>Workfront Planning och AI Assistant (beta) är öppna för ett begränsat antal kunder.
>
>Du måste vara kund hos Workfront för att kunna använda dessa funktioner.
>
>Din kontorepresentant kommer att informera dig om du är en del av det här steget.
>
>Mer information finns i [Översikt över Adobe Workfront-planering](/help/quicksilver/planning/general/planning-overview.md).

Du kan använda AI-assistenten för att generera, uppdatera eller ta bort poster baserat på den aktuella sidkontexten och poststrukturen.

Användarens kommandon och AI:ns körning av dessa kommandon fungerar tillsammans för att se till att ändringar som görs av AI återspeglas korrekt i din miljö.

## Överväganden om AI-assistenten

* AI-assistenten är som standard tillgänglig för den huvudsakliga Workfront-administratören. Mer information finns i [Konfigurera grundläggande information för systemet](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Workfront-administratören måste aktivera AI-assistenten för alla andra användare. Mer information finns i [Aktivera eller inaktivera AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* AI-assistenten fungerar för varje sida. De förfrågningar du skickar för AI-assistenten måste referera till funktioner som är tillgängliga på den sida som du har öppnat.

* De åtgärder som AI-assistenten utför i Planning-området hänger ihop med dina Workfront Planning-behörigheter och din åtkomstnivå i Workfront. Mer information finns i följande artiklar:

   * [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Ändringar som AI-assistenten gör för användarens räkning spåras i postens historikpanel.

* Du kan använda kommandon för att ångra åtgärder. Du kan t.ex. skriva &quot;Ångra den senaste ändringen&quot; för att ångra ändringen.

## Funktioner som är tillgängliga för AI-assistenten

AI Assistant finns för närvarande i Planning-delen av Workfront för följande sidor:

* Workspace page
* Posttypsida
* Postsida

Du kan nu använda AI-assistenten för att utföra följande åtgärder:

* Sök efter poster. Du kan söka efter information i alla postfält.
* Skapa poster. Ett ID med en länk till den nya posten visas när posten har skapats. Du kan ange de fält som du vill uppdatera när du skapar, t.ex. datum eller beskrivning.
* Skapa poster baserat på ett dokument som du överför. Workfront stöder följande dokumentformat för AI-assistenten:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt och de flesta bildformat
* Uppdatera fält för de poster som visas på skärmen
* Ta bort poster
* Återställ poster som du just har tagit bort

## Åtkomst till AI-assistenten

1. Logga in på Workfront och gå till **Planering**.

1. Klicka på ett **arbetsytekort**.

1. (Valfritt) Klicka på ett **posttypskort**.

1. (Valfritt) Klicka på en **post** för att öppna postens **informationssida**.

1. Klicka på ikonen **AI-assistenten** i det övre högra hörnet av skärmen i det globala navigeringsfältet.

   ![](assets/ai-assistant-icon-highlighted.png)

1. Börja skriva kommandon för AI-assistenten och klicka sedan på Enter när du är klar.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Du kan t.ex. skriva något av följande:

   * Skapa en kampanj med startdatumet 4 juli och slutdatumet 30 juli
   * Uppdatera fältet Beskrivning för posten för sommarkampanjen med datumet som ska fastställas
   * Ta bort den sista posten
   * Återställ posten

   En visuell indikator visas medan AI-assistenten bearbetar kommandon och anger förväntad svarstid.

   När du har fått ett svar följer du länkarna eller ser ändringarna till vänster.

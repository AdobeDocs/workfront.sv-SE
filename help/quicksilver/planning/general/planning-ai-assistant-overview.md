---
title: Översikt över Adobe Workfront Planning AI Assistant
description: Du kan använda AI-assistenten för att generera, uppdatera eller ta bort poster baserat på den aktuella sidkontexten och poststrukturen. Användarens kommandon och AI:ns körning av dessa kommandon fungerar tillsammans för att se till att ändringar som görs av AI återspeglas korrekt i din miljö.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant - översikt

<!-- update TOC and miniTOC when making this live-->

>[!IMPORTANT]
>
>Informationen i den här artikeln gäller Adobe Workfront Planning och AI Assistant, som är nya erbjudanden från Adobe Workfront.
>
>För närvarande är Workfront Planning och AI Assistant i ett tidigt skede, som är öppet för ett begränsat antal kunder.
>
>Du måste vara kund hos Workfront för att kunna använda dessa funktioner.
>
>Din kontorepresentant kommer att informera dig om du är en del av det här steget.
>
>Mer information finns i [Adobe Workfront Planning - översikt](/help/quicksilver/planning/general/planning-overview.md).

Du kan använda AI-assistenten för att generera, uppdatera eller ta bort poster baserat på den aktuella sidkontexten och poststrukturen.

Användarens kommandon och AI:ns körning av dessa kommandon fungerar tillsammans för att se till att ändringar som görs av AI återspeglas korrekt i din miljö.

## Överväganden om AI-assistenten

* AI-assistenten är som standard tillgänglig för Workfront-administratörer.

* Workfront-administratören måste aktivera AI-assistenten för alla andra användare. Mer information finns i [Aktivera eller inaktivera AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* AI-assistenten fungerar för varje sida. De förfrågningar du skickar för AI-assistenten måste referera till funktioner som är tillgängliga på den sida som du har öppnat.

* De åtgärder som utförs av AI-assistenten hänger ihop med dina Workfront Planning-behörigheter och din åtkomstnivå i Workfront. Mer information finns i följande artiklar:

   * [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Ändringar som AI-assistenten gör för användarens räkning spåras i postens historikpanel.

* Du kan använda kommandon för att ångra åtgärder.

## Funktioner som är tillgängliga för AI-assistenten

AI Assistant finns för närvarande i Planning-delen av Workfront för följande sidor:

* Posttypsida
* Postsida

Du kan nu använda AI-assistenten för att utföra följande åtgärder:

* Skapa poster. Ett ID med en länk till den nya posten visas när posten har skapats.
* Skapa poster baserat på ett dokument som du överför. Workfront stöder följande dokumentformat för AI-assistenten:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt och de flesta bildformat
* Uppdatera fält för de poster som visas på skärmen
* Ta bort poster
* Återställ poster som du just har tagit bort

## Åtkomst till AI-assistenten

1. Logga in på Workfront och gå till **Planering** område.

1. Klicka på en **arbetsytekort** > **posttypskort**.

1. (Valfritt) Klicka på en **record** för att öppna postens **Information** sida.

1. Klicka på **AI Assistant, ikon** i skärmens övre högra hörn i det globala navigeringsfältet.

   ![](assets/ai-assistant-icon-highlighted.png)

1. Börja skriva kommandon för AI-assistenten och klicka sedan på Enter när du är klar.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Du kan t.ex. skriva något av följande:

   * Skapa en post
   * Uppdatera fältet Beskrivning för posten för sommarkampanjen med datumet som ska fastställas
   * Ta bort den sista posten
   * Återställ posten

   En visuell indikator visas medan AI-assistenten bearbetar kommandon och anger förväntad svarstid.

   När du har fått ett svar följer du länkarna eller ser ändringarna till vänster.

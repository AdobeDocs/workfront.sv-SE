---
title: Översikt över Adobe Workfront Planning AI Assistant
description: Du kan använda AI-assistenten för att generera, uppdatera eller ta bort poster baserat på den aktuella sidkontexten och poststrukturen. Användarens kommandon och AI:ns utförande av dessa kommandon fungerar tillsammans för att säkerställa att ändringar som görs av AI återspeglas korrekt i din miljö.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: a36968bdae5756f0f8283da04a2afca83b4dd94a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---


# Översikt över Adobe Workfront Planning AI Assistant

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

Du kan använda AI-assistenten för att generera, uppdatera eller ta bort poster baserat på den aktuella sidkontexten och poststrukturen.

Användarens kommandon och AI:ns utförande av dessa kommandon fungerar tillsammans för att säkerställa att ändringar som görs av AI återspeglas korrekt i din miljö.

## Att tänka på när det gäller AI-assistenten

* AI-assistenten måste vara aktiverad för din organisation innan den är tillgänglig för användare i ditt företag. Mer information finns i [Översikt](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) över AI Assistant.
* När Workfront har aktiverat AI Assistant för din organisation är den tillgänglig för Workfronts huvudadministratör. Mer information finns i [Konfigurera grundläggande information för systemet](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Workfront-administratören måste aktivera AI Assistant för alla andra användare. Mer information finns i [Aktivera eller inaktivera AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* AI-assistenten fungerar i kontexten för varje sida. De begäranden som du skickar in för AI-assistenten måste referera till funktioner som är tillgängliga på den sida som du har öppen.

* De åtgärder som utförs av AI Assistant i planeringsområdet är i kontexten av dina Workfront Planning-behörigheter och din Workfront-åtkomstnivå. Mer information finns i följande artiklar:

   * [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Översikt över licenstyper när du använder Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Ändringar som görs av AI-assistenten för användarens räkning spåras i postens historikpanel.

* Du kan använda kommandon för att ångra dina åtgärder. Du kan till exempel skriva &quot;Ångra senaste ändring&quot; för att återställa ändringen.

* När du skapar, uppdaterar eller tar bort ett objekt via AI Assistant visar AI Assistant de avsedda åtgärderna och ber om bekräftelse. Du kan sedan bekräfta eller avbryta åtgärderna.

## Funktioner som för närvarande är tillgängliga för AI Assistant

För närvarande är AI-assistenten tillgänglig i området Planering i Workfront för följande sidor:

* Sidan Arbetsyta
* Sida för posttyp
* Sidan Spela in

Du kan använda AI-assistenten för att utföra följande åtgärder just nu:

* Sök efter poster. Du kan söka efter information som finns i alla postfält.
* Skapa poster. Ett ID med en länk till den nya posten visas när posten har skapats. Du kan ange de fält som du vill uppdatera när du skapar dem, till exempel datum eller beskrivning.
* Skapa poster baserat på ett dokument som du laddar upp. Workfront har stöd för följande dokumentformat för AI Assistant:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT och de flesta bildformat
* Uppdatera fält för de poster som visas på skärmen
* Ta bort poster
* Återställa poster som du precis har tagit bort


## Leta reda på AI-assistenten i Workfront Planning

Du hittar AI Assistant i följande områden i Workfront Planning:

* Huvudnavigeringsfältet i det övre högra hörnet av skärmen.
* I informationsområdet för en post, efter att du har öppnat posten i förhandsgranskningen eller efter att du har öppnat postens sida.

## Få åtkomst till AI-assistenten i planeringsområdet

1. Logga in på Workfront och klicka sedan på **huvudmenyikonen** ![Dots huvudmeny](assets/dots-main-menu.png) i det övre högra hörnet av skärmen, eller **på huvudmenyikonen** ![Linjer huvudmeny](assets/lines-main-menu.png) i det övre vänstra hörnet, om den är tillgänglig.

. Klicka på **Planering**. Området Planering öppnas.

1. Klicka på ett **arbetsytekort**.

1. (Valfritt) Klicka på ett kort **för en** posttyp.

1. (Valfritt) Klicka på en **post** för att öppna postens **informationssida** .

1. Klicka på ikonen **för** AI Assistant i det övre högra hörnet av skärmen i det globala navigeringsfältet eller i det övre högra hörnet av postens förhandsgranskning eller sida.

   ![Ikon för AI Assistant](assets/ai-assistant-icon-highlighted.png)

1. I det avsedda utrymmet börjar du skriva kommandon för AI Assistant och klickar sedan på Enter när du är klar.

   ![AI Assistant-panel med tom kommandoruta](assets/ai-assistant-panel-with-empty-command-box.png)

   Du kan till exempel skriva något av följande:

   * Skapa en kampanj med startdatumet den 4 juli och slutdatumet den 30 juli
   * Uppdatera fältet Beskrivning i posten för sommarkampanjen med ett datum som ska fastställas
   * Ta bort den senaste posten
   * Återställa posten

   En visuell indikator visas medan AI Assistant bearbetar kommandon och ställer in förväntningar på svarstiden.

   När du har fått ett lyckat svar följer du länkarna eller märker ändringarna till vänster.




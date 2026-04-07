---
title: Andra kvartal 2026 - förbättringar av företagsfunktioner
description: Andra kvartal 2026 - förbättringar av företagsfunktioner
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 72130462-ae78-4b9b-ae18-848602d4a858
source-git-commit: 59a9725e7697a81be2a827a902ee3d23085a2ecd
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# Andra kvartal 2026 - förbättringar av företagsfunktioner

Den här sidan beskriver förbättringar av företagsåtgärder som gjorts i andra utgåvan av kvartalet 2026 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den andra utgåvan av kvartal 2026 finns i [Översikt över den andra utgåvan av kvartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Enterprise Operations Capabilities finns nu i Adobe Workfront

>[!NOTE]
>
>Förhandsgranska: 2 april 2026
>Production fast release: 15 april 2026
>Produktion för alla: 16 april 2026

Avancerade funktioner från Adobe Workfront är ett enhetligt och skalbart sätt att hantera ekonomi, projekt och företagsåtkomst. Dessa funktioner ger den synlighet och kontroll som företag behöver för att arbeta lönsamt och effektivt.

### Avancerad ekonomisk hantering

>[!NOTE]
>
>De här funktionerna är bara tillgängliga för organisationer i Workflow Ultimate-paketet.

Prognosera, spåra och optimera er ekonomi med kostnads- och faktureringshierarkier på flera nivåer.

Bland förbättringarna av den ekonomiska förvaltningen finns:

* **Graderingsattribut**, som gör att du kan lägga till ytterligare dimensioner till andra nivåer än jobbrollen, så att priset kan variera inte bara efter jobbroll utan även efter faktorer som byrå, plats, varumärke, kostnadsställe eller andra. Genom att kombinera dessa attribut kan Workfront automatiskt välja rätt grad för tilldelningar, vilket garanterar att alla projekt är ekonomiskt korrekta och konsekventa.

  Mer information finns i [Definiera tariffattribut](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

* **Betygsätt kort**, som tillhandahåller ett strukturerat sätt att hantera kundspecifik fakturering, som kombinerar rollbaserade priser och anpassningsbara attribut för att säkerställa korrekt och kontrollerad projektkostnad.

  Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) och [Koppla ett tariffkort till ett projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

* En ny kostnads- och intäktstyp med namnet **Användare och roll per timme**. När den här uppgiftstypen tilldelas, bestämmer en avancerad tariffhierarkilogik fakturerings- och kostnadstariffer från olika nivåer, inklusive tariffkort, projektet, tilldelningen, jobbrollen och användarprofilen. Användare och Roll-timmar är den enda kostnads- och intäktstypen som du kan använda för att tillämpa tariffattribut och tariffkort.

  Mer information finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

* En omdesignad **upplevelse av avancerade uppdrag** med utökad konfigurerbarhet ger bättre synlighet och kontroll över hastigheter, tidsramar och egenskaper.

  Mer information finns i [Skapa avancerade uppdrag](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

  >[!NOTE]
  >
  >Före produktionsreleasen den 16 april kommer en ny version att läggas till så att du kan välja mellan den gamla och den nya versionen av avancerade uppdrag. Den gamla upplevelsen förblir standard.

* En **jobbroll för fakturering**, som gör att du kan fakturera en användare med en annan jobbroll än den primära jobbrollen. Detta är användbart när en person tillfälligt utför arbete som ska faktureras till en annan avgift.

  Mer information finns i [Konfigurera en jobbroll för fakturering](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

* Datumgällande **växelkurser**.

  Mer information finns i [Konfigurera valutakurser](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

* Möjligheten att lägga till en multiplikator för **övertid för aktiviteter**, som multiplicerar alla planerade timmar för den uppgiften och påverkar beräkningarna av planerade intäkter.

  Mer information finns i [Definiera en övertidskvot](/help/quicksilver/manage-work/projects/project-finances/define-overtime-ratio.md).

* En kontroll på projektnivå för att **bevara all faktureringsinformation** och förhindra framtida ändringar.

  Mer information finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* **Ett jobbrollalias**, som definieras på ett tariffkort. När hastighetskortet är kopplat till ett projekt visas aliaset på information som platshållartilldelningar, utgifter och rapporter i stället för den interna jobbrollens namn.

  Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

### Spårning av historiska data

Använd **projektögonblicksbilder** för att hantera projekt effektivare och fatta välgrundade beslut.

Mer information finns i [Skapa och visa projektögonblicksbilder](/help/quicksilver/manage-work/projects/create-projects/create-snapshots.md).

>[!NOTE]
>
>* Ögonblicksbilder av projekt är bara tillgängliga för organisationer i Workflow Ultimate-paketet.
>* Ögonblicksbilder av produkter kommer inte att ha någon förhandsversion och kommer att släppas direkt till Production den 16 april.

### Enterprise permissions

**Affärsprofiler** ger säker, skalbar systemåtkomst och hjälper till att stärka företagsstyrningen.

Mer information finns i [Översikt över affärsprofiler](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md).

>[!NOTE]
>
>Affärsprofiler är bara tillgängliga för organisationer i Workflow Ultimate-paketet.

Behörigheter att visa både kostnads- och faktureringsdata har dessutom separerats från de allmänna behörigheterna för ekonomi, både i åtkomstnivåer för användare och i objektbehörigheter. Mer information finns i [Bevilja åtkomst till ekonomiska data](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) och [Dela ekonomiska behörigheter för ett objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

>[!NOTE]
>
>Separata kostnads- och faktureringsbehörigheter är tillgängliga för organisationer på alla Workfront- och arbetsflödespaket.

### Förbättringar av anpassade formulär och fält

Avancerad logik i skräddarsydda formulär ger tydligare insikter och exaktare projekthantering och finansiell hantering.

Förbättringarna av anpassade formulär är bland annat:

* Nya **avancerade logiktyper**: avancerad visning, standardvärde, villkorsstyrd formatering och redigerbarhet

  Mer information finns i [Lägga till logiska regler i anpassade formulär och fält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

  >[!NOTE]
  >
  >De nya logiktyperna är bara tillgängliga för organisationer i Workflow Prime- och Ultimate-paketen.

* Förbättringar av gränssnittet för formulärdesignern:
   * Formulärnamnet visas nu längst upp till vänster i designern, så att du kan se namnet i ett långt formulär när du rullar.
   * Objekttyper som formuläret kan koppla till finns i en listruta.
   * Du kan välja att visa eller dölja logiska indikatorer i fälten, för alla logiktyper. Visa och hoppa över logiktyper visar indikatorer för båda de påverkade fälten. Alla andra logiktyper påverkar ett fält.

  Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

  >[!NOTE]
  >
  >De här funktionerna är tillgängliga för organisationer på alla Workfront- och Workflow-paket.

* Möjlighet att lägga till anpassade formulär till team, rankningskort och jobbroller.

  Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

  >[!NOTE]
  >
  >* Om du vill lägga till anpassade formulär för att betygsätta kort och jobbroller måste du ha Ultimate-paketet Workflow.
  >* Det går att lägga till anpassade formulär till team för organisationer i alla Workfront- och Workflow-paket.

* En inställning av typen **Ekonomisk behörighet** för valutaformaterade fält, som endast tillåter åtkomst för användare som har vissa behörigheter angivna i åtkomstnivåerna.

  Mer information finns i [Begränsa åtkomst till ekonomiska data i anpassade fält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/restrict-access-to-financial-data.md).

  >[!NOTE]
  >
  >Den här funktionen är tillgänglig för organisationer på alla Workfront- och Workflow-paket.

### Förbättrade layoutmallar

>[!NOTE]
>
>De här funktionerna är tillgängliga för organisationer på alla Workfront- och Workflow-paket.

I layoutmallar kan du anpassa sidhuvuden och vänsternavigeringsmenyer för ytterligare objekt och enklare visa och dölja objekt på huvudmenyn. Du kan också använda en layoutmall för att avgöra vilka alternativ som visas när en användare klickar på menyn **Mer** (menyn med tre punkter) för projekt, uppgifter, utgåvor, portföljer och program.

Mer information finns i [Skapa och hantera layoutmallar](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Anpassad lokalisering

>[!NOTE]
>
>Den här funktionen är endast tillgänglig för organisationer som har Workflow Prime- eller Ultimate-paket.

Med anpassad lokalisering kan du definiera anpassade termer och fraser på olika språk. Workfront visar sedan dessa termer på det språk som angetts i webbläsarinställningarna.

Du kan till exempel ställa in etiketten &quot;Målpublik&quot; till att översätta till det tyska ordet &quot;Zielgruppe&quot;. Alla användare med tyskt format som språk för sina Adobe IMS-konton ser ordet&quot;Zielgruppe&quot; som etikett för alla fält med namnet&quot;Target Audience&quot; på engelska.

Mer information finns i [Konfigurera anpassad lokalisering](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md).

### Automatisera åtgärder med affärsregler

>[!NOTE]
>
>De här funktionerna är bara tillgängliga för organisationer i Workflow Ultimate-paketet.

Workfront-administratörer kan nu konfigurera affärsregler för att automatisera åtgärder för det skapade, redigerade eller ändrade objektet när vissa villkor uppfylls. Tillgängliga åtgärder kan vara att dela objektet eller bifoga ett anpassat formulär till objektet.

Mer information finns i [Skapa och redigera affärsregler](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

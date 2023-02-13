---
title: 2.2 Administratörsförbättringar
description: 2.2 Administratörsförbättringar
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 0%

---

# 2.2 Administratörsförbättringar

Den här sidan beskriver alla administratörsförbättringar som gjorts i version 2.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

den 4 april 2022. En lista över alla ändringar som är tillgängliga i version 2.2 finns i [22.2 Versionsöversikt](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Konfigurera ett anpassat formulär som ska fungera med flera objekttyper

Nu kan du konfigurera ett nytt eller befintligt anpassat formulär så att det fungerar med flera objekttyper, vilket gör formuläret mycket mer användbart. Användarna kan bifoga och fylla i formuläret på objekt av alla typer som du konfigurerar det för.

Tidigare kunde du konfigurera ett anpassat formulär så att det bara fungerar med en objekttyp.

Den här funktionen fungerar med alla anpassade formulär som skapats tidigare i ditt Workfront-system. Om du till exempel redan har ett anpassat formulär som har skapats för objekttypen Task kan du nu konfigurera formuläret så att det även fungerar med andra objekttyper, till exempel Projekt och Problem.

Mer information finns i avsnittet [Börja skapa ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) i artikeln [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* Vid den första förhandsversionen av den här funktionen inaktiverades möjligheten att kopiera ett anpassat formulär med flera objekt tillfälligt. Denna möjlighet aktiverades den 24 mars. Mer information om hur du kopierar ett anpassat formulär finns i [Kopiera ett anpassat formulär och skapa ett nytt](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* I ett beräknat anpassat fält är vissa fält som du refererar till kanske inte kompatibla med objekttyper som har konfigurerats för formuläret. Vår lösning är ett jokertecken som gör det möjligt att beräkna olika värden beroende på vilket objekt som formuläret är kopplat till. Vi lade till jokertecknet den 24 mars. Mer information om hur du använder programmet finns i avsnittet [Beräknade anpassade fält i anpassade formulär med flera objekt](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) i artikeln [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* För avsnittsbrytningar i anpassade formulär har vi skapat en uppsättning gemensamma visnings- och redigeringsbehörigheter som fungerar för alla objekttyper som du kan konfigurera för ett formulär. I ett scenario har vi funnit att en av dessa behörigheter, Begränsad redigering, kan orsaka fel i ett formulär. Den här lagades den 24 mars. Mer information om avsnittsbrytningar finns i [Lägga till en avsnittsbrytning i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>


## Katalogen med utkast är tillgänglig för alla användare, och administratörer kan tillåta förfrågningar

Alla Adobe Workfront-användare kan nu bläddra i katalogen med tillgängliga ritningar. Mer information finns i [Bläddra i katalogen med ritningar och begär installation av ritningar](../../../administration-and-setup/blueprints/browse-catalog.md).

Dessutom kan systemadministratören ge användare åtkomst att begära installation av ritningar. Om du tilldelar en begärandekö för att lagra begäranden kan användarna göra förfrågningar från katalogen med utkast. Mer information finns i [Konfigurera åtkomst till ritningar](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Lägga till en bild i ett anpassat formulär

I ett anpassat formulär som du skapar eller redigerar kan du nu lägga till en bild och inkludera ett informativt eller instruktivt verktygstips som användare kan läsa när de för muspekaren över den.

Det kan vara praktiskt att t.ex. visa varumärken för en ny produkt eller för att ge visuell information som människor behöver när de fyller i formuläret.

Tidigare var anpassade formulär helt textbaserade.

>[!NOTE]
>
>I de nya Adobe Workfront-upplevelseområdena som ännu inte har moderniserats, till exempel den ruta som visas när du redigerar objekt i grupp, visas inte anpassade formulärbilder. De visas allt eftersom vi fortsätter att uppdatera dessa områden.

Mer information finns i [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Nya standardkonfigurationer för åtkomstnivå

För att bättre passa behoven hos de flesta administratörer som skapar nya åtkomstnivåer har vi ändrat standardkonfigurationen för alternativen&quot;Finjustera dina inställningar&quot; nedan. Dessa visas när du klickar på kugghjulsikonen ![](assets/gear-icon-in-access-levels.png) på knappen Redigera.

Alla dessa ändringar inaktiverar ett alternativ som tidigare var aktiverat som standard. Om detta inte passar organisationens behov kan du aktivera dem när du skapar en ny åtkomstnivå eller när som helst senare.

>[!IMPORTANT]
>
>Den här standardkonfigurationsändringen påverkar bara åtkomstnivåer som du skapar från och med nu, inte de som du har skapat tidigare.

* På en ny åtkomstnivå med en planlicenstyp:

   * Dela hela systemet är nu inaktiverat för projekt, uppgifter, utgåvor, portfolior, program, rapporter, filter, dokument och mallar.
   * Visa inbyggda rapporter och Dela rapporter offentligt är också inaktiverat för rapporter.
   * Dela dokument offentligt är även inaktiverat för dokument.

* På en ny åtkomstnivå med en arbetslicenstyp:

   * Delning i hela systemet är nu inaktiverat för filter och dokument.
   * Dela dokument offentligt är även inaktiverat för dokument.

* På en ny åtkomstnivå med en Request- eller Review-licenstyp:

   * Delning i hela systemet är nu inaktiverat för filter.

## Inaktivera en grupp

När de interna organisationerna förändras kan du behöva sluta använda vissa grupper i Workfront och skapa nya. För att underlätta detta har vi lagt till möjligheten att inaktivera en grupp utan att förlora sina historiska data. För vanliga användare som inte behöver se dem rensas inaktiva grupper från grupptypsnittsfält.

Du kan fortfarande hitta och konfigurera alternativ, inställningar och objektassociationer för inaktiva grupper som du hanterar. Om du inaktiverar en grupp ändras inte något om objekten som gruppen är kopplad till.

Tidigare var det inte möjligt att inaktivera en grupp.

Mer information finns i [Inaktivera eller återaktivera en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Förbättrad installationshistorik för utkast

När du installerar en plan visar ett meddelande nu de specifika objekt (t.ex. roller, team eller grupper) som har installerats med planen och eventuella objekt som inte gick att installera. Du kan även visa listan över installerade objekt på sidan Information om utkast genom att klicka på Visa detaljer bredvid en specifik installation i tabellen över installationshistorik.

Mer information finns i [Installera en plan](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## En varning visas nu när du installerar en plan för endast förhandsgranskning i produktionen

Vissa utkast är bara tillgängliga för installation i förhandsvisningsmiljön i testsyfte.

Om du har tillgång till innehåll som bara är för förhandsgranskning i din produktionsmiljö, i sandlåda 1 eller i sandlåda 2, är installationsknappen inte aktiv, och du kan se ett varningsmeddelande.

Mer information finns i [Installera en plan](../../../administration-and-setup/blueprints/blueprints-install.md).

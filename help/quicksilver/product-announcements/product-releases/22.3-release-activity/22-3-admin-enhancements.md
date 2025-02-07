---
title: 2.3 Administratörsförbättringar
description: 2.3 Administratörsförbättringar
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 2.3 Administratörsförbättringar

Den här sidan beskriver alla administratörsförbättringar som gjorts i version 2.3 till förhandsvisningsmiljön. Dessa förbättringar gjordes tillgängliga den 11 juli 2022. En lista över alla ändringar som är tillgängliga i version 2.3 finns i [2.3 versionsöversikt](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrera Adobe Workfront med JumpSeat

Nu kan du integrera JumpSeat med Workfront för att skapa anpassad produktvägledning för dina användare. Du måste ha en Adobe Workfront Enterprise-licens och en aktiv JumpSite-prenumeration för att kunna aktivera integreringen.

Mer information finns i [Konfigurera JumpSite-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Korrekturinställningar har flyttats till Workfront

Nu kan du redigera följande korrekturinställningar i Workfront Setup Area:

* Korrekturinställningar

* Inställningar för beslutsbevis

Mer information finns i [Konfigurera standardkorrekturinställningar](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Använda olåsta statusvärden i en godkännandeprocess

**Obs!** Borttagen från 22.3-produktionsversionen. Den här funktionen är planerad att lanseras till Production den 15 september 2022.

För att du ska få större kontroll över godkännandeprocesserna och statusvärdena i ditt system har vi gjort det möjligt att skapa en godkännandeprocess som baseras på en olåst systemstatus. Dessutom kan du nu låsa upp status som redan används i en godkännandeprocess.

Tidigare var det nödvändigt att låsa en systemstatus som användes i en godkännandeprocess. Detta gjorde den tillgänglig för alla grupper - utan möjlighet att ta bort eller byta namn på den - så att gruppadministratörerna inte kunde effektivisera sin grupps lista över statusar efter deras specifika behov.

Mer information finns i följande artiklar:

* [Skapa en godkännandeprocess för arbetsobjekt](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Skapa eller redigera en status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Låsta och olåsta statusvärden på systemnivå](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Lägga till en PDF-fil i ett anpassat formulär

Vi fortsätter att hjälpa dig att göra anpassade formulär mer visuella och informativa med nya resurswidgetar som du kan lägga till, som bilder och videor. Nu kan du lägga till en länk till en PDF-fil i ett anpassat formulär. När formuläret är kopplat till ett objekt kan användare som arbetar med objektet visa och interagera med PDF i formuläret.

## Redigerare för beräkning av anpassat formulärfält visar felinformation

>[!NOTE]
>
>Den här funktionen är inte tillgänglig för tillfället. Den här sidan uppdateras när funktionen är tillgänglig.

Det är nu enklare att redigera beräkningar för anpassade fält eftersom felinformation som anges direkt i beräkningen är användbar. När du skapar ett beräknat fält i ett anpassat formulär markeras fel i rosa. När du hovrar över den markerade delen visas ett verktygstips som beskriver vad problemet är.

## Anpassning av projekthuvud

Som Workfront- eller gruppadministratör kan du nu anpassa fälten som visas i ett projekts sidhuvud när du använder en layoutmall.

Uppdateringen innehåller följande förbättringar:

* Ta bort befintliga fält från projekthuvudet.

* Lägg till nya, icke-redigerbara fält för projektöversikt. Du kan inte lägga till anpassade fält eller fält som kan redigeras. Redigerbara fält som finns i projekthuvudet kan finnas kvar i rubriken.

* Objektrubriken kan innehålla upp till fem fält.


Före den här versionen gick det inte att anpassa fälten i objektrubrikerna.

Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Kontrollera att ett tomt projekt skapas

Som system- eller gruppadministratör kan du nu styra om användare ska kunna skapa tomma projekt utan att använda en mall. Vi har introducerat en ny inställning under Projektinställningar som gör att du kan inaktivera skapandet av tomma projekt i följande områden:

* Från alternativet Nytt projekt i en lista med projekt

* När ett problem konverteras till ett projekt från utgivningssidan


Den nya inställningen är&quot;Tillåt användare att skapa projekt utan att använda en mall&quot; och den är som standard aktiverad.

**Obs!** Användare kan fortfarande konvertera en aktivitet till ett tomt projekt.

Mer information finns i [Konfigurera systemomfattande projektinställningar](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Inaktivera en grupp från gruppsidan

Nyligen har vi lagt till möjligheten att inaktivera och återaktivera grupper. För att göra den åtgärden snabbare och enklare har vi lagt till den på en grupps sida. När du har klickat på en grupps namn för att gå till dess sida kan du nu markera ikonen Mer ![Huvudmeny](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) bredvid gruppens namn och sedan välja Inaktivera eller Återaktivera.

Tidigare kunde du bara inaktivera eller återaktivera en grupp med kryssrutan Är aktiv på detaljsidan.

Mer information finns i [Inaktivera eller återaktivera en grupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Lägga till videoklipp i anpassade formulär

Nu kan du skapa ett nytt sätt för information, visuellt intresse och kreativitet i ett anpassat formulär genom att lägga till en video. När formuläret är kopplat till ett objekt kan användare som arbetar med objektet spela upp videon när som helst.

Tidigare kunde du bara lägga till textbaserade fält och bilder i ett anpassat formulär.


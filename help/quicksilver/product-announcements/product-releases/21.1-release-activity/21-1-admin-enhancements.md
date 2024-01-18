---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatera
navigation-topic: product-releases
title: 21.1 Förbättringar av administratörer
description: Den här sidan beskriver alla administratörsförbättringar som gjorts i version 21.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 15 februari 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 21.1 Förbättringar av administratörer

Den här sidan beskriver alla administratörsförbättringar som gjorts i version 21.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 15 februari 2021.

En lista över alla ändringar som är tillgängliga i version 21.1 finns i [21.1 - versionsöversikt](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Ny åtkomstnivåinställning för kopiering av projekt

För att du som systemadministratör ska få större kontroll över vad planerare kan göra med ett projekt har vi gjort redigeringsåtkomsten till projekt på åtkomstnivån mer detaljerad genom att införa en ny inställning som gör att du kan aktivera eller inaktivera möjligheten att kopiera projekt. När du aktiverade användarnas åtkomst till redigeringsprojekt hade de automatiskt åtkomst till att kopiera dem före den här ändringen. Med den nya funktionen kan du ge någon åtkomst till redigeringsprojekt utan att nödvändigtvis ha tillgång till kopiera dem genom att inaktivera den nya inställningen Kopiera.

Om dina användare hade åtkomst till Redigera-projekt på sin åtkomstnivå innan den här ändringen gjordes, aktiveras inställningen automatiskt när den här funktionen släpps.

Mer information om åtkomstnivån Planera finns i [Bevilja åtkomst till projekt](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Mer information om hur du kopierar ett projekt finns i [Kopiera ett projekt](../../../manage-work/projects/manage-projects/copy-project.md).

Den här funktionen ingår nu i [Grundläggande om administratörer i den nya Workfront-upplevelsen, del 1: Användarorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) utbildningsväg på Workfront One.

## I ett anpassat formulär på ett objekt markerar du alla objekt i ett flervalsfält

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig när du skickar in en ny begäran.

När du fyller i ett flervalsfält i ett anpassat formulär på informationssidan för ett objekt kan du klicka på Markera alla om du behöver markera alla tillgängliga alternativ.

Mer information om hur du redigerar data i ett anpassat formulär finns i [Redigera information i anpassade formulärfält](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Beräkna om alla anpassade formulärfält för ett objekt

Nu är det enklare att se till att alla data i beräknade anpassade fält är aktuella för ett objekt. Med det nya menyalternativet Beräkna om uttryck kan du snabbt beräkna om alla data i dessa fält.

Detta är särskilt användbart när någon har redigerat data i ett annat objekt som refereras av ett beräknat anpassat fält i objektet.

Tidigare var användarna tvungna att använda tillfälliga lösningar för att säkerställa att alla data i beräknade anpassade fält var aktuella. De redigerade till exempel objektet tillsammans med andra objekt för att använda det omberäkningsalternativ som är tillgängligt för massredigering.

Mer information finns i [Redigera information i anpassade formulärfält](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Lås upp uppgifter och utgivningsinställningar för gruppadministratörer

>[!NOTE]
>
>Fram till 24 juni 2021 var detta endast tillgängligt som en del av en fasad utrullning för kunder som har möjlighet att låsa upp projektinställningar för grupper. Nu finns det för alla kunder.

Adobe Workfront-administratörer kan nu ge gruppadministratörer mer självbestämmande genom att låsa upp enskilda uppgifter och utgåvor. När en inställning är olåst kan gruppadministratörer konfigurera den för sina grupper så att den passar varje grupps unika behov och interna processer.

Mer information finns i [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Den här funktionen ingår nu i [Grundläggande om administratörer i den nya Workfront-upplevelsen, del 2: Projektinställningar](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) utbildningsväg på Workfront One.

## Konfigurera åtkomstnivåinställningar för portföljer och program separat

Nu är det enklare att hantera användaråtkomst till portföljer och program eftersom du kan konfigurera deras åtkomstnivåinställningar separat.

Tidigare kombinerades inställningarna för åtkomstnivå för portföljer och program. Detta innebar att du inte kunde konfigurera åtkomstinställningar för program utan att konfigurera dem på samma sätt för portföljer, och det var samma sak som för portföljer.

Mer information om hur du konfigurerar en åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Mer information om åtkomstinställningar som du kan konfigurera för program och portföljer finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Den här funktionen ingår nu i [Grundläggande om administratörer i den nya Workfront-upplevelsen, del 1: Användarorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) utbildningsväg på Workfront One.

## Markera alla kryssrutor i en serie när du redigerar information i ett anpassat formulär

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig när du skickar in en ny begäran.

När du fyller i ett fält för anpassat formulär som innehåller kryssrutor på informationssidan för ett objekt kan du klicka på Markera alla om du behöver markera alla kryssrutor som är tillgängliga.

Det här alternativet visas bara om fältet innehåller fler än två kryssrutor.

Mer information finns i [Redigera information i anpassade formulärfält](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Konfigurera din Workfront-e-postadress tillåtelselista

För att skydda dina data bättre kan du nu använda en e-postdomän som tillåtslista till:

* Styr var Workfront e-postmeddelanden kan skickas om de innehåller rapporter eller dokument som lagras i Workfront
* Kontrollera e-postdomäner i den e-postadress som användarna kan ange i sina användarprofiler

Om du t.ex. vill skydda känsliga data, t.ex. en rapport med en lista över dina riskkunder, kan du bara inkludera din interna e-postdomän eller domäner i e-postmeddelandet som tillåtslista. På så sätt kan användare inte skicka den rapporten (eller någon annan Workfront-rapport) till en extern e-postadress.

Mer information finns i avsnittet [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) i artikeln [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Tilldela en gruppadministratör för en undergrupp

För att göra det enklare för olika nivåer i organisationen att arbeta oberoende har vi lagt till möjligheten att tilldela en gruppadministratör till en undergrupp. Nu kan du se till att du delegerar hantering av undergrupper till rätt personer.

Tidigare var det bara en grupp på den översta nivån som kunde ha gruppadministratörer och dessa administratörer hanterade alla undergrupper under den översta gruppen.

Mer information finns i avsnittet [Gruppadministratörer för undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) i artikeln [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Den här funktionen ingår nu i [Grundläggande om administratörer i den nya Workfront-upplevelsen, del 1: Användarorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) utbildningsväg på Workfront One.

## Konfigurera händelsemeddelanden för grupper

>[!NOTE]
>
>Finns endast som en del av den stegvisa lanseringen för kunder som kan låsa upp projektinställningar för grupper. Detta omfattar alla kunder i kluster 4 och 6 samt ett litet antal kunder i andra kluster. Den här anteckningen uppdateras när funktionen blir tillgänglig för fler kluster.

Workfront-administratörer kan nu ge gruppadministratörer större självständighet genom att tillåta dem att konfigurera händelsemeddelanden för sina toppnivågrupper. Undergrupper ärver händelseaviseringskonfigurationer från den översta överordnade gruppen.

Tidigare var händelsemeddelanden bara konfigurerbara av en Workfront-administratör på systemnivå, vilket innebär att alla grupper måste använda samma uppsättning händelsemeddelanden.

Mer information finns i följande artiklar:

* [Lås upp eller lås konfigurationen av händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Visa och konfigurera händelseaviseringar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Den här funktionen ingår nu i [Grundläggande om administratörer i den nya Workfront-upplevelsen, del 1: Användarorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) utbildningsväg på Workfront One.

Den här funktionen ingår nu i [E-post och meddelanden i appen i den nya Workfront-upplevelsen](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) utbildningsväg på Workfront One.

## Arbeta med gruppprojekt och godkännandeprocesser i området Grupper

Om du är gruppadministratör är det enkelt att visa och arbeta med gruppens projekt och godkännandeprocesser nu när de listas i gruppområdet. Från en grupps huvudsida kan du:

* Klicka på Projekt på den vänstra menyn för att visa gruppens projekt och skapa nya för gruppen. Om ett markerat projekt har delats med dig kan du använda knapparna i verktygsfältet för att redigera, exportera, kopiera eller ta bort det.

  Mer information finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Klicka på Godkännanden på den vänstra menyn för att visa och hantera alla godkännandeprocesser som är kopplade till gruppen.

  Mer information finns i [Godkännandeprocesser på gruppnivå](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Den här funktionen är även tillgänglig för Workfront-administratörer.

## Visa antalet licenser som används och tilldelas i en grupp

För att avgöra hur bra licenserna distribueras kan du nu visa antalet licenser som används i en grupp och eventuella undergrupper under den.

Om du hanterar en grupp på den översta nivån kan du visa både antalet licenser som används i en grupp (och dess undergrupper) och det maximala antalet licenser som tilldelas för gruppen.

Mer information finns i [Visa antalet licenser som tilldelats och används i en grupp i den nya Adobe Workfront-upplevelsen](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).


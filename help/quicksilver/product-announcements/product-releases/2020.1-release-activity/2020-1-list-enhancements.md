---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Förbättringar av 2020.1-listan
description: Den här sidan beskriver alla förbättringar som gjorts i Listor i version 2020.1. Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön i slutet av mars eller början av april 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efe05da7-ec25-4fbd-a7f9-645364d3e2a8
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# Förbättringar av 2020.1-listan

Den här sidan beskriver alla förbättringar som gjorts i Listor i version 2020.1. Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön i slutet av mars eller början av april 2020.

En lista över alla ändringar som är tillgängliga i version 2020.1 finns på [Översikt över version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Nytt sparningsläge när du gör ändringar i en uppgiftslista: tidslinjens planeringsläge

Beroende på projektets storlek och komplexitet kan det ta längre tid än du önskar att uppdatera uppgiftslistan, särskilt datum och varaktighet. För att göra redigeringarna mycket snabbare har vi introducerat ett nytt sparalternativ när vi redigerar uppgifter i en lista som kallas tidslinjeplaneringsläge. Före det här läget kan du spara ändringarna i uppgiftslistorna automatiskt med Spara automatiskt eller manuellt när du inaktiverar flyttningen automatiskt.

Tänk på följande när du använder tidslinjeplaneringsläget för att spara ändringarna i en uppgiftslista:

* Workfront använder en ny vy med färre fält i uppgiftslistan. På så sätt kan du fokusera på de viktigaste fälten som kan påverka projekttidslinjen.
* Det går snabbare att skicka varje ändring än när du använder läget för att spara automatiskt eller manuellt.
* Du kan ångra ändringarna innan du sparar dem.

Mer information om hur du sparar ändringar i en uppgiftslista finns i avsnittet Redigera uppgifter med planeringsinställningen för tidslinjen i artikeln [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Uppdaterat utseende och känsla för nya listor

>[!NOTE]
>
>När de här funktionerna ursprungligen släpptes för förhandsgranskning var de tillgängliga för alla rapporter och listor utom listorna i inställnings- och rapportområdena. De här funktionerna är nu bara tillgängliga för projekt-, uppgifts- och timlistor.

Listorna Projekt, Uppgifter och Timmar har nu ett uppdaterat utseende och känsla.

Mer information om hur du visar objekt i listor finns i [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Några av uppdateringarna är:

* Ett snabbfilter för att snabbt hitta objekt i listan
* En renare, rutnätsliknande design
* Uppdaterade färger och teckensnitt
* Kolumnrubriker är lättare att läsa
* Det är enklare att läsa textbundna redigeringsfunktioner

## Förbättrad navigering i alla nya listor med tydlig gruppering

Nu kan du se skillnaden mellan flera lager med grupperingar i listor med ett nytt färgschema tydligare. Grupperingsresultaten visas också tydligare i en separat ram. Den här ändringen har tillämpats på alla nya listor.

Mer information om hur du skapar och anpassar grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Markera matchande objekt i listor när du använder snabbfiltren

Det går nu snabbare att hitta objekt i listor: när du söker efter ett objekt med snabbfilter markeras de matchande fälten med gult i resultaten så att du tydligt kan se vilket fältvärde som matchar nyckelordet. Fälten markeras med gult i fristående fält, liksom delade kolumner och komplexa fält. Exempel på komplexa fält är uppdrag, uppdrag och status, Procent färdigt, Föregående, Godkännare och status, Resurshanterare, Kategorier, Villkor, Uppdatera villkor osv.

Mer information om hur du använder snabbfilter finns i [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Begränsa användarnas möjlighet att redigera filter-, vy- och grupperingskontroller i listor och rapporter

Nu kan du använda en åtkomstnivå för att begränsa användarnas möjlighet att redigera kontrollerna Filter, Visa och Gruppering i listor och rapporter. Detta är användbart om du har anpassade fält som du bara vill ska vara synliga för användare på en viss åtkomstnivå.

Mer information finns i [Bevilja åtkomst till filter, vyer och grupperingar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

## Menyn Ny information i uppdateringsområdet

Använd menyn Mer på en uppdatering för att:

* Kopiera brödtexten i en uppdatering
* Kopiera den direkta länken till en uppdateringstråd eller en enskild uppdatering
* Ta bort en uppdatering

Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Ny förloppsindikator i uppdateringsområdet

Förloppsindikatorn för procent färdigt i uppdateringsområdet har ett nytt utseende. Klicka och dra om du vill uppdatera procentvärdet eller dubbelklicka om du vill ange talet manuellt.

Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visa kolumnrubriker i listor och rapporter i inledande versal

I en tidigare version har vi gjort en ändring som visar alla kolumnrubriker med versaler när du visar en lista eller rapport. Baserat på den feedback vi har fått återställer vi nu den här ändringen. Med den här ändringen visas nu alla kolumnrubriker med inledande versal.

## Nytt alternativ för att ange hur grupperingsresultat ska visas i listor

>[!NOTE]
>
>Det här alternativet har tagits bort från Workfront Classic Preview-miljön och kommer inte att ingå i version 2020.1.

För att du ska få större kontroll över hur du visar listresultaten kan du nu ange om du vill att resultaten i grupperingen ska expanderas eller komprimeras som standard när du visar listan eller rapporten. Det här alternativet är tillgängligt i grupperingsverktyget i en lista eller rapport.

Som standard visas resultatet i en utökad lista under grupperingen.

Före den här ändringen visas alltid resultatet i en komprimerad lista.

Mer information om hur du skapar en gruppering finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

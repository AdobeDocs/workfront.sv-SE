---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Översikt över bankkort
description: Den flexibla Scrum-artikelpanelen visas tillsammans med slutförandestatus och nedladdningsschemat.
author: Jenny
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Översikt över [!UICONTROL Scrum]

<!-- Audited: 5/2025 -->

Den [!UICONTROL Scrum] flexibla artikelpanelen visas tillsammans med slutförandestatus och nedladdningsschemat. De här flexibla komponenterna är tillgängliga i följande situationer i [!UICONTROL Adobe Workfront]:

* På rörliga iterationer. Mer information om hur du använder den flexibla artikelpanelen, nedladdningsschemat och slutförandestatusen i en ren, flexibel miljö (med eftersläpningar och en upprepning) finns i [Arbeta i en flexibel miljö](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* När du visar ett projekt i en flexibel vy. Mer information om hur du kan använda den flexibla artikelpanelen, nedladdningsschemat och slutförandestatusen i ett befintligt projekt finns i [Hantera ett projekt i flexibel vy](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Agile iteration](assets/agile-iteration-with-callouts.png)

## Layout och funktioner för artikelanslagstavla

![Agile story board](assets/agile-storyboard-callouts.png)

Artikelpanelen består av följande element:

* **Överordnad artikelkolumn**: Till skillnad från de andra kolumnerna på artikelpanelen är kolumnen [!UICONTROL Parent Story] inte en aktivitetsstatus, utan finns för att placera artiklar som innehåller underaktiviteter i iteration eller projekt. Endast överordnade artiklar som har minst en underuppgift på artikelpanelen kan finnas i den här kolumnen. De överordnade artiklarna går inte från status till status över hela artikelpanelen.

  I en iteration visas den här kolumnen bara på artikelpanelen när en eller flera artiklar på artikelpanelen innehåller minst en underuppgift som uppfyller följande krav:

   * Tilldelad till samma flexibla team som den överordnade aktiviteten.
   * Tillhör iteration.

     I ett projekt visas den här kolumnen när som helst när en uppgift har minst en underaktivitet.

     ![Överordnad artikelkolumn](assets/agile-parentstory-swimlane.png)

* **Aktivitetsstatus**: Ange hur en artikel fortskrider genom iteration eller projekt baserat på vilken statuskolumn artikeln finns i.

  Du kan anpassa uppgiftsstatusvärden för projektet genom att ändra den flexibla vyn.

* **Swim Lane**: När en överordnad artikel och dess underaktiviteter visas på artikelpanelen skapas ett simfält specifikt för artikeln och dess underaktiviteter. Detta ger en visuell distinktion som bättre visar hur en artikels underuppgifter framskrider över hela artikelpanelen.

  I en iteration visas simbanor bara på artikelpanelen när en artikel på artikelpanelen innehåller minst en underuppgift som uppfyller följande krav:

   * Tilldelad till samma flexibla team som den överordnade aktiviteten.
   * Tillhör iteration.

  I ett projekt visas simbanor när en uppgift har minst en underuppgift eller en överordnad uppgift.

* **Enskilda artiklar**: Enskilda artiklar och problem visas under alla simbanor på artikelpanelen. Detta ger en visuell distinktion jämfört med de artiklar som är en del av ett simfält.

## Relation mellan underaktiviteter och artiklar

Om en artikel innehåller underuppgifter kan du inte uppdatera någon information om själva den överordnade artikeln (till exempel punkter/timmar eller procent färdigt). Dessutom kan du inte flytta artikeln över artikelpanelen för att uppdatera dess status. I stället återspeglas alla ändringar du gör i artikelns underuppgifter i artikeln. De kombinerade artikelpunkterna eller timmarna för alla underaktiviteter avgör den överordnade artikelns punkter eller timmar.

Om en artikel t.ex. bara har en underuppgift som har ett värde på 4 punkter, har artikeln också fyra punkter. Om du ändrar värdet för underaktivitetspunkten till 3 ändras punktvärdet för den överordnade artikeln till 3. Om du skapar en annan underaktivitet i samma artikel och anger punktvärdet för den underaktiviteten till 4, ändras punktvärdet för artikeln till 7 för att återspegla det kombinerade punktvärdet för båda underaktiviteterna.

Samma logik gäller för underaktiviteter på andra nivån (underaktiviteter för underaktiviteter). Om en underaktivitet har en eller flera underaktiviteter på andra nivån beräknas underaktiviteten utifrån underaktiviteterna på andra nivån.

## Förhållandet mellan artikelstyrelsen och eftersläpningen

I upprepningens efterlogg visas endast artiklar eller underaktiviteter där du kan ange en uppskattning. Om en överordnad artikel har underaktiviteter som visas på artikelpanelen (eftersom de har tilldelats samma flexibla team och tillhör upprepningen) visas inte den överordnade uppgiften i efterloggen. I det här fallet visas bara underuppgifterna i efterloggen, medan underuppgifterna och den överordnade artikeln visas på artikelpanelen.

Anta till exempel att artikel A innehåller underuppgift 1 och underuppgift 2 (och båda underuppgifterna tilldelas samma flexibla team). I det här fallet visas artikel A på artikelpanelen i ett simfält med Deluppgift 1 och Underuppgift 2. Endast underuppgift 1 och underuppgift 2 visas emellertid i efterloggen.

Samma logik gäller för underaktiviteter på andra nivån (underaktiviteter för underaktiviteter). Om en underuppgift har en eller flera underaktiviteter på andra nivån tilldelade till samma flexibla team och tillhör samma upprepning, visas endast underaktiviteten på andra nivån i efterloggen.

Mer information om eftersläpningen finns i [Hantera Agile-eftersläpningen](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

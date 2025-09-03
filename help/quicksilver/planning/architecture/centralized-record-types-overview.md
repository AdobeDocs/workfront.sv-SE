---
title: Översikt över centraliserade posttyper
description: Centraliserade posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Översikt över centraliserade posttyper


Centraliserade posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning.

## Översikt över centraliserade posttyper

När du implementerar Workfront Planning för en organisation med flera team och gemensamma arbetsflöden kan du behöva definiera en sammanhängande struktur och metadata för nyckelposttyper (som kampanjer och slutprodukter) som kan läggas till i varje teames arbetsytor för att fånga och hantera deras arbete.

Ni kan också behöva varje teames arbete för att komma upp på en central och mer global nivå.

I det här arbetsflödet kan du se till att teamen hämtar sitt arbete på ett enhetligt sätt samtidigt som de låser upp synligheten mellan team, utan att behöva lägga till alla i organisationen till en arbetsyta.

Så här använder du centraliserade posttyper:

1. Konfigurera en posttyp som ska centraliseras.

   Mer information finns i [Konfigurera funktioner för arbetsytan över flera arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Lägg till en befintlig posttyp från en centraliserad typ.

   Mer information finns i [Lägga till befintliga posttyper](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




・ En ny inställning,&quot;Tillåt att posttypen läggs till i andra arbetsytor&quot;, finns i Avancerade inställningar för posttyper.

・ Om den är aktiverad kan arbetsytehanteraren välja användare med standardlicens, team, grupper, roller eller företag som kan lägga till posttypen i de arbetsytor de hanterar.

・ Arbetsytehanteraren som redigerar inställningen läggs automatiskt till i listan över valda användare som standard

o Arbetsytehanteraren kan ta bort sitt eget namn efter att minst en annan entitet har lagts till

o Minst en användare/team/.. måste vara markerad för att inställningen ska kunna sparas

o När posttypen har lagts till på minst en annan arbetsyta kan alla markerade användare tas bort

§ Detta görs så att det inte går att lägga till den globala posttypen i nya arbetsytor, men behålla den i arbetsytor som redan använder den.

・ I fas 1 delas alla poster från de anslutna posttyperna automatiskt med den arbetsyta där posttypen har lagts till.

・ När posttypen är aktiverad som en arbetsyta som fungerar på olika sätt läggs ett systemgenererat&quot;Workspace&quot;-fält till i posttypen

o Den visar arbetsytan där varje post har skapats.

o Det här fältet är skrivskyddat och kan inte tas bort.

o Den kan döljas från visningsfält.

o Arbetsytefältet kan användas för att filtrera, gruppera och sortera, liksom i andra visningsinställningar, precis som andra fält.


Posttyper för flera Workspace-platser i lokala arbetsytor

・ När man försöker lägga till en ny posttyp på arbetsytan ser man ett alternativ att välja bland de globala posttyper som finns tillgängliga

・ När de väljer en av de globala posttyperna läggs den till direkt på arbetsytan

・ Det går att flytta den globala posttypen till valfritt avsnitt och var i den lokala arbetsytan


Behörigheter för den globala posttypen på lokala arbetsytor

Inom lokala arbetsytor får medlemmarna åtkomst till den globala posttypen:

・ I fas 1 får lokala arbetsytehanterare Contribute-behörighet. Detta innebär:

o Lokala arbetsytehanterare kan:

§ Lägg till den globala posttypen

§ Lägg till/redigera/ta bort alla poster i den globala posttypen, oavsett vilken arbetsyta posten lades till från.

§ Ta bort den globala posttypen från den lokala arbetsytan

o Lokala arbetsytehanterare kan inte:

§ Lägg till, redigera, ta bort fält

§ Uppdatera posttypens utseende och etikett

§ Se avancerade inställningar för posttyp

§ Hantera automatisering

§ Hantera förfrågningsformulär

§ Justera posttypsdelningen för arbetsytans omfång

§ Inaktivera den globala posttypsinställningen i avancerade inställningar.

・ Medverkande på den lokala arbetsytan får Contribute-behörighet för den globala posttypen och kan lägga till och hantera poster i den

・ Lokala visningsprogram får behörigheten Visa för den globala posttypen

・ Så snart en post läggs till i den globala posttypen från någon av de lokala arbetsytorna visas namnet på arbetsytan i Workspace-fältet

o För tillfället går det inte att redigera och ändra arbetsytefältet

・ Poster som läggs till på lokala arbetsytor samlas ihop och visas på den primära arbetsytan, och alla medlemmar på den primära arbetsytan får åtkomst till den.

・ Poster som läggs till på lokala arbetsytor visas inte på andra lokala arbetsytor som använder samma globala posttyp och deras medlemmar får inte åtkomst till posterna.



Åtkomst till anslutningar:

・ MVP-scope

o Posttyperna som är kopplade till den globala posttypen blir synliga för lokala arbetsytor där den globala posttypen läggs till så att de kan använda anslutningsfälten för att tagga


API-beteende

Om användaren försöker skapa poster i en global posttyp via API utan att ange arbetsytans ID, kontrollerar systemet om användaren har åtkomst att skapa poster på den primära arbetsytan (där den globala posttypen skapas)

・ Om ja, skapas posten i den primära arbetsytan

・ Om nej, får användaren ett valideringsfel om att han/hon inte har åtkomst till den primära arbetsytan och måste ange det arbetsyte-ID där han/hon har behörighet att skapa.
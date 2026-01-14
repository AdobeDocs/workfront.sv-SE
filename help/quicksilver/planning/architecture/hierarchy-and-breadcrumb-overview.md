---
title: Översikt över hierarki och vägbeskrivningar
description: Som arbetsytehanterare kan du definiera flexibla men strukturerade hierarkier mellan anslutna posttyper och andra objekttyper i Adobe Workfront Planning. Hierarkier är anslutningar mellan posttyper eller mellan posttyper och ett Workfront-projekt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 9a7ab1928bfd25c197fca65eddfba1bc01977ea7
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---



# Översikt över hierarki och vägbeskrivningar

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Som arbetsytehanterare kan du definiera flexibla men strukturerade hierarkier mellan anslutna posttyper och andra objekttyper i Adobe Workfront Planning.

Hierarkier är anslutningar mellan posttyper eller mellan posttyper och ett Workfront-projekt.

Mer information om hur du skapar hierarkier finns i [Skapa arbetsytehierarkier](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Nedan följer några fördelar med att använda hierarkier i dina arbetsytor:

* Organisera arbetet på ett sätt som återspeglar hur era team faktiskt planerar, arbetar och levererar.
* För att användarna ska förstå var de är, hur posttyperna ansluter och hur strategin flödar in i körningen genom att referera till en uppsättning vägbeskrivningar som anger deras plats i systemet.
* För att ge bättre navigering och skapa tydlighet och kontinuitet i alla arbetsflöden.
* För att definiera flöden som passar hur organisationen fungerar, med stöd för både flexibilitet och konsekvens i alla arbetsfaser.

## Att tänka på när du arbetar med hierarkier

* Du kan skapa upp till fem hierarkier för en arbetsyta.
* Du kan ha upp till fyra post- och objekttyper anslutna i en hierarki.
* Du kan bara ansluta följande objekttyper i en arbetsytehierarki:
   * Posttyper som tillhör den arbetsyta som du skapar hierarkierna i.
   * Workfront-projekt. Det går inte att lägga till Workfront-projekt som överordnade för andra posttyper. De är alltid den sista objekttypen i en hierarki.
* Du kan inte lägga till följande objekttyper i en hierarki:
   * Posttyper från andra arbetsytor, även när de är inställda som kopplingsbara eller globala posttyper. Du kan bara lägga till globala posttyper i hierarkier när de har lagts till på arbetsytan som du skapar hierarkin från.
   * Alla andra Workfront-objekt.
   * AEM Assets.
* Hierarkier kan innehålla både Planning-posttyper och Workfront-projekt samtidigt.

  Du kan till exempel ha en Campaign-posttyp med Planning Tactics och Workfront Projects som underordnade i samma arbetsytehierarki.

* Om det redan finns en anslutning mellan de valda posttyperna återanvänds den befintliga anslutningen.
* Om det inte finns någon anslutning skapar Workfront en sådan i hierarkiinställningarna.
* Inställningen **Skapa motsvarande fält för den länkade posttypen** måste aktiveras för det anslutna fältet för poster och objekttyper som du vill ta med i en hierarki.
* Du kan inte ta bort en posttyp om den ingår i en hierarki.
* Du kan inte ta bort ett anslutningsfält om posttypen som refereras i fältet är en del av en hierarki. Du måste först ta bort posttypen från hierarkin eller ta bort hierarkin innan du kan ta bort posttypen.
* Du kan ta bort ett uppslagsfält från en ansluten posttyp. Det går inte att återställa informationen i fältet.
* Följande är regler för hierarkiinställningar:
   * En posttyp kan bara ha en överordnad posttyp på en angiven arbetsyta.

     En taktisk posttyp kan till exempel inte ha både en Campaign- och en målobjekttyp som överordnad på samma arbetsyta.
   * En posttyp kan vara överordnad i flera hierarkier.

     Du kan till exempel ha tre olika hierarkier på en arbetsyta, och var och en av dem kan ha kampanjer som överordnad posttyp.
   * En post kan kopplas till flera överordnade poster av samma typ när du kopplar en till många eller flera posttyper.

     Taktik A kan till exempel tillhöra både Campaign X och Campaign Y.
   * En posttyp kan bara ansluta till en underordnad posttyp åt gången. En underordnad posttyp kan också vara överordnad en annan posttyp.

     En Campaign-posttyp kan till exempel vara överordnad till endast en annan posttyp i samma hierarki (Tactics), och Tactics kan i sin tur vara överordnad Program som kan vara överordnad till Projekt.
   * En posttyp kan inte vara överordnad i en hierarki och underordnad i en annan hierarki i samma arbetsyta.
   * Globala posttyper kan visas i flera arbetsytor i flera hierarkier efter att de har lagts till på dessa arbetsytor.

     Om en Campaign till exempel är en global posttyp och en del av en hierarki i Workspace 1, kan den läggas till som en befintlig posttyp i Workspace 2 och ingå i en hierarki där. Men den kan inte ingå i en hierarki i Workspace 2 endast när den har angetts som en global posttyp i Workspace 1, men inte läggas till i Workspace 2.
   * När anslutna posttyper ingår i hierarkier kan du koppla en post från en underordnad posttyp till upp till 10 poster från en överordnad posttyp.

     Om du till exempel skapar en hierarki mellan kampanjer som överordnad och personlig post som underordnad post, kan du koppla samma person till upp till 10 kampanjer.

## Att tänka på när du visar vägbeskrivningar

När du skapar hierarkier mellan posttyper genereras vägbeskrivningar för poster som tillhör de posttyperna.

Om du t.ex. skapar en hierarki och kopplar ihop kampanjer med taktik, sedan med Aktiviteter, och sedan med Projekt, när du navigerar till en post av någon av de typer som är kopplade till hierarkin, kan du visa var i hierarkin posten placeras.

![Breadcrumb](assets/breadcrumbs-on-project.png)

Tänk på följande:

* Om en posttyp ingår i flera hierarkier kan du växla mellan hierarkier från postens vägbeskrivningar på postens sida.
* Om posttypen i en hierarki har flera poster kan du välja poster från den synliga sökvägen.
* Brödraperier fungerar i Workfront och Planning.

  Om du till exempel tittar på ett projekt som är kopplat till Planering-kampanjer och taktik, och även till Workfront portfolior och program, kan du växla mellan både Planning och Workfront objekttyper från den stora mängden.

  Mer information finns i [Skapa arbetsytehierarkier](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* När du redigerar en post visas ändringarna från alla arbetsytor och alla hierarkier som posten är en del av.



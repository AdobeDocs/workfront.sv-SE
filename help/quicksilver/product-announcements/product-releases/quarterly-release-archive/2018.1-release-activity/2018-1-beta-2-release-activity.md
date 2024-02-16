---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 2-lanseringsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.1 Beta 2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 14 december 2017. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 0%

---

# 2018.1 Beta 2-lanseringsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.1 Beta 2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 14 december 2017. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.1 finns på  [Aktivitetsöversikt för 2018.1-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Beta 2-versionen från 2018.1 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Gruppadministration för användare och layoutmallar](#group-administration-for-users-and-layout-templates)

**För alla användare**

* [Systembred widescreen-skärm](#system-wide-widescreen-display)
* [Ändra storlek på ögonblicksbild av tidslinje i Gantt-schema](#resize-timeline-snapshot-on-the-gantt-chart)
* [Interaktiv resursplanerare i affärsärendet](#interactive-resource-planner-in-the-business-case)
* [Visualisering i resursplaneraren - diagram över användarallokering](#visualization-in-the-resource-planner-user-allocation-chart)
* [Förbättringar i hemområdet](#improvements-in-the-home-area)
* [Förbättringar av nya korrekturläsare](#new-proofing-viewer-improvements) 

## Gruppadministration för användare och layoutmallar {#group-administration-for-users-and-layout-templates}

Nu kan du utse gruppadministratörer i Workfront. Fältet Gruppägare har bytt namn till gruppadministratör, och användare som har utsetts till gruppadministratörer har ytterligare behörigheter för att hantera användare och layoutmallar för de grupper som de hanterar.

* [Användarhantering efter gruppadministratör](#user-management-by-group-administrator)
* [Hantering av layoutmallar per gruppadministratör](#layout-template-management-by-group-administrators)

### Användarhantering efter gruppadministratör {#user-management-by-group-administrator}

Vi introducerar det nya konceptet **gruppadministratör**. Som stöd för detta finns **Gruppägare** fältet har bytt namn till **gruppadministratör** och de användare som har utsetts till gruppadministratörer har ytterligare behörigheter för att hantera användare och grupper.

Förutom de behörigheter som gruppägaren tidigare hade för att hantera användare, har gruppadministratören nu följande extra åtkomst när de hanterar användare i de grupper där de har angetts som gruppadministratör:

* Logga in som en annan användare som tillhör en grupp som de hanterar.
* Återställ lösenordet för en annan användare som tillhör en grupp som de hanterar.
* Skapa layoutmallar som administreras av gruppen. 

Före den här ändringen kunde bara Workfront-administratören utföra de här funktionerna.

Mer information om gruppadministratörer finns i avsnittet &quot;Förstå gruppadministratörer&quot; i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Hantering av layoutmallar per gruppadministratör {#layout-template-management-by-group-administrators}

Vi introducerar det nya konceptet **Grupp med administrationsåtkomst** som du kan koppla till en layoutmall.

Den användare som är utsedd som gruppadministratör för den här gruppen har åtkomst till att hantera den layoutmallen och skapa nya layoutmallar där de grupper som de hanterar är mallarnas administrativa grupper. 

Före den här ändringen kunde bara Workfront-administratören skapa layoutmallar.

Mer information om hur du skapar layoutmallar finns i&quot;Skapa och hantera layoutmallar&quot;.

## Systembred widescreen-skärm {#system-wide-widescreen-display}

När du visar en sida i Workfront fylls hela webbläsarfönstret nu i automatiskt och anpassas till skärmstorleken.

Före den här ändringen visades endast de sidor som var kopplade till följande objekt i widescreen:

* Projekt
* Uppgifter
* Problem
* Rapporter
* Kontrollpaneler
* Kalendrar

## Ändra storlek på ögonblicksbild av tidslinje i Gantt-schema {#resize-timeline-snapshot-on-the-gantt-chart}

Du kan nu expandera ögonblicksbilden av tidslinjen för att visa hela projektet i Gantt-diagrammet.

Före den här förbättringen kan du markera en specifik punkt på ögonblicksbilden av tidslinjen för att navigera till den i Gantt-diagrammet.

Mer information om hur du konfigurerar hur information visas i Gantt-schemat finns i [Konfigurera hur information visas i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Interaktiv resursplanerare i affärsärendet {#interactive-resource-planner-in-the-business-case}

Som resurshanterare kan du nu lägga till resurspooler i avsnittet Resursbudgetering i affärsärendet. Du kan också budgetera dina projektresurser med hjälp av resursplaneringsverktyget på projektnivå. När du budgeterar dina resurser för ett projekt genereras projektets budgeterade arbetskostnad.

Före den här ändringen kunde du visa resursbudgeteringsinformation i affärsärendet om projektet hade budgeterats för resurser i den globala resursplaneraren.

Mer information om hur du slutför budgetering av projektresurser i affärsärendet finns i [Budgetresurser i affärsärendet](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualisering i resursplaneraren - diagram över användarallokering {#visualization-in-the-resource-planner-user-allocation-chart}

Du kan nu visa den totala planerade allokeringen för alla användare mot deras tillgänglighet i ett diagram i resursplaneraren. Diagrammet är tillgängligt när du väljer **Visa efter användare** i resursplaneraren.

Diagrammet innehåller följande information:

* Tillgänglighet % utan överbeläggning för alla användare
* Överbeläggning % för alla användare
* Underutnyttjande % för alla användare
* Det finns en överallokering för minst en användare under den här tidsperioden

Före den här ändringen kunde du bara visa allokeringen och tillgängligheten för enskilda användare i tabellformat.

Mer information om användarallokeringsschemat i resursplaneraren finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Förbättringar i hemområdet {#improvements-in-the-home-area}

Det finns nu flera förbättringar på Hem-området, bland annat:

* Bättre utseende och känsla

   * Den högra panelen är nu större och ger mer utrymme för uppgifter och probleminformation.
   * Försenade objekt visas nu med en ljusare röd nyans när de markeras i den vänstra panelen.
   * Nu kan du enklare se förhållandet mellan den vänstra panelen och den högra panelen. Det markerade dokumentet i den vänstra panelen pekar på den högra panelen.

* Standardfält visas för markerade objekt. 

  Mer information om standardfälten finns i&quot;Skapa och hantera layoutmallar&quot;.

* När du har klickat på&quot;Arbeta med den&quot; på en begäran visas fälten som är kopplade till problemet i den högra panelen.

  Mer information om hur du arbetar med begäranden från hemområdet finns i [Hantera arbets- och teamförfrågningar på Hem-området](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) in [Hantera arbets- och teamförfrågningar på Hem-området](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Peka på en avatar för en användare på ett arbetsobjekt i den vänstra panelen för att visa namnet på användaren.
* Expandera området&quot;Sena&quot; i den vänstra panelen om du vill visa alla sena objekt (när det här området är komprimerat visas endast de första fem objekten).
* När du har markerat ett objekt som fullständigt behålls objektet i den vänstra panelen tills du markerar ett annat objekt.\
  Mer information om hur du visar slutförda objekt finns i [Visa objekt i arbetslista i hemområdet](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in [Visa objekt i arbetslista i hemområdet](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Mer information om hur du använder den nya hemsidan, samt information om skillnader i funktionalitet mellan Mitt arbete och Hem, finns i [Använda området Hem](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Förbättringar av nya korrekturläsare  {#new-proofing-viewer-improvements}

* [Förbättrad layout och design](#improved-layout-and-design)
* [Sök kommentarer efter kommentarnummer](#search-comments-by-comment-number)
* [Alternativ för att redigera kommentar bredvid markeringsindikatorn](#option-to-edit-comment-next-to-the-markup-indicator)
* [Markera alla kommentarer som lästa](#mark-all-comments-as-read)
* [Förbättringar i den vänstra menyn](#left-menu-improvements)

### Förbättrad layout och design {#improved-layout-and-design}

Språkvisningsprogrammet har ett uppdaterat utseende och en uppdaterad känsla. Följande områden i korrekturläsaren uppdaterades:

* Miniatyrområde

  Mer information om hur du använder området för miniatyrbilder finns i .

* Kommentarområde\
  Mer information om kommentarsområdet finns i .
* Vänster menyområde

### Sök kommentarer efter kommentarnummer {#search-comments-by-comment-number}

Nu när du söker i kommentarlistan i korrekturläsaren kan du ange kommentarnumret i sökfältet. Kommentarlistan filtreras sedan för att visa den kommentar du sökte efter. 

Mer information finns i .

### Alternativ för att redigera kommentar bredvid markeringsindikatorn {#option-to-edit-comment-next-to-the-markup-indicator}

Nu kan du enkelt redigera en befintlig kommentar. När du har klickat på en kommentarindikator på korrekturet visas en redigeringsikon bredvid ballongen. 

Innan den här ändringen utfördes var du tvungen att klicka på redigeringsikonen i kommentarsområdet.  

Mer information finns i .

### Markera alla kommentarer som lästa {#mark-all-comments-as-read}

När du visar ett dokument i korrekturläsaren kan du nu markera alla kommentarer som lästa.

### Förbättringar i den vänstra menyn {#left-menu-improvements}

Menyn till vänster i korrekturläsaren innehåller följande förbättringar:

* Uppdaterat utseende och känsla
* Ikon högst upp på menyn om du vill visa eller dölja menyn

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* För musen över menyn för att automatiskt expandera menyn för att visa etiketter förutom ikoner. (Du kan också aktivera alternativet att alltid ha menyn i den komprimerade vyn.)

---
content-type: overview
product-area: projects
navigation-topic: financials
title: Översikt över intäkt och kostnadshierarki
description: I den här artikeln beskrivs den stegvisa processen för att fastställa lämplig fakturerings- och kostnadsnivå för jobbroller och användare för intäktstypen och kostnadstypen för användaren och rollen per timme.
author: Lisa
feature: Work Management
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '3519'
ht-degree: 0%

---

# Översikt över intäkter och kostnadshierarki

{{highlighted-preview-article-level}}

{{ultimate-package}}

För att få exakta ekonomiska beräkningar använder Workfront rätt faktureringstariff vid beräkning av intäkten för en uppgift eller ett projekt. Jobbrollen och användarsiffrorna måste vara väldefinierade på alla nivåer för att man ska kunna göra korrekta ekonomiska beräkningar.

Avsnitten i den här artikeln innehåller information om den stegvisa processen för att fastställa lämplig fakturerings- och kostnadsnivå för jobbroller och användare för intäktstypen och kostnadstypen Användare och Roll per timme.

Mer information om faktureringstariffer, intäktstyper och hur intäkten beräknas finns i [Översikt över fakturering och intäkt](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Översikt över giltighetsdatum

Workfront-administratörer kan också ange giltighetsdatum som avgör när faktureringstariffer, kostnadstariffer och andra finansiella attribut börjar gälla i systemet. En jobbroll eller användare kan till exempel ha en standardfaktureringsfrekvens på 50 USD. När giltighetsdatum används kan priset på 50 USD sättas till förfallodatum den 31 mars och en ny ränta på 55 USD börjar automatiskt den 1 april.

För planerade intäktsberäkningar baseras faktureringsräntan på datumet för de planerade timmarna. De planerade timmarna fördelas jämnt över aktivitetens varaktighet. I föregående exempel används priset $50 för timmar som planerats till 31 mars eller tidigare, och för timmar som planerats till 1 april eller senare används priset $55.

För faktiska intäktsberäkningar baseras faktureringstarifferna på datumet för de loggade timmarna. I det föregående exemplet används priset $50 för timmar som loggades den 31 mars eller tidigare, och för timmar som loggades den 1 april eller senare används priset $55.

>[!NOTE]
>
>Uppgiftstilldelningar definieras inte med giltighetsdatum. I stället hämtar tilldelningar de tillämpliga tarifferna från systemet, oavsett om de kommer från ett tariffkort, en användarprofil eller åsidosättning på tilldelningsnivå. Med giltighetsdatum säkerställs att rätt frekvens används baserat på tidpunkten för arbetet, men tilldelningarna definieras inte direkt.

## Översikt över jobbroll för fakturering

En **jobbroll för fakturering** har angetts för en användare på tilldelningsnivå eller projektnivå. Det gäller endast användare och kan inte användas i andra jobbroller. En användares primära roll är till exempel Designer, men i en uppgift eller ett projekt agerar de som Senior Designer och hastigheten bör återspegla detta.

En jobbroll på tilldelningsnivå för fakturering gäller endast för den specifika tilldelningen och används inte automatiskt för användarens andra tilldelningar. En jobbroll på projektnivå för fakturering gäller för alla användarens tilldelningar i det projektet. Du kan åsidosätta den på den enskilda uppdragsnivån om det behövs.

När en jobbroll för fakturering används på antingen användartilldelningen eller projektnivån, kan den hastighet som är kopplad till jobbrollen för fakturering användas i stället för användar- eller jobbrollstarifferna i intäktsberäkningar. Jobbrollen för fakturering är endast tillgänglig när intäktstypen Användare och Roll per timme används.

>[!NOTE]
>
>En användare kan agera med en annan roll i faktureringssyfte, men kostnadsberäkningarna fortsätter att använda sin primära jobbroll. Jobbrollen för fakturering påverkar endast faktureringsberäkningar.

Mer information finns i [Konfigurera en jobbroll för fakturering](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

## Översikt över bevarade frekvenser

Flaggan **Bevara information om projektfaktureringstariffer** i ett projekt kontrollerar om systemet använder faktureringsinformationen för tilldelningar när tariffkortet slutförs eller tillåter ändringar baserat på ändringar under projektets gång. Eventuella ändringar av användarens jobbroll, lön, rabattkort eller annan faktureringsrelaterad information kommer inte att påverka faktureringsfrekvenserna för tilldelningar. Frekvenserna bevaras enligt det slutliga tariffkortet när projektflaggan aktiveras. Dessa tilldelningsegenskaper (som befattning och lön) uppdateras fortfarande, vilket säkerställer att den verkliga kostnaden för uppdraget är korrekt.

När flaggan är aktiverad låser systemet de datumeffektiva faktureringstarifferna (som anges på det kreditkort som är kopplat till projektet) under hela projektet.

Flaggan kan aktiveras för ett projekt när arbetet har startats och tilldelningar och timmar redan finns. Vid den tidpunkten:

* Den slutliga kreditkortsavgiften blir källan till faktureringstaxor för alla projekttilldelningar.
* Alla tidigare, aktuella och framtida tilldelningar beräknas på nytt med hjälp av de slutgiltiga godkända tarifferna.
* Faktiska och planerade värden beräknas om.

>[!NOTE]
>
>När flaggan är aktiverad för att bevara faktureringstarifferna kan den inte stängas av om projektet inte har några tilldelningar och inga timmar. Detta garanterar att alla finansiella rapporter återspeglar de faktiska avtalstarifferna.
>När flaggan är inaktiverad kan faktureringstarifferna beräknas om eller justeras dynamiskt. Eventuella uppdateringar av användarens roll, lön eller faktureringsfrekvens visas omedelbart i faktureringssatsen för tilldelningen.

Mer information finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) och [Hantera gratulationskort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Planerade intäkter - användare och roll per timme

När intäktstypen för aktiviteten är Användare och Roll-timme använder Workfront tariffhierarkier för både användare och jobbroll för att fastställa faktureringsfrekvensen för planerade intäkter.

Den här bilden visar flödet i den planerade intäktshierarkin:

![Planerad intäkt för användare och roll, timintäktstyp](assets/planned-revenue-chart.png)

När en användare tilldelas till uppgiften söker Workfront i den här hierarkin:

1. Systemet söker först efter en bibehållen frekvens för tilldelningen för användaren.

   En bevarad frekvens följer fortfarande hierarkin, men hastigheten fryses när projektet bevaras. Mer information finns i [Översikt över bevarade frekvenser](#overview-of-preserved-rates).

1. Därefter letar systemet efter faktureringssatsen på ett betalkort, för den primära jobbrollen eller jobbrollen för fakturering av användaren som tilldelats uppgiften. Om det finns en ränta och den är låst används den avgiften i intäktsberäkningen.

   Om det finns en frekvens på tariffkortet och det är olåst, använder systemet inte den frekvensen och söker efter nästa frekvens i hierarkin.

1. Därefter letar systemet efter åsidosättningsfrekvensen på tilldelningsnivå för användaren. Det här är en manuellt tillagd frekvens som är kopplad till den specifika tilldelningen och åsidosätter alla andra avgifter för användaren för den här tilldelningen (förutom en hastighetskortets låsta frekvens). Om en ränta hittas används den avgiften i intäktsberäkningen.
1. Därefter söker systemet efter en jobbroll för fakturering på aktivitetstilldelningsnivå.

   Jobbrollen för fakturering gäller endast för en specifik tilldelning och gäller för tilldelningen i stället för användarens primära rollfrekvens för jobb. En användares primära roll är till exempel Designer, men vid en uppgift agerar han/hon som Senior Designer med en högre faktureringsfrekvens.

   Workfront letar efter jobbrollen för faktureringsavgift:

   * Systemet söker först efter faktureringsfrekvensen för jobbrollen för fakturering från uppdraget (Senior Designer i exemplet), med hänsyn tagen till giltighetsdatum. Du kan se detta under Fakturering i projektet i en **Rate Source: Åsidosättningar > Resurstyp: Jobbroll**-gruppering. Detta är en åsidosättningsfrekvens för projektet.
   * Därefter söker systemet efter jobbrollen för faktureringsavgift från ett betalkort, med hänsyn tagen till giltighetsdatum. Detta visas under Fakturering i projektet i en **Rate Source: Attached Rate Card > Resource Type: Job Role**-gruppering.
   * Om hastigheten för jobbrollen för fakturering inte finns i projektet eller på tariffkortet söker systemet efter rollfrekvensen på systemnivå (Senior Designer i exemplet), med hänsyn tagen till giltighetsdatum.
   * Om en jobbroll för fakturering har tilldelats, och ingen av tarifferna från föregående steg hittas, är faktureringssatsen 0.

     >[!NOTE]
     >
     >När en jobbroll för fakturering har tilldelats, men faktureringssatsen är 0, är detta en indikator som återställer prisinställningen. En nivå på 0 innebär att inga belopp för den rollen (Senior Designer i exemplet) har skapats i Workfront. Du bör antingen lägga till avgifter för jobbrollen eller ta bort jobbrollen för fakturering från tilldelningen.
     >
     >Eftersom uppgifter ärver jobbrollsfrekvenser från projektet när dessa frekvenser är tillgängliga på projektnivå, skulle alla priser från en sökning efter jobbrollen för fakturering av projektet redan ha hittats när Workfront sökte efter jobbrollen för fakturering på aktivitetstilldelningsnivån. Sökningen på projektnivå efter en jobbroll för fakturering finns fortfarande kvar i sökhierarkin.

1. Om en jobbroll för fakturering inte var tillgänglig på aktivitetstilldelningsnivån söker systemet efter faktureringsfrekvensen i projektet för den specifika användare som tilldelats uppgiften, med hänsyn tagen till giltighetsdatum. Du kan se detta under Fakturering för projektet i en **Rate Source: Åsidosättningar > Resurstyp: Användare**. Detta är en åsidosättningsfrekvens för projektet.
1. Därefter letar systemet efter faktureringstaxan på systemnivå för användarens profil, med hänsyn tagen till giltighetsdatum.
1. Därefter letar systemet efter faktureringsfrekvensen för användarens primära jobbroll (Designer i exemplet).

   * Systemet söker först efter faktureringssatsen för projektet, efter användarens primära jobbroll, med hänsyn tagen till giltighetsdatum. Du kan se detta under Fakturering i projektet i en **Rate Source: Åsidosättningar > Resurstyp: Jobbroll**-gruppering. Detta är en åsidosättningsfrekvens för projektet.
   * Därefter söker systemet efter jobbrollfrekvensen från ett priskort, med hänsyn tagen till giltighetsdatum. Detta visas under Fakturering i projektet i en **Rate Source: Attached Rate Card > Resource Type: Job Role**-gruppering.
   * Därefter letar systemet efter rollfrekvensen på systemnivå, med hänsyn tagen till giltighetsdatum.

1. Om ingen av dessa taxor hittas är faktureringstaxan 0.

När en användare inte är tilldelad uppgiften söker Workfront i jobbrollsfrekvenserna enligt den här hierarkin:

1. Systemet söker först efter en bibehållen frekvens i tilldelningen för jobbrollen.
1. Systemet letar efter faktureringssatsen på ett betalkort för den jobbroll som tilldelats uppgiften. Om det finns en ränta och den är låst används den avgiften i intäktsberäkningen.

   Om det finns en frekvens på tariffkortet och det är olåst, använder systemet inte den frekvensen och söker efter nästa frekvens i hierarkin.

1. Därefter letar systemet efter åsidosättningsfrekvensen för tilldelningsuppgifterna för jobbrollen. Det här är en manuellt tillagd hastighet för jobbrollen för den specifika tilldelningen och åsidosätter alla andra satser för jobbrollen för den här aktiviteten. Om en ränta hittas används den avgiften i intäktsberäkningen.
1. Därefter letar systemet efter faktureringssatsen för den jobbroll som tilldelats uppgiften.

   * Systemet söker först efter faktureringssatsen för projektet för jobbrollen, med hänsyn tagen till giltighetsdatum. Du kan se detta under Fakturering i projektet i en **Rate Source: Åsidosättningar > Resurstyp: Jobbroll**-gruppering. Detta är en åsidosättningsfrekvens för projektet.
   * Därefter söker systemet efter jobbrollfrekvensen från ett priskort, med hänsyn tagen till giltighetsdatum. Detta visas under Fakturering i projektet i en **Rate Source: Attached Rate Card > Resource Type: Job Role**-gruppering.
   * Därefter letar systemet efter rollfrekvensen på systemnivå, med hänsyn tagen till giltighetsdatum.

1. Om ingen av dessa taxor hittas är faktureringstaxan 0.

## Faktisk intäkt - användare och roll per timme

När intäktstypen för aktiviteten är Användare och Roll-timme använder Workfront två hierarkier för att fastställa faktureringsfrekvensen för faktiska intäkter. Faktureringsfrekvensen baseras på användarens loggningstid för en uppgift.

&quot;Användaren&quot; i hierarkierna är den person som tilldelats uppgiften. &quot;Ägaren&quot; är den person vars tid är inloggad mot uppgiften, även om den inte är tilldelad uppgiften. Michael har till exempel tilldelats en uppgift men Joanna slutför arbetet eftersom Michael var sjuk. Hanteraren kan logga tiden mot uppgiften och ange ägaren till de loggade timmarna till Joanna. De planerade intäktsvärdena baseras på Michael uppdrag och frekvens i hierarkin, men de faktiska intäktsvärdena baseras på Joannas ränta.

Den här bilden visar flödet i den faktiska intäktshierarkin:

![Faktisk intäkt för kostnadstypen Användare och Roll per timme](assets/actual-revenue-chart.png)

### När ägaren av de loggade timmarna och den tilldelade användaren i uppgiften är samma

Workfront söker först efter en faktureringstaxa efter användartilldelningen. Om en användare inte är tilldelad uppgiften söker den efter en faktureringsfrekvens efter jobbrolltilldelningen.

Hierarkin för det här scenariot är densamma som den planerade intäktshierarkin. Se [Planerade intäkter - Användare och roll per timme](#planned-revenue--user-and-role-hourly) för det här arbetsflödet.

### När ägaren av de loggade timmarna inte är den tilldelade användaren i uppgiften

Workfront söker i användaregenskaperna för ägaren enligt den här hierarkin:

1. Systemet söker först efter en bevarad frekvens för tilldelningen till ägaren.
1. Därefter letar systemet efter faktureringssatsen på ett betalkort för ägarens primära jobbroll. Om det finns en ränta och den är låst används den avgiften i intäktsberäkningen.

   Om det finns en frekvens på tariffkortet och det är olåst, använder systemet inte den frekvensen och söker efter nästa frekvens i hierarkin.

1. Därefter letar systemet efter faktureringstakten för projektet, för ägaren, med hänsyn tagen till giltighetsdatum. Du kan se detta under Fakturering för projektet i en Rate Source: Overrides > Resource Type: User grouping. Detta är en åsidosättningsfrekvens för projektet.
1. Därefter söker systemet efter en jobbroll för fakturering på projektnivå.

   Jobbrollen för fakturering gäller endast ett specifikt projekt och gäller för projektet i stället för ägarens primära rollfrekvens för jobb. Exempel: Ägarens primära arbetsuppgift är Designer, men i ett projekt agerar de som Senior Designer med en högre faktureringsnivå.

   Workfront letar efter jobbrollen för faktureringsavgift:

   * Systemet söker först efter jobbrollen för faktureringsavgift från ett betalkort, med hänsyn tagen till giltighetsdatum. Detta visas under Fakturering i projektet i en **Rate Source: Attached Rate Card > Resource Type: Job Role**-gruppering.
   * Om hastigheten för jobbrollen för fakturering inte finns på avgiftskortet söker systemet efter rollfrekvensen på systemnivå (Senior Designer i exemplet), med hänsyn tagen till giltighetsdatum.
   * Om en jobbroll för fakturering har tilldelats, och ingen av tarifferna från föregående steg hittas, är faktureringssatsen 0.

     >[!NOTE]
     >
     >När en jobbroll för fakturering har tilldelats, men faktureringssatsen är 0, är detta en indikator som återställer prisinställningen. En nivå på 0 innebär att inga belopp för den rollen (Senior Designer i exemplet) har skapats i Workfront. Du bör antingen lägga till avgifter för jobbrollen eller ta bort jobbrollen för fakturering från projektet.

1. Därefter letar systemet efter faktureringstaxan på systemnivå för ägarens användarprofil, med hänsyn tagen till giltighetsdatum.
1. Därefter letar systemet efter faktureringsfrekvensen för ägarens primära jobbroll (Designer i exemplet).

   * Systemet söker först efter faktureringssatsen för projektet, efter ägarens primära befattning, med hänsyn tagen till giltighetsdatum. Du kan se detta under Fakturering i projektet i en **Rate Source: Åsidosättningar > Resurstyp: Jobbroll**-gruppering. Detta är en åsidosättningsfrekvens för projektet.
   * Därefter söker systemet efter jobbrollfrekvensen från ett priskort, med hänsyn tagen till giltighetsdatum. Detta visas under Fakturering i projektet i en **Rate Source: Attached Rate Card > Resource Type: Job Role**-gruppering.
   * Därefter letar systemet efter rollfrekvensen på systemnivå, med hänsyn tagen till giltighetsdatum.

1. Om ingen av dessa taxor hittas är faktureringstaxan 0.

## Planerad kostnad - användare och roll per timme

När kostnadstypen för aktiviteten är Användare och Roll-timme använder Workfront hierarkier för både användare och jobbroll för att fastställa hastigheten för planerad kostnad.

Den här bilden visar flödet i den planerade kostnadshierarkin:

![Planerad kostnad för kostnadstypen Användare och Roll per timme](assets/planned-cost-chart.png)

När en användare tilldelas till uppgiften söker Workfront i den här hierarkin:

1. Systemet letar efter åsidosättningshastigheten för tilldelningsaktiviteten för användaren. Det här är en manuellt tillagd frekvens för användaren för den specifika tilldelningen och åsidosätter alla andra avgifter för användaren för den här uppgiften. Om en ränta hittas används den kursen i kostnadsberäkningen.
1. Därefter letar systemet efter kostnadstariffen för projektet, för den specifika användare som tilldelats uppgiften, med hänsyn tagen till giltighetsdatum. Du kan se detta i området Hastigheter > Kostnad för projektet i en **Rate Source: Åsidosättningar > Resurstyp: Användare**. Detta är en åsidosättningsfrekvens för projektet.
1. Därefter letar systemet efter kostnadsnivån på systemnivå för användarens profil, med hänsyn tagen till giltighetsdatum.
1. Därefter söker systemet efter kostnadstakten för användarens primära jobbroll med kombinationen tilldelade attribut, baserat på attributpoängen.
1. Om ingen av dessa priser hittas är kostnadsnivån 0.

När en användare inte har tilldelats uppgiften söker Workfront igenom kostnadstarifferna för jobbrollen enligt den här hierarkin:

1. Systemet letar efter åsidosättningsfrekvensen för tilldelningsuppgifterna för jobbrollen. Det här är en manuellt tillagd hastighet för jobbrollen för den specifika tilldelningen och åsidosätter alla andra satser för jobbrollen för den här aktiviteten. Om en ränta hittas används den kursen i kostnadsberäkningen.
1. Därefter söker systemet efter kostnadstariff för jobbroller på systemnivå med kombinationen tilldelade attribut, baserat på attributpoängen, med hänsyn tagen till giltighetsdatum.
1. Om ingen av dessa priser hittas är kostnadsnivån 0.

## Faktisk kostnad - användare och roll per timme

När kostnadstypen för aktiviteten är Användare och Roll-timme använder Workfront två hierarkier för att fastställa faktureringsfrekvensen för den faktiska kostnaden. Faktureringsfrekvensen baseras på användarens loggningstid för en uppgift.

&quot;Användaren&quot; i hierarkierna är den person som tilldelats uppgiften. &quot;Ägaren&quot; är den person vars tid är inloggad mot uppgiften, även om den inte är tilldelad uppgiften. Michael har till exempel tilldelats en uppgift men Joanna slutför arbetet eftersom Michael var sjuk. Hanteraren kan logga tiden mot uppgiften och ange ägaren till de loggade timmarna till Joanna. De planerade intäktsvärdena baseras på Michael uppdrag och frekvens i hierarkin, men de faktiska intäktsvärdena baseras på Joannas ränta.

Den här bilden visar flödet i den faktiska kostnadshierarkin:

![Faktisk kostnad för kostnadstypen Användare och Roll per timme](assets/actual-cost-chart.png)

### När ägaren av de loggade timmarna och den tilldelade användaren i uppgiften är samma

Workfront söker först efter en kostnadstariff efter användartilldelningen. Om en användare inte är tilldelad uppgiften söker den efter en kostnadstariff efter jobbrolltilldelningen.

Hierarkin för det här scenariot är densamma som den planerade kostnadshierarkin. Se [Planerad kostnad - Användare och roll per timme](#planned-cost--user-and-role-hourly) för det här arbetsflödet.

### När ägaren av de loggade timmarna inte är den tilldelade användaren i uppgiften

Workfront söker i användaregenskaperna för ägaren enligt den här hierarkin:

1. Systemet letar efter kostnadstariffen för projektet, för ägaren, med hänsyn tagen till gällande datum. Du kan se detta i området Hastigheter > Kostnad för projektet i en **Rate Source: Åsidosättningar > Resurstyp: Användare**. Detta är en åsidosättningsfrekvens för projektet.
1. Därefter letar systemet efter kostnadsnivån på systemnivå för ägarens användarprofil, med hänsyn tagen till giltighetsdatum.
1. Därefter letar systemet efter kostnadsnivån för ägarens primära jobbroll (Designer i exemplet).

   * Systemet söker först efter kostnadstariffen för projektet, för ägarens primära roll i arbetet, med hänsyn tagen till giltighetsdatum. Du kan se det här i området Hastigheter > Kostnad för projektet i en **Rate Source: Åsidosättningar > Resurstyp: Gruppering av jobbroll**. Detta är en åsidosättningsfrekvens för projektet.
   * Därefter söker systemet efter jobbrollfrekvensen från ett priskort, med hänsyn tagen till giltighetsdatum. Du ser detta i området Hastigheter > Kostnad för projektet i en **Rate Source: Attached Rate Card > Resource Type: Job Role**-gruppering.
   * Därefter letar systemet efter rollfrekvensen på systemnivå, med hänsyn tagen till giltighetsdatum.

1. Om ingen av dessa taxor hittas är faktureringstaxan 0.


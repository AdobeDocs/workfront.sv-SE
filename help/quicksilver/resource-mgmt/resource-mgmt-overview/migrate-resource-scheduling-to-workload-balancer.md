---
filename: migrate-resource-scheduling-to-workload-balancer
product-area: resource-management
navigation-topic: resource-management-overview
title: Migrera från resursschemaläggning till [!UICONTROL Workload Balancer]
description: Vi vill att du ska uppleva så lite avbrott som möjligt i arbetet genom att hjälpa dig att utforma en migreringsplan. Med stegen nedan får du hjälp att utbilda ditt team och fastställa den bästa tiden för att gå över till arbetsbelastningsutjämnaren.
author: Alina
exl-id: 4bc08d5f-99c7-40e2-85d6-1de0b585aef8
source-git-commit: d2a8380e3383b97b8245bd2b6d3cb9ff75306e4f
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Migrera från resurs [!UICONTROL Scheduling] till [!UICONTROL Workload Balancer]

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön.</span>

<!-- drafted for res scheduling deprecation blurb for PREVIEW release - Oct 2022 - CHANGE THIS BLURB TO SOMETHING ELSE AT PRODUCTION:-->

>[!CAUTION]
>  
>  
> <span class="preview">Schemaläggningsområdena har tagits bort från förhandsvisningsmiljön och kommer att tas bort från produktionsmiljön i **Januari 2023**. </span>\
> <span class="preview"> Efter januari 2023 måste du schemalägga dina resurser i Arbetsbelastningsutjämnaren. </span>
>  
><span class="preview"> Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i avsnittet [Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/workload-balancer.md).</span>

Informationen i den här artikeln gäller endast dig om du har hanterat planeringen av dina resurser i resursen [!UICONTROL Scheduling] områden i Adobe Workfront. Workfront började ta bort [!UICONTROL Scheduling] i november 2020 och har ersatt dem med [!UICONTROL Workload Balancer].

Mer information om borttagningsplanen för [!UICONTROL Resource Scheduling] och tidslinjen för att ersätta dem med [!UICONTROL Workload Balancer], se [Borttagning av verktygen för resursplanering i Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

Vi vill att du ska uppleva så lite avbrott som möjligt i arbetet genom att hjälpa dig att utforma en migreringsplan. Stegen nedan hjälper dig att få ditt team utbildat och hitta den bästa tiden att gå över till [!UICONTROL Workload Balancer].

## Leta reda på verktygen för resursplanering

Du och dina team kanske använder en del av resursen [!UICONTROL Scheduling] verktyg inom följande områden i Workfront:

* The [!UICONTROL Scheduling] i [!UICONTROL Resourcing] area
* The [!UICONTROL Scheduling] del av ett projekt
* The [!UICONTROL Schedule] del av ett team

Med den här borttagningen [!UICONTROL Workload Balancer] ersätter alla  [!UICONTROL Resource Scheduling] verktyg i alla områden ovan.

## Steg 1: Utbilda era team

Gå kursen [Resource Management Program for the new Adobe Workfront experience](https://one.workfront.com/s/resource-management-program-nwe) (75 minuter) på Workfront One.

Om du får problem med att logga in eller öppna kursen kontaktar du kundsupport. Mer information finns i [Kontakta kundsupport](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Steg 2: Bestäm den bästa tiden för migrering {#step-2-determine-the-best-time-to-migrate}

Följ stegen nedan för att avgöra när den bästa tiden att migrera är för dig:

1. Bestäm vilka funktioner i resursen som ska användas [!UICONTROL Scheduling] verktyg som teamet använder mest och se till att de funktionerna är tillgängliga i [!UICONTROL Workload Balancer]. För information om vilka funktioner som är tillgängliga i [!UICONTROL Workload Balancer], se avsnittet&quot;Funktionstillgänglighet&quot; i artikeln [Borttagning av verktygen för resursplanering i Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

   >[!IMPORTANT]
   >
   >Nästan alla funktioner i schemaläggningsverktygen finns nu i arbetsbelastningsutjämnaren.

1. Avgör om ditt team hanterar användartilldelningar för tilldelningar. Justering eller ändring av användartilldelningar innebär att de planerade timmarna per dag ändras för varje användare under en arbetsuppgifts varaktighet.

   Allokeringar som redigeras i schemaläggningsverktygen överförs inte till arbetsbelastningsutjämnaren. Som standard distribuerar systemet alla planerade timmar för ett arbetsobjekt under hela objektets varaktighet.

   Du måste hantera allokeringar manuellt i belastningsutjämnaren för att se till att allokeringarna matchar dem du har i planeringsverktygen. Mer information finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Sparade filter i området Schemaläggning överförs inte automatiskt till Utjämning av arbetsbelastning. Skapa eventuella filter som du behöver i Utjämning av arbetsbelastning. Mer information om hur du skapar filter i Arbetsbelastningsutjämnaren finns i [Filtrera information i Utjämning av arbetsbelastning](../workload-balancer/filter-information-workload-balancer.md).

<!--
1. Using the information gathered from Steps 1 and Step 2, decide which version of Step 3 you should continue with based on the needs of your organization.
-->

## Steg 3: Migrera till [!UICONTROL Workload Balancer]{#step-3-migrate-to-the-workload-balancer}

Vi har identifierat följande versioner för det här steget, beroende på dina resultat i steg 2:

* [Steg 3a: Du eller dina team använder [!UICONTROL Scheduling] verktyg, men ändra inte användartilldelningen](#step-3a-you-or-your-teams-use-the-scheudling-tools-but-do-not-modify-user-allocation)
* [Steg 3b: Du eller dina team hanterar användartilldelningar i [!UICONTROL Scheduling] verktyg](#step-3b-you-or-your-teams-manage-user-allocations-in-the-scheduling-tools)

### Steg 3a: Du eller dina team använder [!UICONTROL Scheduling] verktyg, men ändra inte användartilldelningen

Om du eller dina team inte ändrar den dagliga timtilldelningen för arbetstilldelningar är du redo att växla schemaläggningsresurser till [!UICONTROL Workload Balancer].

![](assets/nwe-workload-balancer-global-350x125.png)

Gör följande:

* Välj ett övergångsdatum.

   >[!TIP]
   >
   >Ge teamet lite tid att gå igenom kursen om att använda belastningsutjämnaren före övergångsdatumet. Mer information om utbildning finns i avsnittet [Migrera från resursschemaläggning till arbetsbelastningsutjämnaren](#migrate-from-resource-uicontrol-scheduling-to-the-uicontrol-workload-balancer) i den här artikeln.

* Följ de här riktlinjerna för att hjälpa dina team:

   * Uppmuntra era team att besöka [Översikt över [!UICONTROL Workload Balancer]](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) sidan och alla sidor som länkas därifrån för att fördjupa sig i hur [!UICONTROL Workload Balancer] fungerar.
   * Håll möten med Frågor och svar så att era team kan besvara frågor veckan före övergången, byta och sedan hålla ett annat möte med Frågor och svar för att besvara uppföljningsfrågor.
   * Skicka feedback till Workfront med knappen Feedback i det övre verktygsfältet. Våra produktutvecklare är alltid intresserade av att höra dina användningsexempel för hur vi kan skapa [!UICONTROL Workload Balancer] ger mer värde.

### Steg 3b: Du eller dina team hanterar användartilldelningar i [!UICONTROL Scheduling] verktyg

Om ditt arbetsflöde matchar detta scenario bör du vara mer strategisk i din övergångsplan. De dagliga allokeringarna som visas i [!UICONTROL Scheduling] verktyg lagras i en annan databas än den dagliga allokering som visas i [!UICONTROL Workload Balancer]. Detta innebär att justeringarna av dagliga allokeringar som du gör i resursen [!UICONTROL Scheduling] verktygen inte överförs till den dagliga fördelningen i [!UICONTROL Workload Balancer].

>[!CAUTION]
>
>Du har tills **Januari 2023** för att se till att din användartilldelning från schemaläggningsområdena matchar den i arbetsbelastningsutjämnaren i produktionsmiljön. Då tar vi bort schemaläggningsverktygen från produktionsmiljön. Du måste justera allokeringarna i Utjämning av arbetsbelastning manuellt för att matcha allokeringarna i planeringsverktygen. <span class="preview">Schemaläggningsverktygen har redan tagits bort från förhandsvisningsmiljön.</span>


Tänk på följande när du gör övergången till [!UICONTROL Workload Balancer] när du använder [!UICONTROL Scheduling] funktionalitet:

* Spärra hanteringen av allokeringar i [!UICONTROL Scheduling] verktyg när resurshanterarna gör bytet. Så här gör du:

   * Ta reda på den genomsnittliga varaktigheten för uppgifter i aktuella projekt och ta hänsyn till detta när du avgör hur länge du behöver vänta med att hantera användarallokeringarna.

      >[!TIP]
      >
      >Du behöver bara titta på dina aktuella projekt eller planeringsprojekt, dvs. de projekt som era team aktivt arbetar med och hanterar dagliga tilldelningar för.

   * Skapa en aktivitetsrapport och lägg till fältet Varaktighet i vyn och gruppera den efter projektnamn. Sammanfatta kolumnen Varaktighet i vyn med medel och spara sedan rapporten.

      Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) .

   * Analysera uppgiftsrapporten. Om till exempel den genomsnittliga aktivitetstiden är 3 dagar kan det vara bäst med en veckas övergång. Låt teamet sluta hantera användartilldelningar för en vecka. Följande vecka: överför teamet till [!UICONTROL Workload Balancer] och börja hantera användarallokeringar som kommer efter veckan.
   >[!NOTE]
   >
   >Det här förslaget kanske inte fungerar om den genomsnittliga aktivitetstiden är längre än den återstående tiden tills planeringsverktygen har tagits bort.


   ![](assets/timeline-stop-using-resource-scheduler-callouts-350x178.png)

   >[!TIP]
   >
   >Du kan fortsätta att utföra uppgifter och utfärda uppdrag under övergångsperioden. Utvalda uppdrag återspeglas både i Resursplaneraren och [!UICONTROL Workload Balancer].

* Om du är en större organisation där team hanterar resurser för hundratals projekt kan du överväga att gå över från [!UICONTROL Scheduling] verktygen för [!UICONTROL Workload Balancer] en portfölj i taget. Överväg en fasad utrullning genom att skapa anpassade filter i [!UICONTROL Workload Balancer] för att titta på en specifik portfolio i taget.

* Låt resurshanterarna gruppera: ha en person som granskar uppdrag i  [!UICONTROL Resource Scheduling] verktyg och en som justerar i [!UICONTROL Workload Balancer]. När teamet av två förenar båda verktygen får de arbetsflödena att ändras till [!UICONTROL Workload Balancer].

## Behöver mer hjälp

Om du behöver mer information om migreringen kontaktar du den anpassade supporten. Mer information om hur du kontaktar supporten finns i [Kontakta kundsupport](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

---
title: Förbättrad analys - översikt
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Förbättrad analys är ett kraftfullt verktyg i Adobe Workfront med färdiga visualiseringar som gör att du kan titta på projektdata och identifiera trender med planering och slutförande. Denna insikt i era projekt hjälper er att hantera ert nuvarande arbete och gör det möjligt att planera mer korrekt för framtida arbete.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# Förbättrad analys - översikt

Förbättrad analys är ett kraftfullt verktyg i Adobe Workfront med färdiga visualiseringar som gör att du kan titta på projektdata och identifiera trender med planering och slutförande. Denna insikt i era projekt hjälper er att hantera ert nuvarande arbete och gör det möjligt att planera mer korrekt för framtida arbete.

Förbättrade analysfunktioner kan hjälpa er att identifiera:

* Det sätt du planerar projekt på
* När arbete läggs till i projekt
* Mängden arbete som slutförs för olika projekt
* Hur många timmar eller dagar som krävs för att slutföra ett projekt jämfört med de timmar eller dagar som ett hemteam är schemalagt
* Hur ofta användare utför specifika åtgärder under ett projekt
* Projektförloppet samt de enskilda uppgifterna i ett projekt

![](assets/nwe-full-screen-analytics-350x222.png)

Om du vill se användningsexempel eller lära dig mer om hur du hanterar aktuellt arbete och planerar för framtida arbete med Förbättrad analys läser du i [Förbättrade inlärningsvägar för analyser](https://one.workfront.com/s/enhanced-analytics-program).

## Förutsättningar

För att få tillgång till det förbättrade analysområdet måste du:

* Ha en Business- eller Enterprise-plan.

   Mer information finns i [Workfront-planer](https://www.workfront.com/plans).

* Låt Workfront-administratören lägga till förbättrade analysfunktioner i layoutmallen.

   Mer information finns i [Förbättrad analys: Lägga till analyser i layoutmallar](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Om du vill visa information för projekt och uppgifter måste du:

* Ha behörighet att visa i områdena Projekt och uppgifter på din åtkomstnivå.

   Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i [Skapa eller ändra anpassade åtkomstnivåer](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Har behörighet att visa för specifika uppgifter och/eller projekt.

   Mer information om hur du begär ytterligare åtkomst finns i [Begär åtkomst till objekt](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Bästa tillvägagångssätt för förbättrad analys

För att få bästa möjliga data för dina projekt använder du mallar som har korrekta planerade timmar och varaktighetsdagar. Du måste också se till att dina användare anger och uppdaterar fälten nedan så korrekt som möjligt.

>[!NOTE]
>
>Några av följande fält är beräkningar som Workfront utför baserat på information som användarna anger. Du kan inte uppdatera dessa fält manuellt.

* Planerade timmar

   Det här är det viktigaste fältet att fylla i.

   >[!NOTE]
   >
   >Om era team inte använder planerade timmar kan ni fortfarande se vissa data baserat på projektens längd.\
   >Mer information finns i avsnittet [Längdvy](#duration-view) i den här artikeln.

* Projektnamn

   Namnet ska vara beskrivande för projektet.

* Projektvillkor
* Projektstatus
* Projektets planerade startdatum
* Planerat slutförandedatum
* Projektets faktiska startdatum
* Projektets faktiska slutdatum
* Projektets längd - timmar
* Faktiska timmar för projekt
* Uppgiftsstatus (Detta inkluderar märkning av slutförda uppgifter.)
* Aktivitetsnamn
* Procent färdigt för aktivitet
* Startdatum för planerad aktivitet
* Planerat slutförandedatum för uppgift

>[!IMPORTANT]
>
>Det kan ta upp till 24 timmar för ändringar som görs i uppgifter och projekt att återspegla i Förbättrad analys.

## Längdvy {#duration-view}

Som standard baseras treemap-visualiseringarna för nedladdning och projekt på planerade timmar. Om era team inte använder planerade timmar kan ni titta på dessa visualiseringar baserat på projektets längd.

I Förbättrad analys beräknas projektens längd med följande formler:

* Planerad tidsram:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* Antal dagar som har använts:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8 timmar är standardvärdet för **Vanliga timmar per arbetsdag**. En Adobe Workfront-administratör kan uppdatera **Vanliga timmar per arbetsdag** ställa in under **Inställningar** > **Projektinställningar** > **Projekt** > **Tidslinjer**.\
   >Mer information finns på [Konfigurera systemomfattande projektinställningar](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Information om planerad varaktighet finns i [Översikt över projektvaraktighet](../manage-work/projects/planning-a-project/project-duration.md).

## Kortkommandon

Du kan använda följande tangenter på tangentbordet för att navigera eller slutföra specifika åtgärder i området Förbättrad analys:

| Nyckel | Åtgärd |
|---|---|
| **Tabb** | Navigera till varje element på sidan och till en tabell med information om varje visualisering som inte visas på sidan |
| **Retur** | Öppna kalenderwidgeten, ta bort ett befintligt filter, öppna alternativen för att lägga till filter, markera/avmarkera filtervärden, tillämpa ett filter som du har skapat, öppna exportalternativen för varje visualisering, öppna listrutemenyerna i listrutan under Aktiviteter under flygning och i projekttreemap-visualiseringar |
| **Piltangenter** | Navigera till datum i kalenderwidgeten, via filteralternativ när du lägger till ett filter och via alternativ i alla listrutor i visualiseringarna |
| **Blanksteg** | Välj datum i kalenderwidgeten, välj en filtertyp när du lägger till ett filter, välj ett exportalternativ i listrutan för varje visualisering och välj alternativ i listrutorna i listrutan under Aktiviteter under flygning och i projekttreemappningsvisualiseringar |

{style=&quot;table-layout:auto&quot;}

Om du använder ett skärmläsarprogram eller ett plugin-program läser skärmläsaren upp informationen på skärmen och beskriver de åtgärder som du slutför när du använder knapparna ovan.

## Förbättrade analysvyer och funktioner

Om du vill veta mer om en viss funktion i Förbättrad analys, vilka åtgärder du kan utföra för att få mer information och vad du kan lära dig av dessa data, kan du läsa följande artiklar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Artikel</th> 
   <th>Förklaring</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Använd filter i Förbättrad analys</a> </td> 
   <td> <p>Du kan använda anpassade filter, projektfältfilter eller teamfilter för att endast visa projekt som uppfyller vissa villkor. När du lägger till filter uppdateras antalet projekt därefter.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Förstå nyckeltal för förbättrade analyser</a> </td> 
   <td> <p>KPI:er (Key Performance Indicator) för alla projekt inom en viss tidsram finns längst upp på skärmen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Visa flygplansvisualisering i Förbättrad analys</a> </p> </td> 
   <td> <p>The <b>Flygplan</b> visualisering visar att villkoret har ändrats under ett projekts livslängd. Genom att interagera med visualiseringen får du mer information om specifika datum. När du väljer ett projekt öppnas"Burndown" och"Tasks" i flygvisualiseringar.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Visa Burndown-visualisering i Förbättrad analys</a> </td> 
   <td> <p>The <b>Burndown</b> visualisering visar den planerade hastigheten för ett projekt jämfört med det faktiska antalet timmar som har ägnats åt ett projekt. Om du interagerar med visualiseringen får du mer information om projektets villkor ett visst datum.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Visa uppgifter i flygvisualisering i Förbättrad analys</a> </td> 
   <td> <p>The <b>Uppgifter under flygning</b> visualisering visar status för varje uppgift i ett projekt. Genom att interagera med visualiseringen kan du snabbt och enkelt göra ändringar i en uppgift.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Visa projektaktivitetsvisualisering i Förbättrad analys</a> </td> 
   <td> <p>The <b>Projektaktivitet</b> visualisering visar en översikt över när användare tilldelade till ett projekt som är inloggat på Workfront, ändrade status för uppgiften i det projektet och slutförde uppgifter i det projektet. Genom att interagera med visualiseringen kan du se informationen för varje användare. Du kan också se specifika datum för dessa åtgärder samt hur många gånger varje åtgärd har slutförts.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Visa projekttreemap-visualisering i Förbättrad analys</a> </td> 
   <td> <p>The <b>Projekttreemap</b> visualisering visar hur mycket tid som har ägnats åt vissa projekt jämfört med andra. Om du interagerar med visualiseringen får du information om projektets skick, det planerade slutförandet och det faktiska slutförandet av projektet.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visa aktivitetsbaserad teamvisualisering i Förbättrad analys</a> </td> 
   <td> <p>The <b>Aktivitet per team</b> visualisering visar en översikt över när användare i ett hemteam som har loggat in på Workfront, ändrat status för en uppgift och slutfört en uppgift. Genom att interagera med visualiseringen kan du se informationen för varje enskild användare. Du kan också se specifika datum för dessa åtgärder samt hur många gånger varje åtgärd har slutförts.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">Visa resurskapaciteten i Förbättrad analys</a> </td> 
   <td> <p>The <b>Resurskapacitet</b> visualisering visar vilka hemteam som har kapacitet att ta på sig mer arbete och vilka hemteam som har mer arbete än vad de kan utföra. Genom att interagera med visualiseringen kan du se mer information om slutfört arbete och tillgängliga timmar för mer arbete. Om du väljer ett team öppnas teamets kapacitetsvisualisering.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">Visa teamkapacitetvisualisering i Förbättrad analys</a> </td> 
   <td> <p>The <b>Teamkapacitet</b> visualisering visar en procentandel av det arbete som ett hemteam har utfört av den mängd arbete de tilldelats. Genom att interagera med visualiseringen kan du se schemalagda timmar och planerade timmar för ett visst datum, samt kapacitetsprocenten och om hemteamet var över, under eller på kapaciteten den dagen.</p> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Statusöversikt för Iteration-slutförande
description: Fyllningsinformationen som beskrivs i den här artikeln visas ovanför nedladdningsschemat.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Statusöversikt för Iteration-slutförande

Fyllningsinformationen som beskrivs i den här artikeln visas ovanför nedladdningsschemat.

Slutförandeprocent för en iteration:

![](assets/burndown-percentcomplete-350x47.png)

Den här informationen anger slutstatus för upprepningen för den dag som är markerad i nedladdningsschemat. Som standard visas slutförandestatusen baserat på den aktuella dagens datum.

Följande information finns:

* **[!UICONTROL Percent Complete]:** Sammanlagt förlopp för upprepningen

   [!UICONTROL Percent Complete] justerar baserat på hur stor procentandel av varje artikel eller uppgift som är slutförd i arbetsmomentet, inklusive artiklar eller uppgifter som bara är delvis slutförda.

   Färgen på [!UICONTROL Percent Complete] statusfältet visas som rött eller grönt för att matcha färgen för den faktiska nedtoningsfrekvensen. Den visas i rött när nedbränningsgraden är mindre än det idealiska (fler punkter eller timmar återstår per dag än den idealiska nedladdningsberäkningen) och visas i grönt när nedladdningsfrekvensen är lika med eller bättre än det ideala (lika med eller färre punkter återstår per dag än den idealiska nedladdningsberäkningen).

* **[!UICONTROL Completed Stories]:** (Endast tillgängligt i iterationer) Antal markerade artiklar [!UICONTROL Complete]. Detta visas i relation till det totala antalet artiklar i iterationen. Exempel: &quot;3 av 6&quot; anger att 3 av de 6 artiklarna i iteration har markerats [!UICONTROL Complete].
* **[!UICONTROL Completed Points / Hours]:** (Endast tillgängligt i iterationer) Antal markerade punkter eller timmar [!UICONTROL Complete]. Visas i relation till det totala antalet poäng eller timmar i iterationen. Exempel: &quot;5 av 11&quot; anger att 5 av de 11 artiklarna i iteration har markerats [!UICONTROL Complete]. Det här numret är direkt relaterat till [!UICONTROL Percent Complete] beräkning och uppdateras samtidigt [!UICONTROL Percent Complete] uppdateras.

   Punkter och timmar är kopplade till artiklar. När en artikel markeras [!UICONTROL Complete], markeras de punkter eller timmar som är kopplade till artikeln som fullständiga.

   Som standard används punkter. Du kan ändra detta genom att ändra inställningarna för ditt team enligt beskrivningen i [Skapa ett smidigt team](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Points / Hours Per Day]:** (Endast tillgängligt i iterationer) Genomsnittligt antal markerade punkter eller timmar [!UICONTROL Complete] varje dag sedan upprepningens början fram till den aktuella dagen.

   Detta beräknas utifrån det totala antalet punkter eller timmar som har slutförts, dividerat med det totala antalet dagar till den aktuella dagen. (Delvisa dagar registreras som en hel dag.)

   Den här informationen kan vara användbar när du planerar en framtida upprepning.

* **[!UICONTROL Estimated Completion]:** Det beräknade datumet då iterationen ska slutföras, baserat på den aktuella hastigheten i antal poäng/timmar per dag (för iterationer).

   När [!UICONTROL Estimated Completion] datumet är senare än slutdatumet som definierats för iterationen, visas antalet återstående arbetsdagar som rött inom parentes intill [!UICONTROL Estimated Completion] datum.

   När [!UICONTROL Estimated Completion] datumet är tidigare än det planerade slutdatumet för iterationen, visas antalet återstående arbetsdagar i grönt. (Slutdatumet för iterationen anges när iterationen planeras, vilket beskrivs i [Skapa en iteration](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); slutdatumet för projektet är [!UICONTROL Planned Completion Date]eller är det aktuella datumet om [!UICONTROL Planned Completion Date] har redan varit. The [!UICONTROL Planned Completion Date] för projektet beräknas utifrån varaktigheten för uppgifterna i projektet.) När du planerar upprepningen, och anger slutdatumet för iterationen för en arbetsdag som inte är arbetsdag och iterationen spåras till färdig i tid, ställs det beräknade slutdatumet in för den sista arbetsdagen före det iteration-slutdatum som du anger (eftersom arbetet inte är schemalagt att brännas ned på lediga dagar).

   &quot;(+9 dagar)&quot; anger till exempel att det beräknade slutförandedatumet är 9 arbetsdagar senare än det planerade slutdatumet för upprepningen.

   Mer information finns i [Statusöversikt för Iteration-slutförande](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).

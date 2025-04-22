---
content-type: api
navigation-topic: general-api
title: Evenemangsprenumerationsversion
description: API för händelseprenumeration
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 82694183c32938905f1f8542c430d3c453274cb6
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%

---

# Versionshantering för händelseteckning

Workfront har två versioner av abonnemang. I den här artikeln beskrivs skillnaderna mellan dem.

Den nya versionen är inte en ändring av Workfront API, utan snarare en ändring av prenumerationsfunktionen för evenemang.

Möjligheten att uppgradera eller nedgradera abonnemang säkerställer att befintliga prenumerationer inte bryts när händelsestrukturen ändras, vilket gör att du kan testa och uppgradera till den nya versionen utan avbrott i prenumerationen.


När du uppgraderar eller nedgraderar din eventprenumeration till en annan version får du dubbletthändelser för varje eventleverans i fem minuter efter att versionen ändrats. Dubbletterna innehåller en av alla händelseprenumerationer, version 1 och version 2. Detta säkerställer att du inte missar några händelser på grund av att du har ändrat versionen av en händelseprenumeration.

Mer information om slutpunkterna som används för att uppgradera eller nedgradera händelseprenumerationer finns i [Versionsinformation om händelseprenumerationer](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) i artikeln Event-prenumerations-API.

>[!IMPORTANT]
>
>Följande versioner kommer att påverka versionshantering av händelseprenumerationer:
>
>* **25.2 utgåva** (10 april 2025): Alla nya prenumerationer som skapas efter version 25.2 skapas som version 2.
>* **25.3 utgåva** (17 juli 2025): Prenumerationer kan inte längre nedgraderas till version 1 efter version 25.3.
>* **1 september 2025**: Alla återstående prenumerationer på version 1 migreras till version 2.

## Ändringar mellan version 1 och version 2

Följande ändringar har gjorts för händelseprenumerationer version 2:


### Allmänna ändringar


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Påverkade fält</b></p> </th> 
   <th> <p><b>Version 1 (beteendet Föregående)</b></p> </th> 
   <th> <p><b>Version 2 (Ändra)</b></p> </th> 
   <th> <p><b>Åtgärd för reparation</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Parametervärden</p> </td> 
   <td> <p>För alla objekt som skapats från en mall som innehåller ett anpassat formulär, skickades en <code>CREATE</code>-händelse och sedan skickades en <code>UPDATE</code> med parametervärdena (inklusive beräknade fält och deras värden).    </p> </td> 
   <td> <p>När ett objekt skapas från en mall som innehåller ett anpassat formulär med beräknade parametervärden, skickas bara en <code>CREATE</code>-händelse och den kommer att innehålla parametervärden inklusive beräknade fält.</p> </td> 
   <td> <p>Om du prenumererar på <tr><ul><ul><code>UPDATE<code> events and are expecting to receive an <code>UPDATE</code> event after an object is created with calculated parameter values, you will no longer receive that <code>UPDATE</code> event. If you wish to see calculated parameter values on object creation, you must create an additional <code>CREATE</code> subscription.</p> </td> 
  </tr> 
   
   <td> <p>Multi-Select type fields</p> </td> 
   <td> <p>For any type of event that contains a change on a multi-select type field, if the field only contained one value it would be converted to and sent as a string. Otherwise it would be sent as an array. </p><p>Examples:</p><li><code>myMultiSelectField: ["oneValue"]</code> is converted and sent as <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Regardless of how many values are in the array, it will be sent as an array. </p><p>Examples:</p><li><code>myMultiSelectField: ["oneValue"]</code> is sent as <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>If you have a subscription with a filter on a multi-select field, and the value as a string, you must create a new subscription with the same filter that has the value as an array. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Objektspecifika ändringar

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Objektkod</b> </th> 
   <th> <b>Påverkade fält</b> </th> 
   <th> <b>Version 1 (Föregående beteende)</b></th> 
   <th> <b>Version 2 (Ändra)</b> </th> 
   <th> <b>Reparationsåtgärd</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>När det här objektet uppdaterades visade <code>UPDATE</code>-händelsen ibland felaktigt att de påverkade fälten ändras från <code>null</code> till <code>ID value</code>.</td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för de påverkade fälten.</td> 
   <td>Ingen. Om du har ett filter för de berörda fälten får du bara en <code>UPDATE</code>-händelse om dessa fält har ändrats, inte om något annat värde har ändrats.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>När ett parametervärde uppdaterades för det här objektet visade händelsen <code>UPDATE</code> felaktigt ändringen av det påverkade fältet från <code>null</code> till <code>object id</code>. </td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för de påverkade fälten.</td> 
   <td>Ingen. Om du har ett filter för de berörda fälten får du bara en <code>UPDATE</code>-händelse om dessa fält har ändrats, inte om något annat värde har ändrats.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>När ett dokument togs bort visade <code>DELETE</code>-händelsen felaktigt det påverkade fältet som en tom array i det föregående läget.    </td> 
   <td>Händelsen <code>DELETE</code> visar korrekt det påverkade fältet i det föregående läget.</td> 
   <td>Ingen. <code>DELETE</code>-händelsen kommer fortfarande att skickas, men nu visas korrekta data för det påverkade fältet. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>När det här objektet uppdaterades skickas två <code>UPDATE</code>-händelser. Den första innehöll inte de påverkade fälten medan den andra händelsen utfördes.</td> 
   <td>Alla fältuppdateringar, inklusive de påverkade fälten, finns endast i en <code>UPDATE</code>-händelse och en andra onödig händelse skickas inte.     </td> 
   <td>Ingen. Om du har ett filter för de fält som påverkas levereras händelserna i den första händelsen. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>När ett parametervärde uppdaterades för en utgift visade händelsen <code>UPDATE</code> felaktigt ändringen av topReferenceObjCode från <code>EXPNS</code> till <code>PROJ</code> och <code>referenceObjectName</code> ändrades från <code>null</code> till <code>string value of project name</code>.      </td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för de påverkade fälten.</td> 
   <td>Ingen. Om du har ett filter för de berörda fälten får du bara en <code>UPDATE</code>-händelse om dessa fält har ändrats, inte om något annat värde har ändrats.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>När ett utgiftsobjekt togs bort skickades en <code>UPDATE</code>-händelse som ändrade de berörda fälten till null innan <code>DELETE</code>-händelsen skickades.    </td> 
   <td>Den extra <code>UPDATE</code>-händelsen skickas inte. Händelsen <code>DELETE</code> har rätt värden för de påverkade fälten i det föregående läget. </td> 
   <td>Om du har ett filter för de fält som påverkas av <code>UPDATE</code>-händelser och förväntas ta emot det när objektet tas bort, får du inte längre den <code>UPDATE</code> -händelsen. Om du vill se de här fälten när objektet tas bort måste du skapa ytterligare en <code>DELETE</code>-prenumeration.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">TIMME</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>När det här objektet togs bort visade <code>DELETE</code>-händelsen felaktigt de påverkade fälten som <code>null</code> i det föregående läget. </td> 
   <td>Händelsen <code>DELETE</code> visar de fält som påverkas i det föregående läget.</td> 
   <td>Ingen. Händelsen <code>DELETE</code> skickas fortfarande, men nu visas korrekta data för de påverkade fälten. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>När ett parametervärde uppdaterades för det här objektet visade händelsen <code>UPDATE</code> felaktigt ändringen av det påverkade fältet från <code>null</code> till <code>ID value</code>. </td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för det påverkade fältet.</td> 
   <td>Ingen. Om du har ett filter för det påverkade fältet får du bara en <code>UPDATE</code>-händelse om fältet faktiskt har ändrats, inte om något annat parametervärde har ändrats.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>När det här objektet uppdaterades visade <code>UPDATE</code>-händelsen ibland felaktigt att de påverkade fälten ändras från <code>null</code> till <code>ID value</code>.</td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för de påverkade fälten.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>När ett parametervärde uppdaterades för det här objektet visade händelsen <code>UPDATE</code> felaktigt ändringen av det påverkade fältet från <code>null</code> till <code>ID value</code>. </td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för det påverkade fältet.</td> 
   <td>Ingen. Om du har ett filter för det påverkade fältet får du bara en <code>UPDATE</code>-händelse om fältet faktiskt har ändrats, inte om något annat parametervärde har ändrats.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>När det här objektet uppdaterades visade <code>UPDATE</code>-händelsen ibland felaktigt att de påverkade fälten ändras från <code>null</code> till <code>ID value</code>.</td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för det påverkade fältet.</td> 
   <td>Ingen. Om du har ett filter för det påverkade fältet får du bara en <code>UPDATE</code>-händelse om fältet faktiskt har ändrats, inte om något annat parametervärde har ändrats.
  </tr> 
  <tr> 
   <th rowspan="2">UPPGIFT</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>När ett parametervärde uppdaterades för det här objektet visade händelsen <code>UPDATE</code> felaktigt ändringen av det påverkade fältet från <code>null</code> till <code>ID value</code>. </td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för det påverkade fältet.</td> 
   <td>Ingen. Om du har ett filter för det påverkade fältet får du bara en <code>UPDATE</code>-händelse om fältet faktiskt har ändrats, inte om något annat parametervärde har ändrats.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>När det här objektet uppdaterades visade <code>UPDATE</code>-händelsen ibland felaktigt att de påverkade fälten ändras från <code>null</code> till <code>ID value</code>.</td> 
   <td>Alla <code>UPDATE</code>-händelser visar rätt värde för det påverkade fältet.</td> 
   <td>Ingen. Om du har ett filter för det påverkade fältet får du bara en <code>UPDATE</code>-händelse om fältet faktiskt har ändrats, inte om något annat parametervärde har ändrats.
 </tbody> 
</table>


## Uppdatera händelseteckningsversion i ett Workfront Fusion-scenario

Workfront Fusion använder händelseprenumerationer för att hålla utkik efter förändringar i Workfront för att utlösa scenarier. Du kan uppdatera den händelseprenumerationsversion som Fusion använder direkt i ett scenario med hjälp av modulen Workfront > Update Events Payload Version.

Instruktioner om hur du använder den här modulen finns i [Workfront-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules) i dokumentationen för Workfront Fusion.

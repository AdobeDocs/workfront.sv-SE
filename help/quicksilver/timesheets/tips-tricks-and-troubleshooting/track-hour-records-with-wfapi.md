---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Spåra timnoteringar med Adobe Workfront API
description: Om din organisation använder Adobe Workfront för att ange antalet arbetade timmar, men använder ett annat verktyg som registersystem för dessa data, kan du använda Workfront API för att synkronisera data mellan de två systemen.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Spåra timnoteringar med Adobe Workfront API

Om din organisation använder Adobe Workfront för att ange antalet arbetade timmar, men använder ett annat verktyg som registersystem för dessa data, kan du använda Workfront API för att synkronisera data mellan de två systemen.

Det går inte att spåra timposten eftersom hela posten tas bort om timposten tas bort, vilket kräver att du hämtar hela datauppsättningen och jämför den med den gamla datauppsättningen. Som tur är registreras alla timtransaktioner i Workfront Journal Enentries.

När du har hämtat en första uppsättning med alla aktuella timmar i systemet kan du spåra alla ändringar via Journalposter.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"change Typ": "A",<br>"aux2": "Brad Little",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d08d 93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Little",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee 934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Little", <br>"newNumberVal": 1,<br>"old NumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"{3 <br>,<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Little",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f00 08db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Här följer en beskrivning av de inkluderade fälten:

* **changeType:** Den typ av ändring som görs för objektet:

   * **A:** Lägg till

   * **E:** Redigera

   * **D:** Ta bort

* **aux2:** Namnet på användaren som timposten är avsedd för.

* **newNumberVal:** Nytt värde för timposten (detta blir null om changeType är D).

* **oldNumberVal:** Tidigare värde för timposten.

* **subObjCode:** Posttyp som ändras (ska alltid vara HOUR).

* **subObjID:** ID för timposten.

Du kan använda den här informationen för att identifiera vilka timposter som har ändrats, redigerats eller tagits bort. Du kan sedan använda subObjID för att hämta mer information från timposterna om det behövs.

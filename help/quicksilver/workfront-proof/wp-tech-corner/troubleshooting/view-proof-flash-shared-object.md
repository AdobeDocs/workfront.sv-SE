---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problem med att visa korrektur - Flash-delade objekt förklaras
description: '"Obs! Informationen i den här artikeln hänvisar till funktioner som för närvarande är inaktuella och som kommer att tas bort från [!DNL Workfront] 2018. Vi rekommenderar att du använder den nya Web Proofing Viewer (som beskrivs i Granska korrektur i Web Proofing Viewer) eller Desktop Proofing Viewer (som beskrivs i Granska korrektur i Desktop Proofing Viewer).'''
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Problem med att visa korrektur - [!DNL Flash] Förklaring av delade objekt

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>Informationen i den här artikeln hänvisar till funktioner som för närvarande är inaktuella och som kommer att tas bort från [!DNL Workfront] 2018. Vi rekommenderar att du använder den nya Web Proofing Viewer (som beskrivs i [Granska korrektur i Web Proofing Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) eller Desktop Proofing Viewer (enligt beskrivningen i [Granska korrektur i Desktop Proofing Viewer](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## [!DNL Flash] Delade objekt

Ett lokalt delat objekt, ibland kallat[!DNL Flash] cookie&quot; är en datafil som kan skapas på din dator av de webbplatser du besöker. Delade objekt används oftast för att förbättra webbläsarupplevelsen. A [!DNL Flash] cookie är ett meddelande som används i [!DNL Adobe Flash] som skickas från en webbserver till en webbläsare och sedan lagras som en datafil i webbläsaren.

Sedan [!DNL Workfront Proof] Visningsprogrammet är baserat på [!DNL Flash]är det värt att kontrollera vad lagring tillåts för [!DNL Flash] program på datorn.

## [!DNL Flash] Delade objekt - kända fel

Om [!DNL Flash] lagringsinställningen är 0 kB eller har en annan inställning som blockerar [!DNL Flash] program från att spara data lokalt kan orsaka vissa kända fel i [!DNL Workfront Proof] Visningsprogram:

* Popup-fönstret Komma igång visas hela tiden även om alternativet att inte visa det igen valdes
* [!DNL Workfront Proof] Visningsprogrammets prestanda försämras på grund av det ökande antalet kommentarer som läggs till i korrekturet
* Korrektur läses inte in och du får den grå skärmen i stället för en faktisk bild

## Tillåts [!DNL Flash] Delade objekt

Se till att lagra [!DNL Flash] Delade objekt tillåts på datorn och lagringsgränsen är inte 0.

Så här kontrollerar du om delade objekt är tillåtna:

1. Högerklicka i dialogrutan [!DNL Workfront Proof] Visningsprogram.
1. Välj **[!UICONTROL Global Settings]** på snabbmenyn.
1. Gå till **[!UICONTROL Storage]** -fliken.
1. Se till att **[!UICONTROL Allow sites to save information on this computer]** är markerat (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## Ökning [!DNL Flash] lagring

Som standard [!DNL Flash] program kan lagra upp till 100 kB data på användarens enhet, men detta kan enkelt ändras av användarna. Lösningen för de många [!DNL Flash] relaterade problem är att öka den interna [!DNL Flash] lagring. Detta kan göras direkt från [!DNL Workfront Proof] Visningsprogram:

1. Öppna ett bevis.
1. Öppna högerklicksmenyn på korrekturet.
1. Klicka **[!UICONTROL Settings]** för att öppna [!DNL Flash] popup-fönstret för inställningar.
1. Gå till **[!UICONTROL Local]** lagringsflik.
1. Öka lagringsutrymmet upp till t.ex. 100 kB (1).
1. Stäng popup-fönstret med inställningar och öppna korrekturet igen.

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)

---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Uppdatering till e-postadress uppdaterar inte användarnamnet
description: Uppdatering till e-postadress uppdaterar inte användarnamnet
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Uppdatering till e-postadress uppdaterar inte användarnamnet

## Problem

`emailAddr` och `username` är vanligtvis samma attribut. Om du ändrar en användares `emailAddr`-attribut uppdateras därför attributet `username` automatiskt så att det matchar.

När `username` inte matchar `emailAddr` uppdateras inte `username` automatiskt när `emailAddr` uppdateras. Detta gäller för båda `emailAddr`-ändringarna via användargränssnittet och via API:t.

## Orsak

Felmatchningen kan skapas på flera sätt:

* Användare som skapades innan synkroniseringsregeln fanns. Mycket gamla användarkonton kanske inte har dessa attribut synkroniserade.

* Användare som har skapats via enkel inloggning samtidigt som e-postadressen i Workfront var skiftlägeskänslig. Alternativet för automatisk etablering av enkel inloggning skulle köra en skiftlägeskänslig kontroll för användare baserat på användarens attribut från identitetsleverantören. När det inte fanns någon exakt matchning skulle den automatiska etableringstjänsten skapa en ny användare. Om en användare redan fanns fanns fanns det en risk för att användarnamnet och `emailAddr` inte skulle ha samma hölje.

* Användare som har fått attributet `username` uppdaterat direkt via API:t, och deras `emailAddr` har inte uppdaterats. `username` och `emailAddr` matchar eventuellt inte.

## Lösning

Använd API:t för att ändra attributet `username` till samma som `emailAddr`. När attributen har synkroniserats kommer alla uppdateringar av `emailAddr` också att uppdatera `username` så att de matchar (när användarnamnsfältet inte ingår i uppdateringen).

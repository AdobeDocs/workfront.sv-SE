---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Uppdatering till e-postadress uppdaterar inte användarnamnet
description: Uppdatering till e-postadress uppdaterar inte användarnamnet
author: John
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Uppdatering till e-postadress uppdaterar inte användarnamnet

## Problem

Normalt `emailAddr` och `username` är samma attribut. Om du ändrar en användares `emailAddr` -attribut, `username` attributet uppdateras automatiskt för att matcha.

När `username` matchar inte `emailAddr`, en uppdatering av `emailAddr` uppdaterar inte `username` automatiskt. Detta gäller båda `emailAddr` ändringar via användargränssnittet och via API:t.

## Orsak

Felmatchningen kan skapas på flera sätt:

* Användare som skapades innan synkroniseringsregeln fanns. Mycket gamla användarkonton kanske inte har dessa attribut synkroniserade.

* Användare som har skapats via enkel inloggning samtidigt som e-postadressen i Workfront var skiftlägeskänslig. Alternativet för automatisk etablering av enkel inloggning skulle köra en skiftlägeskänslig kontroll för användare baserat på användarens attribut från identitetsleverantören. När det inte fanns någon exakt matchning skulle den automatiska etableringstjänsten skapa en ny användare. Om en användare redan fanns fanns fanns det en risk för att användarnamnet och `emailAddr` skulle inte ha samma hölje.

* Användare som har `username` attribut som uppdateras direkt via API:t och deras `emailAddr` uppdaterades inte. The `username` och `emailAddr` matchar kanske inte.

## Lösning

Använd API för att ändra `username` -attributet ska vara detsamma som `emailAddr`. När attributen har synkroniserats kan du uppdatera `emailAddr` uppdaterar även `username` som matchar (när användarnamnsfältet inte ingår i uppdateringen).

---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API-felmeddelande 400 - Ogiltig begäran
description: API-felmeddelande 400 - Ogiltig begäran
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API-fel: &quot;Fjärrservern returnerade ett fel (400) Ogiltig begäran&quot;

## Problem

Du får följande fel när du försöker använda API:t för att importera ett anpassat fält till ett problem:

`The remote server returned an error: (400) Bad Request`

## Orsak

Det här felet inträffar när du försöker importera ett anpassat fält från ett projekt via API som inte har något anpassat formulär kopplat till ett köämne.

## Lösning

Lägg till rätt anpassat formulär i avsnittet Kö.

Mer information om köämnen finns i [Skapa köämnen](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

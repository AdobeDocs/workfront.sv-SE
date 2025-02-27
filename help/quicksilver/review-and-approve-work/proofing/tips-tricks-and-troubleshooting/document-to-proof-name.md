---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Dokumentnamnet har ändrats efter överföringen och innehåller ett ogiltigt tecken
description: Vissa dokument kan inte konverteras till korrektur.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Dokumentnamnet har ändrats efter överföringen och innehåller ett ogiltigt tecken

## Problem

Vissa dokument kan inte konverteras till korrektur.

## Orsak

Filer som överförs till Workfront får inte innehålla vissa tecken i filnamn. Om en fil innehåller något av följande tecken i filnamnet, tas tecknen bort från filnamnet när filen överförs: `! # % * \ | ' " / ? < > { } [ ]`.

Om ett dokumentnamn uppdateras och innehåller ett ogiltigt tecken efter den första överföringen, kommer korrekturgenereringen att misslyckas.

## Lösning

Ta bort det ogiltiga tecknet från dokumentnamnet:

1. Markera dokumentet och klicka sedan på **Dokumentinformation**.
1. Klicka på dokumentnamnet, ta bort det ogiltiga tecknet och tryck på Retur.

   Ogiltiga tecken: `! # % * \ | ' " / ? < > { } [ ]`

   ![Dokumentnamn](assets/doc-name.png)

1. Uppdatera sidan och generera korrekturet.

---
title: Uppdrag i ett borttaget objekt visas oväntat i tilldelningsrapporter
description: Uppdrag i ett borttaget objekt visas oväntat i tilldelningsrapporter
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Uppdrag i ett borttaget objekt visas oväntat i tilldelningsrapporter

## Problem

När du har tagit bort ett objekt som har ett uppdrag tas både objektet och uppdraget bort. Men uppdraget kan fortfarande visas i vissa rapporter.

Om du t.ex. tar bort en uppgift som tilldelats en användare, tas även tilldelningen till användaren bort. Om du senare kör en uppgiftsrapport som filtreras efter den tilldelade, med den användaren angiven, visar rapporten fortfarande den borttagna uppgiften om uppgiften fortfarande finns i Papperskorgen.

## Orsak

Detta beror på arkitektoniska begränsningar i papperskorgen. Det finns för närvarande inga planer på att ta itu med denna fråga på grund av den omfattande arkitektoniska omdesign som skulle behövas.

---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Förhindra att åtgärden Beräkna om finanser påverkar historiska timmar när priserna ändras
description: Du måste uppdatera timkostnaden för en användare eller jobbroll (på grund av en höjning eller någon annan omständighet), men du vill inte att den här ändringen ska påverka timmar som tidigare har loggats i projekt eller du vill att den bara ska påverka en del av historiska timmar.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Förhindra att åtgärden Beräkna om finanser påverkar historiska timmar när priserna ändras

## Problem

Du måste uppdatera timkostnaden för en användare eller jobbroll (på grund av en höjning eller någon annan omständighet), men du vill inte att den här ändringen ska påverka timmar som tidigare har loggats i projekt eller du vill att den bara ska påverka en del av historiska timmar.

## Lösning

Lägg till de timmar som du inte vill ska ändras till en faktureringspost i projektet och ange status för faktureringsposten till Fakturerad.  Detta låser i den gamla kursen och ignoreras av åtgärden Beräkna om finanser.  Alla timmar som inte tillhör en faktureringspost beräknas till den nya avgiften. Mer information finns i [Beräkna om projektekonomi](../../manage-work/projects/project-finances/recalculate-project-finances.md).

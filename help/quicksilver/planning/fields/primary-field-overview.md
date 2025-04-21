---
title: Översikt över primärt fält
description: I tabellvyn för en posttyp i Adobe Workfront Planning kan du ange ett enradigt text-, tal- eller formelfält som primärt fält. Det primära fältet blir titeln på posterna av den typen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---


# Översikt över primärt fält

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Det primära fältet är det fält som visas i den första kolumnen i en posttypstabellvy i Adobe Workfront Planning.

Som standard är fältet Namn det primära fältet. Du kan dock ange alla fält av följande typer som primära fält för posterna:

* Enkelradigt textfält
* Nummer
* Formel

![Ett annat textfält är markerat som primärt fält](assets/another-text-field-as-a-primary-field-highlighted.png)

Mer information om hur du anger ett fält som primärt fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Översikt över primära fält

* Informationen i det fält som har angetts som primär blir postens titel.

  >[!NOTE]
  >
  >    Namnen&quot;primärt fält&quot; och&quot;posttitel&quot; är synonyma i Workfront Planning. Primärt fält är att föredra när du visar posten i tabellvyn.


* En posts titel visas i följande områden:

   * Rubrikområdet på postens sida och förhandsvisningsruta
   * Kopplade postfält
   * Vyer
* Du kan inte flytta, dölja eller ta bort det primära fältet i tabellvyn, såvida du inte anger ett annat fält som primärt fält.
* Det primära fältet är alltid låst och är inte en del av den vågräta rullningen i tabellvyn.
* Om du ändrar det primära fältet i tabellvyn påverkas vyn för alla andra användare som väljer det.
* Om du ändrar det primära fältet i en tabellvy påverkas alla tabellvyer av posttypen.
* Värdet i det primära fältet är alltid länkat till postens sida.
* Om du har Contribute eller högre behörighet för arbetsytan <span class="preview"> och posttypen </span> kan du redigera värdet för primära fält, förutom formelfält. Formler är beräkningar som uppdateras automatiskt.

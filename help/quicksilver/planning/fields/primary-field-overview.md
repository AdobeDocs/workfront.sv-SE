---
title: Översikt över primärt fält
description: I tabellvyn för en posttyp i Adobe Workfront Planning kan du ange ett enradigt text-, tal- eller formelfält som primärt fält. Det primära fältet blir titeln på posterna av den typen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# Översikt över primärt fält

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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
* Om du har Contribute eller högre behörighet för en arbetsyta <!--<span class="preview">and record type</span>--> kan du redigera värdet för primära fält, förutom för formelfält. Formler är beräkningar som uppdateras automatiskt.

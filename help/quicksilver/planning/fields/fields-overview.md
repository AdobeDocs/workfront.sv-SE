---
title: Fältöversikt
description: Du kan lägga till nya fält i Adobe Workfront Planning som återspeglar organisationens livscykel. Fält är attribut för posttyper.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 3667359ba2c6ea0aab3ce6845f1a537183f304ec
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---


# Fältöversikt

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Du kan lägga till nya fält i Adobe Workfront Planning som återspeglar organisationens livscykel. Fält är attribut för posttyper.


## Att tänka på när det gäller Adobe Workfront Planning Field

* Du kan bara skapa fält från tabellvyn för en posttypsida. Fält visas som kolumner i tabellvyn. Alla fält som är kopplade till en posttyp visas också på postsidan.

  Mer information om hur du hanterar tabellkolumner (eller postfält) finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

  Mer information om hur du hanterar fält finns i följande artiklar:

   * [Redigera fältinställningar](/help/quicksilver/planning/fields/edit-fields.md)
   * [Ta bort fält](/help/quicksilver/planning/fields/delete-fields.md)

* De fält som är associerade med en posttyp är tillgängliga för att associeras med alla poster av den typen. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Fält som är associerade med en posttyp kan inte läggas till i en annan posttyp. <!-- this will change when they open the Field library tab when creating a field-->

* Du kan skapa fält manuellt eller automatiskt på följande sätt:

   * Manuellt:

      * När du lägger till kolumner i tabellvyn på en posttypssida. Kolumnerna i tabellen är de fält som är associerade med posttypen. De är samma fält som visas på en postsida.

        Du kan inte skapa fält från postens sida.

      * När du ansluter posttyper. Du kan skapa länkade postfält när du lägger till en ny anslutning mellan två posttyper, eller en posttyp och en objekttyp från andra program.

        Mer information om att ansluta posttyper finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

      * När du importerar befintliga fält från Workfront.

        Mer information finns i [Importera fält från Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automatiskt:

      * När du skapar en posttyp:

         * Namn
         * Beskrivning
         * Startdatum
         * Slutdatum
         * Status. Standardvärdena för poststatus är:
            * Utveckling
            * Planerad
            * Aktiv
            * Slutförd
            * Parkerad

        Du kan lägga till fler värden eller byta namn på de befintliga.

      * När du skapar en arbetsyta från en mall.

        Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

      * När du importerar posttyper med en Excel- eller CSV-fil.

        Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

* Workfront planeringsfält är inte tillgängliga från Workfront.

* Workfront-fält är bara tillgängliga från Workfront Planning när du kopplar posttyper med Workfront-objekttyper och lägger till länkade fält eller uppslagsfält från Workfront-objekt. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

* Du kan visa och uppdatera inställningarna för de fält som du eller någon annan användare har skapat, om du har behörigheten Hantera på arbetsytan och den posttyp som fältet tillhör.

* Du kan ha upp till 500 fält för en posttyp.

* Fältnamn kan innehålla upp till 250 tecken.

* När du tar bort en posttyp eller arbetsyta tas även alla fält som är kopplade till dem och fältets värden bort och kan inte återställas. <!-- this might change with a possible recycle bin solution?!-->
* När du tar bort fält som ingår i ett formeluttryck ändras formelfältet.
* När du ändrar ett formeluttryck och det formelfältet refereras i andra formelfält påverkas även de andra formlerna.

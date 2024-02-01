---
title: Fältöversikt
description: Du kan lägga till nya fält i Adobe Maestro som återspeglar organisationens livscykel. Fält är attribut för posttyper.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Fältöversikt

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Du kan lägga till nya fält i Adobe Maestro som återspeglar organisationens livscykel. Fält är attribut för posttyper.


## Att tänka på när det gäller Maestro-fält

* Du kan bara skapa fält från tabellvyn för en posttypsida. Fält visas som kolumner i tabellvyn. Alla fält som är kopplade till en posttyp visas också på sidan Detaljer för varje post av den typen.

  Mer information om hur du hanterar tabellkolumner (eller postfält) finns i [Hantera tabellvyn](../views/manage-the-table-view.md).

  Mer information om hur du hanterar fält finns i följande artiklar:

   * [Redigera fält](../fields/edit-fields.md)
   * [Ta bort fält](../fields/delete-fields.md)

* De fält som är associerade med en posttyp är tillgängliga för att associeras med alla poster av den typen. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Fält som är associerade med en posttyp kan inte läggas till i en annan posttyp. <!-- this will change when they open the Field library tab when creating a field-->

* Du kan skapa fält manuellt eller automatiskt på följande sätt:

   * Manuellt:

      * Genom att lägga till kolumner i tabellvyn på en posttypssida. Kolumnerna i tabellen är de fält som är associerade med posttypen. De är samma fält som visas på en posts informationssida.

        Du kan inte skapa fält från detaljsidan för en post.

        I den här artikeln beskrivs hur du skapar fält manuellt.

      * Genom att ansluta posttyper. Du kan skapa länkade postfält när du lägger till en ny anslutning mellan två Maestro-posttyper, eller en posttyp och en objekttyp från andra program.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Mer information om hur du ansluter Maestro-posttyper finns i [Koppla posttyper](../architecture/connect-record-types.md).

      * Genom att importera posttyper med en Excel- eller CSV-fil. Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

   * Automatiskt:

      * Som standard varje gång du skapar en posttyp.

        Följande är standardfält som skapas som standard för varje ny operativ posttyp:

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

        Följande standardfält skapas som standard för varje ny taxonomiposttyp:

         * Namn <!--will more be added? If not, consider rephrasing this bullet-->

      * När du skapar en arbetsyta från en mall. I Maestro skapas fält för driftsposttyper och taxonomier när du skapar en arbetsyta från en mall. Mer information finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

* Makrofält är inte tillgängliga från Workfront.

* Workfront-fält är bara tillgängliga från Maestro när du kopplar Maestro-posttyper till Workfront-objekttyper och lägger till länkade eller sökbara fält från Workfront-objekt. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).

* Du kan visa och uppdatera inställningarna för de fält som du eller någon annan användare har skapat, om du har behörigheten Hantera för den arbetsyta som fältet tillhör.

* Du kan ha upp till 500 fält för en posttyp.

* Fältnamn kan innehålla upp till 250 tecken.

* När du tar bort en operativ posttyp, taxonomi eller arbetsyta tas även alla fält som är kopplade till dem och fältets värden bort och kan inte återställas. <!-- this might change with a possible recycle bin solution?!-->

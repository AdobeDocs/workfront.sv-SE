---
product-area: reports and dashboards
navigation-topic: data-connect
title: Använda vyn Övervaka datauppdateringar i Dataanslutning
description: Med Data Connect kan Workfront-administratörer få tillgång till detaljerade poster om de senaste uppdateringarna som gjorts i Data Lake-datumet under den senaste uppdateringen.
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Använda vyn Övervaka datauppdateringar i Dataanslutning

Vyn Övervaka datauppdateringar visar de senaste uppdateringarna som gjordes på datavjöns datum under den senaste uppdateringen. Den här vyns data uppdateras när en datainläsning har slutförts.

På grund av den stora datavolymen och aggregeringarnas komplexitet visas endast de objektvyer som har uppdaterats de senaste två veckorna i vyn Övervaka datauppdateringar. Om en viss posttyp saknas i den här vyn beror det troligen på att aktiviteten inte har utförts inom den tidsramen.

>[!NOTE]
>
>I den här vyn visas en detaljerad samling med data från programmet och uppdateringsaktiviteter i motsats till en daglig historik eller händelsevy som visar uppdateringsaktivitetshistorik. Om du vill få information om historisk uppdateringsaktivitet kan du använda <code>DL_LOAD_TIMESTAMP</code> datumobjekt.

## Vykolumner för övervakning av datauppdateringar

Vykolumnerna för uppdatering av övervakningsdata innehåller följande information:

<table>
    <tr>
        <td><b>Kolumnnamn</b></td>
        <td><b>Typ</b></td>
        <td><b>Beskrivning</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      Den objekttyp som är associerad med de Workfront-poster som har skickats till datasjön. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Datum</td>
        <td>
   Datumet för den senaste lyckade datauppdateringen för objekttypen som visas i kolumnen OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Tidsstämpel_NTZ</td>
        <td>
 Datum och tid för den senaste datauppdateringen för objekttypen som visas i kolumnen OBJ_TYPE.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Tidsstämpel_NTZ </td>
        <td>
       Datum och tid för den näst senaste datauppdateringen för objekttypen som visas i kolumnen OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Nummer</td>
        <td>
     Den tid i minuter som har gått sedan den senaste datauppdateringen för objekttypen. </td>
    </tr>
            <tr>
        <td>SKAPAD </td>
        <td>Nummer </td>
        <td>Antal CREATE-posthändelser som hämtats mellan föregående och senaste datauppdateringar för objekttypen.  </td>
    </tr>
                <tr>
        <td>UPPDATERAD</td>
        <td>Nummer </td>
        <td>Antal UPDATE-posthändelser som fångats mellan föregående och senaste datauppdateringar för objekttypen.</td>
    </tr>
                <tr>
        <td>BORTTAGEN</td>
        <td>Nummer </td>
        <td>Antal DELETE-posthändelser som samlats in mellan föregående och senaste datauppdateringar för objekttypen. </td>
    </tr>
                <tr>
        <td>TOTALT</td>
        <td>Nummer </td>
        <td>Antal händelser mellan föregående och senaste datauppdateringar för objekttypen. 
        <br> 
        <br><b> Obs! </b> Detta är inte detsamma som det totala antalet poster som påverkas av händelserna CREATE, UPDATE och DELETE eftersom samma post kan skapas och uppdateras flera gånger inom intervallet mellan uppdateringarna.  </td>
    </tr>
   </table>


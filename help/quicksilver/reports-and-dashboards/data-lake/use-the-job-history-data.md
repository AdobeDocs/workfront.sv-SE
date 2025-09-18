---
product-area: reports and dashboards
navigation-topic: data-connect
title: Använda vyn Jobbhistorik i Dataanslutning
description: Med Data Connect kan Workfront-administratörer få tillgång till detaljerade poster för varje datauppdateringsjobb i jobbhistorikvyn.
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 79e8b2b1dd3b7374173c2a930abdf8a0bca2cda6
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Använda vyn Jobbhistorik i Dataanslutning

I vyn Jobbhistorik kan Workfront-administratörer få tillgång till detaljerade poster för varje datauppdateringsjobb. Dessa poster ger värdefull insikt i de jobb som håller dina data uppdaterade och hjälper dig att skapa perfekta tidsramar för när processer ska köras och uppdatera dina affärsvisualiseringar.

![Vyn Jobbhistorik](assets/job-history-tab.png)

Kolumnerna i jobbhistorikvyn innehåller följande information:

* **OBJECT_NAME**: Visar namnet på objektet som är associerat med jobbet.
* **SCHEDULED_TIME**: Visar jobbets starttid.
* **COMPLETED_TIME**: Visar jobbets slutförandetid.
* **LATEST_FLAG**: Anger om jobbet ingick i den senaste uppdateringen.
* **LÄGE**: Visar jobbets status. Mer information finns i följande avsnitt i den här artikeln: [Tillgängliga jobbstatusar](#available-job-statuses).
* **LAST_UPDATED**: Jobbets senaste uppdaterade tidsstämpel.

>[!NOTE]
>
>Vyn Jobbhistorik innehåller information om de senaste 72 timmarna av schemalagda jobb.


## Tillgängliga jobbstatusvärden

Varje dataanslutningsjobb tilldelas en status som anger om det lyckades, hoppades över eller misslyckades.

<table>
    <tr>
        <td><b>Jobbstatus</b></td>
        <td><b>Definition</b></td>
    </tr>
    <tr>
        <td>Slutförd</td>
        <td>Alla tillgängliga uppdateringar har bearbetats och alla uppdateringar för den posttypen visas nu i datasjön.</td>
    </tr>
    <tr>
        <td>Överhoppad</td>
        <td>Jobbet hoppades över eftersom det inte fanns några uppdateringar i kön att bearbeta för posttypen.</td>
    </tr>
    <tr>
        <td>Misslyckades</td>
        <td>Det gick inte att köra jobbet. I dessa fall är det sannolikt att inga data i kön har sparats till datasjön. Poster som finns kvar i kön bearbetas i nästa schemalagda jobb för den posttypen. </td>
    </tr>
   </table>


## Överväganden om jobbkörning och loggningsbeteende

Snowflake använder ett optimeringsverktyg för jobbschemaläggare som kan påverka hur jobbkörningen bearbetas och loggas i jobbhistorikvyn. Detta loggningsbeteende kan variera beroende på om det finns data att bearbeta eller inte.

Om det till exempel inte finns några nya rader att bearbeta för ett givet objekt kan en av följande utfall inträffa:

* **Jobbet körs och markeras som Överhoppat**: Snowflake identifierar att det inte finns några rader att bearbeta, kör jobbet och registrerar det med statusen Överhoppat i tabellen.

* **Jobbet körs inte**: Snowflake fastställer att det inte finns några rader att bearbeta, kör inte jobbet och registrerar det med statusen Överhoppat i tabellen.

  >[!NOTE]
  >
  >I det andra scenariot där jobbet inte körs, kan den senaste posten för det objektet återspegla en tidsstämpel som inte stämmer överens med det förväntade schemat.

Ett jobb kan med andra ord betraktas som kört även om inga rader har bearbetats, och det kan vara eller inte vara loggat beroende på vad jobbschemaläggaren gör för det aktuella jobbet.
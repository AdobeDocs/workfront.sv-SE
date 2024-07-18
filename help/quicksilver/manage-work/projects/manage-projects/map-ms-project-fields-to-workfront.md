---
product-area: projects
navigation-topic: manage-projects
title: Mappa Microsoft Project-fält till Adobe Workfront-projekt
description: Projekt i Adobe Workfront och Microsoft Project är oftast kompatibla. I den här artikeln beskrivs hur de vanligaste projektfälten från de två programmen mappas till varandra.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Mappa Microsoft Project-fält till Adobe Workfront-projekt

Projekt i Adobe Workfront och Microsoft Project är oftast kompatibla. Med de två programmen kan du göra följande:

* Exportera projekt från Microsoft Project och importera dem till Workfront
* Exportera projekt från Workfront och importera dem till Microsoft Project. 

Mer information om hur du importerar projekt från Microsoft Project till Workfront finns i [Importera ett projekt från Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Mer information om hur du exporterar ett projekt från Workfront för att importera det till Microsoft Project finns i [Exportera ett projekt till Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

När du importerar sådana data är det viktigt att förstå hur informationen översätts från ett program till ett annat. I de flesta fall måste du göra några manuella ändringar i projektet när du har slutfört importen. 

## Översikt över fältmappning

>[!NOTE]
>
>Planerade datum stämmer inte alltid överens i båda systemen. Avvikelser kan beaktas genom scheman och skillnader i systeminställningarna mellan Workfront och Microsoft Project. Dessa datumavvikelser kan också leda till skillnader i arbetsinsats, varaktighet och procent färdigt.

| **Microsoft-projektfält** | **Workfront Field** |
|---|---|
| Projektets titel | Projektnamn |
| Start- och slutdatum | Planerade start- och slutförandedatum |
| Aktivitetsnamn | Aktivitetsnamn |
| Aktivitetsvaraktighet | Aktivitetsplanerad varaktighet |
| Uppgiftsarbete | Planerade timmar för aktivitet |
| Aktivitet % slutförd | Aktivitet % slutförd (baserat på aktivitetens varaktighet) |
| Aktivitet, arbete % slutfört | Aktivitet % slutförd (baserat på aktivitetens planerade timmar) |
| Schemalagd start och slut | Planerade start- och slutförandedatum |
| Verklig start och slut | Faktiska start- och slutförandedatum |
| Resursnamn | Uppgiftstilldelning |
| Tilldelningsenheter | Tilldelningsallokeringsprocent |
| Uppgiftsanteckning | Uppgiftsbeskrivning |
| Föregående | Föregående |

## Översikt över data som inte ingår

Det finns ett antal projektfält som inte importeras till eller exporteras från Workfront.

Dessa fält innehåller, men är inte begränsade till, följande:

* Bifogade dokument
* Anpassade fält (på projekt- eller aktivitetsnivå)
* Workfront notes
* Problem
* Negativ fördröjning i uppgifter med relationen Start/Slutför (uppgifter importeras utan fördröjning)
* Uppdrag
* Aktivitetsbegränsningar

  >[!NOTE]
  >
  >Eftersom begränsningar inte avbildas mellan Microsoft Project och Workfront bör du kontrollera att det finns föregående relationer mellan aktiviteterna. I annat fall är det inte säkert att de planerade start- och slutdatumen för aktiviteterna stämmer korrekt i det importerade projektet. 

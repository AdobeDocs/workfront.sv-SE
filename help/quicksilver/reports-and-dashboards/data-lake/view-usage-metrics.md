---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Visa användningsstatistik för Workfront Data Connect
description: På fliken Workfront Data Connect Metrics kan du visa organisationens användningsstatistik utifrån både månatlig beräkningstid och antalet utförda frågor.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Visa användningsstatistik för [!DNL Workfront Data Connect]

På fliken [!DNL Workfront Data Connect] [!UICONTROL Metrics] kan du visa din organisations användningsmått utifrån både antalet beräknade timmar som används och antalet utförda frågor. Organisationer har ett begränsat antal tillgängliga beräkningstimmar per månad baserat på licenstyp och tillägg till Data Connect. Fliken [!UICONTROL Metrics] visar information om tillgängliga månatliga beräkningstimmar i relation till vad som har använts.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Ingår i följande planer:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect är inte tillgängligt för tidigare Workfront-planer.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa användningsstatistik och tillgängliga beräkningstimmar

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på [!UICONTROL **Konfigurera**].

1. Klicka på [!UICONTROL **System**] > [!UICONTROL **Dataåtkomst**] i den vänstra panelen.

1. Klicka på fliken [!UICONTROL **Metrisk**]. Användningsstatistik visas i diagrammet **Beräkna användning**, medan antalet frågor som har utförts visas i diagrammet **Antal frågor**.

   ![Användningsstatistik för Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Valfritt) Du kan använda listrutan [!UICONTROL **Välj en vy**] om du vill ändra tidsintervallet för den information som finns i båda diagrammen.

1. (Valfritt) Du kan använda kryssrutorna ovanför diagrammet **Beräkna användning** för att visa eller dölja:
   * [!UICONTROL **Dagliga arbetstimmar för beräkning**] - Det antal timmar som din organisation använder dagligen.
   * [!UICONTROL **Månadsvis ackumulerade beräkningstimmar**] - Det totala antalet beräkningstimmar som används av organisationen under en månad. Återställs till noll varje månad.
   * [!UICONTROL **Månadsvis timersättning för beräkning**] - Antalet tillgängliga beräkningstimmar för din organisation baserat på licens- och/eller tilläggsköp.

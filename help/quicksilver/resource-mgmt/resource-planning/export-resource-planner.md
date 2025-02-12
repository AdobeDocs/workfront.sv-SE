---
product-area: resource-management
navigation-topic: resource-planning
title: Exportera information från resursplaneraren
description: Du kan exportera information från valfri vy i resursplaneraren till en Excel-fil (.xlsx) som sparas på datorn.
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Exportera information från resursplaneraren

Du kan exportera information från valfri vy i resursplaneraren till en Excel-fil (.xlsx) som sparas på datorn.

>[!IMPORTANT]
>
>Det finns begränsningar för vilken information som visas och vilken information du kan exportera från Resursplaneraren. Mer information om de här begränsningarna finns i [Resursplaneringsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Ljus eller högre</p>
       <p>eller</p>
       <p>Aktuell: Granska eller senare</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till projekt, användare och resurshantering</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportera information från resursplaneraren

{{step1-to-resourcing}}

**Planeraren** visas som standard.

1. Välj vyn för planeraren. Du kan välja något av följande alternativ:

   * Visa efter användare
   * Visa efter projekt
   * Visa efter roll

1. Klicka på **Exportera**.

   Dialogrutan Exportalternativ visas.

   ![Exportalternativ](assets/rp-export-options-box-350x421.png)

1. Ange följande information:\
   **Startdatum**: Startdatum för exporten. Den exporterade filen innehåller information om allokering och tillgänglighet från och med den första veckodagen som innehåller den dag du anger här.\
   **Antal perioder**: Antalet tidsperioder som du vill inkludera i filen. Standardvärdet är fyra perioder.\
   **Typ**: Den typ av tidsperioder som du vill visa informationen i den exporterade filen (veckor, månader eller kvartal).\
   Följande är de maximala tidsperioder som du kan exportera:

   * 52 veckor
   * 36 månader
   * 12 kvartal

   **Välj att exportera**: Beroende på vilken vy du valde kan du välja att exportera tillgänglighets- och budgeteringsinformation för antingen alla objekt som visas på skärmen eller för specifika objekt.
Du kan välja att exportera följande information:

   * I projektvyn väljer du att exportera:

      * Projekt
      * Projekt och roller
      * Allt (det här är standardalternativet)

   * I användarvyn väljer du att exportera:

      * Användare
      * Användare och projekt
      * Allt (det här är standardalternativet)

   * I rollvyn väljer du att exportera:

      * Roller
      * Roller och projekt
      * Allt (det här är standardalternativet)

   **Dataformatering**: Beroende på hur du vill att Excel-filen ska visas väljer du följande alternativ:

   * **Raw**: Välj det här alternativet om du vill visa tillgänglighets- och allokeringsinformation som delats upp av de objekt som det tillhör i Excel-filen. (det här är standardalternativet)
   * **Grupperad**: Välj det här alternativet om du vill visa tillgänglighets- och allokeringsinformation grupperad efter de objekt som den tillhör. Då visas den exporterade informationen så som den visas på skärmen.

   Ett exempel på hur informationen ser ut i den exporterade filen visas i dialogrutan Exportalternativ.

1. Klicka på **Exportera** om du vill exportera informationen från resursplaneraren.\
   Endast den information som du har sparat exporteras.

1. (Villkorligt) Om du har osparade budgeterade timmar i roll- eller projektvyerna klickar du på **Spara och fortsätt.**
En Excel-fil (.xlsx) hämtas till datorn.\
   Det går inte att exportera från resursplaneraren medan filen förbereds för hämtning.\
   (Villkorligt) Om du exporterar en stor mängd data får du ett e-postmeddelande med en länk dit du kan hämta filen.\
   ![RP_email_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Villkorligt) När du får e-postmeddelandet med den exporterade filen klickar du på **Hämta** för att hämta filen.\
   Du kommer då tillbaka till Workfront där du kan ladda ned filen.\
   Du måste vara inloggad på Workfront för att nedladdningen ska slutföras.\
   Om du inte hämtar filen när den levereras, är länken Hämta aktiv i 7 dagar efter att du har initierat exporten.

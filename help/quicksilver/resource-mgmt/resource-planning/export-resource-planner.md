---
product-area: resource-management
navigation-topic: resource-planning
title: Exportera information från resursplaneraren
description: Du kan exportera information från valfri vy i resursplaneraren till en Excel-fil (.xlsx) som sparas på datorn.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Exportera information från resursplaneraren

Du kan exportera information från valfri vy i resursplaneraren till en Excel-fil (.xlsx) som sparas på datorn.

>[!IMPORTANT]
>
>Det finns begränsningar för vilken information som visas och vilken information du kan exportera från Resursplaneraren. Information om dessa begränsningar finns i [Resursplanering - visningsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomst till projekt, användare och resurshantering</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Exportera information från resursplaneraren

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Resurser**. The **Planering** visas som standard.

1. Välj vyn för planeraren. Du kan välja något av följande alternativ:

   * Visa efter användare
   * Visa efter projekt
   * Visa efter roll

1. Klicka **Exportera**.

   Dialogrutan Exportalternativ visas.

   ![](assets/rp-export-options-box-350x421.png)

1. Ange följande information:\
   **Startdatum**: Startdatum för exporten. Den exporterade filen innehåller information om allokering och tillgänglighet från och med den första veckodagen som innehåller den dag du anger här.\
   **Antal perioder**: Antalet tidsperioder som du vill inkludera i filen. Standardvärdet är fyra perioder.\
   **Typ**: Den typ av tidsperioder som du vill visa informationen i den exporterade filen (veckor, månader eller kvartal).\
   Följande är de maximala tidsperioder som du kan exportera:

   * 52 veckor
   * 36 månader
   * 12 kvartal

   **Välj att exportera**: Beroende på vilken vy du har valt kan du välja att exportera tillgänglighets- och budgeteringsinformation för alla objekt som visas på skärmen eller för specifika objekt.
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

   * **Raw**: Välj det här alternativet om du vill visa tillgänglighets- och allokeringsinformation som delats upp av objekten som den tillhör i Excel-filen. (det här är standardalternativet)
   * **Grupperad**: Välj det här alternativet om du vill visa tillgänglighets- och allokeringsinformation grupperad efter de objekt som den tillhör. Då visas den exporterade informationen så som den visas på skärmen.

   Ett exempel på hur informationen ser ut i den exporterade filen visas i dialogrutan Exportalternativ.

1. Klicka **Exportera** om du vill exportera informationen från resursplaneraren.\
   Endast den information som du har sparat exporteras.

1. (Villkorligt) Om du har osparade budgettimmar i roll- eller projektvyerna klickar du på **Spara och fortsätt.**
En Excel-fil (.xlsx) hämtas till datorn.
\
   Det går inte att exportera från resursplaneraren medan filen förbereds för hämtning.\
   (Villkorligt) Om du exporterar en stor mängd data får du ett e-postmeddelande med en länk dit du kan hämta filen.\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Villkorligt) När du får e-postmeddelandet med den exporterade filen klickar du på **Hämta** för att hämta filen.\
   Du kommer då tillbaka till Workfront där du kan ladda ned filen.\
   Du måste vara inloggad på Workfront för att nedladdningen ska slutföras.\
   Om du inte hämtar filen när den levereras, är länken Hämta aktiv i 7 dagar efter att du har initierat exporten.

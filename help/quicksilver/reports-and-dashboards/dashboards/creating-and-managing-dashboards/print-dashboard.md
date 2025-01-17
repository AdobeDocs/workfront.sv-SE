---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Skriva ut en instrumentpanel
description: Du kan skriva ut eller exportera en kontrollpanel till en PDF-fil. Om du vill skriva ut en kontrollpanel måste du ha behörighet att visa den.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Skriva ut en instrumentpanel

<!-- Audited: 1/2025 -->

Du kan skriva ut eller exportera en kontrollpanel till en PDF-fil. Om du vill skriva ut en kontrollpanel måste du ha behörighet att visa den.

>[!NOTE]
>
>Den här funktionen är endast avsedd att användas med den vanliga instrumentpanelsvyn. Den är inte tillgänglig för kontrollpaneler som är inbäddade i området Projekt eller inställda som anpassade flikar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
      <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Arbeta eller högre</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Visa åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong>/td&gt; 
   <td> <p>Visa behörigheter på kontrollpanelen</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Kontrollpanelen måste skapas innan du kan skriva ut den.

Mer information om hur du skapar instrumentpaneler finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Förstå vilken information som skrivs ut när du skriver ut en kontrollpanel

När du skriver ut en kontrollpanel eller sparar den som en .PDF-fil kanske viss information från kontrollpanelen, så som den visas i Adobe Workfront webbprogram, inte visas i den utskrivna eller exporterade filen.

* [Vad visas?](#what-is-displayed)
* [Vad visas inte?](#what-is-not-displayed)

### Vad visas? {#what-is-displayed}

Följande information finns i den utskrivna eller exporterade kontrollpanelsfilen:

* Instrumentpanelens titel
* Rapportrubriker
* Tidsstämpel för när rapporten senast skapades
* Alla objekt på kontrollpanelen, inklusive listvyer, externa webbsidor, rapporter och kalendrar
* Ditt företags logotyp, om din Workfront-administratör har anpassat den i ditt globala navigeringsfält. Mer information om hur du varumärkar Workfront webbplats finns i [Varumärk din Adobe Workfront-instans](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Vad visas inte? {#what-is-not-displayed}

Följande information ingår inte i den utskrivna eller exporterade instrumentpanelsfilen:

* Workfront navigeringsfält
* All annan formatering som är specifik för Workfront
* Beroende på storleken på rapporterna och antalet och bredden på enskilda kolumner kan export och utskrift av en kontrollpanel resultera i att vissa kolumner klipps av.

## Skriva ut en instrumentpanel

1. Gå till kontrollpanelen som du vill skriva ut.
1. Gör något av följande:

   * Klicka på **Instrumentpanelsåtgärder** > **Förhandsgranska utskrift**

   * Tryck på **Ctrl+P** (Windows) eller **Kommando+P** (Mac)

     >[!IMPORTANT]
     >
     >* Inget av dessa alternativ är tillgängliga när kontrollpanelen är inbäddad på en anpassad flik. Mer information om hur du skapar anpassade flikar finns i [Skapa anpassade flikar eller avsnitt](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* Alternativet för kortkommandon är inte tillgängligt när du använder webbläsaren Internet Explorer.

1. I fältet **Mål** väljer du bland de olika utskriftsalternativen som är tillgängliga.\
   Utskriftsalternativen varierar beroende på vilken webbläsare och webbläsarversion du använder.

1. (Valfritt) Spara instrumentpanelen som en .PDF-fil och klicka sedan på **Spara** för att spara .PDF.\
   Mer information om hur du sparar kontrollpanelen som en .PDF-fil finns i [Exportera en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Klicka på **Skriv ut**.

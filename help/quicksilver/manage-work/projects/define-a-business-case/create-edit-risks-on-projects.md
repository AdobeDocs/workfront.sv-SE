---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Skapa och redigera risker i projekt
description: Risker är tänkbara händelser eller faktorer som förhindrar att ett projekt slutförs i tid eller inom budgeten. Du kan registrera projektrisker som en del av skapandet av ett projekts affärsfall eller genom att använda fliken Risker. Du kan lägga till risker i projekt och mallar. Du kan inte associera risker med uppgifter eller ärenden.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 9cfb67f627c06a5926e820860d52ba9f1ab58bcf
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Skapa och redigera risker i projekt

<!--Audited: 01/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

Risker är tänkbara händelser eller faktorer som förhindrar att ett projekt slutförs i tid eller inom budgeten. Du kan registrera risker när du skapar ett affärsärende för ett projekt eller genom att använda fliken Risker.

Du kan bara skapa risker i projekt eller mallar. Du kan inte associera risker med uppgifter eller ärenden.

Risker kan kopplas till kostnad, men den faktiska riskkostnaden påverkar inte projektets faktiska kostnad.

>[!NOTE]
>
>I den här artikeln definieras riskerna som är kopplade till projektet när du definierar dem i projektets affärsmodell eller när du lägger till dem på fliken Risker i projektet.
>
>Information om fältet Risk som är tillgängligt när du redigerar ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> 
   <p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard </p>
   <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter som innehåller Hantera finansiering för det projekt som du vill skapa eller redigera risker för </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa och redigera risker i affärsärendet

Du kan skapa risker som en del av planeringen av ett projekts affärsfall. Du kan redigera dem senare i affärsärendet, t.ex. när det sker ändringar av deras sannolikhet, reduceringsplan eller kostnad. Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Din Workfront-administratör eller gruppadministratör måste aktivera avsnittet **Risker** i ditt affärsärende i området Projektinställningar innan du kan visa det på projektnivå i avsnittet Affärsfall. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Att skapa och redigera risker i affärsärendet är identiskt.

Så här skapar eller redigerar du en risk i ett affärsärende:

1. Gå till det projekt som du vill skapa risker för.
1. Klicka på **Affärsfall** i den vänstra panelen.
1. I avsnittet **Risker** klickar du på **Redigera risker**.
1. Ange eller redigera följande information:

   * **Beskrivning:** beskriver risken.

   * **Potentiell kostnad**: ange den uppskattade kostnaden om risken ska inträffa.

   * **Sannolikhet**: ange sannolikheten för att risken inträffar som ett procentvärde.

   * **Typ:** anger vilken kategori risken tillhör.
   * **Åtgärdsplan**: Uppdatera beskrivningen av planen för att minska risken.

   * **Korrigeringskostnad**: ange kostnaden för den reduceringsplan som du måste installera för att förhindra att risken uppstår.

   ![Risker](assets/crp1-350x117.png)

1. (Valfritt) Klicka på **Lägg till ytterligare risk** om du vill lägga till ytterligare risker.
1. Klicka på **Spara**.

## Skapa och redigera risker i området Risker

Förutom att skapa och redigera risker i affärsärendet kan du göra det i avsnittet **Risker** i ett projekt.

Du kan skapa och redigera risker i avsnittet Risker i ett projekt eller en mall. Att skapa risker för mallar är detsamma som att skapa risker för projekt.

### Skapa risker i området Risker {#create-risks-in-the-risks-area}

1. Gå till det projekt som du vill skapa risker för.
1. Klicka på **Risker** i den vänstra panelen.

   ![Risker i aktiviteten](assets/risks-section-on-project-2022.png)

1. Klicka på **Börja lägga till risker** och skapa risker genom att redigera deras information. **Beskrivning** är ett obligatoriskt fält

   eller

   Klicka på **Ny risk**.

   Rutan **Ny risk** öppnas.

   ![Ny riskruta](assets/new-risk-box.png)

1. (Villkorligt) Om du lägger till en risk i rutan **Ny risk** anger du följande information:

   * **Beskrivning**: Beskriv risken. Detta är ett obligatoriskt fält.
   * **Risktyp**: Ange vilken kategori risken tillhör.\
     Din Workfront-administratör definierar de risktyper som är tillgängliga i din miljö. Mer information om hur du definierar risktyper finns i artikeln [Redigera och skapa risktyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Sannolikhet**: Ange sannolikheten för att risken inträffar som ett procentvärde.
   * **Potentiell kostnad**: Ange den uppskattade kostnaden om risken ska inträffa.
   * **Korrigeringskostnad**: Ange kostnaden för den reduceringsplan som du måste installera för att förhindra att risken uppstår.
   * **Faktisk kostnad**: Ange den faktiska kostnaden för risken om risken inträffade.
   * **Åtgärdsplan**: Uppdatera beskrivningen av planen för att minska risken.

1. (Villkorligt) Klicka på **Ange** om du skapar risken online.

   eller

   Klicka på **Spara** om du redigerar informationen i rutan **Ny risk** .

1. (Valfritt) Välj en annan **status** för risken i listrutan **Status** när du använder vyn **Standard** för listan över risker.

   Som standard är **Status** för en risk **Identifierad**.

### Redigera risker i området Risker {#edit-risks-in-the-risks-area}

Du kan redigera risker under ett projekts livslängd, t.ex. när ändringar sker i sannolikhet, potentiell kostnad eller status.

Du kan redigera en risk i taget eller redigera flera risker samtidigt.

Så här redigerar du risker:

1. Navigera till ett projekt där du vill redigera befintliga risker.
1. Klicka på **Risker** i den vänstra panelen.
1. Börja redigera fälten för de risker du ser i listan för att redigera en risk i taget.

   eller

   Markera en eller flera risker och klicka sedan på **Redigera** för att redigera flera risker samtidigt.

   >[!NOTE]
   >
   >Du använder samma information för alla valda risker när du redigerar flera risker samtidigt. Den information som är associerad med varje risk innan dina ändringar skrivs över i en gruppredigering.

1. Om du har klickat på **Redigera** öppnas rutan **Redigera risk** eller **Redigera risker** .

   Överväg att redigera följande fält:

   * **Beskrivning**: Redigera beskrivningen av risken.
   * **Risktyp**: ange vilken kategori risken tillhör.
   * **Sannolikhet**: Ange sannolikheten för att risken inträffar som ett procentvärde.
   * **Potentiell kostnad**: Ange den uppskattade kostnaden om risken ska inträffa.
   * **Korrigeringskostnad**: Ange kostnaden för den reduceringsplan som du måste installera för att förhindra att risken uppstår.
   * **Faktisk kostnad**: Ange den faktiska kostnaden för risken om risken inträffade.
   * **Åtgärdsplan**: Uppdatera beskrivningen av planen för att minska risken.

1. Klicka på **Spara**.
1. (Valfritt) Redigera **status** för en risk i listrutan **Status** när du använder vyn **Standard** för listan över risker.

   >[!NOTE]
   >
   >Du kan inte redigera **status** för risker i dialogrutan **Redigera risk** . Det kan du bara göra i en textbunden redigering.

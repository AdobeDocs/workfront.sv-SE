---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Skapa och redigera risker i projekt
description: Risker är tänkbara händelser eller faktorer som förhindrar att ett projekt slutförs i tid eller inom budgeten. Risker kan registreras som en del av skapandet av ett projekts affärsfall eller genom att använda fliken Risker. Risker skapas endast i ett projekt. Du kan inte associera risker med uppgifter eller ärenden.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Skapa och redigera risker i projekt

Risker är tänkbara händelser eller faktorer som förhindrar att ett projekt slutförs i tid eller inom budgeten. Risker kan registreras som en del av skapandet av ett projekts affärsfall eller genom att använda fliken Risker. Risker skapas endast i ett projekt. Du kan inte associera risker med uppgifter eller ärenden.

Risker kan kopplas till kostnad, men den faktiska riskkostnaden påverkar inte projektets faktiska kostnad.

>[!NOTE]
>
>I den här artikeln definieras riskerna som är kopplade till projektet när du definierar dem i projektets affärsmodell eller när du lägger till dem på fliken Risker i projektet. Information om vilket riskfält som är tillgängligt när du redigerar ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter som innehåller Hantera finansiering för det projekt som du vill skapa eller redigera risker för </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa och redigera risker i affärsärendet

Du kan skapa risker som en del av planeringen av ett projekts affärsfall. Du kan redigera dem senare i affärsärendet, t.ex. när det sker ändringar av deras sannolikhet, reduceringsplan eller kostnad. Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Workfront-administratören eller gruppadministratören måste aktivera **Risker** -avsnittet i ditt affärsärende i området Projektinställningar innan du kan visa det på projektnivå i avsnittet Affärsfall. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Att skapa och redigera risker i affärsärendet är identiskt.

Så här skapar eller redigerar du en risk i ett affärsärende:

1. Gå till det projekt som du vill skapa risker för.
1. Klicka **Affärsärende** i den vänstra panelen.
1. I **Risker** avsnitt, klicka **Redigera risker**.
1. Ange eller redigera följande information:

   * **Beskrivning:** beskriva risken.

   * **Potentiell kostnad**: Ange den uppskattade kostnaden om risken skulle inträffa.

   * **Sannolikhet**: ange sannolikheten för att risken inträffar som ett procentvärde.

   * **Typ:** ange vilken kategori risken tillhör.
   * **Åtgärdsplan**: uppdatera beskrivningen av planen för att minska risken.

   * **Korrigeringskostnad**: ange kostnaden för den reduceringsplan som du måste införa för att förhindra att risken uppstår.

   ![](assets/crp1-350x117.png)

1. (Valfritt) Klicka på **Lägg till ytterligare risk** för att lägga till ytterligare risker.
1. Klicka **Spara**.

## Skapa och redigera risker i området Risker

Förutom att skapa och redigera risker i affärsärendet kan du göra det med **Risker** del av ett projekt.

* [Skapa risker i området Risker](#create-risks-in-the-risks-area)
* [Redigera risker i området Risker](#edit-risks-in-the-risks-area)

### Skapa risker i området Risker {#create-risks-in-the-risks-area}

1. Gå till det projekt som du vill skapa risker för.
1. Klicka **Risker** i den vänstra panelen.

   ![Risker, aktivitetsavsnittet](assets/risks-section-on-project-2022.png)

1. Klicka **Börja lägga till risker** och skapa risker genom att redigera informationen.

   eller

   Klicka **Ny risk**. The **Ny risk** öppnas.

1. Ange följande information:

   * **Beskrivning**: beskriva risken.
   * **Risktyp**: ange vilken kategori risken tillhör.\
      Din Workfront-administratör definierar de risktyper som är tillgängliga i din miljö. Mer information om hur du definierar risktyper finns i artikeln [Redigera och skapa risktyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Sannolikhet**: ange sannolikheten för att risken inträffar som ett procentvärde.
   * **Potentiell kostnad**: Ange den uppskattade kostnaden om risken skulle inträffa.
   * **Korrigeringskostnad**: ange kostnaden för den reduceringsplan som du måste införa för att förhindra att risken uppstår.
   * **Faktisk kostnad**: Ange den faktiska kostnaden för risken om risken inträffade.
   * **Åtgärdsplan**: uppdatera beskrivningen av planen för att minska risken.

1. (Villkorligt) Klicka **Retur** om du skapar en risk direkt.

   eller

   Klicka **Spara** om du redigerar informationen i **Ny risk** -dialogrutan.

1. (Valfritt) Välj ett annat **Status** för risken, i **Status** nedrullningsbar meny, när **Standard** för att se listan över risker.

   Som standard är status för en risk **Identifierad**.

### Redigera risker i området Risker {#edit-risks-in-the-risks-area}

Du kan redigera risker under ett projekts livslängd, t.ex. när ändringar sker i sannolikhet, potentiell kostnad eller status.

Du kan redigera en risk i taget eller redigera flera risker samtidigt.

Så här redigerar du risker:

1. Navigera till ett projekt där du vill redigera befintliga risker.
1. Klicka **Risker** i den vänstra panelen.
1. Börja redigera fälten för de risker du ser i listan för att redigera en risk i taget.

   eller

   Välj en eller flera risker och klicka sedan på **Redigera** för att redigera flera risker samtidigt.

   >[!NOTE]
   >
   >Du använder samma information för alla valda risker när du redigerar flera risker samtidigt. Den information som är associerad med varje risk innan dina ändringar skrivs över i en gruppredigering.

1. Om du har klickat **Redigera**, **Redigera risk** öppnas.

   Överväg att redigera följande fält:

   * **Beskrivning**: redigera beskrivningen av risken.
   * **Risktyp**: ange vilken kategori risken tillhör.
   * **Sannolikhet**: ange sannolikheten för att risken inträffar som ett procentvärde.
   * **Potentiell kostnad**: Ange den uppskattade kostnaden om risken skulle inträffa.
   * **Korrigeringskostnad**: ange kostnaden för den reduceringsplan som du måste införa för att förhindra att risken uppstår.
   * **Faktisk kostnad**: Ange den faktiska kostnaden för risken om risken inträffade.
   * **Åtgärdsplan**: uppdatera beskrivningen av planen för att minska risken.

1. Klicka **Spara ändringar**.
1. (Valfritt) Redigera **Status** för en risk, i **Status** nedrullningsbar meny, när **Standard** för att se listan över risker.

   >[!NOTE]
   >
   >Du kan inte redigera **Status** riskerna i **Redigera risk** -dialogrutan. Det kan du bara göra i en textbunden redigering.

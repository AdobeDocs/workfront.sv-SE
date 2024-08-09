---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Redigera och skapa risktyper
description: Du kan lägga till risker i ett projekt i planeringsfasen för att identifiera potentiella hinder innan du godkänner något arbete. Risker är tänkbara händelser som kan förhindra att projektet slutförs i tid eller inom budgeten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 1%

---

# Redigera och skapa risktyper

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Du kan lägga till risker i ett projekt i planeringsfasen för att identifiera potentiella hinder innan du godkänner något arbete. Risker är tänkbara händelser som kan förhindra att projektet slutförs i tid eller inom budgeten.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Risktyper

Risktyper är etiketter som du kan använda för att kategorisera risker i rapporteringssyfte. De skapas i området **[!UICONTROL Setup]** av administratören för [!DNL Adobe Workfront]. När risktyper har etablerats i ditt **[!UICONTROL Setup]**-område är de universella för ditt system. Alla projektägare kan använda samma risktyper för sina projekt.

## Redigera och skapa risktyper

Vissa risktyper finns redan i [!DNL Workfront] som standard. För att tillgodose organisationens behov kan du antingen redigera befintliga risktyper eller skapa nya risktyper.

* [Redigera befintliga risktyper](#edit-existing-risk-types)
* [Skapa nya risktyper](#create-new-risk-types)

### Redigera befintliga risktyper {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Risk Types]**.
1. Välj den risktyp som du vill redigera.
1. Klicka på **[!UICONTROL Edit]**.
1. (Valfritt) Ändra namn och beskrivning av risktypen.

   Det finns en teckengräns på 50 tecken för fälten **[!UICONTROL Name]** och **[!UICONTROL Description]**.

1. Klicka på **[!UICONTROL Save Changes].**

### Skapa nya risktyper {#create-new-risk-types}

Du kan skapa nya risktyper, utöver standardrisktyperna, för att återspegla organisationens behov.

Så här skapar du en ny risktyp:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Risk Types]**.
1. Klicka på **[!UICONTROL New Risk Type]**.
1. Ange **[!UICONTROL Name]** (obligatoriskt) och **[!UICONTROL Description]** (valfritt) för risktypen.

   Det finns en teckengräns på 50 tecken för fälten **[!UICONTROL Name]** och **[!UICONTROL Description]**.

1. Klicka på **[!UICONTROL Create Risk Type]**. Om du använde infogad redigering för att lägga till din risktyp klickar du på **[!UICONTROL Enter]** när du är klar.

   >[!NOTE]
   >
   >Om du behöver redigera en anpassad risktyp läser du avsnittet [[!UICONTROL Edit existing] risktyper ](#edit-existing-risk-types) i den här artikeln.

## Bifoga risker med risktyper i projekt

Risktyper kan användas för märkning av risker som läggs till i dina projekt. Mer information om hur du lägger till risker i projekt finns i [Skapa och redigera risker i projekt](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

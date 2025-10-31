---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopiera en projektmall
description: Förutom att skapa en projektmall från grunden kan du även kopiera en befintlig mall och ändra den.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Kopiera en projektmall

<!--Audited: 5/2025-->

Förutom att skapa en projektmall från grunden kan du även kopiera en befintlig mall och ändra den i Adobe Workfront.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

Du måste ha följande åtkomst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller ge högre behörighet till en mall</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på när du kopierar mallar

Följande objekt kopieras alltid från en befintlig mall till en ny:

* Malluppgifter
* Standardinformation för mallaktivitet (process för standardgodkännande av aktivitet, anpassad Forms för standarduppgift)
* Egna formulär
* Risker
* Information om köinställningar
* Portfolio och Program
* Godkännanden
* Dokument
* Dagarna för de ursprungliga malluppgifterna överförs till den nya mallen. Du måste ändra mallens start- eller slutförandedag (beroende på schemaläge) för att uppdatera de dagar som malluppgifterna gäller, om det behövs.

Följande objekt kopieras aldrig från en befintlig mall till en ny:

* Faktureringstaxor
* Användarkommentarer

## Kopiera en mall

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Gå till mallen som du vill kopiera.
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) till höger om mallnamnet i sidhuvudet och klicka sedan på **Kopiera**.

   Rutan **Kopiera mall** öppnas.

   ![Kopiera mallruta](assets/copy-template-box.png)

1. Ange ett namn för mallen i fältet **Nytt mallnamn**.

   Som standard anger Workfront det nya namnet enligt följande format: `Copy of Original template name`.

1. Välj alternativet **Behåll användartilldelningar för uppgifter och mall** om du vill överföra alla uppgifter och malltilldelningar från den ursprungliga mallen till den nya mallen. Uppgiftstilldelningar för mallar, mallägare och sponsor överförs till den kopierade mallen.
1. Klicka på **Spara** för att skapa en kopia av mallen.

   Den nya mallen visas i malllistan i mallområdet i Workfront.

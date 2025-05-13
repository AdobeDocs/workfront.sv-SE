---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopiera en projektmall
description: Förutom att skapa en projektmall från grunden kan du även kopiera en befintlig mall och ändra den.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 0d968a3f398c2e7dc4154cd5a16acf35ca7c86f5
workflow-type: tm+mt
source-wordcount: '322'
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
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td><p>Nytt: Standard</p> 
   <p>Aktuell: Planera </p> </td> 
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
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/qs-more-icon-on-an-object.png) till höger om mallnamnet i sidhuvudet och klicka sedan på **Kopiera**.

   Rutan **Kopiera mall** öppnas.

   <!--![Copy template box](assets/copy-template-box.png)-->

1. Ange ett namn för mallen i fältet **Nytt mallnamn**.

   Som standard är det nya namnet `Copy of Original template name`.

1. Välj alternativet **Behåll användartilldelningar för uppgifter och mall** om du vill överföra alla uppgifter och malltilldelningar från den ursprungliga mallen till den nya mallen. Uppgiftstilldelningar för mallar, mallägare och sponsor överförs till den kopierade mallen.
1. Klicka på **Spara** för att skapa en kopia av mallen.

   Den nya mallen visas i malllistan i mallområdet i Workfront.

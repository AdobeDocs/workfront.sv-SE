---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopiera en projektmall
description: I stället för att skapa en ny projektmall från grunden kan du kopiera en befintlig mall och ändra den om det behövs.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Kopiera en projektmall

I stället för att skapa en ny projektmall från grunden kan du kopiera en befintlig mall och ändra den om det behövs.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mallar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller ge högre behörighet till en mall</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.


## Att tänka på när du kopierar mallar

Följande objekt kopieras alltid från ett befintligt projekt till ett nytt:

* Malluppgifter
* Standardinformation för mallaktivitet (process för standardgodkännande av aktivitet, anpassad Forms för standarduppgift)
* Egna formulär
* Risker
* Information om köinställningar
* Portfolio och Program
* Godkännanden
* Dokument
* Dagarna för de ursprungliga malluppgifterna överförs till den nya mallen. Du måste ändra mallens start- eller slutförandedag (beroende på schemaläge) för att uppdatera de dagar som malluppgifterna gäller, om det behövs.

Följande objekt kopieras aldrig från ett befintligt projekt till ett nytt:

* Faktureringstaxor
* Användarkommentarer

## Kopiera en mall

1. Gå till mallen som du vill kopiera.
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/qs-more-icon-on-an-object.png) och klicka sedan på **Kopiera**.
1. Ange ett namn för mallen i fältet **Nytt mallnamn**.

   Som standard är det nya namnet **Kopia av `<original template name>`.**

1. Välj om du vill **Bevara användartilldelningar för uppgifter och mallar**: välj det här alternativet om du vill överföra alla uppgifter och malltilldelningar från den ursprungliga mallen till den nya mallen.
1. Klicka på **Spara** för att skapa en kopia av mallen.

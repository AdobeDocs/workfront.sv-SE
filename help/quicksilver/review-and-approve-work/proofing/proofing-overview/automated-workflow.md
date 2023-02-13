---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Översikt över automatiserat arbetsflöde
description: Med automatiserade arbetsflöden kan du skapa en serie sekventiella eller parallella granskningsfaser, upprätta beroenden mellan dessa faser och begränsa synligheten för vissa användare. Om granskningsprocessen består av olika steg flyttar automatiserade arbetsflöden automatiskt korrekturet genom de olika stegen och informerar berörda granskare och godkännare längs vägen. Mer information om hur du ställer in ett automatiserat arbetsflöde finns i Skapa ett avancerat korrektur med ett automatiserat arbetsflöde.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Översikt över automatiserat arbetsflöde

Med automatiserade arbetsflöden kan du skapa en serie sekventiella eller parallella granskningsfaser, upprätta beroenden mellan dessa faser och begränsa synligheten för vissa användare. Om granskningsprocessen består av olika steg flyttar automatiserade arbetsflöden automatiskt korrekturet genom de olika stegen och informerar berörda granskare och godkännare längs vägen. Mer information om hur du konfigurerar ett automatiskt arbetsflöde finns i [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Exempel:**  Automatiska arbetsflöden hjälper er att hantera komplexa korrekturgranskningsprocesser som

* När olika grupper eller granskare måste granska innehållet i en viss ordning
* När det finns beroenden mellan användarens aktivitet när de granskar innehållet
* När innehåll granskas regelbundet av samma grupper
* När du vill styra hur länge granskarna tittar på innehållet
* När du vill hålla viss granskningsaktivitet privat

## Steg

För varje automatiserad arbetsflödesfas kan du konfigurera inställningar som en deadline för scenen, ett lås på en scen, en granskare som har valts som beslutsfattare för scenen samt en sekretessinställning som bara tillåter vissa personer att se granskarnas kommentarer på scenen.

Stegen kan aktiveras manuellt, när du skapar ett korrektur, när du har nått en deadline, ett visst datum och en viss tid eller när ett beslut fattas på den överordnade fasen.

Stegen kan låsas manuellt, liksom när nästa steg startar eller när alla beslut fattas på scenen. Du kan också välja att aldrig låsa en scen.

Du kan utse en primär beslutsfattare för en fas. Personens beslut gör alla andra beslut för scenen onödiga.

På samma sätt kan du välja att bara begära ett beslut för en fas. När du gör det markeras granskningsprocessen för scenen som slutförd efter att någon av mottagarna har fattat sitt beslut på scenen.

Du kan låta alla granskare få meddelande om sin inbjudan att granska innehållet när granskningsprocessen påbörjas, eller så kan du låta varje granskare få ett meddelande först när deras scen aktiveras.

## Privata faser

Som standard är kommentarer som lämnas av granskare i alla steg synliga för alla som granskar innehållet och får e-postmeddelanden och kommentarssammanfattningar om granskningsprocessen.

Om du vill förhindra att vissa grupper av granskare ser andra granskares kommentarer, kan du skapa privata faser.

Privata faser är bara synliga för granskare som har lagts till i de stegen. De är också synliga för användare som har redigeringsbehörighet för korrektur eller redigeringsbehörighet för alla objekt som skapas i din organisations Adobe Workfront-konto (Supervisor och senare eller användare med anpassade profiler för vilka redigering av andra personers information är aktiverat).

Kommentarer som lagts till av deltagare på den privata scenen ingår inte i e-postmeddelanden och korrekturkommentarssammanfattningar som begärts av någon som inte har behörighet att visa dem.

## Arbetsflödesdiagram

Arbetsflödesdiagrammet är en visuell representation av korrekturets granskningsprocess. Här visas ordningen för steg och eventuella beroenden mellan faser när du skapar eller visar information om ett korrektur. Alla privata faser visas med en nyckelsymbol.

![intro-to-aw-example-chart.png](assets/intro-to-aw-example-diagram-350x199.png)

I live-korrektur visas scenberoenden med en streckad grå linje för inaktiva stadier eller en heldragen svart linje för aktiva stadier. Stegen visas i grönt om godkännandeprocessen slutfördes inom den angivna tidsgränsen. Fas som närmar sig sina deadlines visas i orange och i faser efter att de har visat sin deadline i rött.

![workflow_2.png](assets/workflow-2-350x183.png)

## Automatiserade arbetsflödesmallar

Om man använder samma granskningsprocess för flera korrektur kan Workfront-administratören skapa mallar för automatiserat arbetsflöde som gör det enklare att skapa korrektur. Du kan välja en mall för automatiserat arbetsflöde när du konfigurerar ett korrektur för att lägga till faserna och granskarna i mallen i korrekturet. Du kan ändra mallen som används för korrekturet efter behov innan och efter det att du har skapat korrekturet.

Din Workfront-administratör kan skapa ett obegränsat antal mallar utifrån ditt företags behov.

Om du vill veta mer om hur du skapar, använder och hanterar mallar kan du kontakta Workfront-administratören.

---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Svara på uppdateringar
description: När någon lägger till eller svarar i en uppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden på fliken Uppdateringar för objektet. Du kan lägga till ett svar på en uppdatering eller gilla det om du har åtkomst till objektet via Visa.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---

# Svara på uppdateringar

När någon lägger till eller svarar i en uppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden på fliken Uppdateringar för objektet. Du kan lägga till ett svar på en uppdatering eller gilla det om du har åtkomst till objektet via Visa.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Begär eller högre för frågor och dokument. Granska eller högre för alla andra objekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>begärande eller högre för frågor och dokument, Granskare eller högre för alla andra objekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till objektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Svara på en uppdatering eller ett svar

1. Gå till det objekt som du vill lägga till ett svar på.
1. På **Uppdateringar** Leta reda på den uppdatering eller det svar som du vill svara på.

   Så här visar du en bild i uppdateringen:

   * Klicka på **Förhandsgranska** icon ![](assets/previewimageicon-31x31.png) på miniatyrbilden för att öppna bilden i full storlek på en ny flik i webbläsaren.
   * Klicka på **Hämta** icon ![](assets/downloadimageicon.png) på miniatyrbilden för att hämta bilden.

   Förutom att se vilka användare som aktivt deltar i konversationen kan du se vilka som är taggade i varje svar högst upp i uppdateringstråden. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet. Du kan också tagga fler användare så att de inkluderas i ditt svar.  Om du vill tagga fler användare läser du [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. Klicka **Svara** på uppdateringen skriver du ett svar i rutan som visas.
1. (Valfritt) Om du vill ta med text från en tidigare uppdatering i ditt svar klickar du på **Mer** -menyn bredvid den uppdatering eller det svar som du vill citera och klicka sedan på **Offertsvar**. Texten från föregående uppdatering visas i indataområdet, markerat med en grå linje.
1. (Valfritt) Använd formatering och känslolägesikoner och inkludera länkar och bilder enligt anvisningarna i avsnittet [Lägga till en uppdatering i en arbetsuppgift](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) i artikeln [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Klicka **Svara** för att spara svaret.

   eller

   Klicka **Klar** om uppgiften eller utgåvan har statusen Slutförd eller Stängd.

## Svara på en uppdatering via e-postmeddelande

Beroende på hur dina e-postmeddelanden är konfigurerade kan du få ett e-postmeddelande när en uppdatering görs för vissa objekt som du har åtkomst till.

>[!NOTE]
>
>Det går inte att svara på uppdateringar via e-post i miljöer med kluster 6.

Följande är ett exempel på ett e-postmeddelande som utlöses som ett resultat av en uppdatering som görs på fliken Uppdateringar för en uppgift:

![email.png](assets/email-350x202.png)

Från e-postmeddelandet kan du enkelt lägga till ett svar direkt i kommunikationstråden för objektet i Workfront. Du kan också lägga till ett svar utan att logga in på Workfront, i ett e-postmeddelande som genereras av kommentarer som gjorts i följande objekt:

* Projekt
* Uppgift
* Problem
* Dokument
* Mall- och malluppgift
* Portfolio
* Program
* Upprepning
* Tidrapport

### Svara på en uppdatering från ett e-postmeddelande

När du får ett e-postmeddelande kan du snabbt öppna det associerade Workfront-objektet och lägga till ett svar direkt i kommunikationstråden.

1. Klicka **Kommentar** i e-postmeddelandet.

   Sidan Detaljer för objektet öppnas i Workfront.

1. Gå till uppdateringen som du vill lägga till ett svar på.

   Förutom att se vilka användare som aktivt deltar i konversationen kan du se vilka som taggats i varje svar högst upp i uppdateringstråden. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får meddelanden när en uppdatering eller ett svar görs för objektet. Om du vill tagga fler användare läser du [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Klicka **Svara,** ange ditt svar och klicka sedan på **Svara**.

### Lägga till en uppdatering till ett objekt utanför Workfront

När du får ett e-postmeddelande från Workfront kan du snabbt lägga till en uppdatering i kommunikationstråden utan att logga in på Workfront.

Så här lägger du till en uppdatering i ett e-postmeddelande från Workfront:

1. Öppna e-postmeddelandet från ditt e-postprogram som du vill svara på och öppna sedan ett svars-e-postfönster.
1. Skriv in uppdateringen.\
   Bifogade filer tillåts inte och eventuell RTF-formatering som används på en uppdatering i ett e-postmeddelande visas inte på uppdateringen när den visas på fliken Uppdateringar.
1. Klicka **Skicka**.

   Din uppdatering läggs till i kommunikationstråden för objektet.

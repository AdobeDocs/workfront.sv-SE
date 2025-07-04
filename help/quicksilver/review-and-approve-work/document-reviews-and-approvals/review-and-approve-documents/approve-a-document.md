---
product-area: projects
navigation-topic: approvals
title: Godkänn ett dokument i Workfront
description: Om du tilldelas som godkännare för ett dokument finns det flera sätt att fatta beslut om godkännande.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 1f7a17206ca77442b501f121f3333d4b60aa85f1
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 0%

---

# Godkänn ett dokument i Workfront

Om du tilldelas som godkännare för ett dokument finns det flera sätt att fatta beslut om godkännande.

Mer information om hur du skapar ett nytt dokumentgodkännande finns i [Skapa en begäran om dokumentgranskning eller godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Innehållet i den här artikeln hänvisar till den uppdaterade funktionen för dokumentgodkännande som bara är tillgänglig för specifika konton. Mer information om standardgodkännandeprocesser finns i artiklarna i [Arbetsgodkännanden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till objekt som är kopplade till godkännanden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för objekt som är associerade med godkännanden</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Godkänn ett dokument från startsidan

1. Klicka på ikonen **Hem** ![Hem](../assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på ikonen **Huvudmeny** ![Huvudmeny](../assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Klicka på **Filter** längst upp till vänster på sidan och kontrollera att **Godkännanden** är markerat.

   Alla arbetsobjekt som kräver ditt godkännande visas i listan.

   >[!NOTE]
   >
   >* Godkännanden som tilldelats till jobbroller eller grupper visas inte i Hem.
   >* Godkännanden som tilldelats team visas i varje enskild teammedlems widget för Mina godkännanden i Hem.

1. Klicka på det dokumentgodkännande i listan som du vill godkänna. Information om godkännandet visas till höger på sidan.

1. Klicka på något av följande två godkännandealternativ i det övre högra hörnet på sidan:

   * Listrutan **Godkänn** innehåller två alternativ:

      * **Godkänn** anger att inga ändringar behövs för den här versionen av dokumentet och att godkännande ges.

      * **Godkänn med ändringar** indikerar att vissa små ändringar fortfarande krävs i dokumentet, men godkännande ges om ändringarna görs. Om du väljer det här alternativet visas ett fönster som innehåller en textruta med namnet **Nästa steg** där du kan ange vilka ändringar som krävs för att dokumentet ska godkännas. Du kan antingen ange den informationen och klicka på **Lägg till meddelande** eller klicka på **Hoppa över** för att skicka godkännandebeslutet utan ytterligare information.

   * **Behöver arbete** indikerar att dokumentversionen inte är godkänd och kräver betydande ändringar.

   Tänk på följande när du visar dokumentgodkännanden i hemmet:

   * Namnet på den användare som begärde godkännandet visas ovanför dokumentnamnet i Hem med texten *Användare A* vill ha ditt godkännande den..., samt under **Skickat av** i godkännandeinformationen som visas till höger när ett godkännande har valts.

   * När ett beslut har fattats om ett godkännande behålls godkännandet på fliken Mina godkännanden med texten &quot;Beslutsfattad&quot; tills du klickar på knappen **Uppdatera** eller tills du uppdaterar webbläsarsidan.

## Godkänn ett dokument från dokumentsidan

1. Gå till dokumentsidan genom att klicka på dokumentets namn.

1. Välj den version av dokumentet som väntar på ditt godkännande i listrutan för version bredvid dokumentets namn. Den senaste versionen väljs som standard.

   Om den aktuella versionen av dokumentet har ett väntande godkännande visas beslutsmenyerna i det övre högra hörnet på sidan. Om andra versioner av dokumentet har väntande godkännanden visas en röd punkt på den nedrullningsbara versionsmenyn.

   <!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Klicka på något av följande två godkännandealternativ i det övre högra hörnet på sidan:

   * Listrutan **Godkänn** innehåller två alternativ:

      * **Godkänn** anger att inga ändringar behövs för den här versionen av dokumentet och att godkännande ges.

      * **Godkänn med ändringar** indikerar att vissa små ändringar fortfarande krävs i dokumentet, men godkännande ges om ändringarna görs. Om du väljer det här alternativet visas ett fönster som innehåller en textruta med namnet **Nästa steg** där du kan ange vilka ändringar som krävs för att dokumentet ska godkännas. Du kan antingen ange den informationen och klicka på **Lägg till meddelande** eller klicka på **Hoppa över** för att skicka godkännandebeslutet utan ytterligare information.

   * **Behöver arbete** indikerar att dokumentversionen inte är godkänd och kräver betydande ändringar.

## Godkänn ett dokument från panelen Dokumentsammanfattning

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.

1. Klicka på dokumentet som ska godkännas och panelen Dokumentsammanfattning öppnas.

1. Välj den version av dokumentet som du vill granska i listrutan. Den senaste versionen väljs som standard.

   Om den aktuella versionen av dokumentet har ett väntande godkännande visas beslutsmenyknapparna i det övre högra hörnet på panelen Dokumentsammanfattning. Om andra versioner av dokumentet har väntande godkännanden visas en röd punkt på den nedrullningsbara versionsmenyn.
<!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
 -->
1. Klicka på något av följande två godkännandealternativ i det övre högra hörnet av panelen Dokumentsammanfattning:

   * Listrutan **Godkänn** innehåller två alternativ:

      * **Godkänn** anger att inga ändringar behövs för den här versionen av dokumentet och att godkännande ges.

      * **Godkänn med ändringar** indikerar att vissa små ändringar fortfarande krävs i dokumentet, men godkännande ges om ändringarna görs. Om du väljer det här alternativet visas ett fönster som innehåller en textruta med namnet **Nästa steg** där du kan ange vilka ändringar som krävs för att dokumentet ska godkännas. Du kan antingen ange den informationen och klicka på **Lägg till meddelande** eller klicka på **Hoppa över** för att skicka godkännandebeslutet utan ytterligare information.

   * **Behöver arbete** indikerar att dokumentversionen inte är godkänd och kräver betydande ändringar.


## Godkänn ett dokument från korrekturläsaren

Så här granskar och godkänner du ett dokument:

1. Gå till e-postmeddelandet för din granskning och klicka på **Gå till granskning**.

1. När du är i Workfront klickar du på **Gå till korrektur**.

1. Granska innehållet och lägg in kommentarer och markeringar. Mer information om hur du använder korrekturläsaren finns i [Granska korrektur i Adobe Workfront: artikelindex](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Välj något av följande:

   * **Godkänn**: Dokumentet behöver inte ändras och är klart att användas.
   * **Godkänn med ändringar**: Dokumentet behöver ändras och är klart att användas när de har gjorts. Ytterligare godkännande krävs inte.
   * **Behöver arbete**: Dokumentet behöver ändras och är inte klart att användas. När de angivna ändringarna har gjorts måste dokumentet överföras som en ny version och gå igenom en ny godkännandeomgång. Mer information om hur du överför en ny version finns i [Skapa en ny version efter behov](#create-a-new-version-as-needed) i den här artikeln.

När du har fattat ett beslut meddelas dokumentägaren via e-post.



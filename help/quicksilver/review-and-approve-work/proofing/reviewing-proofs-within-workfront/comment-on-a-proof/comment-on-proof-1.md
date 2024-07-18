---
product-area: documents
navigation-topic: comment-on-a-proof
title: Kommentera ett korrektur
description: Med kommentarer kan du ge feedback på innehåll och samarbeta med andra användare i korrekturläsaren.
author: Courtney
feature: Digital Content and Documents
exl-id: b0386786-7f90-4d1c-bd3a-1cd545430de1
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Kommentera ett korrektur

Med kommentarer kan du ge feedback på innehåll och samarbeta med andra användare i korrekturläsaren.

När du taggar användare i kommentarer om ett korrektur kan de användare som du kan tagga variera beroende på olika faktorer, till exempel individuella användarbehörigheter och ditt medlemskap i organisationen:

* Om du har skapat, äger eller har aktiverat specifika behörigheter kan du tagga användare utanför korrekturarbetsflödet och dela korrekturet med dem.
* Om du har lagts till i beviset som en extern användare och är medlem i en annan miljö med ett annat korrekturkonto, kan du bara tagga de användarna från din ursprungliga miljö. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturroll</td> 
   <td>Granskare, granskare och godkännare, moderator, författare</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Kommentera ett korrektur

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Leta reda på det korrektur du behöver och klicka sedan på **Öppna korrektur**.

1. Klicka på **Lägg till kommentar** överst i korrekturläsaren.
1. (Villkorligt) Om det här är ett videoklipp spelar du upp videoklippet och klickar sedan på **Lägg till kommentar** vid den punkt i videon där du vill att kommentaren ska använda spelhuvudet

   >[!TIP]
   >
   >1. Gör en paus i videon och klicka på den tidslinje där du vill ha kommentaren.
   >1. För bättre precision kan du klicka på värdena ovanför spelhuvudet och skriva nya värden.
   >1. Om du vill kommentera ett intervall av videoklipp drar du spelhuvudet åt vänster och höger i tidslinjen för att ange ett intervall med tagningar som du vill kommentera i.
   >1. Om du vill kommentera ett intervall av videoklipp drar du spelhuvudet åt vänster och höger i tidslinjen för att ange ett intervall med tagningar som du vill kommentera i.

1. Om du vill rikta uppmärksamheten mot en viss plats i korrekturet klickar du på markeringsverktyget i verktygsfältet och markerar sedan det område i korrekturet som du vill kommentera:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Draw en frihandslinje</strong> </td> 
      <td> <img src="assets/freehand-line.png"> </td> 
      <td>Gör att du kan lägga till en frihandslinje på det markerade området.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Draw a line</strong> </td> 
      <td> <img src="assets/line.png"> </td> 
      <td>Gör att du kan rita en linje på det markerade området.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Draw en pil</strong> </td> 
      <td> <img src="assets/arrow.png"> </td> 
      <td>Gör att du kan lägga till en pil i ett område som du markerar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Markera ett område</strong> </td> 
      <td> <img src="assets/highlight.png"> </td> 
      <td>Markerar det markerade området.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Draw en rektangel</strong> </td> 
      <td> <img src="assets/rectangle.png"> </td> 
      <td>Gör att du kan rita en rektangel runt ett område.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Polyline</strong> </td> 
      <td> <img src="assets/polyline.png"> </td> 
      <td> <p>Ritar en kopplad sekvens med linjesegment som du kan lämna öppna eller nära som en form. Du kan flytta eller ta bort punkter som du lägger till. </p> <p>Det här verktyget är användbart när du arbetar med tekniska bilder och arkitektoniska bilder.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ändra markeringsfärg, tjocklek eller opacitet</strong> </td> 
      <td> <img src="assets/change-color.png"> </td> 
      <td>Här kan du ändra färg, tjocklek och opacitet för markeringsverktygen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Text</strong> </td> 
      <td> <img src="assets/copy-of-text.png"> </td> 
      <td> <p>Det här verktyget visas till vänster om de andra verktygen när korrekturet är ett textbaserat dokument. Det innehåller markeringsverktyg för att kommentera text i korrektur. <br></p> <p>När du klickar på det här verktyget och sedan markerar text i korrekturet visas anteckningsalternativen under den markerade texten.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. I statiskt korrektur kan du markera flera områden på flera sidor för en kommentar. Om du till exempel vill göra samma kommentar på flera sidor, markerar du ett område på en sida, går till nästa sida där du vill göra samma kommentar och markerar ett område där. (Detta gäller endast de vanliga kommentarmarkeringsverktygen, inte textmarkeringsverktygen.)
1. Skriv din kommentar i rutan **Lägg till kommentar** till höger.
1. (Valfritt) Om du vill tagga en annan användare i kommentaren och lägga till dem i korrekturets arbetsflöde skriver du @ i kommentarsrutan, skriver användarens namn eller e-postadress och väljer användaren på menyn som visas. Mer information finns i [Tagga användare för att dela ett korrektur](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md).
1. (Valfritt) Gör något av följande om du vill bifoga en fil till en kommentar:

   * Klicka på ikonen för pappersklipp i det nedre högra hörnet av kommentaren och sök efter och markera sedan den fil som du vill överföra.
   * Dra en fil från en plats på datorn och släpp den i kommentarsområdet.

1. Klicka på **Publicera**.

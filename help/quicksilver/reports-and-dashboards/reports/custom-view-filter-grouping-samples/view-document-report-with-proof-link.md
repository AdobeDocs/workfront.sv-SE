---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: dokumentrapport med länk till ett korrektur'
description: 'Visa: dokumentrapport med länk till ett korrektur'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Visa: dokumentrapport med länk till ett korrektur

I den här dokumentvyn kan du infoga en länk till ett korrektur av den aktuella versionen av dokumentet.

![](assets/view-document-with-proof-link-350x92.png)

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa en dokumentrapport med en länk till ett korrektur

Så här använder du den här vyn:

1. Gå till en lista med dokument.
1. Från **Visa** nedrullningsbar meny, välja **Ny vy**.

1. Klicka **Lägg till kolumn**.
1. Klicka **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Ersätt&quot;Din domän&quot; med din faktiska Workfront-domän. Om företagets Workfront-URL är *Company.my.workfront.com*&#x200B;är din domän&quot;Company&quot;.

1. Klicka **Spara** sedan **Spara vy**.
1. Ange ett namn för vyn och klicka sedan på **Spara vy**.
1. (Valfritt) Om du bara vill visa dokument med korrektur lägger du till ett filter genom att göra följande:

   1. Klicka på **Filter** nedrullningsbar meny och klicka sedan på **Nytt filter**.
   1. Klicka **Lägg till en filterregel** och börja skriva in Korrekturägare och sedan välja **Korrekturägar-ID** när den visas i listan.
   1. Välj **Är inte tom** för filtermodifieraren.
   1. Klicka **Spara filter**, skriv namnet på filtret och klicka sedan på **Spara filter**.

1. Klicka på länken i kolumnen Korrekturlänk för att komma åt korrekturet för den senaste versionen av dokumentet.

---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa en bild i stället för en sträng i en kolumn'
description: Du kan ersätta namnet på ett objekt i en vy med en bild i textläge. Du kan också lägga till en länk till bilden som kan öppna det objekt den ersätter.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Visa: visa en bild i stället för en sträng i en kolumn

Du kan ersätta namnet på ett objekt i en vy med en bild i textläge. Du kan också lägga till en länk till bilden som kan öppna det objekt den ersätter.

>[!NOTE]
>
>Bilderna visas i sin faktiska upplösning, så försök använda små bilder.

![](assets/replace-project-name-with-image-and-link-350x125.png)

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
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Exempel: Ersätt namnet på ett projekt i en projektvy med en bild:

1. Överför en bild till en webbplats eller server utanför Adobe Workfront. Du måste kunna komma åt bilden via webbläsaren.

   >[!TIP]
   >
   >* Alla webbläsartyper är olika, men alla kan visa URL:er.
   >* Undvik att använda bilder som har överförts till Workfront. Eftersom bilder som lagras i Workfront inte är tillgängliga för allmänheten och har en åtkomstnyckel som går ut efter en viss tid, visas dessa bilder inte längre i vyn över tiden.
   >* En bild som sparats på datorn har ingen inbyggd URL. Hitta en webbplats som tillhandahåller bildvärdtjänster och som är värd för din bild där. Din organisation kanske redan har en sådan webbplats.


1. Gå till bilden som du sparade i webbläsaren.
1. Hämta bildens URL genom att göra följande:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Högerklicka och välj **Kopiera bildplats**, eller **Hämta länk**, beroende på webbläsaren. Nu har du URL-adressen för den specifika bilden och kan klistra in den från Urklipp.
   1. Se till att alla med den länken har behörighet att visa bilden genom att bara gå till länken och de behöver ingen inloggning för att komma åt den.

1. Gå till ett projekt och klicka på **Mer** meny ![](assets/more-icon-45x33.png) bredvid namnet på projektet och klicka sedan på **Redigera**.

1. I **URL** lägger du till länken till bilden.
1. Navigera till en projektvy i en lista eller rapport och anpassa vyn.
1. Klicka på kolumnrubriken för **Projektnamn** och sedan klicka **Växla till textläge**.

1. Lägg till följande kod i kolumnen till den befintliga koden:

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   Bilden du valde ersätter projektnamnet i projektvyn och bilden är en länk till projektet.

1. Klicka **Spara vy**.

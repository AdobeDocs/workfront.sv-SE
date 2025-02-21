---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Visa en bild i stället för en sträng i en kolumn'
description: Du kan ersätta namnet på ett objekt i en vy med en bild i textläge. Du kan också lägga till en länk till bilden som kan öppna det objekt den ersätter.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Visa: visa en bild i stället för en sträng i en kolumn

<!--Audited: 11/2024-->

Du kan ersätta namnet på ett objekt i en vy med en bild i textläge. Du kan också lägga till en länk till bilden som kan öppna det objekt den ersätter.

>[!NOTE]
>
>Bilderna visas i sin faktiska upplösning, så försök använda små bilder.

![Ersätt projektnamn med bild och länk](assets/replace-project-name-with-image-and-link-350x125.png)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
    <p>Nytt:</p>
   <ul><li><p>Medarbetare som ändrar ett filter </p></li>
   <li><p>Standard för att ändra en rapport</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Begäran om att ändra ett filter </p></li>
   <li><p>Planera att ändra en rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   1. Högerklicka och välj **Kopiera bildplats** eller **Hämta länk**, beroende på webbläsaren. Nu har du URL-adressen för den specifika bilden och kan klistra in den från Urklipp.
   1. Se till att alla med den länken har behörighet att visa bilden genom att bara gå till länken och de behöver ingen inloggning för att komma åt den.

1. Gå till ett projekt, klicka på **Mer**-menyn ![Mer-ikonen](assets/more-icon-45x33.png) bredvid namnet på projektet och klicka sedan på **Redigera**.

1. Lägg till länken till bilden i fältet **URL**.
1. Gå till en projektvy i en lista med projekt.
1. Klicka på listrutan **Visa** och sedan på **Ny vy**.
1. Klicka på kolumnrubriken för **Projektnamn** och klicka sedan på **Växla till textläge**.

1. Lägg till följande kod i kolumnen till den befintliga koden:

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. Klicka på **Klar** > **Spara vy**.
Bilden du valde ersätter projektnamnet i projektvyn och bilden är en länk till projektet.
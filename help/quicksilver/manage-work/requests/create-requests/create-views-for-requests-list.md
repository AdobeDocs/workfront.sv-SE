---
product-area: requests
navigation-topic: create-requests
title: Skapa och hantera vyer i området Förfrågningar
description: Om du använder den nya begärandefunktionen kan du skapa och spara vyer för området Förfrågningar.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 0%

---


# Skapa och hantera vyer i området Förfrågningar

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Om du använder den nya begärandeupplevelsen i Adobe Workfront kan du skapa och spara vyer för området Förfrågningar. De här vyerna innehåller filter och kolumnupplägg.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Den här funktionen är bara tillgänglig i den nya begärandeupplevelsen i området Begäranden.
>* Visningsinställningarna är också tillgängliga i widgeten Mina förfrågningar i Hem. Vyerna från området Begäranden är dock olika de som finns i widgeten Mina förfrågningar.
>* Listan över förfrågningar i området Begäranden använder den utökade listan i Workfront. Mer information finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla Workfront- eller Workflow-paket</p>

<p>Alla Worfront Planning-licenser, för att visa Workfront Planning-begäranden i begärandelistor</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  <p>Du måste vara Workfront-administratör för att kunna lägga till vyer i layoutmallar</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en vy för begäranden

Du kan skapa en vy under Förfrågningar i Workfront när du använder den nya upplevelsen av förfrågningar.

1. Så här öppnar du listan över förfrågningar:

   {{step1-to-requests}}

1. Kontrollera att inställningen **Använd ny upplevelse** är aktiverad.

1. I listan **Förfrågningar** klickar du på listrutan **Vyer** ![Vyer](assets/view-icon-requests.png) och sedan på **Ny vy**.

   ![Ny vy](assets/create-new-view.png)

1. Ange ett namn för den nya vyn och klicka på **Skapa**.
1. Fortsätt till [Redigera en vy i området Förfrågningar](#edit-a-view-in-the-requests-area).

## Redigera en vy för begäranden

Du kan redigera befintliga vyer, inklusive vyer som du just har skapat under Förfrågningar i Workfront.

Genom att redigera en vy i området Förfrågningar kan du ändra följande element i vyn:

* Namn
* Filter
* Kolumner

De ändringar du gör i en vy är synliga för alla som du delar vyn med.

1. Så här får du åtkomst till en lista med begäranden i listan över förfrågningar:

   {{step1-to-requests}}

1. Kontrollera att inställningen **Använd ny upplevelse** är aktiverad.
1. I listan **Förfrågningar** letar du reda på den vy du vill redigera i listrutan **Vyer** ![Vyer](assets/view-icon-requests.png).

1. Klicka på listrutan **Vyer** ![Vyer](assets/view-icon-requests.png) och klicka på menyn med tre punkter bredvid vyn, välj **Byt namn** och skriv in det nya namnet för vyn.
1. Tryck på Retur för att spara det nya namnet.
1. Klicka på listrutan **Vyer** ![Vyer](assets/view-icon-requests.png) och välj den vy som du vill redigera.
1. Om du vill lägga till ett fält som en kolumn klickar du på ikonen **Lägg till kolumn** ![Lägg till kolumn](assets/add-column.png) i listans övre högra hörn.

   **Kolumnhanteraren** öppnas.
1. Klicka på plusikonen bredvid fältet som du vill lägga till som en kolumn i vyn och klicka sedan på **Spara**.

   Fält som är kopplade till objekten i listan är tillgängliga att lägga till som kolumner. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Fält som du lägger till i kolumnerna måste finnas innan de är tillgängliga i **kolumnhanteraren**.

1. (Valfritt) Klicka på **Kolumner** för att öppna rutan **Fältsynlighet och fältordning**.
1. Aktivera inställningen för varje fält som du vill visa i listan, inaktivera den för att dölja den eller dra och släpp fälten i en annan ordning.

1. (Valfritt) Klicka på **Filter** och börja lägga till villkor för vilka begäranden du vill visa.

   Du kan filtrera efter följande begärandefält:

   * **Workspace**: Den arbetsyta som förfrågningsformuläret är associerat med.
   * **Objekttyp**: Posttypen som begärandeformuläret är associerat med.
   * **Anmälningsdatum**: Datumet då begäran skickades.
   * **Formulär för begäran**: Namnet på det begärandeformulär som användes för att skicka begäran.
   * **Status**: Status för begäran.
   * **Anges av**: Namnet på den användare som lade till begäran. Om begäran har lagts till av någon utanför Workfront visas **Angivet av**-fältet `N/A`.

   Du kan också filtrera efter fält som har lagts till i vyn efter objekt som visas i vyn.

   Du kan ha flera filter kopplade av antingen **And** eller **Or**.
Begärandelistan filtreras automatiskt när du lägger till filtervillkoren.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Ändringar av vyer sparas automatiskt.
> * Ändringar av vyer är synliga för alla som använder vyn.
> * Använd jokertecknet **Jag (inloggad användare)** i alla fält där användare har värdet.

## Lägg till vyn med förfrågningar i en layoutmall.

En Workfront-administratör kan lägga till den nya vyn i layoutmallar.

Instruktioner finns i [Anpassa filter, vyer och grupperingar med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Dela en vy

Du kan dela vyer som du skapar med andra användare, team eller grupper.

1. Så här får du åtkomst till en lista med begäranden i listan över förfrågningar:

   {{step1-to-requests}}

1. Kontrollera att inställningen **Använd ny upplevelse** är aktiverad.
1. Leta reda på den vy du vill dela i listan **Förfrågningar**.
1. Håll muspekaren över den vy du vill dela, klicka på menyn med tre punkter till höger om vynamnet och klicka sedan på **Dela**.
1. I rutan **Dela** anger du personer, team, roller, grupper eller företag som du vill dela vyn med och markerar dem sedan i listan när de visas.
1. Klicka på **Spara**.

   Vyn delas med de enheter som du anger. De kan visa de uppdaterade vyelementen som du har redigerat för vyn innan de delar den. <span class="preview">Om de uppdaterar vyn visas inte ändringarna för andra, såvida de inte kopierar samma vy och behåller ändringarna innan de delar kopian. Mer information finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

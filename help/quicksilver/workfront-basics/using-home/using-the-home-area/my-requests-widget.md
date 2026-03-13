---
product-area: projects
navigation-topic: use-the-home-area
title: Använda widgeten Mina förfrågningar
description: Du kan skicka förfrågningar i widgeten Mina förfrågningar. Du kan också anpassa widgeten med filter och kolumner.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 3893a57fb7ae31a1649b20beccc1f0b79f2421fb
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 0%

---

# Använda widgeten Mina förfrågningar

>[!IMPORTANT]
>
>I den här artikeln beskrivs den nya widgeten Mina förfrågningar. Du måste ha den nya upplevelsen som begär aktiverad för att kunna se den nya widgeten.
>Du kan aktivera den nya begärandeupplevelsen i området Förfrågningar.

Widgeten Mina förfrågningar visar förfrågningar som du har skickat. Du kan filtrera begäranden, söka efter specifika begäranden eller justera kolumnordning och synlighet. Du kan också skapa en ny förfrågan från widgeten Mina förfrågningar.

>[!NOTE]
>
>* När widgeten Mina förfrågningar läses in visas upp till 50 förfrågningar. Bläddra nedåt i listan om du vill visa fler förfrågningar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alla Workfront- eller Workflow-paket</p>
   <p>Alla Workfront Planning-paket som kan användas för att komma åt Workfront Planning-begäranden och skapade objekt</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa eller ge senare åtkomst till objekt som du har taggat i en konversation eller behöver lösa ett godkännande (Projekt, Åtgärder, Problem, Dokument)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View] behörigheter eller högre till projekt, uppgifter, problem, dokument där du är taggad i en konversation eller behöver lösa ett godkännande</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en förfrågan

Du kan skapa en begäran direkt från widgeten Mina förfrågningar.

Instruktioner finns i avsnittet [Skapa en begäran](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) i artikeln [Skapa arbetsobjekt och projekt från Hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Kopiera en begäran

Du kan kopiera en begäran i widgeten Mina förfrågningar, redigera den och skicka den som en ny begäran.

Instruktioner finns i [Kopiera och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Filterförfrågningar

Widgeten Mina förfrågningar har ett anpassningsbart filter som gör att du kan styra vilka förfrågningar som visas i widgeten. Du kan konfigurera det här filtret för olika fält och värden och kan stapla villkor med operatorerna AND och OR.

Så här konfigurerar du filtret i widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. Klicka på **Filter** i widgeten **Mina förfrågningar**.
1. Markera fältet som du vill filtrera efter. Tillgängliga alternativ är:

   * Workspace
   * Objekttyp
   * Anmälningsdatum
   * Formulär för förfrågningar
   * Status
   * Anges av
   * Anpassade fält från begäran eller från det skapade objektet

1. I nästa fält väljer du den operator som du vill använda för det här filtervillkoret. Vilka operatorer som är tillgängliga beror på vilket fält du har valt.
1. (Villkorligt) Om ett fält visas till höger om operatorn markerar du det värde som du vill filtrera efter.
1. (Valfritt) Om du vill lägga till ytterligare ett filtervillkor klickar du på **Lägg till villkor** och upprepar steg 4-6.
1. (Valfritt och villkorligt) Om du har flera villkor växlar du värdet And eller Or genom att klicka på **And** eller **Or** till vänster om villkoret.

Filtret sparas automatiskt.

>[!TIP]
>
>Om din organisation har köpt Workfront Planning förutom Adobe Workfront, kommer widgeten Mina förfrågningar att innehålla både Workfront- och Workfront Planning-förfrågningar.
> 
>* Om du bara vill filtrera efter Workfront-begäranden anger du filtret till **Objekttyp** > **Har något av** > **Problem**.
>* Om du bara vill filtrera efter Workfront Planning-begäranden anger du filtret till **Objekttyp** > **Har inga av** > **Problem**.

## Justera eller lägga till kolumner

Du kan välja vilken av de tillgängliga kolumnerna som ska visas i widgeten Mina förfrågningar och ange ordningen för dem.

Tillgängliga kolumner är:

* Ämne
* Skapat objekt
* Objekttyp
* Status
* Formulär för förfrågningar
* Anmälningsdatum
* Angivet av

Så här justerar du kolumnerna i widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på startskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. Klicka på **Kolumner** i widgeten **Mina förfrågningar**.
1. (Valfritt) Om du vill ändra ordning på kolumnerna klickar du på draghandtaget ![drar i handtaget](assets/drag-handle.png) för den kolumn du vill flytta och drar det till önskad plats. Kolumnen högst upp på listan visas i widgeten Mina förfrågningar som den första kolumnen.
1. (Valfritt) Använd reglaget för att dölja eller visa kolumnen i listan Förfrågningar.
1. Om du vill lägga till ett anpassat fält som en kolumn klickar du på ikonen **Lägg till kolumn** ![Lägg till kolumn](assets/add-column.png) i det övre högra hörnet av listan och klickar på plusikonen bredvid det anpassade fältet som du vill lägga till som en kolumn i widgeten.

   Anpassade fält i formulär som är kopplade till objektet i listan är tillgängliga för tillägg som kolumner.

Kolumninställningarna sparas automatiskt.

## Skapa en vy

Du kan skapa vyer i widgeten Mina förfrågningar om du vill ändra hur informationen visas i listan med förfrågningar.

Tänk på följande när du arbetar med vyer i widgeten Mina förfrågningar:

* En vy i widgeten Mina förfrågningar innehåller de kolumner och filter som har tillämpats på vyn.
* Du kan skapa vyer och dela dem med andra. De filter och kolumner som du väljer för vyn innan du delar den inkluderas i de vyer som du delar.
* Följande är en systemvy som du inte kan redigera, dela eller ta bort:

   * Standardvy för enhetliga Widget-begäranden
* Att skapa och redigera en vy i widgeten Mina förfrågningar liknar förbättrade listor. Mer information finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Sökbegäranden

Så här söker du efter specifika förfrågningar i widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. I sökfältet uppe till höger i widgeten Mina förfrågningar anger du den term som du vill söka efter.

   Förfrågningar som innehåller termen markeras med orange.

1. (Valfritt) Om du vill gå till de markerade förfrågningarna klickar du på upp- eller nedpilarna i sökfältet.

## Gå till ett objekt som skapats av en begäran

Du kan söka efter objekt som har skapats av en begäran i widgeten Mina förfrågningar.

>[!NOTE]
>
>Länkar till skapade objekt är bara tillgängliga i den nya begärandefunktionen för planeringsbegäranden, där själva begäran skapade ett objekt. Om en Workfront-begäran konverteras till ett projekt eller annat objekt är ingen länk till det konverterade objektet tillgänglig i listan över förfrågningar i den nya begärandeupplevelsen.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. Leta reda på den begäran som skapade objektet.
1. Klicka på objektnamnet i kolumnen **Skapat objekt** för den begäran.

   Objektets sida öppnas.


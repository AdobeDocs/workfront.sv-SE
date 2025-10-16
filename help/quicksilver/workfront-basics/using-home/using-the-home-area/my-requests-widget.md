---
product-area: projects
navigation-topic: use-the-home-area
title: Använda widgeten Mina förfrågningar
description: Du kan skicka begäranden i widgeten Mina förfrågningar. Du kan också anpassa widgeten med filter och kolumner.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# Använda widgeten Mina förfrågningar


>[!IMPORTANT]
>
>Den här artikeln beskriver den nya widgeten Mina förfrågningar. Du måste ha den nya upplevelsen som begär aktiverad för att kunna se den nya widgeten.
>&#x200B;>Du kan aktivera den nya begärandeupplevelsen i området Förfrågningar.

Widgeten Mina förfrågningar visar förfrågningar som har skickats till din organisation. Du kan filtrera förfrågningar, söka efter specifika förfrågningar eller justera kolumnordningen och synligheten. Du kan också skapa en ny begäran från widgeten Mina förfrågningar.

>[!NOTE]
>
>* När widgeten Mina förfrågningar läses in visas upp till 50 förfrågningar. Om du vill visa fler begäranden rullar du nedåt i listan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
    <tr> 
   <td role="rowheader"><strong>Ytterligare produkter</strong></td> 
   <td> Du måste ha Adobe Workfront Planning för att kunna visa planeringsförfrågningar eller begära formulär</td> 
  </tr> 
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa åtkomst eller högre till objekt som du har taggat i en konversation eller behöver lösa ett godkännande (Projekt, Åtgärder, Problem, Dokument)</p> </td> 
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

Instruktioner finns i [Skapa en begäran](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) i artikeln Skapa arbetsobjekt och projekt från Hem-området.

## Filterförfrågningar

Widgeten Mina förfrågningar har ett anpassningsbart filter som gör att du kan styra vilka förfrågningar som visas i widgeten. Du kan konfigurera det här filtret för olika fält och värden, och du kan stapla villkor med AND och OR.

Så här konfigurerar du filtret i widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**.
1. Klicka på **Filter** i widgeten Mina förfrågningar.
1. I fältet längst till vänster väljer du vad du vill filtrera efter. Tillgängliga alternativ är:

   * Workspace
   * Objekttyp
   * Anmälningsdatum
   * Formulär för förfrågningar
   * Status
   * Anges av

1. I nästa fält väljer du den operator som du vill använda för det här filtervillkoret. Vilka operatorer som är tillgängliga beror på det valda fältet.
1. (Villkorligt) Om ett fält visas till höger om operatorn väljer du det värde som du vill filtrera efter.
1. (Valfritt) Om du vill lägga till ytterligare ett filtervillkor klickar du på **Lägg till villkor** och upprepar steg 4-6.
1. (Valfritt och villkorligt) Om du har flera villkor växlar du värdet And eller Or genom att klicka på **And** eller **Or** till vänster om villkoret.

Filtret sparas automatiskt.

>[!TIP]
>
>Om din organisation har köpt Workfront Planning kommer widgeten Mina förfrågningar att innehålla förfrågningar från både Workfront och Workfront Planning.
> 
>* Om du bara vill filtrera efter Workfront-begäranden anger du filtret till **Objekttyp** > **Har något av** > **Problem**.
>* Om du bara vill filtrera efter Workfront Planning-begäranden anger du filtret till **Objekttyp** > **Har inga av** > **Problem**.

## Justera kolumner

Du kan välja vilken av de tillgängliga kolumnerna som ska visas i widgeten Mina förfrågningar och ange ordningen för dem.

Tillgängliga kolumner är:

* Ämne
* Skapat objekt
* Objekttyp
* Status
* Formulär för förfrågningar
* Anmälningsdatum
* Anges av

Så här justerar du kolumnerna på widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**.
1. Klicka på **Kolumner** i widgeten Mina förfrågningar.
1. (Valfritt) Om du vill ändra ordning på kolumnerna klickar du på draghandtaget ![drar &#x200B;](assets/drag-handle.png) i den kolumn som du vill flytta och drar den till önskad plats. Kolumnen högst upp i listan visas i widgeten Mina förfrågningar som kolumnen längst till vänster.
1. (Valfritt) Använd växlingsknappen för att kontrollera om en kolumn visas i widgeten Mina förfrågningar.

Kolumninställningarna sparas automatiskt.

## Sökbegäranden

Så här söker du efter specifika förfrågningar i widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**.
1. I sökfältet uppe till höger i widgeten Mina förfrågningar anger du den term som du vill söka efter.

   Förfrågningar som innehåller termen markeras med orange.

1. (Valfritt) Om du vill gå till de markerade förfrågningarna klickar du på upp- eller nedpilarna i sökfältet.

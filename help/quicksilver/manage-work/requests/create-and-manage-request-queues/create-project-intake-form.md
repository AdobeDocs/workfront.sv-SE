---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Skapa Project Input Forms
description: Du kan använda formulär för projektinmatning för att förenkla processen att skapa projekt i Workfront
author: Becky
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: 5ff71313c550d949079e7426b657a0a4e19a656c
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 0%

---

# Skapa formulär för projektinmatning

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Formulär för projektinmatning är en typ av begärandeformulär som gör att användare kan begära projekt. Projekten skapas från formuläret, utan att du behöver skapa ett projekt från ett skickat ärende.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Ny licens: Standard </p>
   eller
   <p>Aktuell licens: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör för att kunna skapa formulär för projektinmatning. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andra produkter</td> 
   <td> <p>Din organisation måste ha köpt Workfront Planning för att kunna använda planeringsfunktioner som automatisering.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Funktioner och begränsningar för Project Intake Forms

### Funktioner

Blanketter för projektinmatning har följande funktioner:

#### Workfront Planning Automations

Workfront blanketter för projektinmatning stöder Workfront Planning Automations, som konfigurerar de projektspecifika egenskaperna.

Mer information om automatiserad planering finns i [Konfigurera Adobe Workfront Planning Automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Godkännandekonfiguration

Man kan också konfigurera godkännare för inskickade begäranden.

### Begränsningar

#### Fälttyper som stöds

Project Input Forms kan innehålla fält från alla anpassade formulär med Project-objekttypen.

Följande fälttyper stöds för närvarande inte i Project Intake Forms:

* Avsnitt
* Formel
* Samlad
* Enkelradssammanslagning
* Planeringsanslutning
* Inbyggda fältreferenser som refereras till inbyggda Project-fält som är skrivskyddade (till exempel `workRequiredExpression`)

#### Begär upplevelse

Formulär för projektinmatning kan endast användas med den nya upplevelsen för att begära.

Mer information om den nya upplevelsen för begärande finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Delning

Projektinmatningsformulär har inte stöd för offentlig delning. Delningsalternativen är:

* **Alla**: Alla i systemet kan använda formuläret för att skicka en projektförfrågan.
* **Angivna användare**: Du kan välja vilka specifika användare som har åtkomst till formuläret för projektförfrågan.

## Skapa ett projektintäktsformulär

{{step1-to-requests}}

1. Aktivera inställningen **Växla till en ny upplevelse** i skärmens övre högra hörn.
1. Klicka på **Begär formulär** i skärmens övre högra hörn.

   >[!NOTE]
   >
   >Eftersom bara Workfront-administratörer kan skapa indragsformulär är knappen Begär formulär bara synlig för administratörer.

   En lista över tillgängliga förfrågningsformulär visas. Detta inkluderar förfrågningsformulär från Workfront Planning.

1. Klicka på **Nytt begärandeformulär** i skärmens övre högra hörn.
1. Ange ett namn för begärandeformuläret. Som standard är formulärets namn **Namnlöst formulär**.
1. Välj objekttypen **Projekt** i den övre delen av listrutan. För närvarande är detta den enda tillgängliga projekttypen för Workfront. Andra objekt i listan tillhör Workfront Planning.
1. (Valfritt) Lägg till en **beskrivning** för begärandeformuläret.
1. Klicka på **Skapa**. Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.

   Byggaren av projektintaget öppnas på fliken Formulär.

   Intag-formuläret innehåller som standard följande information:

   * **Standardavsnitt**: Det här är standardavsnittsbrytningen som Workfront tillämpar på begärandeformuläret. Alla postfält visas i området **Standardavsnitt**.
   * Fältet **Ämne**: Fältet som identifierar begäran i Workfront. Det går inte att redigera konfigurationen och värdet för ämnesfältet.
   * Alla fält som är associerade med projekt.

     Fälten i begärandeformuläret är synliga för alla som skickar en projektförfrågan.

1. Om du vill lägga till fält i formuläret klickar du på fälttypen i den vänstra navigeringen och väljer sedan fältet.
1. (Valfritt) Om du vill ta bort ett fält håller du pekaren över fältet i formuläret som du vill ta bort och klickar sedan på ikonen **x** för att ta bort det.
1. (Valfritt) Så här tar du bort **standardavsnittet** från formuläret:

   1. Ta bort alla fält från standardavsnittet.
   1. Klicka på fliken **Innehållselement** och lägg till ett nytt avsnitt och lägg sedan till ett namn för avsnittet.
   1. Lägg till fält i det nya avsnittet.
   1. Klicka på ikonen **x** för att ta bort **standardavsnittet**.
1. Klicka på ett fält och använd sedan kontrollerna på den högra panelen i formuläret för att definiera deras storlek eller någon av följande information:

   * **Etikett**: Det här är namnet på fältet som det kommer att visas i begärandeformuläret. Detta ändrar inte postfältets namn.
   * **Instruktioner**: Lägg till mer information om fältet.
   * **Gör ett obligatoriskt fält**: När du väljer det här alternativet måste fältet ha ett värde. Annars kan formuläret inte skickas.
   * **Lägg till logik**: Definiera vilka villkor som måste uppfyllas för att fältet ska kunna visas eller döljas.

   >[!TIP]
   >
   >   Fälttypen för varje fält visas längst upp på den högra panelen när du har valt fältet i formuläret.
   >     

1. (Valfritt) Klicka på fliken **Innehållselement** till vänster i formuläret och lägg till något av följande element:

   * **Beskrivande text**
   * **Avsnittsbrytning**

   Mer information om hur du skapar ett anpassat formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på fliken **Automatisering** till vänster i formuläret och gör sedan något av följande:

   * Välj en projektmall
   * Bifoga alla anpassade formulär
   * Ange en projektägare
   * Lägg till projektet i en portfölj eller ett program

   Alla markeringar du gör här kommer att användas för projekt som skapas från det här intagningsformuläret.

1. (Valfritt) Klicka på **Förhandsgranska** om du vill visa hur formuläret kommer att visas för andra användare när de kommer att använda det för att skicka en ny post.

1. (Valfritt) Klicka på fliken **Konfiguration** och lägg sedan till minst en användare eller grupp&lt; i fältet **Godkännare** för att godkänna nya begäranden för det här intagningsformuläret.

   * När du associerar ett intag med godkännare måste alla nya begäranden först godkännas av alla godkännare innan det genererar ett projekt.
   * Du kan lägga till en eller flera godkännare i ett formulär för inmatning.
   * Om minst en godkännare avvisar begäran, avvisas begäran och projektet skapas inte.
   * Alla godkännare måste fatta ett beslut innan ett projekt godkänns eller avvisas.
   * Om ett team utses till godkännare krävs endast ett beslut från teamet.

     Mer information om hur du lägger till godkännanden i begärandeformulär finns i [Lägga till godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Valfritt) Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om formulärets namn i rubriken och klicka sedan på **Redigera** för att uppdatera formulärets namn.

1. Klicka på **Publicera** för att publicera formuläret och få en unik länk för det.

   Följande saker händer:

   * Knappen **Publicera** har tagits bort.
   * Knappen **Avpublicera** läggs till i formuläret. Om du klickar på den går det inte att komma åt formuläret.
   * En **Dela**-knapp läggs till i formuläret.
   * Formuläret blir tillgängligt under Begäranden på huvudmenyn i Workfront.

1. Klicka på **Dela** om du vill dela formuläret med andra.
1. Klicka på vänsterpilen till vänster om formulärets namn i rubriken för att stänga formuläret.

   Tabellvyn **Begär formulär** öppnas och formuläret läggs till i den.

1. (Valfritt) Hovra över namnet på ett begärandeformulär i tabellvyn, klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png) till höger om formulärnamnet och klicka på något av följande:

   * **Redigera formulär**: Klicka här om du vill redigera information i formuläret ytterligare.
   * **Avpublicera**: Klicka här för att avpublicera formuläret som tar bort det från området med förfrågningar i Workfront.
   * **Dela**: Klicka här för att ändra vem som har åtkomst till formuläret.
   * **Kopiera länk**: Klicka här om du snabbt vill kopiera länken för begärandeformuläret utan att öppna formuläret.
   * **Ta bort**: Klicka här för att ta bort formuläret. Alla förfrågningar och poster som lagts till med formuläret tas inte bort. Formuläret kan inte återskapas.

   >[!NOTE]
   >
   >Du kan identifiera formulär för projektinläsning i tabellvyn eftersom de visar&quot;Projekt&quot; i kolumnen Objekttyp.

1. Klicka på vänsterpilen till vänster om **Begär formulär** i sidhuvudet för att stänga tabellen med förfrågningsformulär.


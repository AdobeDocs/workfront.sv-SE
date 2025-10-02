---
title: Skapa Workfront-objekt från Workfront Planning när du kopplar dem till poster
description: Du kan skapa Workfront-objekttyper när du kopplar dem från andra poster i Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 5b9b1f397c76afa2e2ae550e0ce62a6038b8bd86
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Skapa Workfront-objekt från Workfront Planning när du kopplar dem till poster

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">Informationen som är markerad på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan skapa Adobe Workfront-objekt från Workfront Planning på följande sätt:

* Koppla Workfront-objekt från planeringsposter

  I den här artikeln beskrivs hur du skapar Workfront-objekt från Workfront Planning när du kopplar dem från Planning-poster.
* När du använder automatisering från en postsida.

  Mer information om hur du skapar Workfront-objekt med hjälp av automatisering finns i [Skapa objekt med hjälp av postautomatisering för Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

>[!IMPORTANT]
>
>Du kan skapa följande Workfront-objekt från Workfront Planning när du kopplar dem till Planning-poster:
>
>* Projekt
>* Portföljer
>* Program
>
>Du kan koppla följande Workfront-objekt till Planning-poster, men du kan inte skapa dem i anslutningsprocessen:
>
>* Grupper
>* Företag
>

Tänk på följande när du ansluter och skapar Workfront-objekt till Workfront Planning-poster:

* Du kan koppla samman Workfront projekt, portfolior, program, grupper och företag från ett anslutningsfält inom följande områden i Workfront Planning:

   * Registervyn för en posttyp
   * Sidan Detaljer eller förhandsvisningsrutan för en post
   * Fliken Anslutningar för en post

* Du kan skapa projekt från följande områden i Workfront Planning:

   * Registervyn för en posttyp
   * Området Detaljer för en post i anslutningsfältet
   * <span class="preview">Postsidan för den anslutna posten för en post, i området Information</span>

* Du kan skapa portföljer och program från följande områden i Workfront Planning:

   * Registervyn för en posttyp
   * Området Detaljer för en post i anslutningsfältet

Mer information om hur du ansluter Planning-poster med Workfront-objekt finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p> 
   <p>Redigera åtkomst med Skapa objekt i Workfront för de objekttyper som du vill skapa (projekt, portfolior, program). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter på arbetsytan och den posttyp där du vill lägga till poster. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar för att skapa Workfront-objekt när de ansluts till poster från Workfront Planning

Du måste ha följande innan du kan lägga till nya projekt eller portföljer genom att koppla dem från befintliga poster:

* Registrera typer som är kopplade till Workfront projekt, portfolior eller program. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Poster för de posttyper som är kopplade till Workfront-objekt. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Rätt åtkomst och behörigheter i Workfront Planning och Workfront, enligt beskrivningen i avsnittet [Åtkomstkrav](#access-requirements) i den här artikeln.

## Skapa projekt när du kopplar ihop dem med poster från Workfront Planning

Du kan skapa projekt när du kopplar dem till poster i Workfront Planning i följande områden i Workfront Planning:

* Registervyn för en posttyp eller området Detaljer för en post i anslutningsfältet
* <span class="preview">Postsidan för den anslutna posten, i området Detaljer för en post </span>

### Skapa projekt från området Detaljer för en post eller tabellvyn för en posttyp

Så här skapar du projekt när du kopplar dem från andra poster:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-projekt, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

1. (Villkor) Klicka på **Lägg till projekt**
eller
Börja skriva namnet på ett projekt och klicka sedan på **Lägg till projekt** om du inte hittar det. Knappen Lägg till följs av det projektnamn du skrev in.

   ![Lägg till projekt när du ansluter det från ett anslutningsfält](assets/add-project-when-connecting-it-from-connection-field.png)

   Rutan **Skapa projekt** öppnas.

1. (Valfritt) Uppdatera **projektnamnet**. Som standard får projektet ett namn efter det du lade till som sökobjekt när du kopplar det från posten.
1. (Valfritt) Välj en **projektmall**. Om du inte väljer någon mall skapas ett tomt projekt utan några uppgifter.
1. Klicka på **Skapa**.
1. (Villkorligt) Om du valde att skapa ett projekt från en mall följer du stegen i artikeln [Skapa ett projekt med en mall](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)-artikel för att lägga till projektet.

   Det nya projektet skapas och läggs till i det anslutna fältet för den valda posten.

1. (Valfritt) Klicka på namnet på det nya projektet i Workfront Planning för att öppna projektets sida i Workfront och göra ytterligare uppdateringar i projektet.

<div class="preview">

### Skapa projekt från sidan Anslutna poster i en post

1. Koppla objekttypen till en Workfront Planning-posttyp i tabellvyn.

   Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klicka på namnet på en post i valfri vy. Förhandsvisningsrutan Detaljer öppnas.

1. Lägg till sidan **Anslutna poster** för projekt.

   Mer information finns i avsnittet&quot;Lägg till en kopplad post till en post&quot; i artikeln [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

   Sidan Anslutna poster visas i tabellvyn. Kopplade projekt visas i tabellen.

   ![Projekttabellvy på sidan med anslutna poster](assets/projects-connected-records-page-table.png)

1. Klicka på **Ny rad** i projekttabellen om du vill lägga till ett projekt.

   Du kan bara lägga till ett tomt projekt i det här området. Du kan inte lägga till ett projekt med en mall.
1. (Valfritt) Klicka på projektnamnet i tabellvyn för att öppna projektet i Workfront och lägga till mer information.

</div>

## Skapa portfolior när du kopplar ihop dem med dokument från Workfront Planning

Du kan skapa portföljer från tabellvyn för en posttyp eller detaljsidan för en post.

Så här skapar du portföljer när du kopplar dem från Planning records:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-portföljer, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

1. (Villkorligt) Klicka på **Lägg till portfölj**

   eller

   Börja skriva namnet på en portfölj och klicka sedan på **Lägg till portfölj** om du inte hittar den. Knappen Lägg till följs av det portföljnamn som du angav.

   ![Lägg till portfölj när du ansluter den från ett anslutningsfält](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Portföljen skapas och läggs till i anslutningsfältet för den post du valde.

1. (Valfritt) Klicka på namnet på den nya portföljen från Workfront Planning för att öppna portföljens sida i Workfront och göra ytterligare uppdateringar av portföljen.

## Skapa program när du kopplar ihop dem med poster från Workfront Planning

Du kan skapa program från tabellvyn för en posttyp eller detaljsidan för en post.

Så här skapar du program när du kopplar dem från planeringsposter:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-portföljer, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

1. Klicka på **Lägg till program**

   eller

   Börja skriva namnet på ett program och klicka sedan på **Lägg till program** om du inte hittar det. Knappen Lägg till följs av det programnamn som du skrev in.

   ![Lägg till Workfront-program när du ansluter det från anslutningsfältet](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   Rutan **Skapa program** öppnas.

1. Uppdatera **programnamnet**. Detta är ett obligatoriskt fält.
1. Välj en **Portfolio** i listrutan eller börja skriva namnet på en portfölj och markera den när den visas i listan. Detta är ett obligatoriskt fält.
1. Klicka på **Skapa**.

   Programmet skapas och läggs till i anslutningsfältet för den post du har valt.

1. (Valfritt) Klicka på namnet på det nya programmet från Workfront Planning för att öppna programmets sida i Workfront och göra ytterligare uppdateringar.


---
title: Skapa Workfront-objekt från Workfront Planning
description: Du kan skapa Workfront-objekttyper när du kopplar dem från andra poster i Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 92344bc1b2dfc10e6b5ce80cb041c383f36be351
workflow-type: tm+mt
source-wordcount: '1140'
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
* <span class="preview">När du använder automatisering från en postsida.</span>

  <span class="preview">Mer information om hur du skapar Workfront-objekt med automatisering finns i [Skapa objekt med hjälp av postautomatisering för Adobe Workfront Planning ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). </span>

Du kan skapa följande typer av Workfront-objekt från Workfront Planning när du ansluter en Workfront Planning-post med följande Workfront-objekttyper:

* Projekt
* Portföljer
* <span class="preview">Program</span>

>[!IMPORTANT]
>
>* Du kan bara skapa projekt, portföljer och <span class="preview">program</span> i Workfront när du kopplar dem från en post.
>
>* Du kan inte skapa grupper eller företag när du kopplar dem från en post i Workfront Planning.
>

Du kan ansluta projekt, portföljer, <span class="preview"> och program </span> från ett anslutningsfält i följande områden i Workfront Planning:

* Registervyn för en posttyp
* Sidan Detaljer eller förhandsvisningsrutan för en post
* Fliken Anslutningar för en post

Mer information om hur du ansluter Planning-poster med Workfront-objekt finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
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
   <p>Redigera åtkomst i Workfront för de objekttyper som du vill skapa (projekt och portföljer) när du kopplar posterna till dem. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter för den arbetsyta som du vill lägga till poster i. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar för att skapa Workfront-objekt när de ansluts till poster från Workfront Planning

Du måste ha följande innan du kan lägga till nya projekt eller portföljer genom att koppla dem från befintliga poster:

* Posttyper som är kopplade till Workfront-projekt, portföljer eller <span class="preview">program</span>. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Poster. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Rätt åtkomst och behörigheter i Workfront Planning och Workfront, enligt beskrivningen i avsnittet [Åtkomstkrav](#access-requirements) i den här artikeln.

## Skapa projekt när du kopplar ihop dem med poster från Workfront Planning

Så här skapar du projekt när du kopplar dem från andra poster:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-projekt, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

1. (Villkorligt) <span class="preview">Klicka på **Lägg till projekt**</span>
eller
Börja skriva namnet på ett projekt och klicka sedan på **Lägg till projekt** om du inte hittar det.

   Om du inte kan hitta ett projekt när du försöker lägga till det från det anslutna postfältet för en annan post lägger du till ett namn och klickar sedan på **Lägg till projekt**. Knappen Lägg till följs av det projektnamn du skrev in.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![Lägg till projekt när du ansluter det från ett anslutningsfält](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">Rutan **Skapa projekt** öppnas.</span>

1. <span class="preview">(Valfritt) Uppdatera **projektnamnet**. Som standard får projektet ett namn efter det du lade till som sökobjekt när du kopplar det från posten. </span>
1. <span class="preview">(Valfritt) Välj en **projektmall**. Om du inte väljer någon mall skapas ett tomt projekt utan några uppgifter. </span>
1. <span class="preview">Klicka på **Skapa**. </span>
1. <span class="preview">(Villkorligt) Om du valde att skapa ett projekt från en mall följer du stegen i artikeln [Skapa ett projekt med en mall](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) för att lägga till projektet.</span>

   Det nya projektet skapas och läggs till i det anslutna fältet för den valda posten.

1. (Valfritt) Klicka på namnet på det nya projektet i Workfront Planning för att öppna projektets sida i Workfront och göra ytterligare uppdateringar i projektet.

## Skapa portfolior när du kopplar ihop dem med dokument från Workfront Planning

Så här skapar du portföljer när du kopplar dem från Planning records:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-portföljer, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (Villkorligt) <span class="preview">Klicka på **Lägg till portfölj**</span>

   eller

   Börja skriva namnet på en portfölj och klicka sedan på **Lägg till portfölj** om du inte hittar den.—> Om du inte kan hitta en portfölj när du försöker lägga till den från det anslutna postfältet för en annan post lägger du till ett namn och klickar sedan på **Lägg till portfölj**. Knappen Lägg till följs också av det portföljnamn du skrev in.

   ![Lägg till portfölj när du ansluter den från ett anslutningsfält](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Portföljen skapas och läggs till i anslutningsfältet för den post du valde.

1. (Valfritt) Klicka på namnet på den nya portföljen från Workfront Planning för att öppna portföljens sida i Workfront och göra ytterligare uppdateringar av portföljen.

<div class="preview">

## Skapa program när du kopplar ihop dem med poster från Workfront Planning

Så här skapar du program när du kopplar dem från planeringsposter:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-portföljer, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."-->

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

</div>


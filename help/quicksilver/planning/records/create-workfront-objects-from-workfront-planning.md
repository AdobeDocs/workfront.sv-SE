---
title: Skapa Workfront-objekt från Workfront Planning
description: Du kan skapa Workfront-objekttyper när du kopplar dem från andra poster i Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 9db8ea3f26dd7e8b4c8aa52fb9902832db7a6a5c
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Skapa Workfront-objekt från Workfront Planning

<span class="preview">Informationen som är markerad på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan skapa följande typer av Workfront-objekt från Workfront Planning:

* Projekt
* Portfolio

Du kan skapa Workfront-projekt och portföljer från Workfront Planning när du kopplar en Workfront Planning-post till ett projekt eller en portfölj.

>[!IMPORTANT]
>
>* Du kan bara skapa projekt och portföljer i Workfront när du kopplar dem från en post.
>
>* Du kan inte skapa program, grupper eller företag när du kopplar dem från en post i Workfront Planning.
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

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

* Registrera typer som är kopplade till Workfront projekt eller portföljer. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Poster. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Rätt åtkomst och behörigheter i Workfront Planning och Workfront, enligt beskrivningen i avsnittet [Åtkomstkrav](#access-requirements) i den här artikeln.

## Skapa projekt när du kopplar ihop dem med poster från Workfront Planning

Så här skapar du projekt när du kopplar dem från andra poster:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-projekt, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

   Du kan ansluta projekt från ett anslutningsfält i följande områden i Workfront Planning:

   * Registervyn för en posttyp
   * Informationssidan eller förhandsvisningsrutan för en post

1. (Villkorligt) Om du inte kan hitta ett projekt när du försöker lägga till det från det anslutna postfältet för en annan post lägger du till ett namn och klickar sedan på **+ Lägg till**. Knappen **+ Lägg till** följs av namnet på den objekttyp som du ansluter till. Exempel:&quot;Lägg till projekt&quot; när du lägger till ett nytt projekt till en befintlig kampanj. Knappen Lägg till följs också av det projektnamn du skrev in.

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">Rutan **Skapa projekt** öppnas.</span>

1. <span class="preview">(Valfritt) Uppdatera **projektnamnet**. Som standard får projektet ett namn efter det du lade till som sökobjekt när du kopplar det från posten. </span>
1. <span class="preview">(Valfritt) Välj en **projektmall**. Om du inte väljer någon mall skapas ett tomt projekt utan några uppgifter. </span>
1. <span class="preview">Klicka på **Skapa**. </span>
1. <span class="preview">(Villkorligt) Om du valde att skapa ett projekt från en mall följer du stegen i artikeln [Skapa ett projekt med en mall](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) för att lägga till projektet.</span>

   Det nya projektet skapas och läggs till i det anslutna fältet för den valda posten.

1. (Valfritt) Klicka på namnet på det nya projektet i Workfront Planning för att öppna projektets sida i Workfront och göra ytterligare uppdateringar i projektet.

## Skapa portföljer när du kopplar ihop dem med poster från Workfront Planning

Så här skapar du portföljer när du kopplar dem från andra poster:

1. Gå till informationssidan för en post eller till posttypens tabell och börja ansluta Workfront Planning-poster med Workfront-portföljer, enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

   Du kan koppla portföljer från ett anslutningsfält i följande områden i Workfront Planning:

   * Registervyn för en posttyp
   * Informationssidan eller förhandsvisningsrutan för en post

1. (Villkorligt) Om du inte kan hitta en portfölj när du försöker lägga till den från det anslutna postfältet för en annan post lägger du till ett namn och klickar sedan på **+ Lägg till**. Knappen **+ Lägg till** följs av namnet på den objekttyp som du ansluter till. Exempel:&quot;Lägg till portfölj&quot; när du lägger till en ny portfölj till en befintlig kampanj. Knappen Lägg till följs också av det portföljnamn du skrev in.

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Portföljen skapas och läggs till i anslutningsfältet för den post du valde.

1. (Valfritt) Klicka på namnet på den nya portföljen från Workfront Planning för att öppna portföljens sida i Workfront och göra ytterligare uppdateringar av portföljen.

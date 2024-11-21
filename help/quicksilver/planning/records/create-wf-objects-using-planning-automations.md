---
title: Skapa Workfront-objekt med hjälp av Adobe Workfront Planning Record Automations
description: Du kan konfigurera automatisering i Workfront Planning som, när den aktiveras, skapar objekt i Workfront.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 03eedb00ab45b95e87670872cf015c0f6840658e
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Skapa objekt med automatisering av Adobe Workfront Planning Record

<!--add screen shots when UI is finalized-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

Du kan konfigurera automatisering i Adobe Workfront Planning som, när den aktiveras, skapar objekt i Workfront eller Workfront Planning.

Du kan konfigurera och aktivera automatiseringen på postens sida. Objektet som skapas kopplas till Planning-posten och placeras i det fält som du anger i automatiseringen.

Du kan till exempel skapa en automatisering som tar en Workfront Planning-kampanj och skapar ett projekt i Workfront för att spåra kampanjens utveckling. Projektet skulle kopplas till Workfront Planning Campaign.

Mer information om anslutna poster finns i [Översikt över anslutna poster](/help/quicksilver/planning/records/connected-records-overview.md).

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
   <p>Redigera åtkomst i Workfront för de objekttyper som du vill skapa (projekt, portföljer, program). </p>  
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


## Att tänka på när du skapar objekt och poster med hjälp av en automatisering

* Det nya objektet eller postnamnet är samma som det postnamn som du skapade det från.
* Om den post som du använder automatiseringen för redan har objekt av samma typ kopplade i det fält som du väljer att lägga till nya objekt, läggs de nya objekten till i anslutningsfältet och befintliga objekt förblir också kopplade.


## Konfigurera automatisering i Workfront Planning

Du måste konfigurera en automatisering i Workfront Planning innan du kan använda den för att skapa objekt.

{{step1-to-planning}}

1. Klicka på ett posttypskort och klicka sedan på namnet på en post.

   Posttypssidan öppnas.
1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Hantera automatisering**.

   En lista över tillgängliga automatiseringar öppnas.

1. Klicka på **Ny automatisering** i skärmens övre högra hörn.
1. Uppdatera följande fält:

   * **Knapptext**: Ange den text som du vill ska visas på automatiseringsknappen. Användare klickar på den här knappen när de använder automatiseringen för att skapa ett Workfront-objekt.
   * **Knappikon**: Välj en ikon för knappen. En ikon är markerad som standard.
   * **Objekttyp**: Markera det objekt som du vill att automatiseringen ska skapa. Detta är ett obligatoriskt fält.

     Du kan skapa följande objekt från Workfront Planning-poster:

      * Projekt
      * Portfolio
      * Program
      * Grupp
      * Post
1. (Villkorligt) Beroende på vilken typ av objekt du vill skapa uppdaterar du följande fält:

   * **Projekt**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet som det nya projektet ska visas i. Detta är ett obligatoriskt fält
      * **Mall som projektet ska skapas från**: Välj en projektmall som Workfront ska använda för att skapa projektet.
   * **Portfolio**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet där den nya portföljen visas. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till den nya portföljen**: Välj ett anpassat formulär att koppla till den nya portföljen. Du måste skapa ett anpassat portföljformulär innan du kan markera det.
   * **Program**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet som det nya programmet visas i. Detta är ett obligatoriskt fält.
      * **Programportfölj**: Välj en portfölj där det nya programmet ska läggas till. Detta är ett obligatoriskt fält.
      * 
         * **Anpassat formulär att koppla till det nya programmet**: Välj ett anpassat formulär att koppla till det nya programmet. Du måste skapa ett anpassat programformulär innan du kan markera det.
   * **Grupp**:
      * **Anslutet fält där objektet skapas**: Det här är det anslutna fältet där den nya gruppen visas. Detta är ett obligatoriskt fält.
      * **Anpassat formulär att koppla till den nya gruppen**: Välj ett anpassat formulär att koppla till det nya programmet. Du måste skapa ett anpassat programformulär innan du kan markera det.
   * **Post**:
      * **Ansluten posttyp**: Välj den posttyp som du vill skapa.
      * **Anslutet fält där posten skapas**: Det här är det anslutna fältet där den nya posten visas. Detta är ett obligatoriskt fält.
      * **Mappningsfält**: Välj fält från den posttyp som automatiseringen skapas för för att mappa dem till fälten för den anslutna posttypen.
      * **Till anslutet postfält**: Välj fält från den anslutna posten som motsvarar fälten från den posttyp som du skapar automatiseringen för.
1. (Valfritt och villkorligt) Om du inte har något anslutningsfält för en Workfront-objekttyp klickar du på ikonen **Skapa ett anslutningsfält** ![](assets/create-a-connection-field-icon.png) för att lägga till ett fält.
1. (Valfritt och villkorligt) Om du har valt att lägga till en post klickar du på **Lägg till** i området **Mappa anslutna fält** för att lägga till och mappa ytterligare fält.
1. Klicka på **Skapa**

Automatiseringen visas i listan över automatiseringar och finns tillgänglig för arkivering.

## Skapa ett objekt med en Workfront Planning Automation

1. Öppna den posttypssida som innehåller de poster du vill använda för att skapa Workfront-objekt i Workfront Planning.
1. Öppna tabellvyn.
1. Markera en eller flera poster.

   Ett blått fält visas längst ned i tabellen med ytterligare knappar, inklusive automatiseringsknappar.
1. Klicka på knappen för automatisering i skärmens nedre högra hörn.

   ![Automatiseringsknappen](assets/automation-custom-button.png)

   Det nya objektet visas i det anslutna fältet som du angav i inställningarna för knappen för automatisering.

   >[!NOTE]
   >
   >Vi rekommenderar att du kontrollerar att objektet har skapats och anslutits som förväntat.

1. (Valfritt) Klicka på det nya objektet i det anslutna fältet. Objektsidan öppnas och du kan göra ytterligare ändringar i det nya objektet.

<!--you might need to add something about notifications and emails?!-->

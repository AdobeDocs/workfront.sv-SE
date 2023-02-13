---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: ta bort länken till ett objekt i en kolumn'
description: Vissa objekt som du visar i en vy länkar till objektets detaljsida som standard. Kolumnen som visar namnet på ett projekt är till exempel en länk till projektet. kolumnen som visar namnet på en användare är en länk till användarens profilsida.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Visa: ta bort länken till ett objekt i en kolumn

Vissa objekt som du visar i en vy länkar till objektets detaljsida som standard. Kolumnen som visar namnet på ett projekt är till exempel en länk till projektet. kolumnen som visar namnet på en användare är en länk till användarens profilsida.

Du kan ta bort den här länken i textläge i kolumner som visas i alla vyer.

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

## Exempel: Ta bort länken till en uppgift från kolumnen Uppgiftsnamn i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy** för att skapa en ny vy.

   eller

   Klicka på **Ikonen Redigera** ![](assets/edit-icon.png)

   Om du vill redigera en befintlig vy markerar du vyn.

1. Klicka **Lägg till kolumn** om du vill lägga till en ny kolumn.

   eller

   Klicka på en befintlig kolumn med en länk till ett objekt.

1. Klicka **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   <pre>displayName=Aktivitetsnamn<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueFormat=Sammansatt</pre>

   >[!TIP]
   >
   >Du kan använda liknande kod för andra objekt genom att justera följande:
   >
   >   
   >   
   >   * Ersätt **värdefält** kodrad med **värdeuttryck** och behålla samma namn inom klammerparenteser efter likhetstecknet.
   >   
   >   
   >
   >   
   >   
   >   * Ta bort alla rader som börjar med >

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. Klicka **Spara** sedan **Spara vy**.

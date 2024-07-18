---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: ta bort länk till ett objekt i en kolumn'
description: Vissa objekt som du visar i en vy länkar till objektets detaljsida som standard. Kolumnen som visar namnet på ett projekt är till exempel en länk till projektet. Kolumnen som visar namnet på en användare är en länk till användarens profilsida.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Visa: ta bort länk till ett objekt i en kolumn

Vissa objekt som du visar i en vy länkar till objektets detaljsida som standard. Kolumnen som visar namnet på ett projekt är till exempel en länk till projektet. Kolumnen som visar namnet på en användare är en länk till användarens profilsida.

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Exempel: Ta bort länken till en aktivitet från kolumnen Uppgiftsnamn i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa** för att skapa en ny vy.

   eller

   Klicka på ikonen **Redigera** ![](assets/edit-icon.png)

   Om du vill redigera en befintlig vy markerar du vyn.

1. Klicka på **Lägg till kolumn** för att lägga till en ny kolumn.

   eller

   Klicka på en befintlig kolumn med en länk till ett objekt.

1. Klicka på **Växla till textläge**.
1. Hovra över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:
   <pre>displayname=Aktivitetsnamn<br>länkat namn=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueExpression={name}</strong><br>valueFormat=Compound</pre>

   >[!TIP]
   >
   >Du kan använda liknande kod för andra objekt genom att justera följande:
   >
   >* Ersätt kodens **värdefält**-rad med **värdeuttryck** och behåll samma namn inom klammerparenteser efter likhetstecknet.
   >* Ta bort alla rader som börjar med `link.` från den ursprungliga texten i kolumnen. Ta till exempel bort alla följande rader:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Klicka på **Spara** och sedan på **Spara vy**.

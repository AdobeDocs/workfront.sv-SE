---
product-area: projects
navigation-topic: manage-projects
title: Översikt över dokumenthantering för projekt och relaterade objekt
description: Beroende på om din Workfront-administratör väljer att använda standardinställningen för lagring kan du lagra dokument antingen på Workfront-lagring eller på Adobe Enterprise-lagring. I den här artikeln beskrivs hur du kan hantera dokument för projekt, portföljer, program, mallar, uppgifter och utgåvor.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 5c4ffeabf710374b14a2335b47342be4c393a7c8
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Översikt över dokumenthantering för projekt och relaterade objekt

Din Adobe Workfront-administratör kan ange standardinställningen för din organisations lagringsinställning för att ange var dokument ska lagras i Workfront.

Workfront-administratören kan välja något av följande alternativ:

* Workfront
* Adobe Enterprise Storage

Med den här inställningen kan du automatiskt lagra dokument som är kopplade till Workfront-objekt på en av de tillgängliga lagringsplatserna.

>[!IMPORTANT]
>
>Alla kunder har inte tillgång till både Workfront och Adobe lagringsutrymme. Vissa kunder har bara tillgång till Workfront som andra bara har tillgång till Adobe Enterprise-lagring som standard. Ingen konfiguration behövs för kunder som inte har tillgång till Workfront-lagring.

Workfront-administratören kan göra något av följande:

* Välj ett av de två lagringsalternativen som standard för din organisation
* Välj vilket lagringsutrymme du vill använda när du skapar något av följande objekt:

   * Projekt
   * Portföljer
   * Mallar

Mer information om hur du anger lagringsinställningar för Workfront finns i [Aktivera Adobe Enterprise-lagring för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

I den här artikeln beskrivs hur du kan hantera dokument för projekt, portföljer, program, uppgifter, utgåvor, mallar och malluppgifter.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Översikt över dokumentlagring

Kunderna kan ha tillgång till någon av följande dokumentlagringsfunktioner:

* Endast Workfront-lagring. Området Lagringsinställningar i Systeminställningar finns inte.
* Endast Adobe Enterprise-lagring. Området Lagringsinställningar i Systeminställningar finns inte.
* Både Workfront-lagring och Adobe Enterprise-lagring. Workfront-administratören kan välja mellan följande:

   * Väljer en standardlagringsmiljö för hur dokument hanteras i framtiden.
   * Låter användarna välja vilket lagringsutrymme de väljer när de skapar följande objekt:

      * Projekt
      * Portföljer
      * Mallar

  >[!NOTE]
  >
  >* Aktiviteter och problem ärver typen av lagring från projektet.
  >* Malluppgifter ärver lagringstypen från mallen
  >* Program ärver typen av lagring från portföljen.


Dokument som lagras på objekt i Workfront hanteras på ett annat sätt än de som lagras i Adobe Enterprise.

Mer information finns i [Adobe Enterprise-lagringsöversikt](/help/quicksilver/review-and-approve-work/esm-overview.md).

Följande avsnitt visar hur dokumentlagring fungerar för Workfront-objekt när både Workfront och Adobe Enterprise-lagringsalternativ finns på plats.

### Dokumenthantering för projekt

Tänk på följande när du arbetar med projekt:

* När du skapar ett Adobe Enterprise-storage-projekt skapar Workfront en mapp i dokumentavsnittet i projektet där dokument sparas. Mappnamnet är samma namn som projektet. Du kan inte ta bort eller ändra namn på mappen manuellt. Mappens namn ändras om du ändrar namnet på projektet så att det matchar projektets nya namn.
* När du skapar eller flyttar ett Adobe-enterprise-lagringsprojekt till en befintlig Workfront-lagringsportfölj eller ett program konverteras portföljen eller programmet automatiskt till ett Adobe Enterprise-storage-objekt.
* Du kan inte skapa ett Workfront-lagringsprojekt för en företagslagringsportfölj eller ett Adobe-program.

### Dokumenthantering för portföljer

Tänk på följande när du arbetar med portföljer:

* När du skapar en Adobe Enterprise-storage-portfölj skapar Workfront en mapp i avsnittet Dokument i portföljen där dokument sparas. Mappnamnet är samma namn som portföljen. Du kan inte ta bort eller ändra namn på mappen manuellt. Mappens namn ändras om du ändrar namnet på portföljen så att det matchar portföljens nya namn.
* När du skapar eller flyttar ett Adobe-enterprise-lagringsprojekt till en äldre Workfront-lagringsportfölj konverteras portföljen automatiskt till ett Adobe Enterprise-storage-objekt.
* Om den konverterade portföljen tidigare hade dokument bifogade, fortsätter de att lagras i Workfront. Nya dokument lagras också i Workfront.
* Om den konverterade portföljen inte hade några dokument bifogade i Workfront-lagringen lagras nya dokument i Adobe Enterprise-lagring.

### Dokumenthantering för program

Tänk på följande när du arbetar med program:

* När du skapar ett Adobe Enterprise-storage-program skapar Workfront en mapp i dokumentavsnittet i programmet där dokument sparas. Mappnamnet är samma namn som programmet. Du kan inte ta bort eller ändra namn på mappen manuellt. Mappens namn ändras om du ändrar namnet på programmet så att det matchar programmets nya namn.
* När du skapar eller flyttar ett Adobe-enterprise-lagringsprojekt till en äldre Workfront-lagringsportfölj konverteras portföljen automatiskt till ett Adobe Enterprise-storage-objekt.
* Om det konverterade programmet tidigare hade dokument bifogade, kommer de att fortsätta att lagras i Workfront. Nya dokument lagras också i Workfront.
* Om det konverterade programmet inte hade några dokument bifogade i Workfront-lagringen, lagras nya dokument i Adobe Enterprise-lagring.

### Dokumenthantering för uppgifter

Tänk på följande när du arbetar med uppgifter:

* Aktiviteter ärver lagringstypen från projekt.
* När du överför ett dokument till en uppgift i ett Adobe-lagringsprojekt skapas automatiskt en mapp i dokumentavsnittet av uppgiften. Mappnamnet är samma som uppgiften.
* Du kan byta namn på och ta bort dokumentmappen från Adobe Enterprise-storage-aktiviteten, som även tar bort dokumenten i mappen. När du har lagt till nya dokument i uppgiften återskapas mappen automatiskt. Borttagna dokument placeras inte tillbaka i mappen.
* För Adobe Enterprise-storage-projekt visas dokumentmappen för en uppgift som en undermapp i dokumentmappen som skapas automatiskt för projektet.
* Du kan inte kopiera eller flytta en uppgift från ett Workfront-lagringsprojekt till ett Adobe-lagringsprojekt. Det motsatta är inte heller möjligt.

### Dokumenthantering vid problem

Tänk på följande när du arbetar med problem:

* Problem ärver lagringstypen från projekt.
* När du överför ett dokument till ett problem i ett Adobe-lagringsprojekt skapar Workfront automatiskt en mapp i avsnittet Dokument i problemet. Mappnamnet är detsamma som problemet.
* Du kan byta namn på och ta bort dokumentmappen från Adobe Enterprise-storage, som även tar bort dokumenten i mappen. När du har lagt till nya dokument i utgåvan återskapas mappen automatiskt. Borttagna dokument placeras inte tillbaka i mappen.
* För Adobe Enterprise-storage-projekt visas dokumentmappen för ett problem som en undermapp i dokumentmappen som skapas automatiskt för projektet.
* Du kan inte kopiera eller flytta ett problem från ett Workfront-lagringsprojekt till ett Adobe-lagringsprojekt. Det motsatta är inte heller möjligt.

### Dokumenthantering för projektmallar

Tänk på följande när du arbetar med mallar:

* När du skapar en Adobe Enterprise-storage-mall skapar Workfront en mapp i dokumentavsnittet i mallen där dokument sparas. Mappnamnet är samma namn som programmet. Du kan inte ta bort eller ändra namn på mappen manuellt. Mappens namn ändras om du ändrar namnet på mallen så att det matchar mallens nya namn.
* Du kan använda en Workfront-lagringsmall för att skapa Workfront-lagringsprojekt. du kan använda en Adobe-lagringsmall för att skapa ett Adobe-lagringsprojekt.
* Du kan bifoga en Workfront-lagringsmall till ett Adobe-lagringsprojekt och detta ändrar inte lagringsplatsen för projektet.
* Du kan bifoga en Adobe-lagringsmall till ett Workfront-lagringsprojekt och detta ändrar inte lagringsplatsen för projektet.

### Dokumenthantering för malluppgifter

Tänk på följande när du arbetar med malluppgifter:

* Malluppgifter ärver lagringstypen från mallar.
* När du överför ett dokument till en malluppgift på en Adobe-lagringsmall skapas automatiskt en mapp i dokumentavsnittet i malluppgiften i Workfront. Mappnamnet är samma som malluppgiften.
* Du kan byta namn på och ta bort dokumentmappen från Adobe Enterprise-storage-malluppgift som också tar bort dokumenten i mappen. När du har lagt till nya dokument i malluppgiften återskapas mappen automatiskt. Borttagna dokument placeras inte tillbaka i mappen.
* För Adobe Enterprise-storage-mallar visas dokumentmappen för en malluppgift som en undermapp i dokumentmappen som skapas automatiskt för mallen.
* Du kan inte kopiera eller flytta en malluppgift från en Workfront-lagringsmall till en Adobe-lagringsuppgift. Det motsatta är inte heller möjligt.
* När du bifogar ett dokument till ett ärende som du skickar till en begärandekö som är kopplad till Adobe-lagringsutrymmet skapas en mapp för varje skickat problem där dokumenten lagras. Mappen läggs också till som en undermapp i den automatiskt skapade projektmappen i kön.

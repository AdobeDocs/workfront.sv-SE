---
product-area: projects
navigation-topic: manage-issues
title: Flytta problem
description: Du kan flytta problem mellan projekt och uppgifter.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Flytta problem

Du kan flytta problem mellan följande objekt:

* Från ett projekt till ett annat projekt
* Från en uppgift till en annan uppgift i samma projekt eller i ett annat projekt
* Från en uppgift till ett projekt eller till ett annat projekt
* Från ett projekt till en uppgift i samma projekt eller en uppgift i ett annat projekt

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
   <td> <p>Begäran eller senare</p> <p>Granska eller högre licens för att flytta problem i avsnittet Problem i ett projekt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller öka åtkomsten till projekt och uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till problem på din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Bevilja åtkomst till utleveranser</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p>Contribute-behörigheter för det objekt där du flyttar problemet med möjligheten att lägga till problem.</p> <p> Information om hur du beviljar behörigheter för problem finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett ärende </a></p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när det gäller rörliga frågor

Tänk på följande när du flyttar problem som innehåller dokument eller är kopplade till en begärandekö:

* **När ett problem associeras med en frågekö:** När du flyttar ett problem till ett annat objekt och problemet är kopplat till en frågekö, är det flyttade problemet inte längre kopplat till den ursprungliga kön som det första problemet kom från.
* **När ett dokument bifogas till utgåvan:** När du flyttar en utgåva till ett annat objekt och utgåvan har ett bifogat dokument, flyttas även dokumentet, dess versioner och korrektur till den nya utgåvan. Alla godkännanden som är kopplade till dokumentet flyttas inte.
* **När ett problem är länkat till ett dokument eller en mapp:** När du flyttar ett problem som har dokument eller mappar länkade till en tredjepartstjänst som Google Drive, flyttas länkarna till dokumenten med problemet.

## Flytta problem i en lista

Du kan flytta en eller flera utgåvor från en lista med utgåvor eller från en problemrapport.

1. Gå till projektet som innehåller problemet eller problemen som du vill flytta.

   eller

   Gå till en problemrapport.

1. Om du valde att gå till ett projekt klickar du på **Problem** i den vänstra panelen.
1. Markera det eller de problem som du vill flytta och klicka på **Menyn Mer** överst i problemlistan klickar du på **Flytta till**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Fortsätt med att flytta problemet enligt beskrivningen i avsnittet [Flytta ett enstaka ärende](#move-a-single-issue) med början från steg 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Flytta ett enstaka ärende {#move-a-single-issue}

Du kan flytta ett problem när du visar det.

### Flytta ett enstaka problem i förhandsvisningsmiljön

1. Gå till en utgåva som du vill kopiera och klicka på **Mer** meny ![](assets/more-icon.png)till höger om problemnamnet och välj **Flytta** till.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   The **Flytta problem** visas.

   ![](assets/move-issue-box-nwe-350x280.png)

1. I **Välj målprojekt** anger du namnet på det projekt där du vill flytta problemen. Namnet på det aktuella projektet visas som standard.

   >[!TIP]
   >
   >Endast 100 projekt visas i listan.

1. (Villkorligt) Klicka **begära åtkomst** om du inte har åtkomst att flytta utgåvor till projektet.
1. (Villkorligt) Fortsätt att flytta problemet i det valda målprojektet utan att begära åtkomst om du har åtkomst till att lägga till problem i någon av åtgärderna i målprojektet.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Liknande meddelanden visas om det valda projektet väntar på godkännande, är slutfört eller är inaktivt, när Workfront-administratören förhindrar att det uppstår problem i dessa projekt. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Valfritt) I dialogrutan **Alternativ** avmarkerar du något av objekten i tabellen nedan för att ta bort dem från den flyttade utgåvan. Alla alternativ är markerade som standard.

   >[!IMPORTANT]
   >
   >Om du avmarkerar objekt i alternativlistan förlorar du data. Information från den befintliga utgåvan tas bort och kan inte återställas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Markera alla</td> 
      <td>Avmarkera det här alternativet om du vill ta bort all information från problemet när det flyttas till sin nya plats. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td>Tar bort användare, jobbroller eller team som är tilldelade till problemet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förlopp</td> 
      <td>Tar bort procent slutfört, om någon, av utgåvan. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Dokument</p></td> 
      <td> <p>Tar bort allt på dokumentfliken, inklusive dokumentversioner, länkade dokument och mappar.

   <b>ANMÄRKNING</b>

   Om du inte vill att dokumenten ska flyttas med utgåvan, kommer dokumenten att tas bort och placeras i papperskorgen i 30 dagar. En administratör kan återställa dem och de kommer att återställas vid det flyttade problemet.

   Om problemet tas bort efter att det har flyttats placeras de återställda dokumenten i området Dokument på administratörens användarsida, som återställer dem.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Behörigheter</td> 
      <td>Tar bort de entiteter som utgåvan delas med. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdateringar</td> 
      <td>Tar bort kommentarer från uppdateringsavsnittet för problemet.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Valfritt) I dialogrutan **Välj uppgift** väljer du den uppgift där du vill flytta problemet.
1. Klicka **Flytta problem** eller **Flytta problem** om du har valt flera utgåvor i en lista.

   De flyttade problemen läggs till i det angivna projektet.





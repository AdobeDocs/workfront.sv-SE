---
product-area: projects
navigation-topic: manage-issues
title: Kopiera problem
description: Du kan kopiera en utgåva eller en förfrågan och spara dem i samma eller ett annat projekt. Du kan även kopiera ett ärende från en aktivitet till ett annat projekt.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# Kopiera problem

<!--Audited: 08/2025-->

Du kan kopiera en utgåva eller en förfrågan och spara dem i samma eller ett annat projekt. Du kan även kopiera ett ärende från en aktivitet till ett annat projekt.

Du kan kopiera utgåvor från följande objekt:

* Från ett projekt till samma projekt (duplicera det i samma projekt)
* Från en uppgift till samma uppgift (duplicera om den finns i samma uppgift)
* Från ett projekt till ett annat projekt
* Från en uppgift till ett projekt

>[!TIP]
>
>&quot;Issues&quot; och &quot;requests&quot; används utan åtskillnad i Workfront. Du kan registrera problem i både projekt och uppgifter för att indikera oförutsedda arbeten som behöver åtgärdas. Du kan också skicka in begäranden som spelas in som utleveranser i ett projekt som har angetts som en frågekö.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <ul><li><p>Medarbetare eller högre</p> </li>
   <li><p>Ljus eller högre licens för att kopiera ett problem i avsnittet Problem i ett projekt</p></li></ul>
   eller
   <ul><li><p>Begärande eller högre</p> </li>
   <li><p>Granskare eller högre licens för att kopiera ett problem i avsnittet Problem i ett projekt</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller öka åtkomsten till projekt och uppgifter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p>Contribute-behörigheter för det objekt du kopierar problemet till med möjligheten att lägga till problem.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying the issue to with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på när du kopierar problem

### Allmänna överväganden vid kopiering av problem

Du kan välja att kopiera vissa objekt som är kopplade till utgåvan till den kopierade utgåvan under kopieringsprocessen. Vissa objekt överförs dock som standard till den nya utgåvan, medan andra inte gör det, vilket beskrivs i listorna nedan.

Följande objekt kopieras som standard till den nya utgåvan:

* Primär kontakt
* Anpassade formulär. Informationen i de anpassade fälten kopieras endast till den nya utgåvan när du väljer Anpassade data i kopieringsprocessen.
* Godkännanden
* Planerade startdatum och planerade slutförandedatum

Följande objekt kopieras inte till den nya utgåvan som standard:

* Inloggade timmar

### Att tänka på vid problem som rör dokument eller begärandeköer

Tänk på följande när du kopierar problem som innehåller dokument eller är kopplade till en begärandekö:

* **När ett problem är kopplat till en begärandekö:** När du kopierar ett problem till ett annat objekt och problemet är kopplat till en begärandekö, är det kopierade problemet inte längre kopplat till den ursprungliga kö som det första problemet kom från.
* **När ett dokument bifogas till utgåvan:** När du kopierar en utgåva till ett annat objekt och utgåvan har ett bifogat dokument, flyttas även dokumentet och dess versioner till den nya utgåvan. Eventuella korrektur eller godkännanden som är kopplade till dokumentet flyttas inte.
* **När ett problem är länkat till ett dokument eller en mapp:** När du kopierar ett ärende som har dokument eller mappar länkade till en tredjepartstjänst som Google Drive, överförs länkarna till dokumenten till det kopierade problemet.

## Kopiera utgåvor i en lista

Du kan kopiera en eller flera utgåvor från en lista med utgåvor eller från en problemrapport.

1. Gå till projektet som innehåller problemet eller problemen som du vill kopiera.

   eller

   Gå till en problemrapport.

1. Om du valde att gå till ett projekt klickar du på **Problem** i den vänstra panelen.
1. Markera det eller de problem som du vill kopiera och klicka på menyn **Mer** överst i problemlistan och klicka sedan på **Kopiera till**.

   ![Kopiera utgåva i listan](assets/copy-issue-in-list-nwe-350x169.png)

1. Fortsätt med att kopiera problemet, enligt beskrivningen i avsnittet [Kopiera ett enstaka problem](#copy-a-single-issue) med början från steg 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Kopiera en utgåva {#copy-a-single-issue}

Du kan kopiera en utgåva när du visar den.

1. Gå till ett problem som du vill kopiera och klicka sedan på menyn **Mer** ![Mer](assets/more-icon.png) till höger om problemets namn och **Kopiera till**.

   ![Kopiera på problemnivå](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   Rutan **Kopiera utgåva** visas.

   ![Kopiera utgåva](assets/copy-issue-box-nwe-350x285.png)

1. I avsnittet **Välj målprojekt** anger du namnet på det projekt där du vill kopiera problemen. Namnet på det aktuella projektet visas som standard.

   >[!TIP]
   >
   >Endast 100 projekt visas i listan.

1. (Villkorligt) Klicka på **begär åtkomst** om du inte har åtkomst till kopieringsproblem i projektet.
1. (Villkorligt) Fortsätt att kopiera utgåvan till det valda målprojektet utan att begära åtkomst om du har tillgång till att lägga till utgåvor till någon av åtgärderna i målprojektet.

   ![Kopiera problem och begär åtkomst](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Liknande meddelanden visas om det valda projektet väntar på godkännande, är slutfört eller är inaktivt, när Workfront-administratören förhindrar att det uppstår problem i dessa projekt. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Valfritt) I avsnittet **Alternativ** avmarkerar du något av objekten i tabellen nedan för att ta bort dem från den nya utgåvan. Alla alternativ är markerade som standard.

   >[!NOTE]
   >
   >Detta påverkar bara de kopierade utgåvorna och inte de ursprungliga utgåvorna.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td>Tar bort användare, jobbroller eller team som är tilldelade till problemet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förlopp</td> 
      <td>Tar bort procent slutfört, om någon, av utgåvan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td><span style="line-height: 1.5;">Tar bort allt på dokumentfliken, inklusive dokumentversioner, länkade dokument och mappar.</span> <br>Som standard går det inte att kopiera dokumentkorrektur och godkännanden till en annan utgåva.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Behörigheter</td> 
      <td>Tar bort de entiteter som utgåvan delas med. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdateringar</td> 
      <td>Tar bort kommentarer från uppdateringsavsnittet för problemet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassade data</td> 
      <td>Tar bort informationen från det anpassade formuläret i frågan, samt informationen om anpassade formulär som är kopplade till dokument som är kopplade till problemet, om de också kopieras med problemet. De anpassade formulären förblir kopplade till problemen och dokumenten, men informationen i formulären kommer inte att överföras till den nya utgåvan. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) I avsnittet **Välj uppgift** väljer du den uppgift där du vill flytta problemet.
1. Klicka på **Kopiera utgåva** eller **Kopiera utgåvor** om du har markerat flera utgåvor i en lista.

   De kopierade utgåvorna läggs till i det angivna projektet.



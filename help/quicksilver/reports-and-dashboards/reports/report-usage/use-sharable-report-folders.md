---
product-area: reporting
navigation-topic: report-usage
title: Använd delningsbara rapportmappar
description: Använd delningsbara rapportmappar för att ordna de rapporter som du skapar och delar dessa mappar med andra användare i Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 65831f2e-9092-4e99-a86b-40df42c713bf
source-git-commit: 650d24c36c3ccee810b8918ccdf456f607b055e9
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# Använd delningsbara rapportmappar

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

<!-- This article is linked in the UI -->

Du kan använda delningsbara rapportmappar för att ordna rapporter och dela dessa mappar med andra användare. Den här funktionen är avsedd för team som hanterar stora mängder rapporter och behöver skalbar, konsekvent åtkomstkontroll.

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
   <p>alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förstå mappbehörigheter

Delningsbara rapportmappar har två behörighetsnivåer:

* **Visa**: Användare kan öppna rapporter i mappen, men de kan inte redigera mappinformation, lägga till eller ta bort objekt eller ta bort mappen. Du kan tillåta användare med behörigheten Visa att dela mappen genom att aktivera inställningen **Dela** när du beviljar åtkomst.
* **Hantera**: Användare kan redigera mappinformation och lägga till eller flytta rapportobjekt. De får även behörigheten Hantera för rapporter i mappen. Du kan tillåta användare med behörigheten Hantera att dela mappen eller ta bort mappar genom att aktivera inställningarna **Dela** och **Ta bort** när du beviljar åtkomst.

Ytterligare beteende:

* Systemadministratörer kan se alla mappar.
* Andra användare ser bara mappar som de har åtkomst till.
* Behörigheter som ges till en överordnad mapp gäller för alla undermappar och rapporter i mappträdet.
* Användare med åtkomst till en undermapp kan se sina överordnade mappar för navigering, men inte på samma nivå-mappar, om inte åtkomst beviljas.

## Skapa en delbar rapportmapp

Endast systemadministratörer kan skapa mappar på den översta nivån. När en delbar mapp har skapats kan användare med behörigheten Hantera skapa undermappar i den.

{{step1-to-reports}}

1. Aktivera växlingsknappen **Delningsbara rapportmappar**.
1. Klicka på **Skapa mapp**.
1. Ange ett namn för mappen.
1. Klicka på **Skapa**.

![skapa en delbar mapp](assets/add-sharable-folder.png)

## Skapa en undermapp i en delbar rapportmapp

Du kan skapa upp till tre nivåer med undermappar i en delbar rapportmapp. Undermappar ärver behörigheter från den överordnade mappen, men du kan också ange unika behörigheter för varje undermapp.

{{step1-to-reports}}

1. Leta reda på mappen som du vill skapa en undermapp i.
1. Klicka på **Mer** > **Lägg till undermapp**.
1. Ange ett namn för undermappen.
1. Klicka på **Skapa**.

## Dela en rapportmapp med andra användare

När du delar en mapp med användare ärver de åtkomst till alla undermappar i det mappträdet. Användarna måste också ha tillgång till varje rapport, antingen via mappbehörigheter eller direkt rapportdelning.

{{step1-to-reports}}

1. Hitta mappen som du vill dela.
1. Klicka på **Mer** > **Dela**.
1. Lägg till användare, team, roller, grupper eller företag.
1. Välj **Visa** eller **Hantera** åtkomst:
   * Med visningsåtkomst kan användare öppna rapporter i mappen. Du kan också tillåta användare med behörigheten Visa att dela om mappen genom att välja **Dela** i de extra inställningarna.
   * Med Hantera åtkomst kan användare redigera mappinformation och lägga till eller ta bort objekt. Du kan också ge användare med behörigheten Hantera åtkomst att ta bort mappar eller dela mappen genom att välja **Ta bort** och **Dela** i de extra inställningarna.
1. Klicka på **Spara**.

   ![dela en mapp och finjustera åtkomsten](assets/share-settings-sharable-folders.png)

## Flytta en rapport till en delbar mapp

Om du vill flytta en rapport till en mapp måste du ha **Hantera**-behörighet till både rapporten och den delningsbara mappen.

{{step1-to-reports}}

1. Markera kryssrutan bredvid den rapport som du vill flytta.
1. Klicka på **Flytta till mappen** i åtgärdsfältet längst ned på skärmen.
1. Leta reda på mappen som du vill flytta rapporten till och klicka sedan på **Flytta**. Rapportträdet är komprimerat som standard, så du kan behöva expandera mapparna för att hitta målmappen.

   ![flytta en rapport till en delbar mapp](assets/move-to-folder.png)

## Ta bort en delbar rapportmapp

När du tar bort en mapp tas även alla undermappar i den mappen bort. Du måste ha **Hantera**-åtkomst till mappen för att kunna ta bort den. Rapporterna i mappen tas inte bort och finns fortfarande i huvudrapportlistan.

Rapportbehörigheter som beviljats via mappbehörigheter tas bort när mappen tas bort. Rapportbehörigheter som har beviljats direkt från rapporten eller ärvts från en kontrollpanel finns kvar.


{{step1-to-reports}}

1. Klicka på **Mer** > **Ta bort**.
1. Klicka på **Ja, ta bort den** för att bekräfta.


## Ny listupplevelse för delningsbara mappar

När du får åtkomst till delningsbara mappar i området Rapporter visas en ny listupplevelse som gör att du enkelt kan visa och hantera dina mappar och rapporter. Mer information om den nya listupplevelsen finns i [Använda förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
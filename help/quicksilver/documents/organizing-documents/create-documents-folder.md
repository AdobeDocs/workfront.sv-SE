---
product-area: documents
navigation-topic: organize-documents
title: Skapa dokumentmappar
description: Dokument kan ordnas i mappar. Du kan skapa personliga mappar i ditt personliga dokumentområde.
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
source-git-commit: ff05270bd808d26abfed7b0d20b37f0bfc314c08
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Skapa dokumentmappar

Dokument kan ordnas i mappar. Workfront har för närvarande två versioner av dokumentområdet: det gamla dokumentområdet och det nya dokumentområdet. Vilken version din organisation använder beror på om din organisation använder äldre Workfront-lagring eller Enterprise-lagring. Mer information om de här lagringstyperna finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <p>Medarbetare eller högre</p>
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa dokumentmappar i det äldre dokumentområdet

Om ditt företag har äldre Workfront-lagring visas det äldre dokumentområdet när du öppnar dokument i Workfront. Mer information om äldre Workfront-lagring finns i [Skillnader mellan Adobe Enterprise-lagring och äldre Workfront-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>När du ordnar dokument skapas helt enkelt länkar mellan dokumenten och de objekt du associerar dem med. De omplaceras inte i systemet.

### Visa mappar

Du kan visa mappar i miniatyrvyn, standardvyn eller listvyn. Om du vill ändra vyn använder du visningsalternativen i det övre högra hörnet.

{{step1-to-documents}}

eller

Klicka på **Dokument** i den vänstra panelen när ett Workfront-objekt är öppet.

1. Klicka på visningsalternativen ovanför den högra panelen för att ändra hur dokumenten visas.

   ![Alternativ för dokumentvy](assets/screenshot-2016-07-07-12.46.54.png)

### Skapa mappar och undermappar

Skapa mappar för att ordna dina dokument bättre. Du kan skapa upp till 2 000 mappar på ett objekt och upp till 50 undermappar i varje mapp. Undermappar räknas som högst 2 000 mappar.

{{step1-to-documents}}

eller

Klicka på **Dokument** i den vänstra panelen när ett Workfront-objekt är öppet.

1. Om du vill skapa en mapp på den översta nivån kontrollerar du att inget är markerat och klickar sedan på **Lägg till ny** > **Mapp**.

   eller

   Om du vill skapa en undermapp markerar du den mapp där du vill skapa undermappen och klickar sedan på **Lägg till ny** > **Mapp**.

### Dela mappar

Mer information om att dela mappar finns i [Dela en dokumentmapp](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Skapa dokumentmappar i området för nya dokument

Om ditt företag använder Enterprise-lagring visas det nya dokumentområdet när du öppnar dokument i Workfront. Mer information om Enterprise-lagring finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Systemgenererade mappar

När du överför ett dokument till en uppgift eller ett problem skapas automatiskt en systemgenererad mapp som heter efter uppgiften eller problemet. Den här mappen är länkad till uppgiften eller problemet och ärver dess behörigheter. Systemgenererade mappar visas i dokumentområdet på projektnivå.

Mer information om mappbehörigheter finns i [Så här fungerar dokumentbehörigheter](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

### Skapa undermappar

Du kan skapa undermappar i en systemgenererad mapp för att ordna dokumenten ytterligare. Alla undermappar ärver behörigheter från den överordnade mappen.

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.
1. Klicka på den mapp som du vill skapa en undermapp i och klicka sedan på ikonen **Lägg till mapp** ![Lägg till mapp](assets/add-folder-icon.png) .
   ![lägg till undermapp](assets/add-subfolder.png)
1. Ange ett namn för undermappen och klicka sedan på **Skapa**.

### Byta namn på en mapp

Systemgenererade mappar ärver automatiskt namnet på uppgiften eller utgåvan. Du kan byta namn på mapparna genom att klicka på mappnamnet och redigera det.

Ändra namn på en mapp:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.
1. Leta reda på mappen som du vill byta namn på och klicka sedan på ikonen **Mer** ![Mer](assets/more-icon.png) .
1. Klicka på **Byt namn** och ange sedan ett nytt namn för mappen.

   ![ändra namn på mappen](assets/rename-folder.png)

1. Klicka på **Byt namn**.

### Flytta en mapp

Systemgenererade mappar kan flyttas till ett annat projekt, en annan uppgift eller ett annat problem. Om en systemgenererad mapp flyttas till en annan plats, uppdateras dess länkade objekt till det nya objektet och behörigheter ärvs från det nya överordnade objektet. Du kan också flytta undermappar till ett annat projekt, en annan uppgift eller ett annat ärende.

>[!NOTE]
>
>Endast projekt, uppgifter och problem som använder samma lagringstyp är tillgängliga i flyttningsdialogrutan. Om du till exempel flyttar en mapp i ett Enterprise-lagringsprojekt är det bara projekt, uppgifter och utgåvor som använder Enterprise-lagring som går att flytta till.


Flytta en mapp:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.
1. Leta reda på mappen som du vill flytta och klicka sedan på ikonen **Mer** ![Mer](assets/more-icon.png) .
1. Klicka på **Flytta** och välj sedan det projekt, den uppgift eller det problem som du vill flytta mappen till.


   ![flytta mapp](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new documents area -->

### Ta bort en mapp

Ta bort en mapp:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.
1. Leta reda på mappen som du vill ta bort och klicka sedan på ikonen **Mer** ![Mer](assets/more-icon.png) .
1. Klicka på **Ta bort**.

   ![ta bort mapp](assets/rename-folder.png)

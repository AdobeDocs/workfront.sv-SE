---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Hanterade SDL-översättningsmoduler
description: I en [!DNL Adobe Workfront Fusion] kan du ansluta ditt SDL Managed Translation-konto till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# [!DNL SDL Managed Translation] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du ansluta [!DNL SDL Managed Translation] konton för flera tredjepartsprogram och -tjänster.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Moduler

>[!NOTE]
>
>Åtgärdens timeout för anrop till [!DNL SDL Managed Translation] är **120 sekunder**.

### Filer

#### [!UICONTROL Download Translated File]

Den här modulen hämtar innehållet i en översatt fil, som finns i det angivna projektet. Om den begärda filen ännu inte är i läget Nedland kanske inte innehållet i filen är fullständigt översatt. Om filen är i hämtningsstatus, och du har hämtat den, måste du markera filen som slutförd med `Cancel or Complete File` -metod.

#### [!UICONTROL Upload a File]

Den här modulen tillåter överföring av filer för översättning eller för inkludering i ett översättningsprojekt som referensmaterial. Överföringar måste skickas in med multipart/form-data och kan innehålla mer än en fil. Du anger `ProjectOptionId` som ska användas för att utvärdera de överförda filerna. Detta avgör om varje fil som du överför är en möjlig kandidat för översättning eller måste hanteras som referensmaterial. I fråga om arkiv (`zip `, `rar`, `7z`, `tar` filer) som programmet undersöker innehållet i arkivet och anger om arkivet som helhet kan översättas eller om det innehåller en blandning av översättningsbara och icke-översättningsbara filer.

>[!NOTE]
>
>Vi rekommenderar inte att du överför mer än en fil åt gången eftersom det kan öka effekten av eventuella fel.

#### [!UICONTROL Add a Reference File]

Den här modulen lägger till en referensfil.

### Projekt

#### [!UICONTROL Create a project]

Den här modulen skapar det angivna projektet.

#### Avbryt eller slutföra ett projekt

Den här modulen avbryter eller slutför det angivna projektet. Om projektet väntar på att laddas ned, kommer projektet att gå igenom de sista stegen i arbetsflödet och slutligen fortsätta. Om projektet väntar på godkännande eller om leverantörsvalet avbryts. Om projektet har någon annan status kommer begäran att misslyckas.

#### [!UICONTROL Download Project Zip]

Den här modulen hämtar `zip` fil med översatta filer för det angivna projektet.

#### [!UICONTROL Read a Project]

Den här modulen hämtar det angivna projektet.

#### [!UICONTROL Get Projects at Status]

Den här modulen hämtar alla tillgängliga projekt med den angivna statusen. Med den här metoden kan resultaten växlas genom att ange `$top`, `$skip`och `$orderby` frågeparametrar.

#### [!UICONTROL Get Projects List]

Hämtar en enkel lista över alla projekt, med allmän information om varje projekt. Med den här metoden kan resultaten vara sidor, genom att ange `$top`, `$skip`och `$orderby` frågeparametrar.

#### [!UICONTROL Search Project Creation Options]

Den här modulen hämtar alternativ för att skapa projekt.

### Övriga

#### [!UICONTROL Make an API Call]

Den här modulen utför ett godtyckligt auktoriserat API-anrop.

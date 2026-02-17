---
product-area: documents
navigation-topic: approvals
title: Konfigurera varumärken för AI Reviewer
description: Konfigurera varumärken för AI Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
source-git-commit: 07b401c70dfd209d13c34cf62844f334f3260af1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Konfigurera varumärken för AI Reviewer

>[!IMPORTANT]
>
>Den här funktionen är för närvarande i betaversion.

I AI Reviewer används varumärkesriktlinjer för att utvärdera innehåll under granskningsprocessen. Du kan skapa varumärken i Workfront genom att överföra PDF-filer som innehåller varumärkesriktlinjerna eller genom att ange märkeselement manuellt.

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
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara systemadministratör.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console permissions*</td> 
   <td> <p>Du måste ha GenStudio Brand Manager.</p>
    <p>Obs! För att kunna välja GenStudio Brand Manager måste du följa de steg som beskrivs i <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/configure-brand-permissions">Tilldela varumärkesbehörigheter</a>.</p>
   </td> 
  </tr> 
 </tbody> 
</table>





Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Förutsättningar

* Din organisation måste ha migrerat till Adobe IMS (Identity Management System).
* Enhetliga godkännanden måste vara aktiverat för din Workfront-instans.
* Din organisation måste ha GenStudio Foundation.
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands.
Mer information om hur du signerar avtalet finns i [Signera Adobe Gen AI-avtalet](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Skapa ett varumärke med en PDF

{{step-1-to-setup}}

1. Gå till **Granska och godkänn** > **Varumärken** i den vänstra panelen.
1. Klicka på **Lägg till varumärke** i skärmens övre högra hörn.
1. Ge varumärket ett namn.
1. Klicka på Överför PDF-filer för att överföra varumärkesfiler.
   ![överför varumärkesPDF:er](assets/upload-PDF.png)
1. Klicka på **Fortsätt**.
1. Ladda upp en eller flera PDF-filer som innehåller varumärkesriktlinjerna och klicka sedan på **Lägg till varumärke**.
1. När filerna har överförts kan du granska de extraherade varumärkeselementen för att säkerställa att de är i linje med varumärkesriktlinjerna.

   >[!IMPORTANT]
   >
   >Riktlinjer genereras med hjälp av filer och generativ AI-teknik och kan vara felaktiga. Granska extraherade riktlinjer för att hitta felaktiga eller saknade detaljer och redigera dem innan du publicerar det här varumärket.

1. När du är klar klickar du på **Publicera** för att göra varumärket tillgängligt för AI Reviewer.

## Skapa ett varumärke manuellt

{{step-1-to-setup}}

1. Gå till **Granska och godkänn** > **Varumärken** i den vänstra panelen.
1. Klicka på **Lägg till varumärke** i skärmens övre högra hörn.
1. Ge varumärket ett namn.
1. Klicka på **Lägg till manuellt** om du vill skapa ett varumärke med enskilda element.
1. Fyll i varumärkesinformationen efter behov. Du kan lägga till följande element:

   <table>
    <tr>
        <td>När ska du använda</td>
        <td>Låt marknadsförarna veta när de ska använda det här varumärket.</td>
    </tr>
    <tr>
        <td>Röstriktlinjer</td>
        <td>Ge vägledning om tonen och stilen på varumärkets röst.</td>
    </tr>
    <tr>
        <td>Bildriktlinjer</td>
        <td>Ange vilka typer av bilder som passar varumärkesets identitet.</td>
    </tr>
    <tr>
        <td>Kanalriktlinjer</td>
        <td>Skapa en översikt över lämpliga kanaler för varumärkeskommunikation.</td>
    </tr>
    <tr>
        <td>logotyper</td>
        <td>Inkludera de officiella logotyper som är kopplade till varumärket.</td>
    </tr>
    <tr>
        <td>Färger</td>
        <td>Ange varumärkets färgpalett.</td>
    </tr>
    </table>

   ![lägg till märkeselement manuellt](assets/brand-elements.png)


1. När du är klar klickar du på **Publicera** för att göra varumärket tillgängligt för AI Reviewer.

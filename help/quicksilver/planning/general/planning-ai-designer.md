---
title: Kom igång med Adobe Workfront Planning Designer
description: Med Adobe Planning Designer kan du skapa en ny arbetsyta, komplett med posttyper och fält i Workfront Planning, lägga till objekt på en arbetsyta eller visa ändringshistorik för poster.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---


# Kom igång med Adobe Workfront Planning Designer

{{planning-important-intro}}

Med Adobe Planning Designer kan du skapa en ny arbetsyta, komplett med posttyper och fält i Workfront Planning, lägga till objekt på en arbetsyta eller visa ändringshistorik för poster.

>[!IMPORTANT]
>
>Planning Designer är för närvarande endast tillgängligt för användare som deltar i den stängda betaversionen.

## Åtkomstkrav <!--edit theses-->

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Alla Workfront- och Planning-paket</p>
<p>Alla arbetsflödes- och planeringspaket</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anmäl dig till det stängda Beta-programmet för Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

För närvarande kan du begära att få delta i det stängda Beta-programmet för Planning Designer.

## Att tänka på när det gäller Planning Designer

<!--these are from the AI Assistant - edit these-->

* För att kunna använda Planning Designer måste du först aktivera AI-assistenten för din organisation. Följande måste vara aktiverat för att AI-assistenten ska vara tillgänglig för alla i organisationen:

   * AI-assistenten måste aktiveras för din organisation innan den är tillgänglig för användare i ditt företag. Mer information finns i [Översikt över AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * När Workfront har aktiverat AI-assistenten för din organisation är den tillgänglig för den huvudsakliga Workfront-administratören. Mer information finns i [Konfigurera grundläggande information för systemet](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

   * Workfront-administratören måste aktivera AI-assistenten för alla andra användare. Mer information finns i [Aktivera eller inaktivera AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

   * AI-assistenten fungerar för varje sida. De förfrågningar du skickar för AI-assistenten måste referera till funktioner som är tillgängliga på den sida som du har öppnat.

* För att du ska kunna använda Planning Designer måste systemadministratören aktivera det under Systeminställningar i installationsprogrammet.

* De åtgärder som AI-assistenten utför i Planning-området hänger ihop med dina Workfront Planning-behörigheter och din åtkomstnivå i Workfront. Mer information finns i följande artiklar:

   * [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Ändringar som AI-assistenten gör för användarens räkning spåras i postens historikpanel.

* Du kan använda kommandon för att ångra åtgärder. Du kan t.ex. skriva &quot;Ångra den senaste ändringen&quot; för att ångra ändringen.

* När du skapar, uppdaterar eller tar bort ett objekt med hjälp av AI Assistant, visas de tänkta åtgärderna och AI Assistant ombeds bekräfta. Du kan sedan bekräfta eller avbryta åtgärderna.

—>

## Funktioner för Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

Du kan använda Planning Designer eller AI Assistant för att utföra följande åtgärder:

* Skapa och konfigurera arbetsytor

* Skapa posttyper

* Designfält eller formelfält

* Skapa, ta bort, duplicera och återställa poster

* Redigera, uppdatera och lägga till ett fält i en post

* Länka poster till andra poster

* Nå ändringshistorik för poster

* Skapa anpassade vyer

* Skapa poster genom att importera ett dokument. Det går bara att skapa poster från ett importerat dokument i Planning Designer, inte i AI-assistenten. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Hitta Planning Designer i Workfront Planning

Du kommer åt Planning Designer från huvudsidan i Workfront Planning.

<!--add screen shot-->

Du kan också använda AI-assistenten för att utnyttja samma funktioner som Planning Designer.

## Aktivera Designer för planering för din organisation

Som Workfront-administratör måste du först aktivera Planning Designer för din organisation.

<!--add steps here-->

## Skapa eller uppdatera objekt med Planning Designer

Du kan skapa eller uppdatera objekt i Workfront Planning antingen med Planning Designer eller AI Assistant, om inget annat anges.

1. Logga in på Workfront och klicka sedan på ikonen **Huvudmeny** ![Huvudmeny](assets/dots-main-menu.png) i skärmens övre högra hörn eller på ikonen **Huvudmeny** ![Linjernas huvudmeny](assets/lines-main-menu.png) i det övre vänstra hörnet, om den är tillgänglig.

1. Klicka på **Planering**. Planeringsområdet öppnas.

1. Klicka på **Design med AI**.

1. Börja skriva kommandon för AI-assistenten och klicka sedan på Enter när du är klar.

   <!--add screen shot-->

   Du kan t.ex. skriva en begäran som liknar den nedan:

   * Skapa och konfigurera en arbetsyta med fem posttyper för att hantera kampanjer

   * Skapa marknadsföringskampanjer för varje månad det aktuella året

   * Lägg till ett kampanjfält för status för arbetsytan Marketing Design

   * Ta bort alla poster i en inaktuell status

   * Uppdatera alla planeringskampanjer till statusen Aktiv

   * Ansluta kampanjer till personer på arbetsytan för marknadsdesign

   * Visa ändringshistoriken för kampanjen&quot;Alla hjärtans dag&quot;

   * Bygg en tidslinjevy för kampanjer i arbetsytan Marketing Design

   * Skapa poster genom att importera ett dokument. Det går bara att skapa poster från ett importerat dokument i Planning Designer, inte i AI-assistenten.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   En visuell förhandsgranskning visas med ett exempel på vad assistenten kan skapa.

1. När du har fått ett svar följer du länkarna på kommandoraden för att skapa, uppdatera eller granska objektet för din begäran.





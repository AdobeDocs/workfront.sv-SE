---
title: Kom igång med Adobe Workfront Planning Designer
description: Med Adobe Planning Designer kan du skapa en ny arbetsyta, med posttyper och fält i Workfront Planning, lägga till objekt på en arbetsyta eller visa ändringshistorik för poster.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Kom igång med Adobe Workfront Planning Designer

{{planning-important-intro}}

Du kan använda Adobe Planning Designer som drivs av AI för att skapa en ny arbetsyta, lägga till objekt på en arbetsyta (posttyper, poster, vyer eller fält) eller visa ändringshistorik för poster.

>[!IMPORTANT]
>
>Planning Designer är för närvarande endast tillgängligt för användare som deltar i det stängda Beta-programmet.

Mer information om Workfront Planning finns i följande artiklar:

* [Allmän information om Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Kom igång med Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Åtkomstkrav

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

* För att du ska kunna använda Planning Designer måste din organisation uppfylla kraven för att kunna använda Workfront AI Assistant.

  Mer information finns i [Förutsättningar för AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* För att du ska kunna använda Planning Designer måste systemadministratören aktivera det under Systeminställningar i installationsprogrammet.

* Du kan använda uppmaningar för att skapa Planning-objekt antingen med Workfront AI Assistant från Planning-området eller med Planning Designer.

* De åtgärder som AI-assistenten utför i Planning-området eller de som utförs av Planning Designer står i samband med dina Workfront Planning-behörigheter och din åtkomstnivå i Workfront.

  Mer information finns i följande artiklar:

   * [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Ändringar som görs av Planning Designer för användarens räkning spåras i postens historikpanel.

* Du kan använda kommandon för att ångra åtgärder. Du kan t.ex. skriva &quot;Ångra den senaste ändringen&quot; för att ångra ändringen.

* När du skapar, uppdaterar eller tar bort ett objekt via Planning Designer visas de tänkta åtgärderna och en uppmaning om att bekräfta åtgärden. Du kan sedan bekräfta eller avbryta åtgärderna.

* När du skapar arbetsytor och posttyper med Planning Designer skapas även vyer och fält automatiskt.

## Funktioner för Planning Designer

Du kan använda Planning Designer eller AI Assistant för att utföra följande åtgärder:

* Skapa och konfigurera arbetsytor

* Skapa posttyper

* Designfält eller formelfält

* Skapa, ta bort, duplicera och återställa poster

* Redigera, uppdatera och lägga till ett fält i en post

* Länka poster till andra poster

* Nå ändringshistorik för poster

* Skapa anpassade vyer

* Skapa poster genom att importera ett dokument.

  Det går bara att skapa poster från ett importerat dokument i Planning Designer, inte i AI-assistenten.

  Information om godkända filtyper och storlekar finns i avsnittet Dokumentskyddsutkast i artikeln [Använd formulärfyllning från AI för att fylla i en begäran med hjälp av uppmaningar eller dokument](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Aktivera Designer för planering för din organisation

Som Workfront-administratör måste du först aktivera Planning Designer för din organisation.

<!--add steps here-->

1. Logga in på Workfront som systemadministratör.
1. Klicka på **Huvudmeny** ![Huvudmenyikon](assets/main-menu-shell.png) i skärmens övre vänstra hörn och klicka sedan på **Konfigurera**.
1. Klicka på **System** > i den vänstra panelen och gå sedan till området **AI-inställningar**.
1. Aktivera följande inställningar:
   * **Aktivera AI**
   * **Anmäl dig till AI Betas**
   * **Planerar Designer**

   ![Planerar Designer-inställningar i Systeminställningar](assets/planning-designer-toggle-in-system-preferences.png)
1. Klicka på **Spara**.

   Alla användare i systemet som har en standardlicens kan nu se knappen **Design med AI** på arbetsytans huvudsida i Planering-området. <!--check screen shot-->

   ![Designa med AI-knapp på sidan Arbetsytor](assets/design-with-ai-button-on-workspaces-page.png)

   Alla användare kan nu starta och använda Planning Designer för att skapa och uppdatera Workfront Planning-objekt.

## Skapa eller uppdatera objekt med Planning Designer

Du kan skapa eller uppdatera objekt i Workfront Planning antingen med Planning Designer eller AI Assistant, om inget annat anges.

1. Logga in på Workfront och klicka sedan på ikonen **Huvudmeny** ![Rader på huvudmenyn](assets/lines-main-menu.png) i det övre vänstra hörnet.

1. Klicka på **Planering**. Planeringsområdet öppnas.

1. Klicka på **Design med AI**.

   Fönstret **Planerar Designer** öppnas.

   ![Planerar Designer-fönstret](assets/planning-designer-window.png)

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

1. När du har fått ett svar följer du länkarna i promptområdet för att skapa, uppdatera eller granska objektet i din förfrågan.

   När du går med på att skapa dina objekt visas ändringarna till höger om promptområdet.

   Du kan granska arbetsytor, posttyper, fält, vyer och poster i förhandsgranskningsområdet till höger om uppmaningen.
1. (Valfritt) Ange ytterligare uppmaningar för att redigera dina objekt ytterligare.
1. (Valfritt) Klicka på **Växla förhandsvisningsskärmen för AI-arbetsytan** ![Dölj eller visa förhandsvisningsskärmsikonen](assets/hide-show-preview-screen-in-planning-designer.png) för att öppna eller stänga förhandsvisningsskärmen till höger.
1. Klicka på arbetsytan **Öppna i ny flikikon** ![Öppna arbetsytan i en ny flikikon](assets/open-workspace-on-new-tab-icon.png) för att öppna arbetsytan som du uppdaterar på en ny flik.
1. Klicka på ikonen **Stäng** **X** för att stänga Planering Designer och öppna arbetsytan.
1. Öppna arbetsytan som du redigerade med Planning Designer och gör ytterligare ändringar i objekten.





---
title: Kom igång med Adobe Workfront Planning Designer
description: Med Adobe Planning Designer från AI kan du enkelt konfigurera arbetsytor och datastrukturer. Planning Designer har stöd för allt från att skapa och konfigurera arbetsytor till att definiera fält och formler, hantera poster, granska ändringshistorik och skapa anpassade vyer. Vare sig det används direkt eller via AI Assistant är Planning Designer en flexibel och kraftfull miljö för att bygga upp och underhålla strukturerad, ansluten information.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
source-git-commit: 11b72c797203dcf364281665bc60cf67d25c8b5d
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Kom igång med Adobe Workfront Planning Designer

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designer är för närvarande endast tillgängligt för användare som deltar i det stängda Beta-programmet.
>
>Informationen i den här artikeln handlar om Adobe Workfront Planning, en extrafunktion från Adobe Workfront.
>
>En lista över krav för åtkomst till Workfront Planning finns i [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Allmän information om Workfront Planning finns i [Kom igång med Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Med Adobe Planning Designer från AI kan du enkelt konfigurera arbetsytor och datastrukturer. Planning Designer har stöd för allt från att skapa och konfigurera arbetsytor till att definiera fält och formler, hantera poster, granska ändringshistorik och skapa anpassade vyer.

Vare sig det används direkt eller via AI Assistant är Planning Designer en flexibel och kraftfull miljö för att bygga upp och underhålla strukturerad, ansluten information.

Mer information om Workfront Planning finns i följande artiklar:

* [Allmän information om Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Kom igång med Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Åtkomstkrav <!--edit theses??-->

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

## Gå med i det stängda Beta-programmet för Planning Designer

För närvarande kan du begära att få delta i programmet Closed Beta för Planning Designer genom att skicka ett e-postmeddelande till sargism@adobe.com.

När vi har fått e-postmeddelandet aktiverar vårt konstruktörsteam Planning Designer i din Workfront-instans.

>[!IMPORTANT]
>
>Ditt företag måste först godkänna AI Assistant-avtalet innan Planning Designer är tillgängligt i ditt system.

## Skicka feedback om Planning Designer

Du kan lämna feedback om Planning Designer under betaprogrammet.

1. Logga in på Workfront, klicka på ikonen **Huvudmeny** ![Rader-huvudmenyn](assets/lines-main-menu.png) i det övre vänstra hörnet och klicka sedan på **Planering**.

   Området **Planering** öppnas.

1. Klicka på **Skapa med AI**. <!--update this tag name when they change it-->

   Fönstret **Planerar Designer** öppnas.

1. Klicka **Skicka feedback här** längst ned på sidan.
1. Lägg till din feedback i det tillgängliga utrymmet och klicka sedan på **Skicka**.
Dina synpunkter skickas till konstruktörerna och produktteamen.

## Att tänka på när det gäller Planning Designer

* Om du vill använda Planning Designer måste du först aktivera AI-assistenten för din organisation. Följande måste finnas för att AI-assistenten ska vara tillgänglig för alla i organisationen:

   * Workfront måste göra AI-assistenten tillgänglig för din organisation.

     Mer information finns i [Förutsättningar för AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
   * När Workfront har gjort AI-assistenten tillgänglig för din organisation har den huvudsakliga Workfront-administratören åtkomst till den.

     Mer information finns i [Konfigurera grundläggande information för systemet](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).
   * Workfront-administratören måste godkänna AI Assistant-avtalet och sedan aktivera AI Assistant för alla andra användare.

     Mer information finns i [Aktivera eller inaktivera AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).
* När systemadministratören har aktiverat AI-assistenten för din organisation är Planning Designer som standard tillgängligt för alla användare, om det har gjorts tillgängligt för din organisation.
* Åtgärder som utförs av Planning Designer kan också utföras av AI-assistenten när du använder den i Planning.
* De åtgärder som AI-assistenten utför i Planning-området eller de som utförs av Planning Designer står i samband med dina Workfront Planning-behörigheter och din åtkomstnivå i Workfront.

  Mer information finns i följande artiklar:

   * [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Ändringar som görs av AI-assistenten eller Planning Designer för användarens räkning spåras i postens historikpanel.

* Åtgärder som vidtas av Planning Designer är permanenta och kan vara oåterkalleliga. Om du t.ex. tar bort ett fält kan det inte ångras. Granska alla åtgärder som Designer föreslår innan du godkänner dem.

  >[!IMPORTANT]
  >
  >När du skapar, uppdaterar eller tar bort ett objekt via Planning Designer uppmanas du att bekräfta endast för de åtgärder som är oåterkalleliga. Att ta bort en posttyp eller en arbetsyta går till exempel inte att ångra. Det går inte att ta bort en post. Planering-Designer ber bara om bekräftelse när du försöker ta bort en posttyp eller arbetsyta.

* När du skapar arbetsytor och posttyper med Planning Designer skapas även vyer och fält automatiskt.

## Funktioner för Planning Designer

Du kan använda Planning Designer eller AI Assistant för att utföra följande åtgärder:

* Skapa och konfigurera arbetsytor

<!--On March 2: * Edit workspaces-->

* Skapa posttyper, inklusive definiera och lägga till globala posttyper på arbetsytor

* Designfält eller formelfält

* Skapa, ta bort, duplicera och återställa poster

* Redigera, uppdatera och lägga till ett fält i en post

* Länka poster till andra poster

* Nå ändringshistorik för poster

* Skapa anpassade vyer

* Skapa poster genom att importera ett dokument

  Du kan till exempel överföra en bild av ett organisationsschema till ditt företag och du kan skapa en arbetsyta baserad på den i Planning Designer.

  Det går bara att skapa objekt från ett importerat dokument i Planning Designer, inte i AI-assistenten.

  >[!IMPORTANT]
  >
  >Även om vi stöder filtyperna .XLSX och .CSV kan de inte användas för storskalig postimport via Planning Designer.
  >Om du behöver importera ett stort antal poster rekommenderar vi att du gör det med de manuella funktionerna i Planning.
  >
  >Mer information finns i [Skapa poster genom att importera information från en CSV- eller Excel-fil](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Mer information om filtypsbegränsningar finns i avsnittet&quot;Hämta förslag baserat på ett dokument som du överför&quot; i [Använd formulärfyllning från AI för att fylla i en begäran med hjälp av uppmaningar eller dokument](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Skapa eller uppdatera objekt med Planning Designer

Du kan skapa eller uppdatera objekt i Workfront Planning antingen med Planning Designer eller AI Assistant, om inget annat anges.

1. Logga in på Workfront, klicka på ikonen **Huvudmeny** ![Rader-huvudmenyn](assets/lines-main-menu.png) i det övre vänstra hörnet och klicka sedan på **Planering**.

   Området **Planering** öppnas. <!--update screen shot when they change the name of the button-->

   ![Designa med AI-knapp på sidan Arbetsytor](assets/design-with-ai-button-on-workspaces-page.png)

1. Klicka på **Skapa med AI**. <!--update this when they change it to Generate with AI-->

   Fönstret **Planerar Designer** öppnas. <!--remove the Beta tag here when this removes from Beta-->

   ![Planerar Designer-fönstret](assets/planning-designer-window.png)

1. I det tillgängliga utrymmet börjar du skriva meddelanden för AI-assistenten och klickar sedan på Enter när du är klar.

   <!--add screen shot-->

   Du kan t.ex. skriva frågor som liknar dem nedan:

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

   Du kan visa arbetsytor, posttyper, fält, vyer och poster i förhandsgranskningsområdet till höger om uppmaningen.

   >[!TIP]
   >
   >Vissa objekt skapas omedelbart utan att någon bekräftelse behövs.

1. (Valfritt) Ange ytterligare uppmaningar för att redigera dina objekt ytterligare.
1. (Valfritt) Klicka på ikonen **Visa eller dölj förhandsvisningsskärmen** ![Dölj eller visa förhandsvisningsskärmsikonen](assets/hide-show-preview-screen-in-planning-designer.png) för att öppna eller stänga förhandsvisningsskärmen till höger.
1. Klicka på arbetsytan **Öppna i ny flikikon** ![Öppna arbetsytan i en ny flikikon](assets/open-workspace-on-new-tab-icon.png) för att öppna arbetsytan som du uppdaterar på en ny flik.
1. Klicka på ikonen **Stäng** **X** för att stänga Planering Designer och öppna arbetsytan.
1. Öppna arbetsytan som du redigerade med Planning Designer och gör ytterligare ändringar i objekten.

<!-- for March 2 -- replace the last step with this: 
1. (Optional) To edit a workspace, do one of the following:

    * Open the workspace and manually make changes to it. For information, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md). 
    * Click **Edit with AI**. This opens the Planning Designer. Repeat the steps above to use AI and make further changes to the workspace.-->

## Inaktivera Planering av Designer för din organisation

När Workfront-administratören har godkänt AI Assistant-avtalet aktiveras Planning Designer som standard för alla i organisationen.

Så här stänger du av den:

1. Logga in på Workfront som systemadministratör.
1. Klicka på **Huvudmeny** ![Huvudmenyikon](assets/main-menu-shell.png) i skärmens övre vänstra hörn och klicka sedan på **Konfigurera**.
1. Klicka på **System** > i den vänstra panelen och gå sedan till området **AI-inställningar**.
1. Inaktivera inställningen **Planering av introduktion**. <!--add new screen shot with info icon and new name of the toggle; ensure you don't show the AI Reviewer if it is not in Prod yet-->

   ![Planerar Designer-inställningar i Systeminställningar](assets/planning-designer-toggle-in-system-preferences.png)
1. Klicka på **Spara**.

   Detta tar bort Planning Designer för alla användare i systemet.

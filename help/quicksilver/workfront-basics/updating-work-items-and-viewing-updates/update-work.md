---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Uppdatera arbete
description: Du kan lägga till en uppdatering för ett Adobe Workfront-objekt (projekt, uppgift eller problem) för att informera om objektets förlopp. Användare som är tilldelade eller prenumererade till objektet kan visa din uppdatering. Du kan också tagga användare så att de uppmärksammas på uppdateringen.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: ca4b3bc9f88a42102f33537dc7b9fd45e0a108d8
workflow-type: tm+mt
source-wordcount: '3460'
ht-degree: 0%

---

# Uppdatera arbete

<!--for the August 10 release: look for these words to see the edits: "August 10"-->

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers only in the Preview environment.</span>-->

>[!NOTE]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>
>Mer information om de nya kommentarfunktionerna finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Du kan komma åt den nya funktionen för följande objekt:
> * Problem, projekt, uppgifter och dokument.
>
>     Det här är tillgängligt när du aktiverar kommenteringsfunktionen Beta.
>
>     Den här funktionen är bara tillgänglig för uppdateringsavsnittet och är inte tillgänglig för följande områden:
>
>     * Startsida
>     * Panelen Sammanfattning i listor
>     * Sammanfattningspanelen i tidrapporter
>
> * Mål, kort i området för anslagstavlor
>
>   Den nya kommentarsupplevelsen är den enda upplevelsen för mål och kort. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information finns i [Krav för att använda Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Du kan lägga till och visa uppdateringar för kort i kortområdet när du aktiverar avsnitten Kommentarer och Systemaktivitet på ett kort. Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).


## Att tänka på när du uppdaterar arbete

* Du kan lägga till kommentarer till de flesta objekt i Adobe Workfront under Uppdateringar. Mer information om vilka objekt som visas i uppdateringsavsnittet finns i [Översikt över uppdateringsavsnittet](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Du kan lägga till kommentarer till Workfront-objekt från andra program som är integrerade med Workfront eller från Workfront mobilapp.

  Alla program som är integrerade med Workfront kan inte lägga till kommentarer i Workfront-objekt.

  Alla funktioner som är tillgängliga i uppdateringsavsnittet för ett objekt i Workfront är inte tillgängliga i andra program vid åtkomst till Workfront-objekt från programmet. Funktioner för RTF eller privata kommentarer till ett företag kanske inte är tillgängliga när du lägger till kommentarer till ett Workfront-objekt från ett tredjepartsprogram.

* Du kan informera om förloppet för ett Workfront-objekt (projekt, uppgift eller problem) när du kommenterar objektet. Användare som har tilldelats eller prenumererar på objektet kan få ett meddelande om uppdateringen. Alla som har behörighet att visa objektet kan visa din uppdatering.

* Du kan tagga användare så att de uppmärksammas på uppdateringen. Taggade användare får ett meddelande i appen och ett e-postmeddelande om uppdateringen.

  >[!TIP]
  >
  >   I den nya kommentarsfunktionen taggas kommentarägare automatiskt. Mer information finns i [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
  <!--take the "in the new commenting experience" out when this is the only experience-->

* Du kan lägga till en kommentar i ett objekt som du kan visa, eller så kan du logga in som Workfront- eller gruppadministratör och lägga till en kommentar för en annan användares räkning. Mer information finns i [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Du kan lägga till en uppdatering till projekt, uppgifter och utgåvor från följande områden i Workfront:

   * Från ett Workfront-objekt, i uppdateringsavsnittet
   * Från hemområdet (för uppgifter och ärenden)
   * Från panelen Sammanfattning i en lista över objekt eller från en tidrapport (för uppgifter och ärenden)

Informationen på den här sidan beskriver hur du kan kommentera Workfront-objekt och hur du uppdaterar projekt, uppgifter och problem.

Mer information om att kommentera mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md). Du måste ha ytterligare en licens för att få tillgång till Workfront Goals.

Mer information om hur du kommenterar kort i området för anslagstavlor finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).

## Åtkomstkrav

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Begär eller högre för problem och dokument; Granska eller högre för alla andra objekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Visa eller redigera åtkomst för objektet som uppdateringen är aktiverad för</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till objektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Lägga till en uppdatering i en arbetsuppgift

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

Hur du lägger till en uppdatering för en arbetsuppgift varierar beroende på vilken version av uppdateringsavsnittet och vilket objekt du väljer.

### Lägga till en uppdatering för en arbetsuppgift i det aktuella uppdateringsavsnittet

>[!NOTE]
>
>Följande funktionalitet är tillgänglig för alla objekt utom mål och kort. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information om att kommentera mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md).
>
>Du kan lägga till och visa uppdateringar för kort i kortområdet när du aktiverar avsnitten Kommentarer och Systemaktivitet på ett kort. Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).

1. Gå till den arbetsuppgift som du vill uppdatera (till exempel ett projekt, en uppgift eller en utgåva) för.
1. Klicka på **Uppdateringar** -avsnitt.
1. Klicka **Starta en ny uppdatering,** skriv sedan in uppdateringen.
1. (Valfritt) Använd RTF eller lägg till känslolägesikoner, länkar eller bilder i uppdateringen för att förbättra innehållet. Mer information finns i [Använda RTF i en Workfront-uppdatering](#use-rich-text-in-a-workfront-update) i den här artikeln.
1. (Valfritt) Uppdatera någon av följande information om arbetsuppgiften:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Meddela</strong></td> 
      <td>Identifiera användare som måste meddelas om uppdateringen. Användare som tilldelas eller prenumererar på objektet får automatiskt ett meddelande när en uppdatering görs.<br><p>Mer information om hur du inkluderar andra i en uppdatering finns i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bekräftelsedatum</strong></td> 
      <td>I datumväljaren väljer du det datum då du bekräftar att arbetsuppgiften ska slutföras. Mer information om implementeringsdatum finns i <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Genomför datumöversikt</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Villkor</strong></td> 
      <td>Välj ett nytt villkor för uppgiften eller utgåvan. Mer information om hur du väljer ett villkor finns i <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Uppdatera villkor för aktiviteter och ärenden</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Klicka på pilen bredvid aktuell status och välj önskad status i listrutan. Mer information om hur du anger en status finns i <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Uppdatera aktivitetsstatus</a>.<p>När du uppdaterar statusen för en arbetsuppgift ändras inte automatiskt statusen för ett projekt. Beroende på hur projektet är konfigurerat kan du göra uppdateringar av projektstatusen separat. Mer information om olika typer av projektuppdateringar finns i <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj typ av projektuppdatering </a>.</p><p><b>ANMÄRKNING</b>

   Du kan inte ändra status för en arbetsuppgift när den har statusen Väntande godkännande.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Slutförandefält</strong></td> 
      <td>(Endast tillgängligt för uppgifter) Ange hur stor del av arbetet som har slutförts genom att dra förloppsindikatorn till önskad procentandel. Du kan också dubbelklicka på det avslutande fältet och ange ett procenttal som är färdigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Privat till mitt företag</strong></td> 
      <td> <p>Inaktivera det här alternativet om du inte vill att användare utanför företaget ska kunna visa den här uppdateringen.</p> 
      <p><b>ANMÄRKNING</b></p>
      <p>Det här alternativet visas bara när användaren är associerad med ett företag.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Uppdatera** för att lägga till uppdateringen i Workfront-objektet.

   >[!NOTE]
   >
   >Ett litet popup-fönster visas i sju sekunder efter klickningen **Uppdatera** så att du kan ångra uppdateringen och gå tillbaka till redigeringsrutan innan uppdateringen har publicerats. Uppdateringen publiceras om du stänger popup-fönstret Ångra, väntar på att det ska försvinna eller navigerar bort från sidan.
   >
   >Om Workfront-administratören väljer inställningen Tillåt aldrig att användare tar bort kommentarer på din åtkomstnivå kan du inte ångra en kommentar. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Information om hur du svarar på en uppdatering finns i [Svara på uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### Lägga till en uppdatering av ett arbetsobjekt med hjälp av Beta-kommenteringsfunktionen

Information om vilka funktioner som är tillgängliga för den nya kommentarsfunktionen och för vilka objekt finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Leta reda på objektet som du vill uppdatera och klicka sedan på dess namn för att öppna objektets sida.
1. Klicka  **Uppdateringar** till vänster.
1. Aktivera **Kommentera betaversion** i det övre högra hörnet av uppdateringsområdet och klicka sedan på **Godkänn** på betaavtalet. Detta växlar uppdateringsområdet till kommenteringsfunktionen Beta.
The **Kommentar** -fliken är markerad som standard.
1. Börja skriva en kommentar i **Ny kommentar** box.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Om du navigerar bort från uppdateringsavsnittet innan du är klar med att skriva och skicka en kommentar, kommer kommentaren på sidan att vara i utkastläge även efter att du loggat ut och loggat in igen. Alla bilder som läggs till i kommentaren sparas också i utkastet. Utkast sparas i 7 dagar efter vilka de tas bort och kan inte återställas. Kommentarerna är bara synliga för användaren som skriver dem.

1. (Valfritt) Om du vill ångra eller göra om en ändring använder du följande kortkommandon:
   * CTRL + Z ( ⌘ + z för Mac) för att ångra en ändring
   * CTRL + Y ( ⌘+y för Mac) för att göra om en ändring
1. (Valfritt) I dialogrutan **Tagga personer eller team** börjar du skriva namnet på eller e-postadressen till en användare, eller ett team som du vill inkludera i kommentaren, och markerar det sedan när det visas i listan.
1. (Valfritt) Använd RTF eller lägg till <!--hidden for August 10: emojis,--> länkar, eller bilder, till uppdateringen för att förbättra innehållet. Mer information finns i [Använda RTF i en Workfront-uppdatering](#use-rich-text-in-a-workfront-update) i den här artikeln.

   >[!TIP]
   >
   >Om en annan användare skickar en kommentar till samma objekt som du uppdaterar visas en röd linje med en ny indikator som informerar dig om de nyare kommentarerna.
   >
   >Indikatorn visas först när kommentaren har skickats för objektet, inte när kommentaren fortfarande är sammansatt.
   >
   >Indikatorn&quot;Nytt&quot; visas bara när både användaren som angav en ny uppdatering och användaren som håller på att uppdatera använder den nya kommentarfunktionen.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Klicka **Skicka** för att lägga till uppdateringen i Workfront-objektet.
1. (Valfritt) Om du vill redigera en kommentar klickar du på **Mer** meny ![](assets/more-menu.png) till höger om ikonen Gilla och klicka sedan på **Redigera**.
1. Redigera informationen i kommentaren, lägg till eller ta bort bilder eller ta bort någon av de taggade användarna.
Du kan redigera din kommentar inom 15 dagar från det att du har skickat in den. En&quot;redigerad&quot; indikator läggs till till vänster om datumstämpeln som visas när kommentaren uppdaterades.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Ett e-postmeddelande skapas för att meddela användare om din uppdatering endast när du skickar den ursprungliga uppdateringen. Inget e-postmeddelande genereras när du har redigerat uppdateringen.
   >* Datumstämpeln bredvid kommentaren är datumet för den ursprungliga kommentaren, inte datumet för den senaste redigeringen.

1. (Valfritt) Klicka på **Svara** för att svara på en befintlig kommentar, följ sedan stegen 4-8 ovan. <!--(**************insure this stays accurate***********)--> Mer information om hur du svarar på en uppdatering finns i [Svara på uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Villkorligt och valfritt) Om andra användare har lagt till kommentarer som visas utanför det synliga området i uppdateringsavsnittet, klickar du på **Visa** inuti den blå **banner för nya kommentarer** längst ned på skärmen för att visa dessa kommentarer.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Ytterligare kommentarer visas längst ned på skärmen.

   >[!NOTE]
   >
   >   Indikatorn&quot;nya kommentarer&quot; och knappen&quot;Visa&quot; visas bara när både de användare som har öppnat de nya uppdateringarna och de användare som för närvarande tittar på uppdateringsavsnittet använder den nya kommentarsfunktionen.


1. (Valfritt) Klicka på **Gilla** icon![](assets/like-icon.png). Ikonen uppdateras med antalet gilla-markeringar.
1. (Villkorligt och Valfritt) Om du har tagit med ytterligare personer i kommentaren klickar du på antalet medlemmar som ingår i uppdateringen för att visa en lista över entiteter som kommentaren du angav delas med.

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Valfritt) Klicka på **Systemaktivitet** för att visa uppdateringar som loggats av systemet. När objektet eller något av dess underordnade objekt uppdateras, genererar Workfront en anteckning om den uppdateringen och visar den på fliken Systemaktivitet.

   Mer information finns i [Översikt över uppdateringsavsnittet](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Du kan inte lägga till en kommentar i en systemuppdatering.


## Använda RTF i en Workfront-uppdatering{#use-rich-text-in-a-workfront-update}

<!--August 10: remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Vissa av alternativen i verktygsfältet RTF kanske inte är tillgängliga för kommenteringsfunktionen Beta.

Du kan förbättra dina uppdateringar genom att använda RTF eller lägga till olika objekt i den, som känslolägesikoner, länkar eller bilder.

1. Gå till **Uppdateringar** i ett Workfront-objekt och börja skriva en kommentar.
1. (Valfritt) Om du vill lägga till RTF-formatering i uppdateringen använder du attribut på **RTF** när du skriver. <!--on August 10, add a screen shot of the complete Rich Text bar here, before the table-->

   | **Attribut** | **Knappen Verktygsfält** | **Mac kortkommandon** | **Kortkommandon i Windows** |
   |---|---|---|---|
   | Fet | ![mceclip10.png](assets/mceclip10.png) | Jesse+b | Ctrl+B |
   | Kursiv | ![mceclip9.png](assets/mceclip9.png) | Jesse+i | Ctrl+I |
   | Understruken | ![mceclip8.png](assets/mceclip8.png) | Jesse+u | Ctrl+U |
   | Hyperlänk | ![mceclip7.png](assets/mceclip7.png) | <br>Så här öppnar du rutan Skapa länkar eller Lägg till länkar:¥+K</br> <br>Så här klistrar du in en länk över den markerade texten i betafunktionen för kommentarer:</br> | <br>Så här öppnar du rutan Skapa länkar eller Lägg till länkar: Ctrl+K</br> <br>Så här klistrar du in en länk över den markerade texten i betafunktionen för kommentarer: Ctrl+V</br> |
   | Punktlista | ![mceclip6.png](assets/mceclip6.png) | Jesse+Shift+8 | Ctrl+Skift+8 |
   | Numrerad lista | ![mceclip5.png](assets/mceclip5.png) | Jesse+Shift+7 | Ctrl+Skift+7 |
   | Blockcitat | ![](assets/block-quote-icon-large.png) | ¥+Shift+9 | Ctrl+Skift+9 |

   Om du vill avbryta formateringen av text avmarkerar du attributet på **RTF** verktygsfält.

   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment-->

   >[!NOTE]
   >
   >* Formateringen visas även i e-postmeddelanden som användare får med din uppdatering.
   >* RTF-formatering som används på en uppdatering i ett e-postmeddelande visas inte på uppdateringen när den visas på fliken Uppdateringar.
   >* Om din organisation använder Workfront med Internet Explorer förlorar all formaterad text som klistras in i en uppdatering sin RTF-formatering och visas som oformaterad text. Du kan formatera om texten med attributen i verktygsfältet RTF.
   >* RTF-formatering är inte tillgängligt för uppdateringar som gjorts i tidrapporteraren eller för antecknings- och senaste villkorsobjekt som visas i en rapport.

1. (Valfritt) Om du vill ta med text från tidigare uppdateringar eller från andra källor och skilja den från din egen uppdatering, kan du markera den som en blockoffert. Klicka på **Blockcitat** icon ![](assets/block-quote-small.png) och skriv den text du vill citera. Den citerade texten visas markerad med en lodrät grå linje. Klicka på **Blockcitat** om du vill återgå till normal formatering.

   ![](assets/block-quote-marked-350x144.png)

1. (Valfritt) Lägg till känslolägesikoner i uppdateringen.

   >[!NOTE]
   >
   >* Workfront ersätter inte skiljetecken som :) med emojis.
   >* Emojis är inte tillgängligt för objekten Anteckning och Senaste villkor som visas i en rapport.
   >* Funktionen emoji i Workfront använder Unicode-tecken och visas därför bara i webbläsare och operativsystem som stöder Unicode-kodpunkter. Användare på en annan plattform, webbläsare eller operativsystemversion än din har kanske inte tillgång till samma känslolägen.
   >* En oanvändbar emoji representeras av en svart eller vit ruta.
   >* Windows 7 har bara stöd för svartvita känslolägesikoner.
   >* E-mojis som tillämpas på en uppdatering som görs via e-post visas inte på uppdateringen när den visas i uppdateringsområdet.

1. (Valfritt) Så här lägger du till en URL-länk till ytterligare informationskällor:

   1. Klicka i uppdateringen där du vill infoga en länk.
   1. På **RTF** klickar du på **Hyperlänk** icon ![](assets/link-icon.png).

   1. I **Skapa länk** ruta som visas, under **URL** skriver eller klistrar du in URL-adressen för den källa som du vill länka till.

   1. Under **Text som ska visas** skriver du eller klistrar in länktexten.
   1. Klicka **Spara**.

1. (Valfritt) Om du vill bifoga en bild till uppdateringen gör du något av följande, beroende på vilken miljö du använder:

   * Klicka på **Bild** icon ![](assets/addimageicon-35x32.png) och bläddra till bilden på datorn eller dra bilden till uppdateringsområdet när du använder den aktuella uppdateringsupplevelsen

   eller

   Klicka på **Lägg till bilaga** icon ![](assets/add-image-mountain-with-plus-icon.png) och bläddra till bilden på datorn när du använder Beta-kommenteringsfunktionen. <!--**************** the tooltip of this icon might be renamed to "Add image")-->

   >[!NOTE]
   >
   >* Din Workfront-administratör måste aktivera tillägg av bilder i avsnittet Inställningar för uppdatering av feeds i Workfront-gränssnittsområdet innan du kan se ikonerna för bilden eller Lägg till bilaga. Mer information finns i [Konfigurera inställningar för användaruppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* Största bildfilsstorlek är 7 MB. Bildfiltyper som stöds är .jpg, .gif och .png.
   >* Bilder är tillgängliga i uppdateringsavsnittet för ett objekt och är även tillgängliga i dokumentområdet.
   >* Du kan skicka en uppdatering med en bild och utan text.
   >* När du tar bort en kommentar som innehåller en bild, finns följande scenarier beroende på vilken upplevelse du väljer:
   >
   >     * I den aktuella kommentarsfunktionen finns bilden kvar i området Dokument, men visas inte längre i uppdateringsavsnittet.
   >     * I den nya kommentarsfunktionen tas bilden bort både från uppdateringsavsnittet och från dokumentområdet. Bilden tas också bort från dokumentområdet när du redigerar en kommentar och tar bort bilden.
   >* När någon tar bort en bild som är kopplad till en kommentar från dokumentområdet tas den även bort från kommentaren.

1. Klicka **Uppdatera**  eller **Skicka** när du använder betafunktionen för kommentarer.


## Kopiera uppdateringsinformation

Du kan kopiera en uppdatering på flera olika sätt. När du har kopierat en länk kan du dela länken med andra för att dirigera dem till uppdateringen.

Kopieringen av en uppdatering skiljer sig åt beroende på vilken kommentarsfunktion du använder.

### Kopiera en uppdatering i den aktuella kommentarsfunktionen

* [Kopiera uppdateringen](#copy-the-update)
* [Kopiera trådlänken](#copy-the-thread-link)
* [Kopiera uppdateringslänken](#copy-the-update-link)

#### Kopiera uppdateringen {#copy-the-update}

Med det här alternativet kopieras texten från en specifik uppdatering till Urklipp.

1. Gå till den uppdatering eller det svar som du vill kopiera.
1. Klicka på **Mer** menyn och klicka sedan på **Kopiera brödtext**.

   ![Välj Kopiera brödtext](assets/update-stream-copy-body-text-350x152.png)

#### Kopiera trådlänken {#copy-the-thread-link}

Med det här alternativet kopieras den fullständiga trådlänken till Urklipp så att du kan dela tråden med andra användare.

1. Gå till uppdateringstråden som du vill kopiera.

1. Klicka på **Mer** menyn och klicka sedan på **Kopiera trådlänk**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Kopiera uppdateringslänken {#copy-the-update-link}

Med det här alternativet kopieras en specifik uppdateringslänk till Urklipp. När du delar uppdateringslänken ser användaren som följer den en ram runt uppdateringen.

1. Gå till den uppdatering eller det svar som du vill kopiera.
1. Klicka på **Mer** -menyn intill den enskilda uppdateringen och klicka sedan på **Kopiera uppdateringslänk**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)


### Kopiera en uppdatering i den nya kommentarsfunktionen

Information om vilka funktioner som är tillgängliga för den nya kommentarsfunktionen och för vilka objekt finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--when we remove and deprecate the legacy stream, add screen shots in the sections below-->

* [Kopiera länk](#copy-link)
* [Kopiera brödtext](#copy-body-text)

#### Kopiera länk

Med det här alternativet kopieras kommentaren eller länken till Urklipp så att du kan dela kommentaren eller hela tråden med andra användare.

1. Gå till den uppdatering vars länk du vill kopiera.

1. Klicka på **Mer** menyn och klicka sedan på **Kopiera länk**.

#### Kopiera brödtext

Med det här alternativet kopieras texten från en specifik uppdatering till Urklipp.

1. Gå till den uppdatering eller det svar som du vill kopiera.
1. Klicka på **Mer** menyn och klicka sedan på **Kopiera brödtext**.

## Ta bort en uppdatering eller ett svar

Beroende på vilken åtkomst din Workfront-administratör ger kan du ta bort uppdateringar som du har lagt till på fliken Uppdateringar för ett objekt. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) i artikeln [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Ingen Workfront-användare (inklusive Workfront-administratören) kan ta bort uppdateringar som gjorts av en annan användare. Om en användares åtkomstnivå tillåter att användaren tar bort sina egna uppdateringar, kan Workfront-administratören logga in som den användaren och ta bort de uppdateringar han/hon har gjort. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) och [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Gå till den uppdatering eller det svar som du vill ta bort.
1. Klicka på **Mer** -menyn bredvid den uppdatering eller det svar som du vill ta bort och klicka sedan på **Ta bort**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klicka på **Bekräfta** eller klicka **Ta bort** när du använder betafunktionen för kommentarer.

   >[!NOTE]
   >
   >Om du tar bort en uppdatering med en bifogad bild tas både kommentaren och bilden bort. Mer information finns i [Använda RTF i en Workfront-uppdatering](#use-rich-text-in-a-workfront-update) i den här artikeln.

   När kommentaren som du tar bort har tillhörande svar, finns det en indikation på att kommentaren togs bort med namnet på den användare som tog bort den.

   ![](assets/removed-comment-indicator-new-experience.png)

   När du använder betafunktionen för kommentarer tas borttagna kommentarer bort direkt från Workfront. En användare som använder uppdateringsavsnittet ser en kommentar som tas bort av en annan användare i realtid.

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

<!--this is no longer needed - adding timesheet comments is just like adding comments to any other object now

## Add an update on a Timesheet

1. Go to a Timesheet on which you want to make an update.
1. Click the Timesheet to open it.
1. At the bottom of the Timesheet, click **Include a comment**.
1. In the box that displays at the bottom of the Timesheet, type an update.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Conditional) To save your update without submitting the Timesheet for approval, click **Save for Later**.

   Or

   To save your update and submit the Timesheet for approval, click **Submit for Approval**.

   Or

   If your Timesheet is not set up with an approver, click **Save and Close Timesheet** to save your update.

-->

## Aktivera eller inaktivera systemuppdateringar

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->

<!--when the new stream goes to all objects production, consider updating this article also, to say there is no System Activity tab to be disabled for objects anymore: help\quicksilver\administration-and-setup\set-up-workfront\system-tracked-update-feeds\system-tracked-update-feeds.md-->

>[!NOTE]
>
>Det går inte att inaktivera systemuppdateringar när den nya kommentarfunktionen används.
>Informationen i det här avsnittet gäller endast de funktioner som är tillgängliga i det aktuella uppdateringsavsnittet.
>Mer information om systemuppdateringar i betaversionen finns i [Översikt över uppdateringsavsnittet](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


I uppdateringsavsnittet för ett Workfront-objekt visas två typer av information:

* **Användaruppdateringar:** Användaruppdateringar är kommentarer som du och andra användare i ditt system anger.

  ![](assets/user-update-cl-350x277.png)

* **Systemuppdateringar:** Systemuppdateringarna registrerar borttagning av resurser, tillägg eller borttagning av versioner, bifogning eller borttagning av en godkännandebegäran samt ändringar som gjorts i dokumenten i objektet.

  ![](assets/system-updates-cl-350x277.png)

  Beroende på din Workfront-licens kan systemuppdateringar vara aktiverade som standard. Workfront-administratörer kan avgöra vad som spåras i systemuppdateringar, vilket förklaras i [Systemspårade uppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Du kan även filtrera bort systemuppdateringar eller aktiviteter så att du bara ser användaruppdateringar för alla objekt.

  Följande objekt har inga systemgenererade uppdateringar:

   * Team
   * Mall
   * Malluppgift

Så här aktiverar eller inaktiverar du systemuppdateringar:

1. Klicka på **Uppdateringar** på ett objekt.
1. Klicka **Visa systemuppdateringar** för att skjuta växeln åt vänster (inaktiverad) eller åt höger (aktiverad).

   ![](assets/show-system-updates-qs-350x55.png)

   Det här alternativet är beständigt för alla objekt i Workfront och behåller sin plats även om du loggar ut från Workfront.

   >[!TIP]
   >
   >   Objekt som inte registrerar systemuppdateringar har inte alternativet Visa systemuppdateringar i uppdateringsområdet.

   <!--when Anna adds the new updates stream to ALL objects, she will remove the System Activity tab from the objects that don't record system updates - add another line to the TIP above to say: The System Activity tab is not available for objects that don't record system-generated updates.*************** OR: maybe make this part of the statement where we list which objects these are, above???  -->



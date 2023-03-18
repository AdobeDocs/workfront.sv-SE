---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Uppdatera arbete
description: Du kan lägga till en uppdatering för ett Adobe Workfront-objekt (projekt, uppgift eller problem) för att informera om objektets förlopp. Användare som är tilldelade eller prenumererade till objektet kan visa din uppdatering. Du kan också tagga användare så att de uppmärksammas på uppdateringen.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 0%

---

# Uppdatera arbete

<!-- Drafted for commenting experience: 

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the way you update work when using the Updates section of an object. 
>You can access the new design by enabling the commenting Beta. 
>Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

Du kan lägga till kommentarer till de flesta objekt i Adobe Workfront under Uppdateringar. Mer information om vilka objekt som visas i uppdateringsavsnittet finns i [Översikt över uppdateringsavsnittet](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

Du kan lägga till en uppdatering för ett Workfront-objekt (projekt, uppgift eller problem) för att informera om objektets förlopp när du kommenterar objektet. Användare som är tilldelade eller prenumererade till objektet kan visa din uppdatering. Du kan också tagga användare så att de uppmärksammas på uppdateringen. Taggade användare får ett meddelande i appen och ett e-postmeddelande om uppdateringen.

Informationen på den här sidan beskriver hur du kan kommentera Workfront-objekt och hur du uppdaterar projekt, uppgifter och problem. Mer information om att kommentera mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md). Du måste ha ytterligare en licens för att få tillgång till Workfront Goals.


Du kan lägga till en uppdatering till projekt, uppgifter och utgåvor från följande områden i Workfront:

* Från ett Workfront-objekt, i uppdateringsavsnittet
* Från hemområdet (för uppgifter och ärenden)
* Från panelen Sammanfattning i en lista över objekt (för uppgifter och ärenden)
* Från tidrapporten (för uppgifter och ärenden)

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
   <td> <p>Begär eller högre för frågor och dokument. Granska eller högre för alla andra objekt</p> </td> 
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

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects

Adding an update to a work item differs depending on what version of the Updates section and what object you choose. 

### Add an update to a work item in the current Updates section

>[!NOTE]
>
>The following functionality is available for all objects except for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. Gå till den arbetsuppgift som du vill uppdatera (till exempel ett projekt, en uppgift eller en utgåva) för.
1. Klicka på **Uppdateringar** -avsnitt.
1. Klicka **Starta en ny uppdatering,** skriv sedan in uppdateringen.
1. (Valfritt) Använd RTF eller lägg till känslolägesikoner, länkar eller bilder i uppdateringen för att förbättra innehållet. Mer information finns i avsnittet&quot;Använd RTF i en Workfront-uppdatering&quot; i den här artikeln
1. (Valfritt) Uppdatera någon av följande information om arbetsuppgiften:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Meddela</strong></td> 
      <td>Identifiera de användare som måste meddelas om uppdateringen. Användare som tilldelas eller prenumererar på objektet får automatiskt ett meddelande när en uppdatering görs.<br><p>Mer information om hur du inkluderar andra i en uppdatering finns i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bekräftelsedatum</strong></td> 
      <td>I datumväljaren väljer du det datum då du ska slutföra arbetsuppgiften. Mer information om implementeringsdatum finns i <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Genomför datumöversikt</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Villkor</strong></td> 
      <td>Välj ett nytt villkor för uppgiften eller utgåvan. Mer information om hur du väljer ett villkor finns i <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Uppdatera villkor för aktiviteter och ärenden</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Klicka på pilen bredvid aktuell status och välj önskad status i listrutan. Mer information om hur du anger en status finns i <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Uppdatera aktivitetsstatus</a>.<p>När du uppdaterar statusen för en arbetsuppgift ändras inte automatiskt statusen för ett projekt. Beroende på hur projektet är konfigurerat kan du behöva göra uppdateringar av projektstatusen separat. Mer information om olika typer av projektuppdateringar finns i <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj typ av projektuppdatering </a>.</p><p><b>ANMÄRKNING</b>

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
   >Ett litet popup-fönster visas i sju sekunder efter att du klickat **Uppdatera** så att du kan ångra uppdateringen och gå tillbaka till redigeringsrutan innan uppdateringen har publicerats. Uppdateringen publiceras om du stänger popup-fönstret Ångra, väntar på att det ska försvinna eller navigerar bort från sidan.
   >
   >Om Workfront-administratören väljer inställningen Tillåt aldrig att användare tar bort kommentarer på åtkomstnivån kan du inte ångra en kommentar. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Information om hur du svarar på en uppdatering finns i [Svara på uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--

### Add an update to a work item using the commenting Beta experience


>[!NOTE]
>
>The functionality described in this section is available for the following objects:
>
>* <span class="preview">Issues, when you enable the commenting Beta experience.</span>
>
>   <span class="preview">This functionality is available only for the Updates section of issues, and it is not available for the following areas:</span>
>
>   * <span class="preview">Home</span>
>   * <span class="preview">Summary panel in lists</span>
>   * <span class="preview">Summary panel in timesheets</span>
>* Goals
>
>   The commenting experience Beta is the default current experience for goals.
>   You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


1. Locate the object you want to update, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Click **Try out the commenting Beta** button in the lower-right corner of the Updates area, then click **Agree** on the Beta agreement. This switches the Updates area to the commenting Beta experience. 
   The **Comments** tab is selected by default. 
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any of the following options from the **Rich Text** toolbar to enhance your text: 

   * Bold
   * Italics
   * Underline
   * Link
   * Bulleted List
   * Numbered List
   * Add attachment (mark this parenthesis as draft: ************ this might be renamed)
   
   For more information, see the "Use Rich Text in a Workfront update" section in this article.

   >[!TIP]
   >
   >   If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
   >
   > ![](assets/real-time-new-red-indicator-unified-commenting.png)



1. Click **Submit** to add the update to the Workfront object. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment, or remove any of the tagged users. 
   You can edit your comment within 15 from submitting it. An "Edited" indicator is added to the left of the date stamp that displays when the comment was updated. 

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********). For information about replying to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Optional) Click the **Like** icon![](assets/like-icon.png). The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When the object or any of its children are updated, Workfront generates a note about that update and displays it in the System Activity tab. 

   For more information see [Updates section  overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >You cannot add a comment to a system update.
-->


## Använda RTF i en Workfront-uppdatering

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.

>[!NOTE]
>
>Some of the options in the Rich Text toolbar are not available for the commenting Beta experience.-->


Du kan förbättra dina uppdateringar genom att använda RTF eller lägga till olika objekt i den, som känslolägesikoner, länkar eller bilder.

1. Gå till uppdateringsområdet och börja skriva en kommentar.
1. (Valfritt) Om du vill lägga till formaterad text i uppdateringen använder du attribut på **RTF** när du skriver.

   | **Attribut** | **Verktygsfältsknapp** | **Mac kortkommandon** | **Kortkommandon för PC** |
   |---|---|---|---|
   | Fet | ![mceclip10.png](assets/mceclip10.png) | Jesse+b | Ctrl+B |
   | Kursiv | ![mceclip9.png](assets/mceclip9.png) | Jesse+i | Ctrl+I |
   | Understruken | ![mceclip8.png](assets/mceclip8.png) | Jesse+u | Ctrl+U |
   | Hyperlänk | ![mceclip7.png](assets/mceclip7.png) | Jesse+K | Ctrl+K |
   | Punktlista | ![mceclip6.png](assets/mceclip6.png) | Jesse+Shift+8 | Ctrl+Skift+8 |
   | Numrerad lista | ![mceclip5.png](assets/mceclip5.png) | Jesse+Shift+7 | Ctrl+Skift+7 |
   | Blockcitat | ![](assets/block-quote-icon-large.png) | ¥+Shift+9 | Ctrl+Skift+9 |

   Om du vill avbryta formateringen av text avmarkerar du attributet på **RTF** verktygsfält.

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
   >* E-mojis är inte tillgängligt för uppdateringar som gjorts i tidrapporteringsområdet eller för antecknings- och senaste villkorsobjekt som visas i en rapport.
   >* Funktionen emoji i Workfront använder Unicode-tecken och visas därför bara i webbläsare och operativsystem som stöder Unicode-kodpunkter. Användare på en annan plattform, webbläsare eller operativsystemversion än din har kanske inte tillgång till samma känslolägen.
   >* En oanvändbar emoji representeras av en svart eller vit ruta.
   >* Windows 7 har bara stöd för svartvita känslolägesikoner.
   >* E-mojis som tillämpas på en uppdatering som görs via e-post visas inte på uppdateringen när den visas i uppdateringsområdet.


1. (Valfritt) Så här lägger du till en URL-länk till ytterligare informationskällor:

   1. Klicka på den plats i uppdateringen där du vill infoga en länk.
   1. På **RTF** klickar du på **Hyperlänk** ikon. ![](assets/link-icon.png)

   1. I **Skapa länk** ruta som visas, under **URL** skriver eller klistrar du in URL-adressen för den källa som du vill länka till.

   1. Under **Text som ska visas** skriver du eller klistrar in länktexten.
   1. Klicka **Spara**.

1. (Valfritt) Om du vill bifoga en bild till uppdateringen klickar du på **Bild** icon ![](assets/addimageicon-35x32.png) och bläddra till bilden på datorn.\
   eller\
   Dra bilden till uppdateringsområdet.

   >[!NOTE]
   >
   >* Workfront-administratören måste aktivera bildtillägg innan du kan se bildikonen.
   >* Största bildfilsstorlek är 7 MB. Bildfiltyper som stöds är .jpg, .gif och .png.
   >* Bilder är bara tillgängliga från fliken Uppdateringar på ett objekt och är inte tillgängliga på fliken Dokument.
   >* Du kan skicka en uppdatering med en bild och utan text.

1. Klicka **Uppdatera**  <!--<span class="preview">or **Submit**</span>, in the commenting Beta experience-->.


## Kopiera uppdateringsinformation

<!--drafted for beta release toggle - remove when copying an update will be available: 

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

Du kan kopiera en uppdatering på flera olika sätt. När du har kopierat en länk kan du dela länken med andra för att dirigera dem till uppdateringen.

* [Kopiera uppdateringen](#copy-the-update)
* [Kopiera trådlänken](#copy-the-thread-link)
* [Kopiera uppdateringslänken](#copy-the-update-link)

### Kopiera uppdateringen {#copy-the-update}

Med det här alternativet kopieras texten från en specifik uppdatering till Urklipp.

1. Gå till den uppdatering eller det svar som du vill kopiera.
1. Klicka på **Mer** menyn och klicka sedan på **Kopiera brödtext**.

   ![Välj Kopiera brödtext](assets/update-stream-copy-body-text-350x152.png)

### Kopiera trådlänken {#copy-the-thread-link}

Med det här alternativet kopieras den fullständiga trådlänken till Urklipp så att du kan dela tråden med andra användare.

1. Gå till uppdateringstråden som du vill kopiera.
1. Klicka på **Mer** menyn och klicka sedan på **Kopiera trådlänk**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Kopiera uppdateringslänken {#copy-the-update-link}

Med det här alternativet kopieras en specifik uppdateringslänk till Urklipp. När du delar uppdateringslänken ser användaren som följer den en ram runt uppdateringen.

1. Gå till den uppdatering eller det svar som du vill kopiera.
1. Klicka på **Mer** -menyn intill den enskilda uppdateringen och klicka sedan på **Kopiera uppdateringslänk**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Ta bort en uppdatering eller ett svar

Beroende på vilken åtkomst din Workfront-administratör ger kan du ta bort uppdateringar som du har lagt till på fliken Uppdateringar för ett objekt. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) i artikeln [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Ingen Workfront-användare (inklusive Workfront-administratören) kan ta bort uppdateringar som gjorts av en annan användare. Om en användares åtkomstnivå tillåter att användaren tar bort sina egna uppdateringar, kan Workfront-administratören logga in som den användaren och ta bort de uppdateringar han/hon har gjort. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) och [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Gå till den uppdatering eller det svar som du vill ta bort.
1. Klicka på **Mer** -menyn bredvid den uppdatering eller det svar som du vill ta bort och klicka sedan på **Ta bort**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klicka på **Bekräfta** <!--<span class="preview">or **Delete**</span>, in the commenting Beta experience-->.

>[!NOTE]
>
>Om du tar bort en uppdatering med en bifogad bild tas både kommentaren och bilden bort.

## Lägga till en uppdatering i en tidrapport

1. Gå till en tidrapport som du vill uppdatera.
1. Klicka på tidrapporten för att öppna den.
1. Klicka på längst ned i tidrapporten **Inkludera en kommentar**.
1. Skriv en uppdatering i rutan som visas längst ned i tidrapporten.

   ![tidrapport_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Villkorligt)Om du vill spara uppdateringen utan att skicka in tidrapporten för godkännande klickar du på **Spara senare**.

   eller

   Om du vill spara uppdateringen och skicka in tidrapporten för godkännande klickar du på **Skicka för godkännande**.

   eller

   Om din tidrapport inte har konfigurerats med en godkännare klickar du på **Spara och stäng tidrapport** för att spara uppdateringen.

## Aktivera eller inaktivera systemuppdateringar

<!--remove preview with 23.2 production: 

<div class="preview">
>[!NOTE]
>
>It is not possible to disable system updates when using the Beta commenting experience. 
>The information in this section refers only to functionality available in the current Updtes section. 
>For more information about system updates in the Beta version, see [Updates section overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md) 
</div>
-->

I uppdateringsavsnittet för ett Workfront-objekt visas två typer av information:

* **Användaruppdateringar:** Användaruppdateringar är kommentarer som du och andra användare i ditt system anger.

   ![](assets/user-update-cl-350x277.png)

* **Systemuppdateringar:** Systemuppdateringarna registrerar borttagning av resurser, tillägg eller borttagning av versioner, bifogning eller borttagning av en godkännandebegäran samt ändringar som gjorts i dokumenten i objektet.

   ![](assets/system-updates-cl-350x277.png)

Beroende på din Workfront-licens kan systemuppdateringar vara aktiverade som standard. Workfront-administratörer kan avgöra vad som spåras i systemuppdateringar, vilket förklaras i [Systemspårade uppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Du kan även filtrera bort systemuppdateringar eller aktiviteter så att du bara ser användaruppdateringar för alla objekt.

Mer information om skillnaden mellan användar- och systemuppdateringar finns i [Systemspårade uppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Så här aktiverar eller inaktiverar du systemuppdateringar:

1. Klicka på **Uppdateringar** på ett objekt.
1. Klicka **Visa systemuppdateringar** för att skjuta växeln åt vänster (inaktiverad) eller åt höger (aktiverad).

   ![](assets/show-system-updates-qs-350x55.png)

   Det här alternativet är beständigt för alla objekt i Workfront och behåller sin plats även om du loggar ut från Workfront.


---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Uppdatera arbete
description: Du kan lägga till en uppdatering för ett Adobe Workfront-objekt (projekt, uppgift eller problem) för att informera om objektets förlopp. Användare som är tilldelade eller prenumererade till objektet kan visa din uppdatering. Du kan också tagga användare så att de uppmärksammas på uppdateringen.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 36b5c534e0a454b3c890d7a5c7c5b6a5a954088b
workflow-type: tm+mt
source-wordcount: '2758'
ht-degree: 0%

---

# Uppdatera arbete

<!--take "Beta" references out when we remove the beta-->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön.</span>

>[!NOTE]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>Mer information om den nya uppdateringsfunktionen finns i [Ny kommentarsfunktion](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).
>
>Du kommer åt den nya designen för följande objekt:
> * <span class="preview">Problem när du aktiverar kommenteringsfunktionen Beta. </span>
   >
   >     <span class="preview">Den här funktionen är bara tillgänglig för uppdateringsavsnittet av utgåvor och är inte tillgänglig för följande områden:</span>
   >
   >     * <span class="preview">Startsida</span>
   >     * <span class="preview">Panelen Sammanfattning i listor</span>
   >     * <span class="preview">Sammanfattningspanelen i tidrapporter</span>
>
> * Mål
   >   Den nya kommentarsfunktionen är standardinställningen för målen. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information finns i [Krav för användning av Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   >
   >    Mer information om att kommentera mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md).


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

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

Hur du lägger till en uppdatering för en arbetsuppgift varierar beroende på vilken version av uppdateringsavsnittet och vilket objekt du väljer.

### Lägga till en uppdatering för en arbetsuppgift i det aktuella uppdateringsavsnittet

>[!NOTE]
>
>Följande funktionalitet är tillgänglig för alla objekt utom mål. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information om att kommentera mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md)

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
      <td>Identifiera användare som måste meddelas om uppdateringen. Användare som tilldelas eller prenumererar på objektet får automatiskt ett meddelande när en uppdatering görs.<br><p>Mer information om hur du inkluderar andra i en uppdatering finns i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a>.</p></td> 
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
      <td>Klicka på pilen bredvid aktuell status och välj önskad status i listrutan. Mer information om hur du anger en status finns i <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Uppdatera aktivitetsstatus</a>.<p>När du uppdaterar statusen för en arbetsuppgift ändras inte automatiskt statusen för ett projekt. Beroende på hur projektet är konfigurerat kan du behöva göra separata uppdateringar av projektstatusen. Mer information om olika typer av projektuppdateringar finns i <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj typ av projektuppdatering </a>.</p><p><b>ANMÄRKNING</b>

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

<div class="preview">

### Lägga till en uppdatering av ett arbetsobjekt med hjälp av Beta-kommenteringsfunktionen

1. Leta reda på objektet som du vill uppdatera och klicka sedan på dess namn för att öppna objektets sida.
1. Klicka  **Uppdateringar** i den vänstra panelen.
1. Aktivera **Kommentera betaversion** i det övre högra hörnet av uppdateringsområdet och klicka sedan på **Godkänn** på betaavtalet. Detta växlar uppdateringsområdet till kommenteringsfunktionen Beta.
The **Kommentarer** -fliken är markerad som standard.
1. Börja skriva en kommentar i **Ny kommentar** box.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Om du navigerar bort från uppdateringsavsnittet innan du är klar med att skriva och skicka en kommentar, kommer kommentaren på sidan att vara i utkastläge även efter att du loggat ut och loggat in igen. Kommentarerna är bara synliga för användaren som skriver dem.

1. (Valfritt) I dialogrutan **Tagga personer eller team** börjar du skriva namnet på eller e-postadressen till en användare, eller ett team som du vill inkludera i kommentaren, och markerar det sedan när det visas i listan.
1. (Valfritt) Om du vill lägga till RTF-formatering i uppdateringen använder du något av följande alternativ i dialogrutan **RTF** verktygsfältet för att förbättra texten:

   * Fet
   * Kursiv
   * Understruken
   * Länk
   * Punktlista
   * Numrerad lista
   * Lägg till bifogad fil <!--(mark this parenthesis as draft: ************ this might be renamed to "Add image")-->

   Mer information finns i avsnittet&quot;Använd RTF i en Workfront-uppdatering&quot; i den här artikeln. <!--remove this list, above, when we get to parity for Rich Text-->

   >[!TIP]
   >
   >Om en annan användare skickar en kommentar till samma objekt som du uppdaterar visas en röd linje med en ny indikator som informerar dig om de nyare kommentarerna.
   >
   >Indikatorn visas bara när kommentaren har skickats för objektet och inte när kommentaren fortfarande är sammansatt.
   >
   >Indikatorn&quot;Nytt&quot; visas bara när både användaren som angav en ny uppdatering och användaren som håller på att uppdatera använder den nya kommentarfunktionen.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)


1. Klicka **Skicka** för att lägga till uppdateringen i Workfront-objektet.
1. (Valfritt) Om du vill redigera en kommentar klickar du på **Mer** meny ![](assets/more-menu.png) till höger om ikonen Gilla och klicka sedan på **Redigera**.
1. Redigera informationen i kommentaren eller ta bort någon av de taggade användarna. <!--check to make sure you can still remove the users in preview or production. At one point, they were removing this functionality-->
Du kan redigera din kommentar inom 15 dagar från det att du skickat in den. En&quot;redigerad&quot; indikator läggs till till vänster om datumstämpeln som visas när kommentaren uppdaterades.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   Ett e-postmeddelande skapas för att meddela användare om din uppdatering endast när du skickar den ursprungliga uppdateringen. Inget e-postmeddelande genereras när du har redigerat uppdateringen.
1. (Valfritt) Klicka på **Svara** för att svara på en befintlig kommentar, följ sedan stegen 4-7 ovan. <!--(**************insure this stays accurate***********)-->. Mer information om hur du svarar på en uppdatering finns i [Svara på uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Valfritt) Klicka på **Gilla** icon![](assets/like-icon.png). Ikonen uppdateras med antalet gilla-markeringar.
1. (Villkorligt och Valfritt) Om du har tagit med ytterligare personer i kommentaren klickar du på antalet medlemmar som ingår i uppdateringen för att visa en lista över entiteter som kommentaren du angav delas med.

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Valfritt) Klicka på **Systemaktivitet** för att visa uppdateringar som loggats av systemet. När objektet eller något av dess underordnade objekt uppdateras, genererar Workfront en anteckning om den uppdateringen och visar den på fliken Systemaktivitet.

   Mer information finns i [Översikt över uppdateringsavsnittet](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Du kan inte lägga till en kommentar i en systemuppdatering.

</div>

## Använda RTF i en Workfront-uppdatering

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Vissa av alternativen i verktygsfältet RTF kanske inte är tillgängliga för kommenteringsfunktionen Beta.

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

1. Klicka **Uppdatera**  <span class="preview">eller **Skicka**</span> i kommenteringsfunktionen Beta.


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
1. Klicka på **Mer** menyn och klicka sedan på **Kopiera trådlänk** <span class="preview">eller **Kopiera länk** när du använder betaupplevelsen</span>.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Kopiera uppdateringslänken {#copy-the-update-link}

Med det här alternativet kopieras en specifik uppdateringslänk till Urklipp. När du delar uppdateringslänken ser användaren som följer den en ram runt uppdateringen.

1. Gå till den uppdatering eller det svar som du vill kopiera.
1. Klicka på **Mer** -menyn intill den enskilda uppdateringen och klicka sedan på **Kopiera uppdateringslänk** <span class="preview">eller **Kopiera länk** när du använder betaupplevelsen</span>.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Ta bort en uppdatering eller ett svar

Beroende på vilken åtkomst din Workfront-administratör ger kan du ta bort uppdateringar som du har lagt till på fliken Uppdateringar för ett objekt. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) i artikeln [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Ingen Workfront-användare (inklusive Workfront-administratören) kan ta bort uppdateringar som gjorts av en annan användare. Om en användares åtkomstnivå tillåter att användaren tar bort sina egna uppdateringar, kan Workfront-administratören logga in som den användaren och ta bort de uppdateringar han/hon har gjort. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) och [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Gå till den uppdatering eller det svar som du vill ta bort.
1. Klicka på **Mer** -menyn bredvid den uppdatering eller det svar som du vill ta bort och klicka sedan på **Ta bort**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klicka på **Bekräfta** <span class="preview">eller **Ta bort**</span> i kommenteringsfunktionen Beta.

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

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->



>[!NOTE]
>
><span class="preview">Det går inte att inaktivera systemuppdateringar när du använder betakommentarsfunktionen. </span>
><span class="preview">Informationen i det här avsnittet gäller endast de funktioner som är tillgängliga i det aktuella uppdateringsavsnittet. </span>
><span class="preview">Mer information om systemuppdateringar i betaversionen finns i [Översikt över uppdateringsavsnittet](../updating-work-items-and-viewing-updates/updates-tab-overview.md). </span>


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


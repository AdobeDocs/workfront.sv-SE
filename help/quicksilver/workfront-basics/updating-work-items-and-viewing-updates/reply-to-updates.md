---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Svara på uppdateringar
description: När någon lägger till eller svarar i en uppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden i avsnittet Uppdateringar för objektet. Du kan lägga till ett svar på en uppdatering eller gilla det om du har åtkomst till objektet via Visa.
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '1099'
ht-degree: 0%

---

# Svara på uppdateringar

{{highlighted-preview}}

<!--remove legacy and new experience references when we remove the legacy updates in the UI - Jan 2024???-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 

-->

>[!IMPORTANT]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>
>Beroende på vilka objekt du har tillgång till kommentarfunktionerna för kan du se följande funktionalitet för uppdateringsavsnittet:
>* Den nya upplevelsen
>* Den gamla upplevelsen
>* Det nya och gamla gränssnittet
>
>Mer information om den nya kommentarsfunktionen och dess tillgänglighet finns på [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Den nya kommentarsupplevelsen är bara tillgänglig för uppdateringsavsnittet för Workfront-objekt och är inte tillgänglig när du öppnar objekt från följande områden:
>
> * Startsida
> * Panelen Sammanfattning i listor
> * Sammanfattningspanelen i tidrapporter
> * Panelen Sammanfattning i Utjämning av arbetsbelastning
>
><span class="preview">Den nya kommentarsfunktionen är tillgänglig på panelen Sammanfattning i listor, tidrapporter och arbetsbelastningsutjämnaren i förhandsvisningsmiljön.</span> <!--and in the Production environment for customers who have opted for the fast release process. For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).-->

När någon svarar på en kommentar eller en systemuppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden i avsnittet Uppdateringar för objektet.

>[!IMPORTANT]
>
>Det går inte att svara på systemuppdateringar i den nya kommentarsfunktionen. Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--adjust the sentence before the second IMPORTANT and remove this important note when we remove legacy from the system-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Begärande eller högre för problem och dokument; Granskare eller högre för alla andra objekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till objektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Svara på en uppdatering eller ett svar i Workfront

Du kan svara på en kommentar i tråden för ett objekt som du kan visa, eller så kan du logga in som Workfront- eller gruppadministratör och svara på en kommentar för en annan användares räkning. Mer information finns i [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Hur du svarar på en kommentar eller ett svar varierar beroende på vilken upplevelse och vilket objekt du väljer.

### Svara på en kommentar när du använder den nya kommentarsfunktionen

Information om vilka funktioner som är tillgängliga i den nya kommentarsfunktionen och för vilka objekt finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Gå till det objekt som du vill lägga till ett svar på.
1. Klicka **Uppdateringar** och klickar sedan på **Kommentar** -fliken för objektet och hitta den kommentar eller det svar som du vill svara på

   eller

   <span class="preview">Klicka på **Alla** tabbtangenten och klicka sedan på **Svara i kommentarer** för att öppna kommentaren på fliken Kommentarer och svara på den. Du kan inte svara på fliken Alla.</span>

1. (Valfritt) Om du vill ta med text från en tidigare uppdatering i ditt svar klickar du på **Mer** i det övre högra hörnet av kommentaren som du vill svara på och klicka sedan på **Offertsvar**. Texten från föregående uppdatering visas i indataområdet, markerat med en lodrät grå linje.
1. Klicka **Svara**.

   ![](assets/reply-to-update-empty-box.png)

   Du kan se de användare som aktivt deltar i konversationen längst ned i **Lägg till svar...** och du kan lägga till fler eller ta bort de som inte längre är relevanta. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet. Du kan också tagga fler användare så att de inkluderas i ditt svar.  Om du vill tagga fler användare läser du [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   Om du vill lägga till fler svar i ett befintligt svar kan du börja skriva i **Lägg till svar ...** eller klicka **Svara** på den ursprungliga kommentaren. Svaret läggs till i slutet av tråden.

1. Börja skriva ditt svar och använd eventuella ytterligare alternativ från verktygsfältet RTF. Mer information om hur du använder RTF eller andra uppdateringsfunktioner finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).

1. Klicka **Skicka** för att spara svaret.

1. (Valfritt) Klicka på **Mer** meny ![](assets/more-menu.png) i det övre högra hörnet av kommentaren som du vill svara på om du vill ha fler alternativ för att hantera svaret. Mer information finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).

### Svara på en uppdatering eller ett svar i det äldre uppdateringsavsnittet

1. Gå till det objekt som du vill lägga till ett svar på.
1. På **Uppdateringar** Leta reda på den uppdatering eller det svar som du vill svara på.

1. (Valfritt) Gör något av följande om du vill visa en bild i den befintliga uppdateringen:

   * Klicka på **Förhandsgranska** icon ![](assets/previewimageicon-31x31.png) på miniatyrbilden för att öppna bilden i full storlek på en ny flik i webbläsaren.
   * Klicka på **Ladda ned** icon ![](assets/downloadimageicon.png) på miniatyrbilden för att hämta bilden.

1. Klicka **Svara** på uppdateringen skriver du ett svar i rutan som visas.

   De användare som aktivt deltar i konversationen eller taggas i varje svar visas högst upp i uppdateringstråden. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet. Du kan också tagga fler användare så att de inkluderas i ditt svar.  Om du vill tagga fler användare läser du [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (Valfritt) Om du vill ta med text från en tidigare uppdatering i ditt svar klickar du på **Mer** -menyn bredvid den uppdatering eller det svar som du vill citera och klicka sedan på **Offertsvar**. Texten från föregående uppdatering visas i indataområdet, markerat med en lodrät grå linje.
1. (Valfritt) Använd formatering, känslolägesikoner, inkludera länkar eller bilder enligt beskrivningen i avsnittet&quot;Använd RTF i en Workfront-uppdatering&quot; i artikeln [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Klicka **Svara** för att spara svaret.

## Svara på en uppdatering från ett e-postmeddelande

Beroende på hur dina e-postmeddelanden är konfigurerade kan du få ett e-postmeddelande när en uppdatering görs för vissa objekt som du har åtkomst till.

Du kan svara på en uppdatering från ett e-postmeddelande på följande sätt:

* Svara på det e-postmeddelande du får. Ditt e-postmeddelande läggs till som ett svar från Workfront på den ursprungliga kommentaren.
* Använd knappen Kommentar i e-postmeddelandet för att gå tillbaka till Workfront och svara på uppdateringen i uppdateringsområdet.

Följande är ett exempel på ett e-postmeddelande som utlöses som ett resultat av en uppdatering som görs på fliken Uppdateringar för en uppgift:

![email.png](assets/email-350x202.png)

Mer information finns i [Svara på e-postmeddelanden](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).







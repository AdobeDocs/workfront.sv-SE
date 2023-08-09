---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Svara på uppdateringar
description: När någon lägger till eller svarar i en uppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden i avsnittet Uppdateringar för objektet. Du kan lägga till ett svar på en uppdatering eller gilla det om du har åtkomst till objektet via Visa.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# Svara på uppdateringar

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
>   Den nya kommentarsupplevelsen är den enda upplevelsen för mål och kort. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information finns i [Krav för användning av Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Du kan lägga till och visa uppdateringar för kort i kortområdet när du aktiverar avsnitten Kommentarer och Systemaktivitet på ett kort. Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).


När någon svarar på en kommentar eller en systemuppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden i avsnittet Uppdateringar för objektet.

>[!IMPORTANT]
>
>Det går inte att svara på systemuppdateringar i den nya kommenteringsfunktionen Beta. Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


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

### Svara på en uppdatering eller ett svar i det aktuella uppdateringsavsnittet

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

### Svara på en kommentar när du använder kommenteringsfunktionen Beta

Information om vilka funktioner som är tillgängliga för den nya kommentarsfunktionen och för vilka objekt finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Gå till det objekt som du vill lägga till ett svar på.
1. Klicka **Uppdateringar** och klickar sedan på **Kommentar** -fliken för objektet och hitta den kommentar eller det svar som du vill svara på.
1. (Valfritt) Om du vill ta med text från en tidigare uppdatering i ditt svar klickar du på **Mer** -menyn bredvid den uppdatering eller det svar som du vill citera och klicka sedan på **Offertsvar**. Texten från föregående uppdatering visas i indataområdet, markerat med en lodrät grå linje.
1. Klicka **Svara**.

   Du kan se de användare som aktivt deltar i konversationen längst ned i **Ny kommentar** och du kan lägga till fler eller ta bort de som inte längre är relevanta. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet. Du kan också tagga fler användare så att de inkluderas i ditt svar.  Om du vill tagga fler användare läser du [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Börja skriva ditt svar och använd eventuella ytterligare alternativ från verktygsfältet RTF. Mer information om hur du använder RTF eller andra uppdateringsfunktioner finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).

1. Klicka **Skicka** för att spara svaret.

1. (Valfritt) Klicka på **Mer** meny ![](assets/more-menu.png) bredvid uppdateringen om du vill ha fler alternativ för att hantera svaret. Mer information finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).


## Svara på en uppdatering från ett e-postmeddelande

Beroende på hur dina e-postmeddelanden är konfigurerade kan du få ett e-postmeddelande när en uppdatering görs för vissa objekt som du har åtkomst till.

Du kan svara på en uppdatering från ett e-postmeddelande på följande sätt:

* Svara på det e-postmeddelande du får. Ditt e-postmeddelande läggs till som ett svar från Workfront på den ursprungliga kommentaren.
* Använd kommentarsknappen i e-postmeddelandet för att gå tillbaka till Workfront och svara på uppdateringen i uppdateringsområdet.

Följande är ett exempel på ett e-postmeddelande som utlöses som ett resultat av en uppdatering som görs på fliken Uppdateringar för en uppgift:

![email.png](assets/email-350x202.png)

Mer information finns i [Svara på e-postmeddelanden](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).







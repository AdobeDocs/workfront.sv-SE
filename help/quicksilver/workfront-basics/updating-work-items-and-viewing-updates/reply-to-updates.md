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
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Svara på uppdateringar

<!-- Audited: April 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

När någon svarar på en kommentar eller en systemuppdatering för ett arbetsobjekt visas deras svar i kommunikationstråden på flikarna Kommentarer och Alla i objektets uppdateringsavsnitt.

>[!IMPORTANT]
>
>Det går inte att svara på systemuppdateringar på fliken Systemaktivitet. Eventuella svar på systemuppdateringar som gjorts i den tidigare kommentarsfunktionen före 11 april 2024 visas som skrivskyddade.

I den här artikeln beskrivs hur du svarar på kommentarer från de flesta objekt i Workfront. Skillnader mellan uppdateringsavsnitten för olika objekt finns i [Översikt över uppdateringsavsnittet](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront package</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td> <p>För ärenden och dokument:</p>

<ul><li><p>Medarbetare eller högre</p></li>
   <li><p>Begäran eller senare</p></li></ul>

<p>För alla andra objekt:</p>
   <ul><li><p>Ljus eller högre</p></li>
   <li><p>Granska eller högre</p></li></ul>

</td>  
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa eller redigera åtkomst för objektet som uppdateringen är aktiverad för</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa behörigheter för objektet</p> </td> 
  </tr> 
 </tbody> 
   </table>

Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p> 
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Svara på en uppdatering eller ett svar i Workfront

Du kan svara på en kommentar i tråden för ett objekt som du kan visa, eller så kan du logga in som Workfront- eller gruppadministratör och svara på en kommentar för en annan användares räkning. Mer information finns i [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

### Svara på en kommentar

Svara på en kommentar i uppdateringsavsnittet för ett objekt liknar svaret för de flesta objekt i Workfront.

1. Gå till det objekt som du vill lägga till ett svar på.
1. Klicka på **Uppdateringar** och sedan på fliken **Kommentarer** för objektet och leta reda på kommentaren eller svaret som du vill svara på

   eller

   Klicka på fliken **Alla** och sedan på **Svara i kommentarer** för att öppna kommentaren på fliken Kommentarer och svara på den. Du kan inte svara på fliken Alla.

1. (Valfritt) Om du vill ta med text från en tidigare uppdatering i ditt svar klickar du på menyn **Mer** i det övre högra hörnet av kommentaren som du vill svara på och sedan på **Offertsvar** . Texten från föregående uppdatering visas i indataområdet, markerat med en lodrät grå linje.
1. Klicka på **Svara**.

   ![Svara för att uppdatera tom ruta](assets/reply-to-update-empty-box.png)

   Du kan se de användare som aktivt deltar i konversationen längst ned i rutan **Lägg till svar..** och du kan lägga till fler eller ta bort de som inte längre är relevanta. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet. Du kan också tagga fler användare så att de inkluderas i ditt svar.  Mer information om hur du taggar fler användare finns i [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   Om du vill lägga till ytterligare svar i ett befintligt svar kan du börja skriva i rutan **Lägg till svar ...** eller klicka på **Svara** på den ursprungliga kommentaren. Svaret läggs till i slutet av tråden.

1. Börja skriva ditt svar och använd eventuella ytterligare alternativ från verktygsfältet RTF. Mer information om hur du använder RTF eller andra uppdateringsfunktioner finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).

1. Klicka på **Skicka** för att spara svaret.

1. (Valfritt) Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) i det övre högra hörnet av kommentaren som du vill svara på om du vill ha fler alternativ för att hantera svaret. Mer information finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).

<!--
### Reply to an update or reply in the legacy Updates section

1. Go to the object to which you want to add a reply.
1. On the **Updates** tab for the object, find the update or reply to which you want to reply.

1. (Optional) To view an image in the existing update do one of the following:

   * Click the **Preview** icon ![Preview image icon](assets/previewimageicon-31x31.png) on the image thumbnail to open the full-size image in a new browser tab.
   * Click the **Download** icon ![Download image icon](assets/downloadimageicon.png) on the image thumbnail to download the image.

1. Click **Reply** on the update, then type a reply in the box that appears.

   You can see the users who are actively engaged in the conversation or tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![Tagging transparency](assets/tagging-transparency-350x192.png)
   
1. (Optional) To include text from a previous update in your reply, click the **More** menu next to the update or reply you want to quote, then click **Quote Reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. (Optional) Use formatting, emojis, include links, or images as explained in the section "Use Rich Text in a Workfront update" in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Click **Reply** to save the reply.

-->

## Svara på en uppdatering från ett e-postmeddelande

Beroende på hur dina e-postmeddelanden är konfigurerade kan du få ett e-postmeddelande när en uppdatering görs för vissa objekt som du har åtkomst till.

Du kan svara på en uppdatering från ett e-postmeddelande på följande sätt:

* Svara på det e-postmeddelande du får. Ditt e-postmeddelande läggs till som ett svar från Workfront på den ursprungliga kommentaren.
* Använd knappen Kommentar i e-postmeddelandet för att gå tillbaka till Workfront och svara på uppdateringen i uppdateringsområdet.

Följande är ett exempel på ett e-postmeddelande som utlöses som ett resultat av en uppdatering som görs på fliken Uppdateringar för en uppgift:

![email.png](assets/email-350x202.png)

Mer information finns i [Svara på e-postmeddelanden](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).







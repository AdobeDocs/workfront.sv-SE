---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Tagga användare för att dela ett korrektur
description: När du kommenterar ett korrektur i korrekturläsaren kan du tagga andra användare så att de uppmärksammas på din kommentar via e-post och lägger till dem i korrekturets arbetsflöde.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Tagga användare för att dela ett korrektur

När du kommenterar ett korrektur i korrekturläsaren kan du tagga andra användare så att de uppmärksammas på din kommentar via e-post och lägger till dem i korrekturets arbetsflöde.

När du taggar användare i kommentarer om ett korrektur kan de användare som du kan tagga variera beroende på olika faktorer, till exempel individuella användarbehörigheter och ditt medlemskap i organisationen:

* Om du har skapat, äger eller har aktiverat specifika behörigheter kan du tagga användare utanför korrekturarbetsflödet och dela korrekturet med dem.
* Om du har lagts till i beviset som en extern användare och är medlem i en annan miljö med ett annat korrekturkonto, kan du bara tagga de användarna från din ursprungliga miljö. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Åtkomstkrav {#access-requirements}

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Gammal plan: Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Korrekturroll</td> 
   <td>Författare, moderator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Ansvarig eller administratör</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Tagga användare för att dela ett korrektur

Användare med rollen Korrekturprofil eller Korrektur som beskrivs i avsnittet [Åtkomstkrav](#access-requirements) ovan kan tagga användare att dela ett korrektur som standard. Du kan även tagga användare så att de delar ett korrektur oavsett rollen Korrekturprofil eller Korrektur om du är korrekturägare eller skapare. Du kan göra det möjligt för användare med lägre behörighetsprofil för korrektur eller korrekturroller att tagga användare att dela ett korrektur när de skapar ett korrektur. Mer information finns i avsnittet [Konfigurera arbetsflödet och lägg till granskare](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) i artikeln [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).

>[!NOTE]
>
>Du kan endast tagga en extern medarbetare med deras e-postadress om något av följande är sant:>
>* En användare på din organisations Workfront-konto har lagt till medarbetarens e-postadress i ett tidigare korrektur.
>* Medarbetaren har använt e-postadressen för att prenumerera på ett bevis i din organisations Workfront-konto tidigare.
>

Så här taggar du någon och delar ett korrektur i en kommentar:

1. När du kommenterar ett korrektur skriver du ett snabel-a (@) följt av personens namn eller e-postadress. När du börjar skriva visas tillgängliga namn i en nedrullningsbar lista.
1. Markera personens namn när du ser det i listrutan.

   >[!TIP]
   >
   >Om du vill stänga listrutan utan att markera någon kan du trycka på **Esc** eller klicka någonstans utanför listan.

1. Upprepa steg 1-2 för alla andra användare som du vill tagga i kommentaren.
1. Slutför kommentaren och klicka sedan på **Publicera**.
1. (Villkorligt) Om du taggar någon som inte redan har lagts till i korrekturet anger du en inställning för **korrekturroll** och **e-postaviseringar** för varje användare som visas i rutan som visas. Klicka sedan på **Lägg till personer och skicka kommentar**.

   ![](assets/add-people-to-proof-350x220.png)

   Mer information om korrekturroller finns i . Mer information om korrekturmeddelanden via e-post finns i avsnittet i artikeln [Konfigurera e-postaviseringsinställningar i Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Om korrekturet har ett automatiserat arbetsflöde läggs de användare du taggar till på den scen du befinner dig i. Mer information finns i [Översikt över automatiserat arbetsflöde](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Alla som du taggar får ett e-postmeddelande om din korrekturkommentar, oavsett vilka e-postvarningsinställningar de använder:

   * Om användaren får en daglig sammanfattning eller en timsammanfattning skickar Workfront meddelandet separat och innehåller information om korrekturkommentaren i det sammanfattande e-postmeddelandet.
   * Om användaren får varningar för alla aktiviteter eller om svar på kommentarer från dem, ersätts meddelandena om dessa kommentarer och svar.

Mer information om andra sätt att lägga till användare i ett korrektur finns i [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

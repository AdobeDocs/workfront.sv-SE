---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Hantera [!DNL Adobe Workfront] meddelanden i [!DNL Microsoft] team
description: Du kan få meddelanden från  [!DNL Adobe Workfront] om objekt som du måste godkänna, uppdrag som du har fått eller kommentarer och ändringar i objekt som du är kopplad till.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 7720d51864428e6d7cf493f88bbee13b5203774b
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---

# Hantera [!DNL Adobe Workfront] meddelanden i [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>När [Microsoft övergår till New Teams-klienten](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) är Classic Teams-klienten inte längre tillgänglig efter 1 juli 2025. För att kunna fortsätta använda Microsoft Teams och integrerade program som Workfront måste kunderna gå över till nya Teams-klienten före detta datum.
>
>Den uppdaterade Workfront-integreringen är nu tillgänglig och helt kompatibel med New Teams. I de flesta fall visas Workfront automatiskt när användaren har gått över. Om så inte är fallet kan integreringen installeras manuellt från Microsoft Teams App Store. Information om hur du installerar eller verifierar Workfront-integreringen i klienten New Teams finns i [Installera [!DNL Adobe Workfront] för Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

Du kan få meddelanden från [!DNL Adobe Workfront] om objekt som du måste godkänna, uppdrag som du har fått eller kommentarer och ändringar i objekt som du är kopplad till.

De här meddelandena innehåller [!DNL Workfront] åtgärder som du kan vidta inom [!DNL Microsoft Teams] utan att navigera bort från [!DNL Microsoft Teams] för att slutföra dem.

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Om du vill använda [!DNL Adobe Workfront for Microsoft Teams integration] måste du använda en annan webbläsare än [!DNL Internet Explorer].




## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Arbeta eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Krav för att ta emot [!DNL Workfront] meddelanden i [!DNL Microsoft Teams]

Du kan ta emot [!DNL Workfront] meddelanden i [!DNL Microsoft Teams] om följande villkor uppfylls:

* En teamägare har installerat och konfigurerat [!DNL Workfront for Microsoft Teams] för ditt team.
* Du är inloggad på [!DNL Workfront] från [!DNL Microsoft Teams].
* Du har aktiverat snabbmeddelanden i [!DNL Workfront]. Information om hur du aktiverar snabbmeddelanden finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Information om hur du installerar [!DNL Workfront for Microsoft Teams] och loggar in på [!DNL Workfront from Microsoft Teams] finns i [Installera [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Hantera [!DNL Workfront] meddelanden i [!DNL Microsoft Teams]

När appen [!DNL Workfront for Microsoft Teams] installeras skapas en [!DNL Workfront] chattkanal i [!DNL Microsoft Teams] för varje medlem i det teamet. När en viss åtgärd utförs i [!DNL Workfront] kan du konfigurera inställningarna för att [!DNL Workfront for Microsoft Teams] ska få meddelanden om den åtgärden i [!DNL Workfront] chattkanalen i [!DNL Microsoft Teams].

Tänk på följande när du arbetar med [!DNL Workfront] meddelanden från [!DNL Microsoft Teams]:

* Du kan inte ta emot alla, men bara ett visst antal [!DNL Workfront] meddelanden i [!DNL Microsoft Teams].
* Alla meddelanden som du får från [!DNL Workfront] visas i chattkanalen [!DNL Workfront].

  Information om hur du installerar robotkanalen [!DNL Workfront] finns i avsnittet [Logga in på [!DNL Workfront] från [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) i artikeln [Installera [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

* Det kan dröja upp till fem minuter mellan den tidpunkt då en uppdatering görs i [!DNL Workfront] och den tidpunkt då du får ett meddelande om den i [!DNL Microsoft Teams].
* Du får även ett e-postmeddelande för varje [!DNL Microsoft Teams]-meddelande.

Så här hanterar du [!DNL Workfront]-meddelanden som du kan ta emot i [!DNL Microsoft Teams]:

1. Klicka på ikonen **[!UICONTROL More added]** (tre punkter) appar i det vänstra navigeringsfältet i [!DNL Microsoft Teams].

1. Klicka på [!DNL Workfront] i listan som visas.
1. Klicka på fliken **[!UICONTROL Settings]**.  

   ![Inställningsfliken för MS Teams](assets/ms-teams-settings-tab-350x552.png)

1. Inaktivera alla meddelanden som du inte vill ta emot. Du kan aktivera eller inaktivera grupper av meddelanden, till exempel informations- eller godkännandemeddelanden, eller så kan du hantera meddelanden individuellt.

   Alla meddelanden är aktiverade som standard.

   Meddelandeinställningarna för [!DNL Workfront for Microsoft] team sparas automatiskt.

   >[!NOTE]
   >
   >Du kan inte lägga till fler meddelanden till de som är tillgängliga som standard.

## Svara på [!DNL Workfront] aviseringar och godkännandebegäranden i [!DNL Microsoft Teams]

1. Logga in på [!DNL Workfront] från [!DNL Microsoft Teams].\
   Mer information om hur du loggar in på [!DNL Workfront] finns i [Installera [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Gå till området **[!UICONTROL Chat]** och klicka på robotkanalen **[!DNL Workfront]**.\
   Den här kanalen är till för din personliga chatt med roboten [!DNL Workfront]. Alla [!DNL Workfront]-meddelanden visas här.
1. Beroende på vilken typ av meddelande du får går du vidare till relevant avsnitt:

   * [Godkännandemeddelanden](#approval-notifications-approval-notifications)
   * [Uppdragsmeddelanden](#assignment-notifications-assignment-notifications)
   * [Kommentarsmeddelanden](#comment-notifications-comment-notifications)
   * [Uppdatera meddelanden](#update-notifications-update-notifications)
   * [Meddelanden om datumändring](#date-change-notifications-date-change-notifications)

### Godkännandemeddelanden {#approval-notifications}

Du får godkännandemeddelanden när du ombeds godkänna ett objekt, som en uppgift, tidrapport eller korrektur. Du kan dock fortfarande kommentera meddelandet.Från godkännandemeddelandet kan du utföra följande åtgärder:

* **[!UICONTROL Approve]**: Klicka för att godkänna objektet.
* **[!UICONTROL Change]**: Klicka för att godkänna objektet med ändringar.
* **[!UICONTROL Reject]**: Klicka för att avvisa objektet.
* **[!UICONTROL Comment]**: Klicka för att göra en kommentar. Din kommentar visas också i [!DNL Workfront] som en uppdatering av objektet som meddelandet gäller.
* **[!UICONTROL Go to Proof]**: Klicka för att öppna korrekturet. Du kan sedan fatta ett beslut direkt i beviset. Mer information finns i [Ta beslut om ett korrektur i korrekturläsaren](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>När du väl har fattat ett beslut om godkännande kan du inte ändra det från meddelandet.

#### Tillgängliga åtgärder för specifika godkännandemeddelanden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Meddelande</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Go to Proof] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Du måste godkänna ett projekt</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Du måste godkänna en uppgift</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Du måste godkänna ett ärende</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Du måste godkänna ett dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Du måste godkänna åtkomst till ett objekt</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Du måste godkänna en tidrapport</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Någon vill att du ska godkänna det här beviset</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Din tidrapport har avvisats</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Din tidrapport öppnas igen</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">En begäran om dokumentgodkännande som du har begärt godkänns*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">En begäran om dokumentgodkännande som du har begärt godkänns med ändringar*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">En begäran om dokumentgodkännande som du har begärt avvisas*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Din tidrapport är godkänd</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Dessa meddelanden avser godkännanden av äldre dokument. Meddelanden om enhetliga dokumentgodkännanden stöds för närvarande inte i [!DNL Microsoft Teams]. Mer information om de olika godkännandesystemen i Workfront finns i [Tillgänglig funktion för dokumentgodkännanden](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).

### Uppdragsmeddelanden {#assignment-notifications}

Du får tilldelningsmeddelanden när du, eller ett team du är på, tilldelas en uppgift eller ett problem i Workfront. Från tilldelningsmeddelandet kan du utföra följande åtgärder:

* **[!UICONTROL Work on it]**: Välj att implementera för att arbeta med objektet. Ett kort meddelande visas som bekräftar att ett nytt objekt har lagts till i din arbetslista.
* **[!UICONTROL View in [!DNL Workfront]]**: Välj det här alternativet om du vill visa den tilldelade utgåvan eller uppgiften i Workfront, som öppnar en ny flik.
* **[!UICONTROL Start]**: Klicka för att börja arbeta med objektet. Ett kort meddelande visas som bekräftar att ett nytt objekt har lagts till i din arbetslista.
* **[!UICONTROL Comment]**: Klicka för att kommentera objektet. Din kommentar visas också i objektets uppdateringsström i Workfront.
* **[!UICONTROL Status]**: Klicka och välj sedan den nya statusen för arbetsobjektet i listrutan.

#### Tillgängliga åtgärder för specifika tilldelningsmeddelanden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Meddelande</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Du har tilldelats en uppgift</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Du har tilldelats en utgåva</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ett team som du är tilldelad får en arbetsförfrågan för en uppgift</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ett team som du är tilldelad får en arbetsförfrågan om ett problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Kommentarsmeddelanden {#comment-notifications}

Du får ett kommunikationsmeddelande när någon kommenterar ett objekt som du är kopplad till, eller inkluderar dig i en uppdatering. I kommunikationsmeddelandet kan du utföra följande åtgärder:

* **Svaraly**: Klicka för att svara på kommentaren eller [!UICONTROL update]. Ditt svar visas också i uppdateringsströmmen där kommentaren visas i Workfront.
* **[!UICONTROL View in Workfront]**: Välj det här alternativet om du vill visa kommentaren och objektet i Workfront, som öppnas på en ny flik.
* **[!UICONTROL Status]**: Klicka och välj sedan en ny status för det arbetsobjekt som kommentaren eller uppdateringen gäller.

#### Tillgängliga åtgärder för specifika kommunikationsmeddelanden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Meddelande</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">En kommentar har lagts till på din begäran</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ett svar har skickats på din arbetsförfrågan</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Någon kommenterar en tråd som du är i</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Någon kommenterar något av dina arbetsobjekt</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Någon kommenterar i en tidrapport som du godkänner</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">En kommentar läggs till på din användarprofilsida eller genom att flera användare redigeras gruppvis</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">En kommentar läggs till i en av dina uppdateringar</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">En kommentar läggs till i din tidrapport</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Uppdatera meddelanden {#update-notifications}

Du får ett informationsmeddelande när det finns en uppdatering av ett objekt som du är kopplad till, men du behöver inte vidta några åtgärder för objektet. Från informationsmeddelandet kan du utföra följande åtgärder:

* **[!UICONTROL Reply]**: Klicka för att svara på [!UICONTROL update]. Ditt svar visas också i objektets uppdateringsström i Workfront.
* **Visa i Workfront**: Välj det här alternativet om du vill visa kommentaren och objektet i Workfront, som öppnas på en ny flik.
* **[!UICONTROL Status]**: Klicka och välj sedan den nya statusen för objektet i listrutan.

#### Tillgängliga åtgärder för specifika informationsmeddelanden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Meddelande</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">En uppdatering görs av en aktivitet, ett problem eller ett projekt som du prenumererar på</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Någon inkluderar dig i en dirigerad uppdatering</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Någon inkluderar ditt team på en [!UICONTROL directed update]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Meddelanden om datumändring {#date-change-notifications}

Du får ett meddelande om datumändring när datumet ändras för en arbetsuppgift som du har tilldelats. Du kan utföra följande åtgärder från meddelandet om datumändring.

* **[!UICONTROL Comment]**: Klicka för att kommentera objektet. Din kommentar visas också i objektets uppdateringsström i Workfront.
* **[!UICONTROL Status]**: Klicka och välj sedan den nya statusen för arbetsobjektet i listrutan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Meddelande</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Förfallodatumet ändras för en uppgift som du har tilldelats till</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

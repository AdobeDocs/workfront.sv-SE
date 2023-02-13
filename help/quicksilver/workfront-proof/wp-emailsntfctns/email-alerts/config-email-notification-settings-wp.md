---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Konfigurera e-postaviseringsinställningar i [!DNL Workfront Proof]
description: E-postmeddelanden informerar medarbetare om den senaste aktiviteten i korrektur, som kommentarer, svar, beslut.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1814'
ht-degree: 0%

---

# Konfigurera e-postaviseringsinställningar i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

E-postmeddelanden informerar medarbetare om den senaste aktiviteten i korrektur, som kommentarer, svar, beslut.

E-postmeddelanden till granskarna kan anges på sidan Nytt korrektur. [!UICONTROL New version] och hanteras i [!UICONTROL Workflow] i [!UICONTROL Proof details] sida. Mer information finns i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Alla användare kan också ange egna e-postaviseringsinställningar som automatiskt tillämpas när ett korrektur delas med dem. Om medarbetarna har sina inställningar, eller kontoadministratörerna har sina rekommendationer om hur ofta aviseringar ska göras. Detta kan anges som korrekturstandard på användarnas informationssidor.

>[!NOTE]
>
>De här inställningarna föreslås när användare skapar korrektur och lägger till dessa medarbetare. Det här är dock bara förslag, så de kan justeras när som helst under granskningsprocessen och ändringarna gäller för alla aktiviteter som görs efter ändringen. Korrekturinställningarna åsidosätts av inställningarna på korrekturnivå.

Användare med [!UICONTROL Administrator] eller [!UICONTROL Billing Administrator] profiler kan också ange korrekturinställningar för andra användare på deras konto inifrån kontoinställningarna.

Mer information om profiler finns i [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Konfigurera korrekturinställningar i personliga inställningar ([!DNL Workfront Proof] endast användare)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [Ändra e-postaviseringar för en mottagare](#change-email-alerts-for-a-recipient)
* [Konfigurera korrekturinställningar för en användare](#configure-proof-defaults-for-a-user)

## Konfigurera korrekturinställningar i personliga inställningar ([!DNL Workfront Proof] endast användare)

Du kan konfigurera korrekturinställningar för korrektur som du skapar.

Information om korrekturinställningar finns i [!DNL Workfront] administratör eller [!DNL Workfront Proof] -administratören kan konfigurera, se .

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**.

1. Klicka på **[!UICONTROL Proofing defaults]** -fliken.
1. Klicka **[!UICONTROL Default email notification settings]** för att utöka den.
1. I listrutan till höger om följande två inställningar väljer du ett av alternativen som förklaras i tabellen nedan.

   * **[!UICONTROL Default email alert]**: Påverkar alla korrektur som delas med dig. Den här inställningen kan åsidosättas på korrekturnivån.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Påverkar granskare som inte tidigare fanns som kontakter i ditt konto.

   >[!NOTE]
   >
   >Om du inte väljer något av följande alternativ [!DNL Workfront Proof] skickar dig en daglig sammanfattning av aktiviteten på dina korrektur.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront] skickar ett e-postmeddelande till granskaren varje gång det finns någon aktivitet i korrekturet, t.ex. en ny kommentar, ett svar eller ett beslut. <p>Detta är ett bra alternativ för den som hanterar korrekturläsningen eftersom det gör att personen kan se aktiviteten som den är. </p><p>Användarna får ingen e-postavisering om sin egen aktivitet.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Replies to my comments]</td> 
      <td>Ett e-postmeddelande skickas till granskaren endast om någon uttryckligen svarar på kommentaren (detta utesluter att personen själv svarar på sina kommentarer). Det innebär att om någon i korrekturet gör en ny kommentar så meddelas inte granskaren.<p>Den här inställningen rekommenderas för dina kunder på korrekturet så att de inte meddelas om några andra kommentarer på korrekturet och endast får svar på sina egna kommentarer.</p><p>Även om granskare med den här e-postaviseringsinställningen inte meddelas om andra nya kommentarer, kan de fortfarande visa alla kommentarer i korrekturläsaren.</p><p>Mer information om kommentarer finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visa och svara på korrekturkommentarer</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] skickar ett e-postmeddelande till granskaren endast när någon fattar ett beslut.<p>Detta kan vara användbart för den som hanterar godkännandeprocessen (t.ex. en projektledare) och måste övervaka korrekturets förlopp och se vilka användare som har fattat sitt beslut.</p><p>Du meddelas inte om ditt eget beslut såvida du inte väljer ett bekräftelsealternativ för e-post när du skickar ditt beslut.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Final decision]</td> 
      <td>[!DNL Workfront] skickar ett e-postmeddelande när den sista godkännaren på beviset har fattat sitt beslut.<p>Den här varningen används ofta av designern som vanligtvis inte behöver delta i själva granskningsdiskussionen. När det slutliga beslutet fattas meddelas formgivaren och kan sedan vidta eventuella nödvändiga åtgärder.</p><p>Den här varningen kan även vara användbar för en avdelningsledare som behöver få ett meddelande endast när granskningsprocessen är klar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly Summary]</td> 
      <td>[!DNL Workfront] skickar ett e-postmeddelande till granskaren varje timme med en sammanfattning av alla kommentarer, svar och beslut som har fattats inom en timme.<p>E-postmeddelandet skickas bara när andra aktiviteter än din egen inträffar under den senaste timmen. </p><p>Den här varningen är ett bra sätt att se en översikt över projektet.</p><p>Ett exempel på hur man kan använda den här sammanfattningen är en erfaren granskare som behöver en översikt över projektet, men som inte behöver underrättas omedelbart om all aktivitet på beviset.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Daily Summary]</td> 
      <td>[!DNL Workfront] skickar ett e-postmeddelande med alla kommentarer, svar och beslut listade endast dagar när det finns aktiviteter utöver din egen.<p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.</p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.</p><p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Hantera meddelanden för korrekturkommentarer och beslut</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] skickar inga e-postaviseringar.<br>Detta är användbart för en person som endast läggs till i ett korrektur för referens och som inte behöver underrättas om några ändringar.<p>Systemstandard är [!UICONTROL Daily summary] (ses även som [!UICONTROL Not Set]). Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ändra något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Ange om du vill få en [!UICONTROL Proof made] e-post när du skapar ett korrektur. Mer information finns i <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The [!UICONTROL Proof Made] e-post</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Format of emails sent to me]</strong> </td> 
      <td> <p>Välj mellan e-postmeddelanden med HTML och e-postmeddelanden med vanlig text. </p> <p>Obs!  Standardinställningarna för korrektur åsidosätts av inställningarna på korrekturnivå. Om korrekturmeddelanden via e-post inaktiveras för hela kontot i [!UICONTROL Account] inställningar skickas inga e-postaviseringar till medarbetarna även om [!UICONTROL Disabled email alert] är inte markerat på korrektur.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Under **[!UICONTROL Message settings]**&#x200B;ändrar du något av följande:

   | **[!UICONTROL Proof subject template]** | Visas på sidan Nytt korrektur, Ny version, Meddelande och Påminn. Kan redigeras innan det skickas. |
   |---|---|
   | **[!UICONTROL Proof message template]** | Visas på sidan Nytt korrektur, Ny version, Meddelande och Påminn. Kan redigeras innan det skickas. |

   {style=&quot;table-layout:auto&quot;}

## Ändra e-postaviseringar för en mottagare

Du kan ändra e-postaviseringar för en viss mottagare i en gruppåtgärd.

1. Klicka **[!UICONTROL Contacts]** i den vänstra navigeringspanelen.
1. Klicka på **[!UICONTROL More]** (tre punkter) för mottagaren och klicka sedan på **[!UICONTROL View member details]** i listrutan.

1. Öppna **[!UICONTROL Shared items]** -avsnitt.
1. Markera kryssrutan till vänster om varje objekt som du vill ändra e-postaviseringen för.
1. Klicka **[!UICONTROL More]** ovanför listan med delade objekt och klicka sedan på **[!UICONTROL Change email alert]** i listrutan.

1. Ändra e-postaviseringen och klicka sedan på **[!UICONTROL Submit]**.

## Konfigurera korrekturinställningar för en användare

Om du är en [!DNL Workfront Proof] kan du ange standardvärden för korrektur för användare i ditt konto.

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account settings]**.

1. Öppna **[!UICONTROL Users]** -fliken.
1. Öppna **[!UICONTROL  More]** till höger om användarens namn. ![More_button_small.png](assets/more-button-small.png)

1. Klicka **[!UICONTROL View users details]** i listrutan.
1. Under **[!UICONTROL Settings]**, klicka **[!UICONTROL Default email alert settings]** för att utöka den.

1. Välj ett av alternativen i tabellen nedan i listrutan till höger om följande två inställningar:

   * **[!UICONTROL Default email alert]**: Påverkar alla korrektur som delas med dig. Den här inställningen kan åsidosättas på korrekturnivån.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Påverkar granskare som inte tidigare fanns som kontakter i ditt konto.

   >[!NOTE]
   >
   >Om du inte väljer något av följande alternativ för en användare, [!DNL Workfront Proof] skickar en daglig sammanfattning om aktiviteten till sina korrektur.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] skickar ett e-postmeddelande till granskaren varje gång det finns någon aktivitet i korrekturet, t.ex. en ny kommentar, ett svar eller ett beslut. <p>Detta är ett bra alternativ för den som hanterar korrekturläsningen eftersom det gör att personen kan se aktiviteten som den är. </p><p>Användarna får ingen e-postavisering om sin egen aktivitet.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Replies to my comments]</td>
      <td>Ett e-postmeddelande skickas till granskaren endast om någon uttryckligen svarar på kommentaren (detta utesluter att personen själv svarar på sina kommentarer). Det innebär att om någon i korrekturet gör en ny kommentar så meddelas inte granskaren.<p>Den här inställningen rekommenderas för dina kunder på korrekturet så att de inte meddelas om några andra kommentarer på korrekturet och endast får svar på sina egna kommentarer.</p><p>Även om granskare med den här e-postaviseringsinställningen inte meddelas om andra nya kommentarer, kan de fortfarande visa alla kommentarer i korrekturläsaren.</p><p>Mer information om kommentarer finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visa och svara på korrekturkommentarer</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] skickar ett e-postmeddelande till granskaren endast när någon fattar ett beslut.<p>Detta kan vara användbart för den som hanterar godkännandeprocessen (t.ex. en projektledare) och måste övervaka korrekturets förlopp och se vilka användare som har fattat sitt beslut.</p><p>Du meddelas inte om ditt eget beslut såvida du inte väljer ett bekräftelsealternativ för e-post när du skickar ditt beslut.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Final decision]</td>
      <td>[!DNL Workfront] skickar ett e-postmeddelande när den sista godkännaren på beviset har fattat sitt beslut.<p>Den här varningen används ofta av designern som vanligtvis inte behöver delta i själva granskningsdiskussionen. När det slutliga beslutet fattas meddelas formgivaren och kan sedan vidta eventuella nödvändiga åtgärder.</p><p>Den här varningen kan även vara användbar för en avdelningsledare som behöver få ett meddelande endast när granskningsprocessen är klar.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Hourly Summary]</td>
      <td>[!DNL Workfront] skickar ett e-postmeddelande till granskaren varje timme med en sammanfattning av alla kommentarer, svar och beslut som har fattats inom en timme.<p>E-postmeddelandet skickas bara när andra aktiviteter än din egen inträffar under den senaste timmen. </p><p>Den här varningen är ett bra sätt att se en översikt över projektet.</p><p>Ett exempel på hur man kan använda den här sammanfattningen är en erfaren granskare som behöver en översikt över projektet, men som inte behöver underrättas omedelbart om all aktivitet på beviset.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Daily Summary]</td>
      <td>[!DNL Workfront] skickar ett e-postmeddelande med alla kommentarer, svar och beslut listade endast dagar när det finns aktiviteter utöver din egen.<p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.</p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.</p><p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Hantera meddelanden för korrekturkommentarer och beslut</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] skickar inga e-postaviseringar.<br>Detta är användbart för en person som endast läggs till i ett korrektur för referens och som inte behöver underrättas om några ändringar.<p>Systemstandard är [!UICONTROL Daily summary] (ses även som [!UICONTROL Not Set]). Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.</p></td>
     </tr>
    </tbody>
   </table>

1. I de övriga **[!UICONTROL Default email alert settings]**&#x200B;ändrar du något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Ange om du vill få en [!UICONTROL Proof made] e-post när du skapar ett korrektur. Mer information finns i <a href="https://support.workfront.com/hc/en-us/article">The [!UICONTROL Proof Made] E-post.</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Format of emails sent to me]</strong> </td> 
      <td> <p>Välj mellan e-postmeddelanden med HTML och e-postmeddelanden med vanlig text. </p> <p>Obs!  Standardinställningarna för korrektur åsidosätts av inställningarna på korrekturnivå. Om korrekturmeddelanden via e-post inaktiveras för hela kontot i [!UICONTROL Account] inställningar skickas inga e-postaviseringar till medarbetarna även om [!UICONTROL Disabled email alert] är inte markerat på korrektur.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Konfigurera e-postaviseringsinställningar i  [!DNL Workfront Proof]
description: E-postmeddelanden som genererats från Workfront Proof informerar medarbetarna om den senaste aktiviteten i korrektur, som kommentarer, svar eller beslut.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '1878'
ht-degree: 0%

---

# Konfigurera e-postmeddelandeinställningar i [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

E-postmeddelanden informerar medarbetare om den senaste aktiviteten i korrektur, som kommentarer, svar eller beslut.

Du kan ange e-postmeddelanden för granskare inom följande områden:

E-postmeddelanden för granskare kan anges på sidan Nytt korrektur, sidan [!UICONTROL New version], och hanteras i avsnittet [!UICONTROL Workflow] på sidan [!UICONTROL Proof details]. Mer information finns i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* Sidan Nytt korrektur
* Sidan [!UICONTROL New version]
* Avsnittet [!UICONTROL Workflow] på sidan [!UICONTROL Proof details].

Mer information finns i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Alla användare kan också ange egna e-postaviseringsinställningar som automatiskt tillämpas när ett korrektur delas med dem om medarbetarna har sina inställningar eller kontoadministratörer har sina rekommendationer om hur ofta aviseringar ska göras. Detta kan anges som korrekturstandard på användarnas informationssidor.

Alla användare kan också ange egna e-postaviseringsinställningar som automatiskt tillämpas när ett korrektur delas med dem. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>De här inställningarna föreslås när användare skapar korrektur och lägger till dessa medarbetare. Det här är dock bara förslag, så de kan justeras när som helst under granskningsprocessen och ändringarna gäller för alla aktiviteter som görs efter ändringen. Korrekturinställningarna åsidosätts av inställningarna på korrekturnivå.

Användare med [!UICONTROL Administrator]- eller [!UICONTROL Billing Administrator]-profiler kan också ange korrekturinställningar för andra användare i sina konton inifrån kontoinställningarna.

Mer information om profiler finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Produkt</td> 
   <td>Fristående Workfront Proof</td> 
  </tr> 
</table>

+++

## Konfigurera korrekturinställningar i personliga inställningar ([!DNL Workfront Proof] användare endast)

Du kan konfigurera korrekturinställningar för korrektur som du skapar.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Klicka på din profilbild i det övre högra hörnet och klicka sedan på **[!UICONTROL Personal settings]**.

1. Klicka på fliken **[!UICONTROL Proofing defaults]**.
1. Klicka på **[!UICONTROL Default email notification settings]** för att expandera den.
1. I listrutan till höger om följande två inställningar väljer du ett av alternativen som förklaras i tabellen nedan.

   * **[!UICONTROL Default email alert]**: Påverkar alla korrektur som delas med dig. Den här inställningen kan åsidosättas på korrekturnivån.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Påverkar granskare som inte tidigare fanns som kontakter i ditt konto.

   >[!NOTE]
   >
   >Om du inte väljer något av följande alternativ skickar [!DNL Workfront Proof] dig en daglig sammanfattning om aktiviteten på dina korrektur.

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
      <td>[!DNL Workfront] skickar ett e-postmeddelande med alla kommentarer, svar och beslut listade endast dagar när det finns aktiviteter utöver din egen.<p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.</p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.</p><p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Hantera meddelanden om korrekturkommentarer och beslut</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] skickar inga e-postaviseringar.<br>Det här är användbart för en person som bara läggs till i ett korrektur för referens och som inte behöver informeras om några ändringar.<p>Systemstandard är [!UICONTROL Daily summary] (visas även som [!UICONTROL Not Set]). Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.</p></td> 
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
      <td>Ange om du vill få ett [!UICONTROL Proof made]-e-postmeddelande när du skapar ett korrektur. Mer information finns i <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-postmeddelandet [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>Välj mellan e-postmeddelanden med HTML och e-postmeddelanden med vanlig text. </p> <p><b>ANMÄRKNING</b></p>
      <p>Standardinställningarna för korrektur åsidosätts av inställningarna på korrekturnivå. Om korrekturmeddelanden via e-post inaktiveras för hela kontot i inställningarna för [!UICONTROL Account] skickas inga e-postaviseringar till medarbetarna, även om [!UICONTROL Disabled email alert] inte har valts för korrektur.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ändra något av följande under **[!UICONTROL Message settings]**:

   | Korrekturmall | Beskrivning |
   |---|---|
   | **[!UICONTROL Proof subject template]** | Visas på sidan Nytt korrektur, Ny version, Meddelande och Påminn. Kan redigeras innan det skickas. |
   | **[!UICONTROL Proof message template]** | Visas på sidan Nytt korrektur, Ny version, Meddelande och Påminn. Kan redigeras innan det skickas. |

## Ändra e-postaviseringar för en mottagare

Du kan ändra e-postaviseringar för en viss mottagare i en gruppåtgärd.

1. Klicka på **[!UICONTROL Contacts]** i den vänstra navigeringspanelen.
1. Klicka på **[!UICONTROL More]**-menyn ![Mer meny](assets/more-button-small.png) för mottagaren och klicka sedan på **[!UICONTROL View member details]** i listrutan.

1. Öppna avsnittet **[!UICONTROL Shared items]**.
1. Markera kryssrutan till vänster om varje objekt som du vill ändra e-postaviseringen för.
1. Klicka på **[!UICONTROL More]** ovanför listan med delade objekt och klicka sedan på **[!UICONTROL Change email alert]** i listrutan.

1. Ändra e-postaviseringen och klicka sedan på **[!UICONTROL Submit]**.

## Konfigurera korrekturinställningar för en användare

Om du är [!DNL Workfront Proof]-administratör kan du ange standardvärden för korrektur för användare i ditt konto.

1. Klicka på **[!UICONTROL Account settings]** högst upp på skärmen.

1. Öppna fliken **[!UICONTROL Users]**.
1. Öppna **[!UICONTROL  More]**-menyn ![More_button_small.png](assets/more-button-small.png) till höger om användarens namn.

1. Klicka på **[!UICONTROL View users details]** i listrutan.
1. Klicka på **[!UICONTROL Default email alert settings]** under **[!UICONTROL Settings]** för att expandera den.

1. Välj ett av alternativen som förklaras i tabellen nedan i listrutan till höger om följande två inställningar:

   * **[!UICONTROL Default email alert]**: Påverkar alla korrektur som delas med dig. Den här inställningen kan åsidosättas på korrekturnivån.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Påverkar granskare som inte tidigare fanns som kontakter i ditt konto.

   >[!NOTE]
   >
   >Om du inte väljer något av följande alternativ för en användare skickar [!DNL Workfront Proof] en daglig sammanfattning om aktiviteten på sina korrektur till användarna.

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
      <td>[!DNL Workfront] skickar ett e-postmeddelande med alla kommentarer, svar och beslut listade endast dagar när det finns aktiviteter utöver din egen.<p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.</p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.</p><p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Hantera meddelanden om korrekturkommentarer och beslut</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] skickar inga e-postaviseringar.<br>Det här är användbart för en person som bara läggs till i ett korrektur för referens och som inte behöver informeras om några ändringar.<p>Systemstandard är [!UICONTROL Daily summary] (visas även som [!UICONTROL Not Set]). Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.</p></td>
     </tr>
    </tbody>
   </table>

1. Ändra något av följande i återstående **[!UICONTROL Default email alert settings]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Ange om du vill få ett [!UICONTROL Proof made]-e-postmeddelande när du skapar ett korrektur. Mer information finns i <a href="https://support.workfront.com/hc/en-us/article">E-postmeddelandet [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>Välj mellan e-postmeddelanden med HTML och e-postmeddelanden med vanlig text. </p> <p><b>ANMÄRKNING</b></p> <p>Standardinställningarna för korrektur åsidosätts av inställningarna på korrekturnivå. Om korrekturmeddelanden via e-post inaktiveras för hela kontot i inställningarna för [!UICONTROL Account] skickas inga e-postaviseringar till medarbetarna, även om [!UICONTROL Disabled email alert] inte har valts för korrektur.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

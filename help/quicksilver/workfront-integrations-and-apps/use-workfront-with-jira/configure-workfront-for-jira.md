---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Konfigurera [!DNL Adobe Workfront for Jira]
description: Du kan använda  [!DNL Adobe Workfront for Jira] för att integrera dina [!DNL Jira] och [!DNL Workfront] system.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '2292'
ht-degree: 0%

---

# Konfigurera [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen kommer integreringen av Workfront för Jira inte att vara tillgänglig efter **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Jira.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration Module för Jira finns i [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Du kan använda [!DNL Adobe Workfront for Jira] för att integrera dina [!DNL Jira]- och [!DNL Workfront]-system.

När du har installerat tillägget kan du definiera arbetsflöden som skapar [!DNL Jira] utgåvor automatiskt när [!DNL Workfront] arbetsobjekt skapas. Objekten i båda programmen länkas och en del av deras information uppdateras automatiskt i båda systemen.

Alla användare i [!DNL Workfront] och [!DNL Jira] kan dra nytta av den här integreringen. De behöver bara en licens för det system där de arbetar mest, inte för båda systemen.

Det här tillägget är tillgängligt för både [!UICONTROL Server]- och [!UICONTROL OnDemand]- (eller [!UICONTROL Cloud]) versionerna av programvaran [!DNL Jira].

En lista över [!DNL Jira] versioner som [!DNL Workfront for Jira] har stöd för finns på [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) på [!DNL Atlassian Marketplace].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira-åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt: Vi rekommenderar att du skapar separata systemadministratörskonton i Jira och Workfront för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan konfigurera [!DNL Workfront for Jira] måste du:

* Installera [!DNL Workfront for Jira].
Instruktioner om hur du installerar [!DNL Workfront for Jira] finns i [Installera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Konfigurera [!DNL Workfront for Jira]

Genom att konfigurera [!DNL Workfront for Jira] kan du:

* Definiera utlösare som skapar [!DNL Jira] objekt när [!DNL Workfront] objekt skapas.
* Ange vilka fält som ska synkroniseras mellan objekt länkade mellan [!DNL Jira] och [!DNL Workfront].

>[!NOTE]
>
>* När du har konfigurerat [!DNL Workfront for Jira] i [!DNL Jira]-miljön visas en [!DNL Jira] högerpanel för alla [!DNL Workfront]-objekt för alla [!DNL Jira]-användare. Panelen innehåller information om objekt som kan vara länkade från [!DNL Workfront] eller anger att inga [!DNL Workfront]-objekt är länkade till [!DNL Jira]-objekt.
>* När du använder installationen av [!DNL Jira Server] visas endast de problem som är kopplade till projekt som identifieras som utlösare för Workfront-integreringen på Workfront-panelen. Mer information om hur du ställer in utlösare för arbetsflödet [!DNL Workfront to Jira] finns i [Konfigurera utlösare för automatisk länkning av objekt mellan  [!DNL Jira]  och [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Konfigurera [!DNL Workfront for Jira]:

1. Logga in på [!DNL Jira] som [!DNL Jira]-administratör.
1. Klicka på **[!UICONTROL Settings]** i huvudmenyn för [!DNL Jira].
1. Klicka på **[!UICONTROL Add-ons]** och sedan på **[!UICONTROL Manage add-ons]**.

1. Expandera tillägget **[!DNL Workfront]**.
1. Klicka på **[!UICONTROL Configure]**.
1. Logga in på [!DNL Workfront] genom att följa anvisningarna.

   >[!NOTE]
   >
   >Användaren måste ha en giltig `apiKey` i [!UICONTROL Workfront] för att kunna skapa en lyckad anslutning.

   Du måste logga in på [!DNL Workfront] som [!DNL Workfront]-administratör för att kunna fortsätta med konfigurationen.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] ansluter till [!DNL Jira] med OAuth 2.0, en standard som används av de flesta webbaserade integreringar för autentisering och auktorisering av användare.
   >* När du uppmanas att ange domänen för ditt [!DNL Workfront]-konto skriver du den i det här formatet: *ditt företags sDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.
   >* Förbättrad autentisering är inte tillgängligt förrän en [!DNL Workfront]-administratör har aktiverat den för den här integreringen.

1. I Jira väljer du fliken **[!UICONTROL Triggers]** för att konfigurera det automatiska skapandet av [!DNL Jira] objekt när nya [!DNL Workfront] objekt skapas.

   Mer information om hur du konfigurerar utlösare för arbetsflödet Workfront till [!DNL Jira] finns i [Konfigurera utlösare för automatisk länkning av objekt mellan  [!DNL Jira]  och [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Välj fliken **[!UICONTROL Setup]** för att konfigurera synkroniseringen av fält mellan länkade [!DNL Jira]- och [!DNL Workfront]-objekt.

   Mer information om hur du konfigurerar synkroniseringen av fält mellan [!DNL Jira] och [!DNL Workfront] finns i [Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] objekt](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >När du har definierat utlösarna och synkroniseringen av fält mellan de två programmen kan alla [!DNL Workfront]-användare som kan skapa aktiviteter eller problem potentiellt utlösa skapandet av ett objekt i [!DNL Jira]. Användaren kan skapa ett objekt om villkoren för det objekt som de skapar matchar utlösarna i [!DNL Jira], även om användaren inte har någon [!DNL Jira]-licens. Alla [!DNL Jira]-användare kan också börja arbeta med [!DNL Jira]-objektet omedelbart, och deras uppdateringar visas i [!DNL Workfront], utan att de har en [!DNL Workfront]-licens. Alla uppdateringar i [!DNL Workfront] visas också för [!DNL Jira]-objekten.

1. (Valfritt) Välj fliken **[!UICONTROL Activity Log]** om du vill granska eventuella fel som kan ha inträffat under integreringen.

   Mer information om [!UICONTROL Activity Log] finns i [Visa  [!DNL Jira] [!UICONTROL Activity Log]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Konfigurera utlösare för automatisk länkning av objekt mellan [!DNL Jira] och [!DNL Workfront]

Som [!DNL Jira]-systemadministratör kan du definiera utlösare som automatiskt skapar problem i [!DNL Jira] när ett objekt i [!DNL Workfront] uppfyller vissa villkor.

>[!NOTE]
>
>Det kan ta upp till 10 minuter för integreringen att skapa nya utgåvor i [!DNL Jira].

Tänk på följande när du konfigurerar att aktivera skapandet av [!DNL Jira] objekt när [!DNL Workfront] objekt skapas:

* Integrationen är enkelriktad: Du kan bara utlösa objekt som du skapar i [!DNL Workfront] som automatiskt skapas i [!DNL Jira]. Du kan inte utlösa objekt som du skapar i [!DNL Jira] som automatiskt skapas i [!DNL Workfront].
* Det finns ingen gräns för hur många utlösare du kan ha.
* Om ett objekt som du skapar i [!DNL Workfront] matchar fler än en av utlösarna skapas bara ett objekt i [!DNL Jira]. Objektet skapas i [!DNL Jira] enligt den första utlösaren (i den ordning som de har definierats i [!DNL Jira]). Alla andra utlösare ignoreras.
* Endast ett objekt i [!DNL Workfront] kan länkas till ett objekt i Jira. Du kan aldrig länka ett [!DNL Workfront]-objekt till flera [!DNL Jira]-utgåvor eller ett [!DNL Jira]-problem till flera [!DNL Workfront]-objekt.

Så här konfigurerar du utlösare för att automatiskt skapa objekt i [!DNL Jira]:

1. Logga in på [!DNL Jira] som systemadministratör.
1. Klicka på **[!UICONTROL Settings]** i huvudmenyn för [!DNL Jira].
1. Klicka på **[!UICONTROL Add-ons]** och sedan på **[!UICONTROL Manage add-ons]**.
1. Expandera tillägget **[!DNL Workfront]**.
1. Klicka på **[!UICONTROL Configure]**.
1. Logga in på [!DNL Workfront] som systemadministratör.

   Fliken **[!UICONTROL Triggers]** är markerad som standard i Jira.

1. Klicka på **[!UICONTROL Add trigger]** om du vill lägga till en ny utlösare.
1. I fältet **[!UICONTROL Workfront team/user/role]** anger du namnet på ett [!DNL Workfront]-team, en användare eller en jobbroll och klickar sedan på det för att markera det när det visas i listan.

   >[!NOTE]
   >
   >Du kan inte ha flera utlösare för samma team, användare eller roll.

   När någon skapar en aktivitet eller ett problem och tilldelar den till någon av dessa enheter skapas ett problem automatiskt i [!DNL [!DNL Jira]].

1. I fältet **[!UICONTROL [!DNL Jira] project]** börjar du skriva namnet på ett [!DNL Jira]-projekt och klickar sedan på det för att markera det när det visas i listan.

   När utgåvan [!DNL Jira] skapas placeras den i det projekt som du väljer här.

1. Välj en **I[!UICONTROL ssue type]** i listrutan.

   Detta anger den problemtyp som skapas i [!DNL Jira] när villkoren för den här utlösaren uppfylls, baserat på dina inställningar för det aktuella projektet i [!DNL Jira].

1. Klicka på **[!UICONTROL Save]**.

   Med den här konfigurationen skapas ett nytt problem i [!DNL Workfront] varje gång en [!DNL Jira]-användare skapar ett objekt som matchar de angivna utlösarna.

## Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] objekt

Som [!DNL Jira]-administratör kan du definiera vilka fält som ska synkroniseras automatiskt på objekt som är länkade mellan [!DNL Workfront] och Jira. Vissa fält kan synkroniseras från [!DNL Workfront] till [!DNL Jira]-objektet och andra synkroniseras från Jira till Workfront.

Så här definierar du vilka fält som ska synkroniseras automatiskt på objekt som är länkade mellan de två programmen:

1. Logga in på [!DNL Jira] som Jira-administratör.
1. Klicka på **[!UICONTROL Settings]** i huvudmenyn för [!DNL Jira].
1. Klicka på **[!UICONTROL Add-ons]** och sedan på **[!UICONTROL Manage add-ons]**.
1. Expandera tillägget **[!DNL Workfront]**.
1. Klicka på **[!UICONTROL Configure]**.
1. Logga in på [!DNL Workfront] som Workfront-administratör.
1. I Jira klickar du på fliken **[!UICONTROL Setup]**.
1. I avsnittet **[!UICONTROL Synchronize from Workfront to Jira]** markerar du de fält som du vill uppdatera i [!DNL Jira] när de uppdateras i Workfront.

   1. Välj någon av följande frekvenser som fälten synkroniseras med:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>De fält du anger synkroniseras mellan de länkade Workfront- och [!DNL Jira]-objekten när objektet skapas i Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>De fält du anger synkroniseras mellan de länkade Workfront- och [!DNL Jira]-objekten när fälten uppdateras i Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>De fält du anger synkroniseras aldrig mellan de länkade [!DNL Workfront]- och [!DNL Jira]-objekten. Det finns ingen indikation i [!DNL Jira] om att fältet uppdaterades i [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Välj något av följande för att synkronisera fälten från [!DNL Workfront] till [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Namnet på en aktivitet eller ett problem i [!DNL Workfront] blir namnet på det problem som den är länkad till i [!DNL Jira].</p><p>Obs! När nya objekt skapas automatiskt i [!DNL Jira] uppdateras alltid [!DNL Workfront]-namnet på [!DNL Jira]-objektet, oavsett om det här fältet är aktiverat här eller inte. När ett [!DNL Jira]-objekt länkas manuellt till ett [!DNL Workfront] -objekt uppdateras namnet på [!DNL Workfront]-objektet endast i [!DNL Jira] när du väljer att <strong>alltid</strong> synkronisera det här fältet. Mer information om att länka objekt manuellt eller automatiskt finns i <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>Beskrivningen av en aktivitet eller ett problem i [!DNL Workfront] blir beskrivningen av det problem som den är länkad till i [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Dokument</td>
         <td><p>Dokument som är kopplade till en aktivitet eller ett problem i [!DNL Workfront] är också kopplade till det problem som den är länkad till i Jira. Nya dokumentversioner från [!DNL Workfront] läggs till som separata dokument till Jira och bifogas med <i>_v&lt;versionsnummer&gt;</i> för att ange den numrerade versionen i Workfront. </p><p>Om namnet på ett dokument i [!DNL Workfront] till exempel är <strong>Main Ad</strong> och du lägger till en ny version i [!DNL Workfront], överförs den nya versionen till [!DNL Jira] som ett nytt dokument med namnet <strong>Main Ad_v2</strong>.</p><p>Viktigt: <p>Tänk på följande när du synkroniserar dokument:</p>
           <ul>
            <li><p>Dokument som är större än 5 MB synkroniseras inte. Om en dokumentsynkronisering misslyckas på grund av att dokumentet är för stort, loggas ett fel i aktivitetsloggen. </p><p>Mer information om aktivitetsloggen finns i <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Visa aktivitetsloggen för Jira</a>.</p></li>
            <li><p>Dokument som är länkade till aktiviteter och problem från externa servrar överförs inte till [!DNL Jira]-objekten. Endast dokument som har överförts direkt till aktiviteten eller utgåvan i [!DNL Workfront] överförs till det länkade utgåvan i [!DNL Jira].</p></li>
            <li><p>Om du vill skapa ett korrektur från ett dokument måste du generera korrekturet i [!DNL Workfront]. </p><p>Mer information om hur du skapar ett korrektur finns i <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Skapa ett korrektur för ett befintligt dokument </a> i <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Skapa ett korrektur för ett dokument</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>[!UICONTROL Planned Completion Date] för en aktivitet eller ett problem i [!DNL Workfront] blir [!UICONTROL Due Date] för det problem som den är länkad till i [!DNL Jira].</p><p>Obs! Kontrollera att du visar <strong>[!UICONTROL Due Date]</strong> i [!DNL Jira] utgåvor för att det här värdet ska synkroniseras.</p></td>
        </tr>
       </tbody>
      </table>

1. I avsnittet **[!UICONTROL Synchronize from [!DNL Jira] to [!DNL Workfront]]** markerar du de fält som du vill uppdatera i [!DNL Workfront] när de uppdateras i [!DNL Jira].

   1. Välj någon av följande frekvenser som fälten synkroniseras med:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>De fält du anger synkroniseras alltid mellan de länkade [!DNL Workfront]- och [!DNL Jira]-objekten när fälten uppdateras i [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>De fält du anger synkroniseras aldrig mellan de länkade [!DNL Workfront]- och [!DNL Jira]-objekten. Det finns ingen indikation i [!DNL Workfront] om att fältet uppdaterades i [!DNL Jira]. </p><p>Obs! När du väljer Aldrig kan [!DNL Workfront] fält fortfarande uppdateras manuellt från [!DNL Jira] i den vänstra [!DNL Workfront] panelen i utgåvan [!DNL Jira]. Dessa uppdateringar visas endast för [!DNL Workfront] objekt i [!DNL Jira] och [!DNL Workfront] och inte för [!DNL Jira] objekt.</p></td>
        </tr>
       </tbody>
      </table>

   1. Välj det här alternativet om du vill synkronisera något av följande fält från [!DNL Jira] till [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>[!UICONTROL Status] för ett problem i [!DNL Jira] blir [!UICONTROL Status] för aktiviteten eller problemet som det är länkat till i [!DNL Workfront].<br>Mer information om [!DNL Workfront]-status finns i <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Skapa eller redigera en status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>[!UICONTROL Assignee] för ett problem i [!DNL Jira] blir [!UICONTROL Assignee] för aktiviteten eller problemet som det är länkat till i [!DNL Workfront].</p><p>Viktigt! När du tilldelar ett objekt i [!DNL Jira] till en användare som inte har något [!DNL Workfront]-konto, skapas en ny aktiv användare i [!DNL Workfront] endast när <strong>Skapa en användare automatiskt i [!DNL Workfront] om [!DNL Jira]-användaren inte har något [!DNL Workfront]-konto </strong> är inställt på <strong>[!UICONTROL Always]</strong>. Den här användaren har ingen [!DNL Workfront]-licens. Aktiva användare kan tilldelas arbetsobjekt i [!DNL Workfront], men kan inte inkluderas i uppdateringar. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Bifogade filer för ett problem i [!DNL Jira] bifogas även till uppgiften eller problemet som den är länkad till i [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>En kommentar om ett [!DNL Jira]-problem har också publicerats för det länkade [!DNL Workfront]-objektet i området [!UICONTROL Updates]. Omvänt har en kommentar publicerats i området [!UICONTROL Updates] för en [!DNL Workfront]-aktivitet eller ett problem synkroniserats till den ursprungliga kommentarströmmen för det länkade problemet i [!DNL Jira]. </p><p>Detta är inställt på <strong>[!UICONTROL Always]</strong> som standard. Om du väljer <strong>[!UICONTROL Never]</strong> här kan du fortfarande publicera kommentarer manuellt för ett länkat objekt i [!DNL Workfront] eller i [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. I avsnittet **[!UICONTROL OTHER]** väljer du vilka ytterligare fält som ska uppdateras mellan länkade objekt.

   1. Välj ett alternativ för att avgöra om fälten som du anger **[!UICONTROL Always]** eller **[!UICONTROL Never]** ska uppdateras i [!DNL Jira] eller [!DNL Workfront] när de ändras.

   1. Välj bland följande fält och uppdateringar:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Anpassade data i den högra panelen i [!DNL Jira]]</td>
         <td><p>Visar [!DNL Workfront] anpassade data för ett objekt på den högra panelen i [!DNL Workfront].</p><p>Obs! Anpassade formuläravsnitt visas på den högra panelen i [!DNL Workfront] med åtkomstnivån för systemadministratören i [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Prioritet i den högra panelen i [!DNL Jira]]</td>
         <td>Visar [!DNL Workfront]-prioritet för ett objekt på den högra panelen i [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Fliken Uppdateringar om förfallodatumändringar i [!DNL Jira]]</td>
         <td>Lägger till en kommentar på fliken [!UICONTROL Update] för [!DNL Workfront]-objektet när [!UICONTROL Due Date] ändras i det länkade [!DNL Jira]-objektet.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] om användaren [!DNL Jira] inte har något [!DNL Workfront]-konto]</td>
         <td><p>Följande scenarier finns:</p>
          <ul>
           <li>När du väljer <strong>[!UICONTROL Always]</strong> aktiverar du integreringen för att skapa en ny Workfront-användare varje gång en [!DNL Jira]-användare utan ett [!DNL Workfront]-konto utför följande åtgärder på ett länkat [!DNL Jira]-problem:
            <ul>
             <li>Har tilldelats en [!DNL Jira]-utgåva</li>
             <li><p>Loggar tid till ett [!DNL Jira]-problem</p><p>Den nya användaren har ingen [!DNL Workfront]-licens. Standardinställningen är Alltid. Användaren skapade på det här sättet i [!DNL Workfront] har lagt till [!UICONTROL Jira] i sitt namn.</p></li>
            </ul></li>
           <li>När du väljer <strong>[!UICONTROL Never]</strong> händer följande:
            <ul>
             <li>Du kan inte se några [!DNL Jira]-tilldelningar för [!DNL Workfront]-objekten. I det här fallet visas bara tilldelningar som gjorts i [!DNL Workfront] för [!DNL Workfront]-objekten.</li>
             <li>Den tid som en användare loggade på ett länkat [!DNL Jira]-problem utan ett [!DNL Workfront]-konto överförs inte automatiskt till det länkade [!DNL Workfront]-objektet. Du kan fortfarande logga tid på objektet [!DNL Workfront] på den högra panelen i utgåvan [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klicka på **[!UICONTROL Save]**.

   Varje gång en användare uppdaterar något av fälten som anges i den här konfigurationen för ett objekt i antingen [!DNL Jira] eller [!DNL Workfront] uppdateras även det länkade objektet i det andra programmet.

## Felsökning

### Det går inte att skapa objekt i [!DNL Jira] på grund av utlösarfält markerade [!UICONTROL Couldn't be found]

#### Problem

När ett fel inträffar med programmet [!DNL Workfront for Jira] inaktiverar [!DNL Workfront] utlösarna för att förhindra ytterligare komplikationer. När dessa utlösare är inaktiverade visas de som [!UICONTROL Couldn't be found].

#### Lösning

Leta reda på felet som inaktiverade utlösarna. Du kan hitta felet i [!DNL Workfront for Jira] [!UICONTROL Activity Log].

Den vanligaste orsaken till detta beteende är felet [!UICONTROL Field 'duedate' cannot be set. It is not on the appropriate screen, or unknown.]

Detta fel innebär att du försöker synkronisera [!UICONTROL Planned Completion Date] från [!DNL Workfront] till [!DNL Jira]. För att kunna göra detta måste du se till att dina [!DNL Jira]-objekt har ett fält med namnet [!UICONTROL Due Date]. Om de inte har det här fältet kan [!DNL Workfront] inte synkronisera det planerade slutförandedatumet från [!DNL Workfront] och inaktiverar dina utlösare.

Försök med något av följande för att lösa problemet:

* Be administratören för [!DNL Jira] att uppdatera de [!DNL Jira]-objekt som påverkas så att de har ett förfallodatumfält.
* Inaktivera synkroniseringen av det planerade slutförandedatumet för [!DNL Workfront] på Workfront [!UICONTROL Setup]-sidan.

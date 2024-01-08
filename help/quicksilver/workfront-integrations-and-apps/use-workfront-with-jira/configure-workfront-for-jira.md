---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Konfigurera [!DNL Adobe Workfront for Jira]
description: Du kan använda [!DNL Adobe Workfront for Jira] integrera [!DNL Jira] och [!DNL Workfront] system.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '2205'
ht-degree: 0%

---

# Konfigurera [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->

Du kan använda [!DNL Adobe Workfront for Jira] integrera [!DNL Jira] och [!DNL Workfront] system.

När du har installerat tillägget kan du definiera arbetsflöden som skapar [!DNL Jira] automatiskt när [!DNL Workfront] arbetsobjekt skapas. Objekten i båda programmen länkas och en del av deras information uppdateras automatiskt i båda systemen.

Alla användare i [!DNL Workfront] och [!DNL Jira] kan dra nytta av den här integreringen. De behöver bara en licens för det system där de arbetar mest, inte för båda systemen.

Det här tillägget är tillgängligt för båda [!UICONTROL Server] och [!UICONTROL OnDemand] (eller [!UICONTROL Cloud]) versioner av [!DNL Jira] Programvara.

För en lista med [!DNL Jira] versioner som [!DNL Workfront for Jira] för närvarande stöds, se [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) på [!DNL Atlassian Marketplace].

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] plan]</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: [!UICONTROL Pro] eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: [!UICONTROL Standard] </p>
       <p>eller</p> 
       <p>Aktuell: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt: Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] att ägna sig åt den här integreringen, i stället för att använda befintliga integreringar som kan kopplas till användare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Innan du kan konfigurera [!DNL Workfront for Jira]måste du:

* Installera [!DNL Workfront for Jira].
Instruktioner för installation [!DNL Workfront for Jira], se [Installera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Konfigurera [!DNL Workfront for Jira]

Genom att konfigurera [!DNL Workfront for Jira]kan du:

* Definiera utlösare som ska skapas [!DNL Jira] objekt när [!DNL Workfront] objekt skapas.
* Ange vilka fält som ska synkroniseras mellan objekt som är länkade mellan [!DNL Jira] och [!DNL Workfront].

>[!NOTE]
>
>* När du har konfigurerat [!DNL Workfront for Jira] på [!DNL Jira] miljö, alla [!DNL Jira] användare ser en [!DNL Workfront] höger panel på alla [!DNL Jira] objekt. Panelen innehåller information om objekt som kan vara länkade från [!DNL Workfront] eller anger att ingen [!DNL Workfront] objekt är länkade till [!DNL Jira] objekt.
>* När du använder [!DNL Jira Server] vid installationen visas endast de problem som är kopplade till projekt som identifieras som utlösare för Workfront-integreringen på Workfront-panelen. Mer information om hur du ställer in utlösare för [!DNL Workfront to Jira] arbetsflöde, se [Konfigurera utlösare för automatisk länkning av objekt mellan [!DNL Jira] och [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Konfigurera [!DNL Workfront for Jira]:

1. Logga in på [!DNL Jira] som [!DNL Jira] administratör.
1. Klicka **[!UICONTROL Settings]** i huvudfönstret [!DNL Jira] -menyn.
1. Klicka **[!UICONTROL Add-ons]** och sedan klicka **[!UICONTROL Manage add-ons]**.

1. Expandera **[!DNL Workfront]** tillägg.
1. Klicka på **[!UICONTROL Configure]**.
1. Följ instruktionerna för att logga in på [!DNL Workfront].

   >[!NOTE]
   >
   >Användaren måste ha en giltig `apiKey` in [!UICONTROL Workfront] för att skapa en lyckad anslutning.

   Du måste logga in på [!DNL Workfront] som [!DNL Workfront] administratör om du vill fortsätta med konfigurationen.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] ansluter till [!DNL Jira] med OAuth 2.0, en standard som används av de flesta webbaserade integreringar för autentisering och auktorisering av användare.
   >* När du uppmanas att ange domänen för din [!DNL Workfront] konto, skriv in det i följande format: *ditt företagsDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.
   >* Förbättrad autentisering är inte tillgängligt förrän en [!DNL Workfront] administratören aktiverar det för den här integreringen.

1. I Jira väljer du **[!UICONTROL Triggers]** för att konfigurera det automatiska skapandet av [!DNL Jira] objekt som nya [!DNL Workfront] objekt skapas.

   Mer information om hur du ställer in utlösare för Workfront till [!DNL Jira] arbetsflöde, se [Konfigurera utlösare för automatisk länkning av objekt mellan [!DNL Jira] och [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Välj **[!UICONTROL Setup]** för att konfigurera synkronisering av fält mellan länkade [!DNL Jira] och [!DNL Workfront] objekt.

   Mer information om hur du konfigurerar synkronisering av fält mellan [!DNL Jira] och [!DNL Workfront], se [Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] Objekt](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >När du har definierat utlösarna och synkroniseringen av fälten mellan de två programmen kan du [!DNL Workfront] användare som kan skapa uppgifter eller problem skulle kunna aktivera skapandet av ett objekt i [!DNL Jira]. Användaren kan skapa ett objekt om villkoren för det objekt som de skapar matchar utlösarna i [!DNL Jira], även om användaren inte har en [!DNL Jira] licens. Dessutom kan [!DNL Jira] kan du börja arbeta direkt med [!DNL Jira] objekt och deras uppdateringar visas i [!DNL Workfront], utan att de har [!DNL Workfront] licens. Eventuella uppdateringar i [!DNL Workfront] är också synliga på [!DNL Jira] objekt.

1. (Valfritt) Välj **[!UICONTROL Activity Log]** för att granska eventuella fel som kan ha inträffat under integreringen.

   Mer information om [!UICONTROL Activity Log], se [Visa [!DNL Jira] [!UICONTROL Activity Log]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Konfigurera utlösare för automatisk länkning av objekt mellan [!DNL Jira] och [!DNL Workfront]

Som [!DNL Jira] systemadministratör kan du definiera utlösare som automatiskt skapar problem i [!DNL Jira] när ett objekt i [!DNL Workfront] uppfyller vissa kriterier.

>[!NOTE]
>
>Det kan ta upp till 10 minuter för integreringen att skapa nya problem i [!DNL Jira].

Tänk på följande när du konfigurerar som utlöser skapandet av [!DNL Jira] objekt som [!DNL Workfront] objekt skapas:

* Integreringen är enkelriktad: Du kan bara utlösa objekt som du skapar i [!DNL Workfront] som automatiskt skapas i [!DNL Jira]. Du kan inte aktivera objekt som du skapar i [!DNL Jira] som automatiskt skapas i [!DNL Workfront].
* Det finns ingen gräns för hur många utlösare du kan ha.
* Om ett objekt som du skapar i [!DNL Workfront] matchar mer än en av utlösarna, endast ett objekt skapas i [!DNL Jira]. Objektet skapas i [!DNL Jira] enligt den första utlösaren (i den ordning som de har definierats i [!DNL Jira]). Alla andra utlösare ignoreras.
* Endast ett objekt i [!DNL Workfront] kan länkas till ett objekt i Jira. Du kan aldrig länka en [!DNL Workfront] objekt till flera [!DNL Jira] problem, eller ett [!DNL Jira] utgåva till flera [!DNL Workfront] objekt.

Så här konfigurerar du utlösare för att automatiskt skapa objekt i [!DNL Jira]:

1. Logga in på [!DNL Jira] som systemadministratör.
1. Klicka **[!UICONTROL Settings]** i huvudfönstret [!DNL Jira] -menyn.
1. Klicka **[!UICONTROL Add-ons]** sedan **[!UICONTROL Manage add-ons]**.
1. Expandera **[!DNL Workfront]** tillägg.
1. Klicka på **[!UICONTROL Configure]**.
1. Logga in på [!DNL Workfront] som systemadministratör.

   The **[!UICONTROL Triggers]** -fliken markeras som standard i Jira.

1. Klicka **[!UICONTROL Add trigger]** för att lägga till en ny utlösare.
1. I **[!UICONTROL Workfront team/user/role]** fält, ange namnet på ett [!DNL Workfront] team, användare eller jobbroll. Klicka sedan för att markera den när den visas i listan.

   >[!NOTE]
   >
   >Du kan inte ha flera utlösare för samma team, användare eller roll.

   När någon skapar en aktivitet eller ett problem och tilldelar den till någon av dessa enheter skapas ett problem automatiskt i [!DNL [!DNL Jira]].

1. I **[!UICONTROL [!DNL Jira] project]** fält, börja skriva namnet på ett [!DNL Jira] och klicka sedan på det när det visas i listan.

   När [!DNL Jira] skapas placeras den i det projekt som du väljer här.

1. Välj en **I[!UICONTROL ssue type]** i listrutan.

   Detta anger vilken typ av problem som skapades i [!DNL Jira] när villkoren för den här utlösaren är uppfyllda, baserat på dina inställningar för det specifika projektet i [!DNL Jira].

1. Klicka på **[!UICONTROL Save]**.

   Med den här konfigurationen, varje gång [!DNL Workfront] användare skapar ett objekt som matchar de angivna utlösarna, en ny utgåva skapas i [!DNL Jira].

## Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] Objekt

Som [!DNL Jira] kan du definiera vilka fält som ska synkroniseras automatiskt på objekt som är länkade mellan [!DNL Workfront] och Jira. Vissa fält kan synkroniseras från [!DNL Workfront] till [!DNL Jira] och andra synkroniserar från Jira till Workfront.

Så här definierar du vilka fält som ska synkroniseras automatiskt på objekt som är länkade mellan de två programmen:

1. Logga in på [!DNL Jira] som Jira-administratör.
1. Klicka **[!UICONTROL Settings]** i huvudfönstret [!DNL Jira] -menyn.
1. Klicka **[!UICONTROL Add-ons]** sedan **[!UICONTROL Manage add-ons]**.
1. Expandera **[!DNL Workfront]** tillägg.
1. Klicka på **[!UICONTROL Configure]**.
1. Logga in på [!DNL Workfront] som Workfront-administratör.
1. I Jira, klicka på **[!UICONTROL Setup]** -fliken.
1. I **[!UICONTROL Synchronize from Workfront to Jira]** markerar du de fält som du vill uppdatera i [!DNL Jira] när de uppdateras i Workfront.

   1. Välj någon av följande frekvenser som fälten synkroniseras med:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>De fält du anger synkroniseras mellan den länkade Workfront-filen och [!DNL Jira] objekt när objektet skapas i Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>De fält du anger synkroniseras mellan den länkade Workfront-filen och [!DNL Jira] objekt när fälten uppdateras i Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>De fält du anger synkroniseras aldrig mellan de länkade [!DNL Workfront] och [!DNL Jira] objekt. Det finns ingen indikation på [!DNL Jira] att fältet uppdaterades i [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Välj något av följande för att synkronisera fälten från [!DNL Workfront] till [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Namnet på en aktivitet eller ett problem i [!DNL Workfront] blir namnet på den utgåva som den är länkad till [!DNL Jira].</p><p>Obs! När nya objekt skapas i [!DNL Jira] automatiskt [!DNL Workfront] Namnge alltid uppdateringar på [!DNL Jira] oavsett om det här fältet är aktiverat här eller inte. När en [!DNL Jira] objektet är manuellt länkat till ett [!DNL Workfront] objekt, namnet på [!DNL Workfront] uppdaterar endast objekt i [!DNL Jira] när du väljer att <strong>Alltid</strong> synkronisera fältet. Mer information om att länka objekt manuellt eller automatiskt finns i <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>Beskrivningen av en aktivitet eller ett problem i [!DNL Workfront] blir en beskrivning av det problem som det är länkat till i [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Dokument</td>
         <td><p>Dokument som är kopplade till en uppgift eller ett problem i [!DNL Workfront] är också kopplade till frågan som den är kopplad till i Jira. Nya dokumentversioner från [!DNL Workfront] läggs till som separata dokument till Jira och bifogas med <i>_v&lt;version number=""&gt;</i> för att ange den numrerade versionen i Workfront. </p><p>Om till exempel namnet på ett dokument i [!DNL Workfront] är <strong>Huvudannons</strong>och du lägger till en ny version i [!DNL Workfront]överförs den nya versionen till [!DNL Jira] som ett nytt dokument med namnet <strong>Main Ad_v2</strong>.</p><p>Viktigt: <p>Tänk på följande när du synkroniserar dokument:</p>
           <ul>
            <li><p>Dokument som är större än 5 MB synkroniseras inte. Om en dokumentsynkronisering misslyckas på grund av att dokumentet är för stort, loggas ett fel i aktivitetsloggen. </p><p>Mer information om aktivitetsloggen finns i <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Visa aktivitetsloggen för Jira</a>.</p></li>
            <li><p>Dokument som är länkade till uppgifter och problem från externa servrar överförs inte till [!DNL Jira] objekt. Endast dokument som överförts direkt till uppgiften eller utgåvan i [!DNL Workfront] överförs till den länkade utgåvan i [!DNL Jira].</p></li>
            <li><p>Om du vill skapa ett korrektur av ett dokument måste du generera korrekturet i [!DNL Workfront]. </p><p>Mer information om hur du genererar ett korrektur finns i <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Skapa ett korrektur för ett befintligt dokument </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Skapa ett korrektur för ett dokument</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>The [!UICONTROL Planned Completion Date] en uppgift eller ett problem i [!DNL Workfront] blir [!UICONTROL Due Date] av den utgåva som den är kopplad till [!DNL Jira].</p><p>Obs! Kontrollera att du visar <strong>[!UICONTROL Due Date]</strong> på [!DNL Jira] problem, för att det här värdet ska synkroniseras.</p></td>
        </tr>
       </tbody>
      </table>

1. I **[!UICONTROL Synchronize from [!DNL Jira] to [!DNL Workfront]]** markerar du de fält som du vill uppdatera i [!DNL Workfront] när de uppdateras i [!DNL Jira].

   1. Välj någon av följande frekvenser som fälten synkroniseras med:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>De fält du anger synkroniseras alltid mellan de länkade [!DNL Workfront] och [!DNL Jira] objekt när fälten uppdateras i [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>De fält du anger synkroniseras aldrig mellan de länkade [!DNL Workfront] och [!DNL Jira] objekt. Det finns ingen indikation på [!DNL Workfront] att fältet uppdaterades i [!DNL Jira]. </p><p>Obs! När du väljer Aldrig [!DNL Workfront] fält kan fortfarande uppdateras manuellt från [!DNL Jira] till vänster [!DNL Workfront] panelen i [!DNL Jira] problem. Uppdateringarna visas bara på [!DNL Workfront] objekt i [!DNL Jira] och [!DNL Workfront] och inte på [!DNL Jira] objekt.</p></td>
        </tr>
       </tbody>
      </table>

   1. Markera om du vill synkronisera något av följande fält från [!DNL Jira] till [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>The [!UICONTROL Status] av en utgåva i [!DNL Jira] blir [!UICONTROL Status] för uppgiften eller utgåvan som den är länkad till [!DNL Workfront].<br>Mer information om [!DNL Workfront] status, se <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Skapa eller redigera en status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>The [!UICONTROL Assignee] av en utgåva i [!DNL Jira] blir [!UICONTROL Assignee] för uppgiften eller utgåvan som den är länkad till [!DNL Workfront].</p><p>Viktigt: När du tilldelar ett objekt i [!DNL Jira] till en användare som inte har [!DNL Workfront] kontot skapas en ny aktiv användare i [!DNL Workfront] endast när <strong>Skapa automatiskt en användare i [!DNL Workfront] om [!DNL Jira] användaren inte har [!DNL Workfront] konto</strong> är inställd på <strong>[!UICONTROL Always]</strong>. Den här användaren upptar inte en [!DNL Workfront] licens. Aktiva användare kan tilldelas arbetsobjekt i [!DNL Workfront], men kan inte inkluderas i uppdateringar. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Bilagor till en utgåva i [!DNL Jira] är också kopplade till uppgiften eller utgåvan som den är länkad till i [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>En kommentar om en [!DNL Jira] utgåvan har också bokförts på den länkade [!DNL Workfront] objekt i [!UICONTROL Updates] område. Omvänt har en kommentar publicerats i [!UICONTROL Updates] område för en [!DNL Workfront] uppgifter eller problem synkroniseras till [!DNL Jira]Inbyggd kommentarström för det länkade problemet. </p><p>Detta är inställt på <strong>[!UICONTROL Always]</strong> som standard. Om du väljer <strong>[!UICONTROL Never]</strong> här kan du fortfarande publicera kommentarer manuellt för ett länkat objekt antingen i [!DNL Workfront] eller in [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. I **[!UICONTROL OTHER]** väljer du vilka ytterligare fält som ska uppdateras mellan länkade objekt.

   1. Välj ett alternativ som avgör om fälten du anger **[!UICONTROL Always]** eller **[!UICONTROL Never]** uppdatera i [!DNL Jira] eller [!DNL Workfront] när de ändras.

   1. Välj bland följande fält och uppdateringar:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Anpassade data i den högra panelen i [!DNL Jira]]</td>
         <td><p>Visar [!DNL Workfront] Anpassade data för ett objekt i [!DNL Workfront] den högra panelen.</p><p>Obs! Anpassade formuläravsnitt visas i [!DNL Workfront] den högra panelen med åtkomstnivån för [!DNL Workfront] Systemadministratör.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Prioritet i den högra panelen i [!DNL Jira]]</td>
         <td>Visar [!DNL Workfront] Prioritet för ett objekt i [!DNL Workfront] den högra panelen.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Fliken Uppdateringar om förfallodatumändringar i [!DNL Jira]]</td>
         <td>Lägger till en kommentar i [!UICONTROL Update] -fliken i [!DNL Workfront] objekt när [!UICONTROL Due Date] förändringar i länkade [!DNL Jira] objekt.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] om [!DNL Jira] användaren inte har [!DNL Workfront] konto]</td>
         <td><p>Följande scenarier finns:</p>
          <ul>
           <li>När du väljer <strong>[!UICONTROL Always]</strong>kan du använda integreringen för att skapa en ny Workfront-användare varje gång [!DNL Jira] användare utan [!DNL Workfront] kontot utför följande åtgärder på ett länkat [!DNL Jira] utgåva:
            <ul>
             <li>Är tilldelad till en [!DNL Jira] problem</li>
             <li><p>Loggar tid till en [!DNL Jira] problem</p><p>Den nya användaren tar inte upp en [!DNL Workfront] licens. Standardinställningen är Alltid. Användaren skapade på det här sättet [!DNL Workfront] har "[!UICONTROL Jira]" har lagts till i namnet.</p></li>
            </ul></li>
           <li>När du väljer <strong>[!UICONTROL Never]</strong>händer följande:
            <ul>
             <li>Du kan inte se några [!DNL Jira] tilldelningar på [!DNL Workfront] objekt. I det här fallet är det bara tilldelningar som gjorts i [!DNL Workfront] visa på [!DNL Workfront] objekt.</li>
             <li>Den tid som är inloggad på en länkad [!DNL Jira] av en användare utan [!DNL Workfront] kontot inte automatiskt överförs till det länkade [!DNL Workfront] objekt. Du kan fortfarande logga tid på [!DNL Workfront] objekt på den högra panelen i [!DNL Jira] problem.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klicka på **[!UICONTROL Save]**.

   Varje gång en användare uppdaterar något av fälten som anges i den här konfigurationen för ett objekt i [!DNL Jira] eller [!DNL Workfront], uppdateras även det länkade objektet i det andra programmet.

## Felsökning

### Det går inte att skapa objekt i [!DNL Jira] därför att utlösarfält har markerats som &quot;[!UICONTROL Couldn't be found]&quot;

#### Problem

När ett fel inträffar med [!DNL Workfront for Jira] applikation, [!DNL Workfront] inaktiverar utlösarna för att förhindra ytterligare komplikationer. När dessa utlösare är inaktiverade visas de som[!UICONTROL Couldn't be found].&quot;

#### Lösning

Leta reda på felet som inaktiverade utlösarna. Felet finns i [!DNL Workfront for Jira] [!UICONTROL Activity Log].

Den vanligaste orsaken till detta beteende är felet &quot;[!UICONTROL Field 'duedate' cannot be set. It is not on the appropriate screen, or unknown.]&quot;

Det här felet innebär att du försöker synkronisera[!UICONTROL Planned Completion Date]&quot; från [!DNL Workfront] till [!DNL Jira]. För att kunna göra detta måste du se till att [!DNL Jira] objekt har ett fält som heter[!UICONTROL Due Date].&quot; Om de inte har det här fältet [!DNL Workfront] kan inte synkronisera det planerade slutförandedatumet från [!DNL Workfront] och inaktiverar dina utlösare.

Försök med något av följande för att lösa problemet:

* Fråga [!DNL Jira] administratör för att uppdatera den drabbade [!DNL Jira] objekt för att säkerställa att de har ett förfallodatumfält.
* Inaktivera synkronisering av [!DNL Workfront]det planerade slutförandedatumet i Workfront [!UICONTROL Setup] sida.

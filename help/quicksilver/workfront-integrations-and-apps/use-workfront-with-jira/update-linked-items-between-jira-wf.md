---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Uppdatera länkade objekt mellan  [!DNL Jira] och [!DNL Adobe Workfront]
description: När du länkar [!DNL Jira] utgåvor till [!DNL Adobe Workfront] aktiviteter eller problem kan dina användare uppdatera objekt i ett program och motsvarigheten till det objektet uppdaterar även för de användare som arbetar i det andra programmet.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1529'
ht-degree: 0%

---

# Uppdatera länkade objekt mellan [!DNL Jira] och [!DNL Adobe Workfront]

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen kommer integreringen av Workfront för Jira inte att vara tillgänglig efter **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Jira.
>
>Åtta färdiga mallar för automatisering och integrering av Workfront för Jira kommer att vara tillgängliga i augusti för att hjälpa till att replikera vanliga arbetsflöden och snabba upp implementeringen. Mallarna är helt anpassningsbara för att uppfylla specifika affärsbehov och kan utökas i takt med att behoven utvecklas.
> 
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration Module för Jira finns i [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

När du länkar [!DNL Jira] utgåvor till [!DNL Adobe Workfront] uppgifter eller problem kan dina användare uppdatera objekt i ett program och motsvarigheten till det objektet uppdateras även för de användare som arbetar i det andra programmet.

Mer information om hur du länkar objekt mellan [!DNL Workfront] och [!DNL Jira] finns i [Länka objekt mellan Adobe Workfront och Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

När du konfigurerar [!DNL Workfront] för [!DNL Jira] kan du som [!DNL Jira]-systemadministratör konfigurera vissa fält från ett program så att de synkroniseras med fält från länkade objekt i det andra programmet.

Mer information om synkronisering av fält mellan länkade [!DNL Jira]- och [!DNL Workfront]-objekt finns i [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: [!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
       <p>eller</p>
       <p>Aktuell: [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt! Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Innan du kan länka objekt mellan [!DNL Workfront] och [!DNL Jira] måste du:

* Installera [!DNL Workfront for Jira].

  Instruktioner om hur du installerar [!DNL Workfront for Jira] finns i [Installera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurera [!DNL Workfront for Jira].

  Instruktioner om hur du konfigurerar [!DNL Workfront for Jira] finns i [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Länka objekt mellan [!DNL Workfront] och [!DNL Jira].

  Instruktioner finns i [Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Uppdatera länkade objekt i [!DNL Workfront]

Om du främst arbetar i [!DNL Workfront] kan du uppdatera dina arbetsobjekt i [!DNL Workfront] och deras motsvarigheter i [!DNL Jira] också uppdatera. Den här uppdateringen sker genom integreringen av [!DNL Workfront] för [!DNL Jira] som inte kräver att du har en [!DNL Jira]-licens.

Så länge som [!DNL Workfront]-administratören har konfigurerat [!DNL Workfront for Jira] för att synkronisera fälten mellan länkade objekt, uppdateras även vissa fält som du uppdaterar i [!DNL Workfront] för det länkade [!DNL Jira]-problemet. Mer information om hur du uppdaterar objekt i [!DNL Workfront] finns i [Redigera problem](../../manage-work/issues/manage-issues/edit-issues.md) och [Redigera uppgifter](../../manage-work/tasks/manage-tasks/edit-tasks.md).

I följande lista visas vilka [!DNL Workfront] fält som synkroniseras med [!DNL Jira] fält på länkade objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Uppdaterat [!DNL Workfront]-fält</strong> </th> 
   <th><strong>Synkroniserat [!DNL Jira] fält/uppdatering</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>En kommentar om namnändringen läggs till på fliken <strong>[!DNL Workfront]</strong> i utgåvan [!DNL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>En kommentar om den uppdaterade beskrivningen läggs till på fliken <strong>[!DNL Workfront]</strong> i utgåvan [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Obs! Dokument som är länkade till [!DNL Workfront] objekt från en extern server överförs inte till [!DNL Jira] utgåvor. Endast dokument som har överförts direkt till [!DNL Workfront] objekt uppdateras även till de länkade [!DNL Jira]-utgåvorna. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>En kommentar om de överförda bifogade filerna läggs till på fliken <strong>[!DNL Workfront]</strong> i utgåvan [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>En kommentar om att [!UICONTROL Due Date] har ändrats läggs till på fliken [!DNL Workfront] i utgåvan [!DNL Jira]. </p> <p>Obs! Du måste aktivera <strong>[!UICONTROL Due Date]</strong> för att dina [!DNL Jira]-utgåvor ska kunna se fältet uppdaterat i [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Anpassade Forms- och anpassade fält</td> 
   <td> <p> Visa i den högra panelen [!DNL Workfront] för utgåvan [!DNL Jira]. <br>Endast anpassade fält som har ett verkligt värde visas på panelen.<br></p> <p>Obs! Anpassade formuläravsnitt visas med åtkomstnivån för administratören för [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Visas i den högra panelen [!DNL Workfront] i utgåvan [!DNL Jira]. <br>Det uppdaterar inte fältet <strong>[!UICONTROL Priority]</strong> i [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>En kommentar om loggad tid läggs till på fliken <strong>[!DNL Workfront]</strong> i utgåvan [!DNL Jira]. Detta inkluderar namnet på den användare som loggar tiden samt den användare som tiden är loggad för, om de är olika. Ingen tid har loggats på fliken <strong>[!UICONTROL Work log]</strong> i [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>Kommentaren läggs till på fliken <strong>[!DNL Workfront]</strong> i utgåvan [!DNL Jira]. Den har inte lagts till på fliken <strong>[!UICONTROL Comments]</strong> i utgåvan [!DNL Jira]</p> <p>Obs! När du länkar två befintliga objekt manuellt synkroniseras inte kommentarerna som lades till i [!DNL Workfront]-objektet innan det länkades till [!DNL Jira] med [!DNL Jira]-utgåvan. </p> <p>Jira-kommentarer synkroniseras till Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## Uppdatera länkade objekt i [!DNL Jira]

Om du främst arbetar i [!DNL Jira] kan du uppdatera dina arbetsobjekt i [!DNL Jira] och deras motsvarigheter i [!DNL Workfront] också uppdatera. Du behöver inte ha någon [!DNL Workfront]-licens för de [!DNL Workfront]-objekt som är länkade till dina [!DNL Jira]-utgåvor för att få de uppdateringar du gör i [!DNL Jira].

Om administratören för [!DNL Workfront] har konfigurerat [!DNL Workfront] för [!DNL Jira] att synkronisera fälten mellan länkade objekt, uppdateras även vissa fält som du uppdaterar i [!DNL Jira] för det länkade [!DNL Workfront]-objektet.

I följande lista visas vilka [!DNL Jira] fält som synkroniseras med [!DNL Workfront] fält på länkade objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Uppdaterat [!DNL Jira]-fält</strong> </th> 
   <th><strong>Synkroniserat [!DNL Workfront] fält/uppdatering</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>Ärendestatus i [!DNL Jira] synkroniseras med följande statusvärden, eller statusvärden som motsvarar följande statusvärden, i Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Obs! Statusen [!DNL Jira] synkroniseras med den första [!DNL Workfront]-statusen som är lika med rätt status.</p> <p>Mer information om status för objekt i [!DNL Workfront] finns i <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Skapa eller redigera en status</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>En kommentar om hur du överför ett nytt dokument i [!DNL Jira] läggs till på fliken [!UICONTROL Updates] i utgåvan eller aktiviteten [!DNL Workfront] .  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> En kommentar om ändringen av [!UICONTROL Due Date] i [!DNL Jira] läggs till på fliken [!UICONTROL Updates] i utgåvan eller aktiviteten [!DNL Workfront]. </p> <p>Obs! Inga datumändringar har gjorts för utgåvan eller aktiviteten [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td> Loggtid i den högra panelen [!DNL Workfront] eller från menyn [!UICONTROL More] i utgåvan [!DNL Jira]<br></td> 
   <td> <p>Timmar<br>Förutom att lägga till de timmar som är inloggade med Jira till det länkade [!DNL Workfront] -objektet, läggs en kommentar om loggningstid till på fliken [!UICONTROL Updates] i [!DNL Workfront] -objektet.</p> <p>Mer information om loggningstid för länkade [!DNL Jira]-problem, inklusive uppdatering av den [!DNL Jira]-användare som loggar in [!DNL Workfront], finns i <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Loggtid för länkade [!DNL Jira] och [!DNL Workfront] objekt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Kommentar <br><br></td> 
   <td> <p>Kommentarer läggs till på fliken [!UICONTROL Updates] i [!DNL Workfront] -utgåvan eller -aktiviteten om inställningen <strong>[!UICONTROL Comments]</strong> i avsnittet [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] på fliken [!UICONTROL Setup] är <strong>[!UICONTROL Always]</strong>.</p> <p>Mer information om hur du konfigurerar Workfront-inställningar i [!DNL Jira] finns i <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md"> Konfigurera [!DNL Workfront for Jira]</a>.</p> <p>Information om hur du kommenterar objekt från länkade [!DNL Jira]-problem finns i <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Kommentera från ett länkat [!DNL Jira]-problem</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Logga tid från länkade [!DNL Jira]-problem

Den tid du registrerar för ett [!DNL Jira]-objekt i [!DNL Jira] överförs också till det länkade [!DNL Workfront]-objektet, oavsett var i [!DNL Jira] du loggar tiden.\
När du loggar tid i Jira på panelen [!DNL Workfront] registreras tiden endast i [!DNL Workfront].\
Den tid du registrerar i [!DNL Workfront] påverkar inte tiden för det länkade problemet i [!DNL Jira].

>[!NOTE]
>
>Om tiden läggs till i ett [!DNL Jira]-objekt som är länkat till en [!DNL Workfront]-aktivitet är [!UICONTROL Hour Type] för tiden i [!DNL Workfront] [!UICONTROL Task Time]. Om tiden läggs till i ett [!DNL Jira]-objekt som är länkat till ett [!DNL Workfront] -problem är [!UICONTROL Hour Type] för tiden i [!DNL Workfront] [!UICONTROL Issue Time].

En kommentar läggs till på fliken **[!DNL Workfront]** i [!DNL Jira] och på fliken **[!UICONTROL Updates]** för objektet i [!DNL Workfront] för att registrera loggningstiden.\
Tiden visas också på fliken **[!UICONTROL Hours]** i objektet [!DNL Workfront].

* [Loggtid för länkade [!DNL Jira] och [!DNL Workfront] objekt](#log-time-for-linked-jira-and-workfront-items)
* [Logga tid från [!DNL Jira] till ett [!DNL Workfront] objekt](#log-time-from-jira-to-a-workfront-item)

### Loggtid för länkade [!DNL Jira]- och [!DNL Workfront]-objekt

Du kan logga tid från ett [!DNL Jira]-problem som är länkat till ett [!DNL Workfront]-objekt, och tiden registreras både i [!DNL Jira]-utgåvan och i [!DNL Workfront]-objektet.

>[!IMPORTANT]
>
>Om användaren inte loggar tiden i [!DNL Jira] finns i [!DNL Workfront] skapas en ny aktiv användare i Workfront om **[!UICONTROL Automatically create a user in [!DNL Workfront]&#x200B;if the [!DNL Jira] user does not have a* [!DNL Workfront]&#x200B;account]** är inställt på **[!UICONTROL Always]**. Den här användaren har ingen [!DNL Workfront]-licens. Du kan tilldela aktiva användare till arbetsobjekt i [!DNL Workfront], men du kan inte inkludera dem i uppdateringar. Mer information om hur du konfigurerar det automatiska skapandet av [!DNL Workfront] användare från [!DNL Jira] finns i [Konfigurera [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Så här loggar du tid för ett objekt i [!DNL Jira] och sparar det både i [!DNL Jira] och [!DNL Workfront]:

1. Logga in på [!DNL Jira].
1. Gå till utgåvan [!DNL Jira] som är länkad till objektet [!DNL Workfront].
1. Expandera menyn **[!UICONTROL More]** och klicka på **[!UICONTROL Log work]**.

1. I fältet **[!UICONTROL Time Spent]** anger du hur mycket tid som har ägnats åt att arbeta med det här problemet. Du måste ange tiden med följande tidsperioder:

   * [!UICONTROL Weeks] (b)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Hours] (h)

1. Fortsätt lägga till information till din tidspost, inklusive en **[!UICONTROL Work Description]**, och klicka sedan på **[!UICONTROL Log]**.\
   Tiden läggs till på fliken **[!UICONTROL Work log]** för [!DNL Jira]-objektet samt till det [!DNL Workfront]-objekt som är länkat till det.\
   Arbetsbeskrivningen för tidsposten registreras som en anteckning för timposten i [!DNL Workfront].

### Logga tid från [!DNL Jira] till ett [!DNL Workfront]-objekt

Du kan logga tid enbart till det länkade [!DNL Workfront]-objektet från utgåvan [!DNL Jira] utan att den här gången spela in till utgåvan [!DNL Jira].

1. Logga in på [!DNL Jira].
1. Navigera till ett [!DNL Jira]-problem som är länkat till ett [!DNL Workfront]-objekt.

   Information om objektet [!DNL Workfront] ska visas på den högra panelen i problemet i [!DNL Workfront] .

1. Klicka på ikonen **[!UICONTROL Log Time]**.

1. Ange hur mycket **[!UICONTROL Hours]** och **[!UICONTROL Minutes]** du vill logga för problemet.

1. Klicka på **[!UICONTROL Log Time]**.

   Tiden läggs till i objektet [!DNL Workfront].

   Den här tiden läggs inte till på fliken [!UICONTROL Work Log] i utgåvan [!DNL Jira].

## Kommentar från ett länkat [!DNL Jira]-problem {#comment-from-a-linked-jira-issue}

När du kommenterar ett [!DNL Jira]-objekt från den [!DNL Workfront] högra panelen i [!DNL Jira] läggs kommentaren också till på fliken [!UICONTROL Updates] för det länkade objektet i Workfront.

Så här kommenterar du från [!DNL Jira] till ett [!DNL Workfront]-objekt:

1. Logga in på [!DNL Jira].
1. Navigera till ett [!DNL Jira]-problem som är länkat till ett [!DNL Workfront]-objekt.

   Information om objektet [!DNL Workfront] ska visas på den högra panelen i problemet i [!DNL Workfront] .

1. Klicka på ikonen **[!UICONTROL Comments]** på panelen [!DNL Workfront] eller på fliken **[!UICONTROL Comments]**.

1. Börja skriva en kommentar och klicka sedan på **[!UICONTROL Send]**.

   Kommentaren läggs till i följande:

   * Fliken **[!DNL Workfront]** i utgåvan [!DNL Jira].
   * Fliken **[!UICONTROL Comments]** i utgåvan [!DNL Jira].
   * Fliken **[!UICONTROL Updates]** för det länkade objektet i Workfront.

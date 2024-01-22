---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Uppdatera länkade objekt mellan [!DNL Jira] och [!DNL Adobe Workfront]
description: När du länkar [!DNL Jira] problem med [!DNL Adobe Workfront] uppgifter eller problem kan dina användare uppdatera objekt i ett program och motsvarigheten till det objektet uppdaterar även för de användare som arbetar i det andra programmet.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# Uppdatera länkade objekt mellan [!DNL Jira] och [!DNL Adobe Workfront]

När du länkar [!DNL Jira] problem med [!DNL Adobe Workfront] uppgifter eller problem kan dina användare uppdatera objekt i ett program och motsvarigheten till det objektet uppdaterar även för de användare som arbetar i det andra programmet.

Mer information om att länka objekt mellan [!DNL Workfront] och [!DNL Jira], se [Länka objekt mellan Adobe Workfront och Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Under konfigurationen [!DNL Workfront] for [!DNL Jira], som [!DNL Jira] systemadministratören kan du konfigurera vissa fält från ett program så att de synkroniseras med fält från länkade objekt i det andra programmet.

Mer information om synkronisering av fält mellan länkade [!DNL Jira] och [!DNL Workfront] objekt, se [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

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

Innan du kan länka objekt mellan [!DNL Workfront] och [!DNL Jira]måste du:

* Installera [!DNL Workfront for Jira].

  Instruktioner för installation [!DNL Workfront for Jira], se [Installera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurera [!DNL Workfront for Jira].

  Instruktioner om konfigurering [!DNL Workfront for Jira], se [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Länka objekt mellan [!DNL Workfront] och [!DNL Jira].

  Instruktioner finns i [Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Uppdatera länkade objekt i [!DNL Workfront]

Om du arbetar huvudsakligen i [!DNL Workfront]kan du uppdatera dina arbetsuppgifter i [!DNL Workfront] och deras motparter i [!DNL Jira] uppdateras också. Uppdateringen görs genom integreringen av [!DNL Workfront] for [!DNL Jira] som inte kräver att du har [!DNL Jira] licens.

Bara [!DNL Workfront] administratören har konfigurerat [!DNL Workfront for Jira] för att synkronisera fälten mellan länkade objekt, vissa fält som du uppdaterar i [!DNL Workfront] uppdaterar även för den länkade [!DNL Jira] problem. Mer information om hur du uppdaterar objekt i [!DNL Workfront], se [Redigera problem](../../manage-work/issues/manage-issues/edit-issues.md) och [Redigera uppgifter](../../manage-work/tasks/manage-tasks/edit-tasks.md).

I följande lista visas vilka [!DNL Workfront] fält synkroniseras med [!DNL Jira] fält på länkade objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Uppdaterat [!DNL Workfront] fält</strong> </th> 
   <th><strong>Synkroniserad [!DNL Jira] fält/uppdatera</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>En kommentar om namnändringen läggs till i <strong>[!DNL Workfront]</strong> -fliken i [!DNL Jira] problem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>En kommentar om den uppdaterade beskrivningen läggs till i <strong>[!DNL Workfront]</strong> -fliken i [!DNL Jira] problem.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Obs! Dokument som är länkade till [!DNL Workfront] objekt från en extern server överförs inte till [!DNL Jira] problem. Endast dokument som överförts direkt till [!DNL Workfront] objekten uppdateras även till de länkade [!DNL Jira] problem. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>En kommentar om de överförda bilagorna läggs till i <strong>[!DNL Workfront]</strong> -fliken i [!DNL Jira] problem.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>En kommentar om [!UICONTROL Due Date] har ändrats läggs till i [!DNL Workfront] -fliken i [!DNL Jira] problem. </p> <p>Obs! Du måste aktivera <strong>[!UICONTROL Due Date]</strong> för [!DNL Jira] problem som ska kunna se det här fältet uppdaterat i [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Anpassade Forms- och anpassade fält</td> 
   <td> <p> Visa i [!DNL Workfront] den högra panelen i [!DNL Jira] problem. <br>Endast de anpassade fält som har ett verkligt värde visas på panelen.<br></p> <p>Obs! Anpassade formuläravsnitt visas med åtkomstnivån för [!DNL Workfront] administratör. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Skärmar i [!DNL Workfront] den högra panelen i [!DNL Jira] problem. <br>Den uppdaterar inte problemet <strong>[!UICONTROL Priority]</strong> fält i [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>En kommentar om loggad tid läggs till i <strong>[!DNL Workfront]</strong> -fliken i [!DNL Jira] problem. Detta inkluderar namnet på den användare som loggar tiden samt den användare som tiden är loggad för, om de är olika. Ingen tid är inloggad i <strong>[!UICONTROL Work log]</strong> tabba in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>Kommentaren läggs till i <strong>[!DNL Workfront]</strong> -fliken i [!DNL Jira] problem. Den läggs inte till i <strong>[!UICONTROL Comments]</strong> -fliken i [!DNL Jira] problem</p> <p>Obs! När du länkar två befintliga objekt manuellt läggs kommentarerna till i [!DNL Workfront] objekt innan det länkas till [!DNL Jira] synkronisera inte med [!DNL Jira] problem. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Uppdatera länkade objekt i [!DNL Jira]

Om du arbetar huvudsakligen i [!DNL Jira]kan du uppdatera dina arbetsuppgifter i [!DNL Jira] och deras motparter i [!DNL Workfront] uppdateras också. Du behöver inte ha en [!DNL Workfront] licens för [!DNL Workfront] objekt länkade till [!DNL Jira] för att få de uppdateringar du gör i [!DNL Jira].

På villkor att din [!DNL Workfront] administratören har konfigurerat [!DNL Workfront] for [!DNL Jira] för att synkronisera fälten mellan länkade objekt, vissa fält som du uppdaterar i [!DNL Jira] uppdaterar även för den länkade [!DNL Workfront] objekt.

I följande lista visas vilka [!DNL Jira] fält synkroniseras med [!DNL Workfront] fält på länkade objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Uppdaterat [!DNL Jira] Fält</strong> </th> 
   <th><strong>Synkroniserad [!DNL Workfront] Fält/uppdatering</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>Ärendestatus i [!DNL Jira] synkroniserar med följande statusvärden, eller statusvärden som motsvarar följande statusvärden, i Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Obs! [!DNL Jira] status synkroniseras med den första [!DNL Workfront] status som är lika med rätt status.</p> <p>Mer information om objektstatus i [!DNL Workfront], se <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Skapa eller redigera en status</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>En kommentar om att överföra ett nytt dokument i [!DNL Jira] läggs till i [!UICONTROL Updates] -fliken i [!DNL Workfront] problem eller uppgifter.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> En kommentar om ändringen av [!UICONTROL Due Date] in [!DNL Jira] läggs till i [!UICONTROL Updates] -fliken i [!DNL Workfront] problem eller uppgifter. </p> <p>Obs! Inga datumändringar på [!DNL Workfront] problem eller uppgifter. </p> </td> 
  </tr> 
  <tr> 
   <td> Loggtid i [!DNL Workfront] den högra panelen eller från [!UICONTROL More] på [!DNL Jira] problem<br></td> 
   <td> <p>Timmar<br>Förutom att lägga till de timmar som är inloggade med Jira till de länkade [!DNL Workfront] objekt, en kommentar om loggningstid läggs till i [!UICONTROL Updates] -fliken i [!DNL Workfront] objekt.</p> <p>Mer information om loggningstid för länkade [!DNL Jira] problem, inklusive uppdatering av [!DNL Jira] användare som loggar in [!DNL Workfront], se <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Loggtid för länkade [!DNL Jira] och [!DNL Workfront] objekt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Kommentar <br><br></td> 
   <td> <p>Kommentarer läggs till i [!UICONTROL Updates] -fliken i [!DNL Workfront] utleverans eller uppgift om <strong>[!UICONTROL Comments]</strong> i [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] i [!UICONTROL Setup] tabba till <strong>[!UICONTROL Always]</strong>.</p> <p>Mer information om hur du konfigurerar Workfront-inställningar i [!DNL Jira], se <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Konfigurerar [!DNL Workfront for Jira]</a>.</p> <p>Mer information om att kommentera objekt från länkade [!DNL Jira] problem, se <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Kommentera från en länkad [!DNL Jira] problem</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Loggtid från länkad [!DNL Jira] problem

Den tid du spelar in för en [!DNL Jira] artikel i [!DNL Jira] kommer också att överföras till den länkade [!DNL Workfront] objekt, oavsett var i [!DNL Jira] loggar du tiden.\
När du loggar tid i Jira i [!DNL Workfront] panel, tiden registreras endast i [!DNL Workfront].\
Den tid du loggar in [!DNL Workfront] påverkar inte tidpunkten för det länkade problemet i [!DNL Jira].

>[!NOTE]
>
>Om tiden läggs till i en [!DNL Jira] objekt länkat till ett [!DNL Workfront] uppgift, [!UICONTROL Hour Type] för tiden i [!DNL Workfront] är [!UICONTROL Task Time]. Om tiden läggs till i en [!DNL Jira] objekt länkat till ett [!DNL Workfront] utgåva, [!UICONTROL Hour Type] för tiden i [!DNL Workfront] är [!UICONTROL Issue Time].

En kommentar läggs till i **[!DNL Workfront]** tabba in [!DNL Jira] och **[!UICONTROL Updates]** fliken för objektet i [!DNL Workfront] för att registrera loggningstiden.\
Tiden visas också i **[!UICONTROL Hours]** -fliken i [!DNL Workfront] objekt.

* [Loggtid för länkade [!DNL Jira] och [!DNL Workfront] objekt](#log-time-for-linked-jira-and-workfront-items)
* [Loggtid från [!DNL Jira] till [!DNL Workfront] artikel](#log-time-from-jira-to-a-workfront-item)

### Loggtid för länkade [!DNL Jira] och [!DNL Workfront] objekt

Du kan logga tid från en [!DNL Jira] problem som är kopplade till en [!DNL Workfront] och tiden registreras både på [!DNL Jira] och [!DNL Workfront] objekt.

>[!IMPORTANT]
>
>Om användaren loggar in [!DNL Jira] finns inte i [!DNL Workfront]skapas en ny aktiv användare i Workfront om **[!UICONTROL Automatically create a user in [!DNL Workfront]&#x200B;if the [!DNL Jira] user does not have a* [!DNL Workfront]&#x200B;account]** är inställt på **[!UICONTROL Always]**. Den här användaren upptar inte en [!DNL Workfront] licens. Du kan tilldela aktiva användare till arbetsobjekt i [!DNL Workfront], men du kan inte inkludera dem i uppdateringar. Mer information om hur du konfigurerar det automatiska skapandet av [!DNL Workfront] användare från [!DNL Jira], se [Konfigurerar [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Logga tid för ett objekt i [!DNL Jira] och få det inspelat både [!DNL Jira] och [!DNL Workfront]:

1. Logga in [!DNL Jira].
1. Gå till [!DNL Jira] problem som är länkat till [!DNL Workfront] objekt.
1. Expandera **[!UICONTROL More]** meny och klicka **[!UICONTROL Log work]**.

1. I **[!UICONTROL Time Spent]** anger du hur mycket tid som har ägnats åt att arbeta med det här problemet. Du måste ange tiden med följande tidsperioder:

   * [!UICONTROL Weeks] (b)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Hours] (h)

1. Fortsätt lägga till information i tidsregistreringen, inklusive en **[!UICONTROL Work Description]** och sedan klicka **[!UICONTROL Log]**.\
   Tiden läggs till i **[!UICONTROL Work log]** -fliken i [!DNL Jira] och [!DNL Workfront] objekt som är länkat till det.\
   Arbetsbeskrivningen för tidsposten registreras som en anteckning på timposten i [!DNL Workfront].

### Loggtid från [!DNL Jira] till [!DNL Workfront] artikel

Du kan logga tiden bara till den länkade [!DNL Workfront] objekt från [!DNL Jira] utan att spela in den här gången [!DNL Jira] problem.

1. Logga in [!DNL Jira].
1. Navigera till en [!DNL Jira] problem som är länkat till en [!DNL Workfront] objekt.

   Information om [!DNL Workfront] objektet ska visas i [!DNL Workfront] den högra panelen för problemet.

1. Klicka på **[!UICONTROL Log Time]** -ikon.

1. Ange mängden **[!UICONTROL Hours]** och **[!UICONTROL Minutes]** du vill logga in på problemet.

1. Klicka på **[!UICONTROL Log Time]**.

   Tiden läggs till i [!DNL Workfront] objekt.

   Den här gången läggs inte till i [!UICONTROL Work Log] -fliken i [!DNL Jira] problem.

## Kommentera från en länkad [!DNL Jira] problem {#comment-from-a-linked-jira-issue}

När du kommenterar en [!DNL Jira] objekt från [!DNL Workfront] den högra panelen i [!DNL Jira]läggs kommentaren också till i [!UICONTROL Updates] för det länkade objektet i Workfront.

Om du vill kommentera från [!DNL Jira] till [!DNL Workfront] objekt:

1. Logga in [!DNL Jira].
1. Navigera till en [!DNL Jira] problem som är länkat till en [!DNL Workfront] objekt.

   Information om [!DNL Workfront] objektet ska visas i [!DNL Workfront] den högra panelen för problemet.

1. Klicka på **[!UICONTROL Comments]** ikonen i [!DNL Workfront] eller på **[!UICONTROL Comments]** -fliken.

1. Börja skriva en kommentar och klicka sedan **[!UICONTROL Send]**.

   Kommentaren läggs till i följande:

   * The **[!DNL Workfront]** -fliken i [!DNL Jira] problem.
   * The **[!UICONTROL Comments]** -fliken i [!DNL Jira] problem.
   * The **[!UICONTROL Updates]** för det länkade objektet i Workfront.

---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Synkronisera rutmappar med [!DNL Workfront Proof]
description: Du kan synkronisera en Box-mapp med en mapp i Workfront Proof. Alla ändringar du gör i filerna i Box-mappen återspeglas i Workfront-korrektur (så att du överför en ny fil, lägger till en ny version, byter namn på en fil osv.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Synkronisera [!DNL Box] Mappar med [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan synkronisera en [!DNL Box] mapp med en mapp i [!DNL Workfront Proof]. Alla ändringar du gör i filerna i Box-mappen återspeglas i Workfront-korrektur (så att du överför en ny fil, lägger till en ny version, byter namn på en fil osv.).

Mer information om mappar finns i [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Endast användare med profiler för [!UICONTROL Managers] eller senare kan synkronisera mappar. The [!DNL Box] användare som överför filen till en mapp som synkroniseras med [!DNL Workfront Proof]blir ägaren till det bevis som skapas i [!DNL Workfront Proof] (om de är en användare inom samma [!DNL Workfront Proof] konto). Om [!DNL Box] användaren är en användare i en annan [!DNL Workfront Proof] eller inte har något konto hos [!DNL Workfront Proof]blir den person som skapade synkroniseringen mellan mapparna ägare till korrekturet. Mer information finns i *&quot;Redigera användarprofiler och behörigheter.&quot;*

Synkronisera en [!DNL Box] mapp med en mapp i [!DNL Workfront Proof]:

1. I [!DNL Box] konto, gå till [!UICONTROL All Files and Folders] sida.
1. Klicka på **[!UICONTROL More options]** -menyn bredvid mappen som du vill synkronisera med [!DNL Workfront Proof] (1).
1. Välj **[!UICONTROL More Actions]** (2).
1. Klicka **[!UICONTROL Sync with [!DNL Workfront Proof]]** (3).
1. I [!UICONTROL Sync folder] som visas (om du är inloggad) [!DNL Workfront Proof]) gör du något av följande:

   * Klicka på en [!DNL Workfront Proof] mappnamn för synkronisering med motsvarande mapp i Box (4).
   * Klicka **[!UICONTROL New folder]** för att skapa en ny mapp i [!DNL Workfront Proof] (5).\

      ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Om du väljer att skapa en ny mapp uppmanas du att ange information om den nya mappen.

1. Klicka på **[!UICONTROL Save]**.\
   The [!UICONTROL Folder details] sidan för den synkroniserade mappen öppnas i [!DNL Workfront Proof]. Den här sidan innehåller information om mappen.\
   På den här sidan kan du även pausa och inaktivera synkroniseringen. Om du pausar synkroniseringen kommer mappen inte längre att uppdateras med ändringarna från [!DNL Box]men synkroniseringen kan återupptas när som helst. Om du inaktiverar synkroniseringen avbryts anslutningen mellan mapparna och synkroniseringen måste återupprättas från [!DNL Box] konto.\
   The [!UICONTROL Folder details] sidan innehåller följande information och funktioner i relation till din mapp i [!DNL Box]:

   * **[!UICONTROL Pause syncing]**: The [!DNL Workfront Proof] mappen kommer inte längre att uppdateras med ändringarna i Box. Synkroniseringen kan återupptas när som helst (1).
   * **[!UICONTROL Disable folder sync]**: Anslutningen mellan mapparna förloras och synkroniseringen måste konfigureras igen från [!DNL Box] konto (2).

   * Endast den användare som startade mappsynkroniseringen kan inaktivera eller pausa den. Mer information finns i  [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Gå till [!DNL Box] mapp**: Om du delade mapp-URL:en (i [!DNL Box] (mappalternativ) blir det här alternativet tillgängligt och du kommer direkt till [!DNL Box] mapp (3).
   * **[!UICONTROL Folder sync details]**: Det här avsnittet innehåller information om [!DNL Box] mapp (4).
   * **[!UICONTROL [!DNL Box] folder link]**: URL till [!DNL Box] mapp (5).
   * **[!UICONTROL Activity]:** Visar aktivitetsloggarna för [!DNL Workfront Proof] här kan du kontrollera vem som startade mappsynkroniseringen (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Du kan även synkronisera [!DNL Box] mapp från [!UICONTROL Folder options] -menyn.
>* Om du har din egen varumärke [!DNL Workfront Proof] inloggningssidan kommer du till den sidan istället för till standardsidan [!DNL Workfront Proof] inloggningssida. Se artiklarna under [Varumärke](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) om du behöver mer information.
>* Om du har aktiverat [!UICONTROL Single Sign-On (SSO)] funktionalitet i [!DNL Workfront Proof] kommer du till inloggningssidan för enkel inloggning och uppmanas att ange inloggningsuppgifterna för enkel inloggning, men bara om du använder samma e-postadress för [!DNL Box] konto och [!DNL Workfront Proof]. Om du behöver mer information kan du läsa [[!UICONTROL Single Sign-On] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Om du inte använder samma e-postadress för båda dina [!DNL Box] konto och [!DNL Workfront Proof] kommer du alltid att tas med i standardinställningarna [!DNL Workfront Proof] inloggningssida.
>




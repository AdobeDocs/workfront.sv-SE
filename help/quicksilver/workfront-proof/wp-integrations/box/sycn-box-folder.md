---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Synkronisera rutmappar med  [!DNL Workfront Proof]
description: Du kan synkronisera en Box-mapp med en mapp i Workfront Proof. Alla ändringar du gör i filerna i Box-mappen återspeglas i Workfront Proof (så att du kan överföra en ny fil, lägga till en ny version, byta namn på en fil osv.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Synkronisera [!DNL Box] mappar med [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan synkronisera en [!DNL Box]-mapp med en mapp i [!DNL Workfront Proof]. Alla ändringar du gör i filerna i Box-mappen återspeglas i Workfront Proof (så att du kan överföra en ny fil, lägga till en ny version, byta namn på en fil osv.).

Mer information om mappar finns i [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Endast användare med profiler från [!UICONTROL Managers] eller senare kan synkronisera mappar. [!DNL Box]-användaren som överför filen till en mapp som är synkroniserad med [!DNL Workfront Proof], blir ägare av det korrektur som skapas i [!DNL Workfront Proof] (om de är en användare inom samma [!DNL Workfront Proof]-konto). Om användaren [!DNL Box] är en användare i ett annat [!DNL Workfront Proof]-konto eller inte har något konto hos [!DNL Workfront Proof], blir den person som skapade synkroniseringen mellan mapparna ägare till korrekturet. Mer information finns i *&quot;Redigera användarprofiler och behörigheter.&quot;*

Synkronisera en [!DNL Box]-mapp med en mapp i [!DNL Workfront Proof]:

1. Gå till sidan [!UICONTROL All Files and Folders] i ditt [!DNL Box]-konto.
1. Klicka på menyn **[!UICONTROL More options]** bredvid mappen som du vill synkronisera med [!DNL Workfront Proof] (1).
1. Välj **[!UICONTROL More Actions]** (2).
1. Klicka på **[!UICONTROL Sync with [!DNL Workfront Proof]]** (3).
1. Gör något av följande i rutan [!UICONTROL Sync folder] som visas (om du är inloggad på [!DNL Workfront Proof]):

   * Klicka på mappnamnet [!DNL Workfront Proof] för att synkronisera det med motsvarande mapp i Box (4).
   * Klicka på **[!UICONTROL New folder]** om du vill skapa en ny mapp i [!DNL Workfront Proof] (5).\

     ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Om du väljer att skapa en ny mapp ombeds du ange information om den nya mappen.

1. Klicka på **[!UICONTROL Save]**.\
   Sidan [!UICONTROL Folder details] för den synkroniserade mappen öppnas i [!DNL Workfront Proof]. Den här sidan innehåller information om mappen.\
   På den här sidan kan du även pausa och inaktivera synkroniseringen. Om du pausar synkroniseringen uppdateras inte mappen längre med ändringarna från [!DNL Box], men synkroniseringen kan återupptas när som helst. Om du inaktiverar synkroniseringen avbryts anslutningen mellan mapparna och synkroniseringen måste återupprättas från kontot [!DNL Box].\
   Sidan [!UICONTROL Folder details] innehåller följande information och funktioner i relation till din mapp i [!DNL Box]:

   * **[!UICONTROL Pause syncing]**: Mappen [!DNL Workfront Proof] uppdateras inte längre med ändringarna från Box. Synkroniseringen kan återupptas när som helst (1).
   * **[!UICONTROL Disable folder sync]**: Anslutningen mellan mappar förloras och synkroniseringen måste konfigureras igen från [!DNL Box]-kontot (2).

   * Endast den användare som startade mappsynkroniseringen kan inaktivera eller pausa den. Mer information finns i [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Gå till [!DNL Box] mapp**: Om du delade mapp-URL:en (i mappalternativen [!DNL Box]) blir det här alternativet tillgängligt och du kommer att gå direkt till mappen [!DNL Box] (3).
   * **[!UICONTROL Folder sync details]**: Det här avsnittet innehåller information om mappen [!DNL Box] (4).
   * **[!UICONTROL [!DNL Box] folder link]**: URL till mappen [!DNL Box] (5).
   * **[!UICONTROL Activity]:** Visar aktivitetsloggarna för mappen [!DNL Workfront Proof], här kan du kontrollera vem som startade mappsynkroniseringen (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Du kan också synkronisera mappen [!DNL Box] från menyn [!UICONTROL Folder options].
>* Om du har en egen inloggningssida med namnet [!DNL Workfront Proof] kommer du till den sidan i stället för till standardinloggningssidan för [!DNL Workfront Proof]. Se artiklarna under [Varumärkning](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) om du behöver mer information.
>* Om du har aktiverat funktionen [!UICONTROL Single Sign-On (SSO)] i ditt [!DNL Workfront Proof]-konto, kommer du till inloggningssidan för enkel inloggning och uppmanas att ange dina inloggningsuppgifter för enkel inloggning, men bara om du använder samma e-postadress för ditt [!DNL Box]-konto och [!DNL Workfront Proof]. Om du behöver mer information kan du läsa [[!UICONTROL Single Sign-On] i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Om du inte använder samma e-postadress för både ditt [!DNL Box]-konto och ditt [!DNL Workfront Proof]-konto, kommer du alltid att gå till standardinloggningssidan för [!DNL Workfront Proof].
>



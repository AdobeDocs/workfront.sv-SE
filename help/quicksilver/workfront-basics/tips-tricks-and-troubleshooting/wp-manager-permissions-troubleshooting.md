---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Felsökning av behörigheter för Workfront Proof Manager
description: De behörighetsprofiler som finns i [!DNL Adobe] Workfront för korrekturläsare är Administrator, Supervisor och Manager.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] Proof Manager] behörigheter felsökning

Följande behörighetsprofiler är tillgängliga i [!DNL Adobe Workfront] för korrekturläsare:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

När en användare beviljas [!UICONTROL Manager] behörighet finns följande felsökningsinformation:

* **PROBLEM:** Användare med [!UICONTROL Manager] behörigheter kan inte visa korrektur som har skapats av andra användare. Istället ser de [!UICONTROL Access Denied] skärm.

   ![](assets/access-denied-350x161.png)

   **LÖSNING:** Användare med [!UICONTROL Manager] behörigheter måste läggas till explicit i korrekturet. Korrektur ska alltid skapas via [!UICONTROL Advanced proofing options] fönster och användare ska alltid läggas till via det här alternativet.

* **PROBLEM:** Användare med [!UICONTROL Manager] behörigheter kan inte lägga till korrekturversioner i korrektur som skapats av andra användare (de kan eventuellt skicka ett korrektur i dokumentuppsättningen, men versionerna är INTE anslutna till den ursprungliga uppsättning som skapats av en annan användare).\
   **LÖSNING:** Användare med [!UICONTROL Manager] behörighet att skicka in versioner till en annan användares korrektur endast om användaren med [!UICONTROL Manager] behörigheter när båda följande gäller:

   * Uttryckligen tillagd i korrektur
   * Ange som [!UICONTROL Authors] (korrekturroll) på korrektur

* **PROBLEM:** Användare med [!UICONTROL Manager] behörigheter kan inte redigera kommentarer från andra användare på ett korrektur som de inte äger eller som de inte skapade.\
   **LÖSNING:** Om användare med [!UICONTROL Manager] behörigheter inte äger korrekturet, men de bör kunna redigera kommentarer, lägga till dem som [!UICONTROL Authors] (eller [!UICONTROL Moderators]).\
   Dessa tre typer av behörigheter är tillgängliga i [!DNL Workfront] for [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester], [!UICONTROL Reviewer] typlicenser. Systemadministratör eller användaradministratör i [!DNL Workfront] kan redigera användarprofiler och justera [!DNL Workfront Proof] behörigheter därifrån.

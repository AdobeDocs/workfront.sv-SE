---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Felsökning av behörigheter i Workfront Proof Manager
description: Behörighetsprofilerna i  [!DNL Adobe] Workfront för korrekturanvändare är Administratör, Supervisor och Hanterare.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] Proof Manager] behörigheter felsökning

Följande behörighetsprofiler är tillgängliga i [!DNL Adobe Workfront] för korrekturanvändare:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Följande felsökningsinformation är tillgänglig när du beviljar behörigheter för en användare [!UICONTROL Manager]:

* **PROBLEM:** Användare med [!UICONTROL Manager] behörighet kan inte visa korrektur som skapats av andra användare. I stället visas skärmen [!UICONTROL Access Denied].

  ![](assets/access-denied-350x161.png)

  **LÖSNING:** Användare med [!UICONTROL Manager] behörighet måste läggas till explicit i korrektur. Korrektur ska alltid skapas via [!UICONTROL Advanced proofing options]-fönstret och användare ska alltid läggas till via det här alternativet.

* **PROBLEM:** Användare med behörigheten [!UICONTROL Manager] kan inte lägga till korrekturversioner i korrektur som skapats av andra användare (de kan eventuellt skicka ett korrektur i dokumentuppsättningen, men versionerna är INTE anslutna till den ursprungliga uppsättning som skapats av en annan användare).\
   **LÖSNING:** Användare med [!UICONTROL Manager]-behörighet kan skicka versionerna till en annan användares korrektur endast om användaren har [!UICONTROL Manager]-behörighet när båda följande gäller:

   * Uttryckligen tillagd i korrektur
   * Ange som [!UICONTROL Authors] (korrekturroll) för korrekturen

* **PROBLEM:** Användare med [!UICONTROL Manager] behörighet kan inte redigera kommentarer från andra användare på ett korrektur som de inte äger eller som de inte har skapat.\
   **LÖSNING:** Om användare med [!UICONTROL Manager] behörighet inte äger korrektur, men de bör kunna redigera kommentarer, lägger du till dem som [!UICONTROL Authors] (eller [!UICONTROL Moderators]).\
   Dessa tre typer av behörigheter är tillgängliga i [!DNL Workfront] för typlicenserna [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester] och [!UICONTROL Reviewer]. Systemadministratör eller Användaradministratör i [!DNL Workfront] kan redigera användarprofiler och justera [!DNL Workfront Proof]-behörigheter därifrån.

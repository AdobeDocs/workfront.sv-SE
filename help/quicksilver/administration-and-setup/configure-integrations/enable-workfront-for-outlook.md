---
title: Aktivera [!DNL Adobe Workfront] för Outlook
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Innan användare kan börja använda  [!DNL Adobe Workfront]  för Outlook måste du först aktivera det för ditt system.
author: Lisa, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: be523b27-191f-46ca-9a87-d512f9a15a1e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Aktivera [!DNL Adobe Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.
>
>* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**
>
>Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**


Innan användare kan börja använda [!DNL Adobe Workfront for Outlook] måste du först aktivera det för ditt system.

Mer information om hur du använder [!DNL Workfront for Outlook] efter att det har aktiverats finns i [[!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/workfront-for-outlook.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information om [!DNL Workfront] administratörer finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Aktivera tillägget [!DNL Workfront] [!DNL Outlook]

1. Logga in på [!DNL Workfront] som administratör.

{{step-1-to-setup}}

1. Expandera **[!UICONTROL System]** och klicka sedan på **[!UICONTROL Preferences]**.

1. Kontrollera att **[!UICONTROL Let people use Workfront's mobile applications and the [!DNL Workfront] [!DNL Outlook] Add-In]** är markerat.\
   Förutom att tillåta att mobilprogrammen [!DNL Workfront] används, tillåter den här inställningen även att tilläggsprogrammet [!DNL Workfront] [!DNL Outlook] används.

   Det här alternativet är aktiverat som standard.

1. Klicka på **[!UICONTROL Save]**.

## Installerar tillägget [!DNL Workfront] [!DNL Outlook]

Mer information om systemkrav för [!DNL Workfront]-tillägget för [!DNL Outlook] finns i [Systemkrav](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#system-requirements-and-prerequisites) i [Konfigurera Adobe Workfront för  [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

Mer information om hur du installerar tillägget [!DNL Workfront] för [!DNL Outlook] finns i [Installera tillägget](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#downloading-and-installing-the-add-in) i [Konfigurera [!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

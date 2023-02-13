---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Konfigurera POP i Microsoft Exchange
description: Ett POP-e-postkonto i [!DNL Microsoft Exchange] är inaktiverat.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Konfigurera POP in [!DNL Microsoft Exchange]

## Problem

Ett POP-e-postkonto i [!DNL Microsoft Exchange] är inaktiverat.

## Lösning

Innan du lägger tid på att felsöka problemet måste du kontrollera att användarens POP-konto är korrekt konfigurerat. Om du fortfarande får problem efter att du har bekräftat att POP-kontot är korrekt konfigurerat ska du kontakta [!DNL Microsoft] Support eller någon av deras partners för ytterligare hjälp.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera POP in [!DNL Microsoft Exchange]

>[!NOTE]
>
>Följande steg kan användas som en allmän guide för konfiguration av POP i [!DNL Microsoft Exchange] för produktion [!DNL Workfront] system. Stegen kan variera avsevärt beroende på vilken version av Exchange du har eller vilka kodändringar Microsoft har gjort.

1. Starta och aktivera POP3-tjänsten på Exchange 2010-servern.

   >[!NOTE]
   >
   >POP3-tjänsten har inte startats som standard.

   1. Starta [!DNL Microsoft]Serverhanteraren.
   1. Navigera: **[!UICONTROL Server Manager]** > **[!UICONTROL Configuration]** >**[!UICONTROL Windows Firewall with Advanced Security]** > **[!UICONTROL Services]**.

   1. Högerklicka **[!DNL Microsoft Exchange]POP3** och sedan klicka **[!UICONTROL Properties]**.

   1. (Villkorligt) Kontrollera att POP-tjänsten startar automatiskt på **[!UICONTROL General]** -fliken, ange **[!UICONTROL Startup]** skriv till [!UICONTROL Automatic].

1. Konfigurera POP3 för servern.

   1. Starta [!DNL Microsoft Exchange] Hanteringskonsol.
   1. Navigera: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Client Access]**.

   1. Välj **[!UICONTROL POP3]**.

      POP3 finns i listan under [!UICONTROL POP3] och [!UICONTROL IMAP4] -tabbar.

   1. Till höger under **[!UICONTROL Actions]**, markera **[!UICONTROL POP3]** väljer du **[!UICONTROL Properties]**.

   1. Klicka **[!UICONTROL POP3 Properties]**&#x200B;öppnar du **[!UICONTROL Binding]** -fliken.

      Alla tillgängliga IP-adresser och portnummer som har konfigurerats för POP3-servervisning. Den övre rutan visar Okrypterad och den nedre rutan visar IP och portar för SSL-/TLS-anslutningar.

   1. Klicka **[!UICONTROL POP3 Properties]**&#x200B;öppnar du **[!UICONTROL Authentication]** -fliken.

   1. **[!UICONTROL Select Secure]** inloggning.

      En TLS-anslutning krävs för att klienten ska kunna autentisera mot servern.

1. Aktivera eller tillåt användare att ansluta till POP.

   1. Starta [!DNL Microsoft Exchange] Hanteringskonsol.
   1. Navigera: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Recipient Configuration]** > **[!UICONTROL Mailbox]**.

      En lista över postlådor eller användare visas.

   1. Markera det e-postmeddelande som används i [!DNL Workfront].
   1. Till höger under **[!UICONTROL Actions]**, markera **[!UICONTROL Properties]**&#x200B;öppnar du **[!UICONTROL Mailbox Features]** -fliken.

   1. (Villkorligt) Om POP3 är inaktiverat klickar du på **[!UICONTROL POP3]** och sedan klicka **[!UICONTROL Enable]**.

      En lista över postlådor eller användare visas.

1. Konfigurera mottagaranslutningar.

   1. Starta [!DNL Microsoft Exchange] Hanteringskonsol.
   1. Navigera: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Hub Transport]**.

      En lista över mottagningsanslutningar visas.

   1. Bekräfta mottagningsanslutaren *Klient* *EX01* är aktiverat.

      Plats *Klient* *EX01* är namnet på Exchange-servern.

   1. Välj *Klient EX01*, sedan till höger under **[!UICONTROL Actions]**, markera **[!UICONTROL Properties]**.

   1. Öppna **[!UICONTROL Authentication]** tabba och kontrollera **[!UICONTROL Transport Layer Security (TLS)]** är markerad.

      >[!NOTE]
      >
      >Om du vill ha grundläggande autentisering kan du behöva starta TLS och integrerad Windows-autentisering.

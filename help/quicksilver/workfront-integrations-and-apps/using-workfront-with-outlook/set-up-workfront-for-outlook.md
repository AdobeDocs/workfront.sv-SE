---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Konfigurera [!DNL Adobe Workfront] för [!DNL Outlook]
description: Med  [!DNL Adobe Workfront] [!DNL Outlook]-tillägget kan du utföra  [!DNL Workfront] nyckelåtgärder direkt från Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Konfigurera [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.
>
>* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**
>
>Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**


Med tillägget [!DNL Adobe Workfront] [!DNL Outlook] kan du utföra följande viktiga [!DNL Workfront]-åtgärder direkt från Outlook:

* Uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett e-postmeddelande. Mer information finns i [Uppdatera ett befintligt objekt från ett [!DNL Outlook] e-postmeddelande](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Skapa en [!DNL Workfront]-begäran baserat på ett e-postmeddelande i [!DNL Outlook]. Mer information finns i [Skapa en Adobe Workfront-begäran från ett [!DNL Outlook] e-postmeddelande](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Lägg till ett e-postmeddelande som en uppgift i området [!UICONTROL My Work]. Mer information finns i [Lägga till ett [!DNL Outlook] e-postmeddelande som en uppgift i din arbetslista](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Svara på kommentarer via tillägget [!DNL Workfront] för [!DNL Outlook]. Mer information om hur du svarar på kommentarer från Workfront för [!DNL Outlook] finns i [Svara på en kommentar från [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Skapa uppgifter och ärenden från grunden eller skapa dem från befintliga e-postmeddelanden (med dra-och-släpp-funktionen). Mer information finns i [Lägga till ett [!DNL Outlook] e-postmeddelande till ett projekt som en aktivitet eller ett problem](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Du måste lägga till tillägget [!DNL Workfront] i ditt [!DNL Outlook]-konto innan du kan använda [!DNL Workfront for Outlook].

Om du inte kan installera [!DNL Workfront]-tillägget med ditt [!DNL Outlook]-konto kontaktar du [!DNL Workfront]-administratören för att se till att [!DNL Outlook]-tillägg är aktiverade för din organisation.

Mer information om hur du aktiverar integreringen av [!DNL Outlook] för din organisation finns i [Aktivera [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> 
   <p>Ny plan: [!UICONTROL Standard]</p> 
   <p>Aktuell plan:[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

[!DNL Workfront]-administratören måste aktivera [!DNL Outlook for Office] med [!DNL Workfront] innan du kan använda den här integreringen.

## Systemkrav

Följande program är tillgängliga:

* **[!DNL Outlook]på webben:** Tillägget [!DNL Workfront] är tillgängligt när du använder [!DNL Outlook] från en webbläsare på en dator eller mobil enhet. Den här funktionen är också tillgänglig när du använder webbappen [!DNL Outlook].
* **[!DNL Outlook]Datorprogram:** Tillägget [!DNL Workfront] är tillgängligt när du använder skrivbordsversionerna [!DNL Windows] och [!DNL Mac] av [!DNL Outlook] som ingår i paketet [!DNL Office].

Tillägget [!DNL Workfront] för [!DNL Outlook] stöds i miljöer som uppfyller följande krav:

* [Klientkrav](#client-requirements-client-requirements)
* [Krav för e-postserver](#mail-server-requirements-mail-server-requirements)

### Klientkrav {#client-requirements}

Workfront stöder följande versioner av [!DNL Outlook]:

* [!DNL Outlook 2013] eller senare [!DNL Windows]
* [!DNL Outlook 2016] eller senare [!DNL Windows]
* [!DNL Outlook] på [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] på [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] på webben

Du måste vara ansluten till en [!DNL Exchange Server] eller [!DNL Office 365] med en direktanslutning.

När klienten konfigureras måste användaren välja någon av följande kontotyper:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Om klienten är konfigurerad att ansluta med POP3 eller IMAP läses inte tillägget [!DNL Workfront] in.

### Krav för e-postserver {#mail-server-requirements}

E-postserverns krav uppfylls som standard när du ansluter till [!DNL Office 365] eller [!DNL Outlook.com]. Om du är ansluten till en lokal installation av [!DNL Exchange Server] gäller dock följande krav:

* Workfront stöder alla [!DNL Exchange On-Premise]-servrar
* [!DNL Exchange Web Services] (EWS) måste vara aktiverat och måste vara exponerat för Internet.
* Servern måste ha ett giltigt autentiseringscertifikat för att servern ska kunna utfärda giltiga identitetstoken. Nya installationer av [!DNL Exchange Server] innehåller ett standardautentiseringscertifikat.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Om du vill komma åt [!DNL Workfront]-tillägget från [[!DNL Office] Store](https://store.office.com/) måste klientåtkomstservrarna kunna kommunicera med [https://store.office.com](https://store.office.com/).

Mer information om miljöer som stöds finns på [[!DNL Microsoft Office 365] hemsidan](https://products.office.com/en-us/office-365-home).

## Installera tillägget

Du kan hämta Workfront-tillägget för Outlook från [Microsoft Store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] för [!DNL Outlook 365] {#workfront-for-outlook-365}

1. I [!DNL Outlook 365] klickar du på ikonen **[!UICONTROL Browse Add-ins]** ![Bläddra bland tillägg](assets/outlook-add-in-26x26.png) högst upp i Office 365-gränssnittet och sedan på **[!UICONTROL Manage add-ins]**.

1. Sök efter **[!DNL Workfront]** i rutan **[!UICONTROL Search add-ins]** och tryck sedan på [!UICONTROL Enter].

1. Klicka på **[!UICONTROL Add]**.

### [!DNL Workfront] för [!DNL Outlook] på webben {#workfront-for-outlook-on-the-web}

1. Öppna [!DNL Microsoft Outlook] i en webbläsare.
1. Klicka på ikonen **[!UICONTROL Browse]-tillägg** ![Bläddra bland tillägg](assets/outlook-add-in-web-version-20x20.png).

   Information om hur du hittar ikonen finns i [Använda tillägg i [!DNL Outlook]  på webben](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) i Microsoft-dokumentationen.

1. Sök efter **[!DNL Workfront]** i fältet **[!UICONTROL Search add-ins]** och tryck sedan på **[!UICONTROL Enter]**.

1. Klicka på **Lägg till** när den visas i listan.

### [!DNL Workfront for Outlook] på [!UICONTROL Windows] eller [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Klicka på **[!UICONTROL Home]** > **[!UICONTROL Store]** på menyfliksområdet.

1. Sök efter **[!DNL Workfront]** i fältet **[!UICONTROL Search]** och tryck sedan på **[!UICONTROL Enter]**.

1. Klicka på växlingsknappen för att aktivera **[!UICONTROL [!DNL Workfront] add-in]**.

## Logga in på [!DNL Workfront] från [!DNL Outlook]

1. I [!DNL Outlook] markerar du ett e-postmeddelande och klickar sedan på ikonen **[!DNL Workfront]** i e-posthuvudet.
1. Klicka på **Logga in på Workfront** på inloggningssidan.
1. Följ instruktionerna för att logga in på [!DNL Workfront] med OAuth 2.0. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Om du uppmanas att ange domänen för ditt [!DNL Workfront]-konto skriver du den i det här formatet: *ditt företags sDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->

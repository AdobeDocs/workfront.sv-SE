---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Konfigurera [!DNL Adobe Workfront] for [!DNL Outlook]
description: The [!DNL Adobe Workfront] [!DNL Outlook] kan du använda nyckeln [!DNL Workfront] uppgifter direkt från Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: fe370eee9e1fa53edc615f82ece8bc46a9cdb0ce
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Konfigurera [!DNL Adobe Workfront for Outlook]

The [!DNL Adobe Workfront] [!DNL Outlook] kan du använda följande tangent [!DNL Workfront] uppgifter direkt från Outlook:

* Uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett e-postmeddelande. Mer information finns i [Uppdatera ett befintligt objekt från ett [!DNL Outlook] e-post](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Skapa en [!DNL Workfront] förfrågan baserad på ett e-postmeddelande inom [!DNL Outlook]. Mer information finns i [Skapa en Adobe Workfront-förfrågan från en [!DNL Outlook] e-post](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Lägg till ett e-postmeddelande som en uppgift i [!UICONTROL My Work] område. Mer information finns i [Lägg till en [!DNL Outlook] e-post som en uppgift i din arbetslista](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Svara på kommentarer via [!DNL Workfront] tillägg för [!DNL Outlook]. Mer information om hur du svarar på kommentarer från Workfront för [!DNL Outlook], se [Svara på en kommentar från [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Skapa uppgifter och ärenden från grunden eller skapa dem från befintliga e-postmeddelanden (med dra-och-släpp-funktionen). Mer information finns i [Lägg till en [!DNL Outlook] e-post till ett projekt som en uppgift eller ett problem](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Du måste lägga till [!DNL Workfront] tillägg i [!DNL Outlook] kontot innan du kan använda [!DNL Workfront for Outlook].

Om du inte kan installera [!DNL Workfront] tillägg med [!DNL Outlook] konto, kontakta [!DNL Workfront] administratören för att säkerställa att [!DNL Outlook] tillägg är aktiverade för din organisation.

Mer information om hur du aktiverar [!DNL Outlook] integrering för din organisation, se [Aktivera [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> 
   <p>Ny plan: [!UICONTROL Standard]</p> 
   <p>Aktuell plan:[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Förutsättningar

Dina [!DNL Workfront] administratör måste aktivera [!DNL Outlook for Office] med [!DNL Workfront] innan du kan använda den här integreringen.

## Systemkrav

Följande program är tillgängliga:

* **[!DNL Outlook]på webben:** The [!DNL Workfront] tillägg är tillgängligt när du använder [!DNL Outlook] från en webbläsare på en dator eller mobil enhet. Den här funktionen är även tillgänglig när du använder [!DNL Outlook] Webbprogram.
* **[!DNL Outlook]Datorprogram:** The [!DNL Workfront] är tillgängligt när du använder [!DNL Windows] och [!DNL Mac] datorversioner av [!DNL Outlook] ingår i [!DNL Office] paket.

The [!DNL Workfront] tillägg för [!DNL Outlook] stöds i miljöer som uppfyller följande krav:

* [Klientkrav](#client-requirements-client-requirements)
* [Krav för e-postserver](#mail-server-requirements-mail-server-requirements)

### Klientkrav {#client-requirements}

Workfront stöder följande versioner av [!DNL Outlook]:

* [!DNL Outlook 2013] eller senare [!DNL Windows]
*[!DNL  Outlook 2016] eller senare [!DNL Windows]
* [!DNL Outlook] på [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] på [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] på webben

Du måste vara ansluten till en [!DNL Exchange Server] eller [!DNL Office 365] med en direktanslutning.

När klienten konfigureras måste användaren välja någon av följande kontotyper:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B; Om klienten är konfigurerad att ansluta med POP3 eller IMAP, [!DNL Workfront] tillägget läses inte in.

### Krav för e-postserver {#mail-server-requirements}

E-postserverns krav uppfylls som standard när du ansluter till [!DNL Office 365] eller [!DNL Outlook.com]. Om du är ansluten till en lokal installation av [!DNL Exchange Server]gäller följande krav:

* Workfront stöder alla [!DNL Exchange On-Premise] servrar
* [!DNL Exchange Web Services] (EWS) måste vara aktiverat och måste vara exponerat för Internet.
* Servern måste ha ett giltigt autentiseringscertifikat för att servern ska kunna utfärda giltiga identitetstoken. Nya installationer av [!DNL Exchange Server] innehåller ett standardautentiseringscertifikat.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* För att få tillgång till [!DNL Workfront] tillägg från [[!DNL Office] Butik](https://store.office.com/)måste klientåtkomstservrarna kunna kommunicera med  [https://store.office.com](https://store.office.com/).

Mer information om vilka miljöer som stöds finns i [[!DNL Microsoft Office 365] hemsida](https://products.office.com/en-us/office-365-home).

## Installera tillägget

Du kan hämta Workfront-tillägget för Outlook från [Microsoft Store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] for [!DNL Outlook 365] {#workfront-for-outlook-365}

1. I [!DNL Outlook 365]klickar du på **[!UICONTROL Browse Add-ins]** icon ![](assets/outlook-add-in-26x26.png)överst i Office 365-gränssnittet klickar du på **[!UICONTROL Manage add-ins]**.

1. I **[!UICONTROL Search add-ins]** ruta, sök efter **[!DNL Workfront]** tryck [!UICONTROL Enter].

1. Klicka på **[!UICONTROL Add]**.

### [!DNL Workfront] for [!DNL Outlook] på webben {#workfront-for-outlook-on-the-web}

1. Öppna [!DNL Microsoft Outlook] i en webbläsare.
1. Klicka på **[!UICONTROL Browse]tillägg** icon ![](assets/outlook-add-in-web-version-20x20.png).

   Information om hur du hittar ikonen finns i [Använda tillägg i [!DNL Outlook] på webben](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) i Microsoft-dokumentationen.

1. Sök efter **[!DNL Workfront]** i **[!UICONTROL Search add-ins]** fält och tryck sedan på **[!UICONTROL Enter]**.

1. När den visas i listan klickar du på **Lägg till**.

### [!DNL Workfront for Outlook] på [!UICONTROL Windows] eller [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Klicka **[!UICONTROL Home]** > **[!UICONTROL Store]** på menyfliksområdet.

1. Sök efter **[!DNL Workfront]** i **[!UICONTROL Search]** fält och tryck sedan på **[!UICONTROL Enter]**.

1. Klicka på växlingsknappen för att aktivera **[!UICONTROL [!DNL Workfront] add-in]**.

## Logga in på [!DNL Workfront] från [!DNL Outlook]

1. I [!DNL Outlook], markerar ett e-postmeddelande och klickar sedan på **[!DNL Workfront]** -ikonen i e-posthuvudet.
1. Följ instruktionerna för att logga in på [!DNL Workfront] med Förbättrad autentisering, OAuth 2.0 eller en SAML-URL (Security Assertion Markup Language).

   Innan användarna kan logga in på [!DNL Workfront] tillägg med SAML, [!DNL Workfront] måste först aktivera [!DNL Office 365] tillägg för autentisering med SAML 2.0-lösning. Mer information finns i avsnittet [Konfigurera [!DNL Adobe Workfront] med SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) i artikeln [Konfigurera [!DNL Adobe Workfront] med SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* När du uppmanas att ange domänen för din [!DNL Workfront] konto, skriv in det i följande format: *ditt företagsDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.
   >* Förbättrad autentisering är inte tillgängligt förrän en [!DNL Workfront] administratören aktiverar det för den här integreringen.


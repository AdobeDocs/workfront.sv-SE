---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installera och öppna Adobe Workfront för XD
description: Du kan installera plugin-programmet Adobe Workfront for XD från Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: a5c4479833243bb5817196a3af8acaa063a16747
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Installera och öppna [!DNL Adobe Workfront for XD]

Du kan installera plugin-programmet [!DNL Adobe Workfront for XD] från Adobe Marketplace. Plugin-programmet har stöd för följande språk:

* Engelska
* Franska
* Tyska
* Italienska
* Spanska
* Portugisiska
* Japanska
* Förenklad kinesiska
* Traditionell kinesiska
* Koreanska

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td><p>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</p><p>Mer information finns i <a href="https://helpx.adobe.com/se/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Creative Cloud supportpolicy</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

* Du måste installera appen [!DNL Adobe XD] innan du installerar plugin-programmet för Workfront.

## Installera plugin-programmet [!DNL Adobe Workfront for XD] för din organisation

Om du är [!DNL Adobe Admin Console]-administratör kan du inkludera plugin-programmet i [!DNL Creative Cloud] distributionspaket. Mer information finns i [Inkludera plugin-program i ditt paket](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Visa en självstudiekurs här](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

[!DNL Adobe Admin Console]-administratörer kan också skapa paket som bara innehåller plugin-program för distribution till användare. Mer information finns i [Skapa [!UICONTROL [!DNL Adobe Workfront] för [!DNL Creative Cloud]] paket för dina användare i  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Installera plugin-programmet [!DNL Adobe Workfront for XD] separat

Du kan installera plugin-programmet [!DNL Adobe Workfront for XD] själv från [!DNL Adobe Exchange].

1. Gå till installationssidan för [Adobe Workfront för XD](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&amp;workflow=share) på Adobe Exchange.
1. Klicka på **Öppna [!DNL Adobe Creative Cloud] skrivbordsapp** i den dialogruta som visas.
1. När plugin-hanteraren för [!DNL Adobe XD] öppnas klickar du på **[!UICONTROL Install]**.
1. Läs informationen i dialogrutan och klicka sedan på **[!UICONTROL OK]**.
1. Fortsätt till följande avsnitt för information om hur du öppnar plugin-programmet.

## Öppna plugin-programmet [!DNL Adobe Workfront for XD]

1. Öppna [!DNL Adobe XD].

1. Skapa en ny fil eller öppna en befintlig.

1. Klicka på ikonen **Plugins** längst ned till vänster.

![XD plug-in-fönster](assets/xd-plugin-window-350x620.png)

1. I **[!UICONTROL Plugins Panel]** söker du efter **[!UICONTROL Adobe Workfront for XD]**.

1. Fortsätt till följande avsnitt för information om hur du loggar in på plugin-programmet.

## Logga in på [!DNL Adobe Workfront for XD]

1. Kontrollera att panelen Plugin-program är öppen och klicka sedan på **[!DNL Adobe Workfront for XD]**.
1. Ange din domän och klicka sedan på **[!UICONTROL Log in]**. En webbläsarsida öppnas.

   >[!TIP]
   >
   >* Om du vill hitta din domän öppnar du en webbläsare, navigerar till din [!DNL Workfront]-instans och kopierar den första delen av URL-adressen:\
   >![Hitta domän](assets/domain-350x50.png)
   >
   > * Om din Workfront-instans är integrerad med Experience Cloud ber du administratören att ge dig den Workfront-domän som finns under Produkt > Workfront i Admin Console.

1. Ange dina [!DNL Workfront]-inloggningsuppgifter i webbläsaren och klicka sedan på **[!DNL Log in]**. Om ditt företag använder en enkel inloggning (SSO) dirigeras du till din SSO-leverantörs sida för att logga in.

   >[!NOTE]
   >
   >Du behöver inte ange dina [!DNL Workfront]-inloggningsuppgifter om du nyligen har loggat in.

   Logga in på [!DNL Workfront] genom att följa anvisningarna.

   >[!NOTE]
   >
   >* [!DNL Workfront] ansluter till [!DNL Adobe Creative Cloud] med OAuth 2.0, en säker standard som används av de flesta webbaserade integreringar för autentisering och auktorisering av användare.
   >* När du uppmanas att ange [domän eller värd] för ditt [!DNL Workfront]-konto skriver du det i det här formatet: *ditt företags sDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.

1. Klicka på **[!UICONTROL Allow Access]** för att slutföra inloggningen och gå tillbaka till [!DNL Adobe XD] för att se ditt arbete.

### Felsöka inloggningsfel

Felet **&quot;Något gick fel&quot; visas när du försöker logga in**


Du kan inte använda en URL som börjar med `experience.adobe.com` för att logga in i plugin-programmet.

![inloggningsfel](assets/plugin-log-in-error.png) ![domän](assets/incorrect-domain.png)


För att åtgärda problemet

1. Avinstallera och installera om plugin-programmet Adobe Workfront for XD för att rensa domänen och felet.

1. Ange din Workfront-domän. Domänen måste vara `company-name.my.workfront.com` och inte `experience.adobe.com`.

Om du är med i Adobe Unified Experience kan du hitta din Workfront-domän på

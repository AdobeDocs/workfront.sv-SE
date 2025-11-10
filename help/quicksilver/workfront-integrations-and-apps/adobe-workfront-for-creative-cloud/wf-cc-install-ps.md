---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installera och öppna [!DNL Adobe Workfront for Photoshop]
description: Du kan installera plugin-programmet Adobe Workfront for Photoshop från Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f5e9f121-a711-4b75-8564-54f29c5cfa48
source-git-commit: 61e5b763ec527aeb846e975e06842dc2c4c69918
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# Installera och öppna [!DNL Adobe Workfront for Photoshop]

Du kan installera plugin-programmet [!DNL Adobe Workfront for Photoshop] från [!DNL Adobe Marketplace]. Plugin-programmet har stöd för följande språk:

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ytterligare produkter</td> 
   <td><p>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

* Du måste installera appen [!DNL Adobe Photoshop] innan du installerar plugin-programmet [!DNL Workfront].

## Installera plugin-programmet [!DNL Adobe Workfront for Photoshop] för din organisation

Om du är [!DNL Adobe Admin Console]-administratör kan du inkludera plugin-programmet i [!DNL Creative Cloud] distributionspaket. Mer information finns i [Inkludera plugin-program i ditt paket](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Visa en självstudiekurs här](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

[!DNL Adobe Admin Console]-administratörer kan också skapa paket som bara innehåller plugin-program för distribution till användare. Mer information finns i [Skapa [!UICONTROL [!DNL Adobe Workfront] för [!DNL Creative Cloud]] paket för dina användare i  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Installera plugin-programmet [!DNL Adobe Workfront for Photoshop] separat

Du kan installera plugin-programmet [!DNL Adobe Workfront for Photoshop] själv från [!DNL Adobe Exchange].

1. Gå till installationssidan för [Adobe Workfront för Photoshop](https://adobe.com/go/cc_plugins_discover_plugin?pluginId=37722a55&workflow=share) på Adobe Exchange.
1. Klicka på **Öppna [!DNL Adobe Creative Cloud] skrivbordsapp** i den dialogruta som visas.
1. När plugin-hanteraren för [!DNL Adobe Photoshop] öppnas klickar du på **[!UICONTROL Install]**.
1. Läs informationen i dialogrutan, klicka sedan på **[!UICONTROL OK]** och följ eventuella instruktioner på skärmen för att slutföra installationen.

1. Fortsätt till följande avsnitt för information om hur du öppnar plugin-programmet.

## Öppna plugin-programmet [!DNL Adobe Workfront for Photoshop]

1. Öppna [!DNL Photoshop].

1. Skapa en ny fil eller öppna en befintlig.

1. Klicka på **[!UICONTROL Plugins]** > **[!UICONTROL Plugins Panel]** på den översta menyn.

   ![Panelen Plugins](assets/plugins-panel-ps.png)

1. I **[!UICONTROL Plugins Panel]** väljer du fliken **[!UICONTROL Plugins]** och söker efter **[!UICONTROL Workfront for Adobe Photoshop]**.

   >[!TIP]
   >
   >   Om du inte ser plugin-programmet när du har öppnat det från [!UICONTROL Plugins Panel] kan det finnas bakom Photoshop-appen. Försök minimera Photoshop för att hitta plugin-programmet.

1. Fortsätt till följande avsnitt för information om hur du loggar in på plugin-programmet.

## Logga in på [!DNL Adobe Workfront for Photoshop]

1. Välj **[!UICONTROL Plugins]** på menyn **[!UICONTROL Plugin Panel]** överst på skärmen.
1. Välj **[!DNL Adobe Workfront for Photoshop]**.
1. Ange din domän och klicka sedan på **[!UICONTROL Log in]**. En webbläsarsida öppnas. Du kanske måste ge Photoshop tillstånd att öppna webbläsaren.

   >[!TIP]
   >
   >* Om du vill hitta din domän öppnar du en webbläsare, navigerar till din [!DNL Workfront]-instans och kopierar den första delen av URL-adressen:\
   >![Hitta domän](assets/domain-350x50.png)
   >
   >* Om din Workfront-instans är integrerad med Experience Cloud och domänen börjar med `experience.adobe.com` ber du din administratör att ge dig den Workfront-domän som finns under Produkt > Workfront i Admin Console.

1. Ange dina [!DNL Adobe]-inloggningsuppgifter i webbläsaren och klicka sedan på **[!UICONTROL Log in]**. Om ditt företag använder en enkel inloggning (SSO) dirigeras du till din SSO-leverantörs sida för att logga in.

   >[!NOTE]
   >
   >Du behöver inte ange dina [!DNL Workfront]-inloggningsuppgifter om du nyligen har loggat in.

1. Logga in på [!DNL Workfront] genom att följa anvisningarna.

   >[!NOTE]
   >
   >* [!DNL Workfront] ansluter till [!DNL Adobe Creative Cloud] med OAuth 2.0, en säker standard som används av de flesta webbaserade integreringar för autentisering och auktorisering av användare.


1. Klicka på **[!UICONTROL Allow Access]** för att slutföra inloggningen.
1. Gå tillbaka till [!UICONTROL Adobe Photoshop] för att se ditt arbete.

### Felsökning av inloggningsfel

Felet **&quot;Något gick fel&quot; visas när du försöker logga in**


Du kan inte använda en URL som börjar med `experience.adobe.com` för att logga in i plugin-programmet.

![inloggningsfel](assets/plugin-log-in-error.png) ![domän](assets/incorrect-domain.png)


För att åtgärda problemet

1. Ta bort mappen som lagrar domänen för plugin-programmet.

   >[!TIP]
   >
   >Gå till Finder på en Mac och tryck på **Kommando+Skift+.** om du vill visa dolda mappar går du till **/Users//Library/Application Support** och tar sedan bort mappen **Workfront**.


1. Gå tillbaka till plugin-programmet och ange din Workfront-domän. Domänen måste vara `company-name.my.workfront.com` och inte `experience.adobe.com`.

   Om du vill [hitta din Workfront-domän](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md) om du använder Adobe Unified Experience går du till Konfigurera, Kundinformation.

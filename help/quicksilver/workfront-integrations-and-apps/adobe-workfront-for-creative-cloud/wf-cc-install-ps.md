---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installera och öppna [!DNL Adobe Workfront for Photoshop]
description: Du kan installera plugin-programmet Adobe Workfront for Photoshop från Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f5e9f121-a711-4b75-8564-54f29c5cfa48
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Installera och öppna [!DNL Adobe Workfront for Photoshop]

Du kan installera [!DNL Adobe Workfront for Photoshop] plugin-program från [!DNL Adobe Marketplace]. Plugin-programmet har stöd för följande språk:

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
 <col> 
 <tbody> 
  <!--<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td><p>Du måste ha en [!DNL Adobe Creative Cloud] utöver en [!DNL Workfront] licens.</p><p>Mer information finns i <a href="https://helpx.adobe.com/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Creative Cloud supportpolicy</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

+++

## Förutsättningar

* Du måste installera [!DNL Adobe Photoshop] innan du installerar [!DNL Workfront] plugin-program.

## Installera [!DNL Adobe Workfront for Photoshop] plugin-program för din organisation

Om du är [!DNL Adobe Admin Console] kan du inkludera plugin-programmet i [!DNL Creative Cloud] distributionspaket. Mer information finns i [Inkludera plugin-program i paketet](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Se en självstudiekurs här](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

[!DNL Adobe Admin Console] administratörer kan också skapa paket som bara innehåller plugin-program för distribution till användare. Mer information finns i [Skapa [!UICONTROL [!DNL Adobe Workfront] for [!DNL Creative Cloud]] paket för dina användare i [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Installera [!DNL Adobe Workfront for Photoshop] plugin-program individuellt

Du kan installera [!DNL Adobe Workfront for Photoshop] plugin-program för dig själv från [!DNL Adobe Exchange].

1. Gå till [Adobe Workfront för Photoshop - installationssida](https://adobe.com/go/cc_plugins_discover_plugin?pluginId=37722a55&amp;workflow=share) på Adobe Exchange.
1. Klicka på **Öppna [!DNL Adobe Creative Cloud] datorprogram**.
1. En gång [!DNL Adobe Photoshop] plugin-hanteraren öppnas, klicka **[!UICONTROL Install]**.
1. Läs informationen i dialogrutan och klicka sedan på **[!UICONTROL OK]**.

1. Fortsätt till följande avsnitt för information om hur du öppnar plugin-programmet.

## Öppna [!DNL Adobe Workfront for Photoshop] plugin

1. Öppna [!DNL Photoshop].

1. Skapa en ny fil eller öppna en befintlig.

1. Klicka på i den övre menyn **[!UICONTROL Plugins]** > **[!UICONTROL Plugins Panel]**.

   ![](assets/plugins-panel-ps.png)

1. I **[!UICONTROL Plugins Panel]** väljer du **[!UICONTROL Plugins]** flik och hitta **[!UICONTROL Workfront for Adobe Photoshop]**.

   >[!TIP]
   >
   >   Om du inte ser plugin-programmet när du har öppnat det från [!UICONTROL Plugins Panel]kan det ligga bakom Photoshop app. Försök minimera Photoshop för att hitta plugin-programmet.

1. Fortsätt till följande avsnitt för information om hur du loggar in på plugin-programmet.

## Logga in på [!DNL Adobe Workfront for Photoshop]

1. Från **[!UICONTROL Plugins]** menyn längst upp på skärmen väljer du **[!UICONTROL Plugin Panel]**.
1. Välj **[!DNL Adobe Workfront for Photoshop]**.
1. Ange din domän och klicka sedan på **[!UICONTROL Log in]**. En webbläsarsida öppnas. Du kanske måste ge Photoshop tillstånd att öppna webbläsaren.

   >[!TIP]
   >
   >* Om du vill hitta din domän öppnar du en webbläsare och navigerar till [!DNL Workfront] -instans och kopiera den första delen av URL:en:\
   >![](assets/domain-350x50.png)
   >
   > * Om din Workfront-instans är integrerad med Experience Cloud ber du din administratör att ge dig den Workfront-domän som finns under Product > Workfront i Admin Console.

1. Ange [!DNL Workfront] inloggningsuppgifter och klicka sedan på **[!UICONTROL Log in]**. Om ditt företag använder en enkel inloggning (SSO) dirigeras du till din SSO-leverantörs sida för att logga in.

   >[!NOTE]
   >
   >Du behöver inte ange [!DNL Workfront] autentiseringsuppgifter om du loggade in nyligen.

   Följ instruktionerna för att logga in på [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] ansluter till [!DNL Adobe Creative Cloud] med OAuth 2.0, en säker standard som används av de flesta webbaserade integreringar för autentisering och auktorisering av användare.
   >* När du uppmanas att ange [domän eller värd] på [!DNL Workfront] konto, skriv in det i följande format: *ditt företagsDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.

1. Klicka **[!UICONTROL Allow Access]** för att slutföra inloggningen.
1. Gå tillbaka till [!UICONTROL Adobe Photoshop] för att se ditt arbete.

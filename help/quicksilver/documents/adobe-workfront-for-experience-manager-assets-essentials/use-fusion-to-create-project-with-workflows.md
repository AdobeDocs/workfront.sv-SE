---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Använd Workfront Fusion för att skapa ett Workfront-projekt med Adobe Experience Manager arbetsflöden
description: Om du skapar ett projekt via Workfront Fusion och vill inkludera Adobe Experience Manager-arbetsflöden i projektet måste du använda en specifik konfiguration för Fusion-modulen som beskrivs i den här artikeln.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
source-git-commit: 308118e94f76ac1fb070282d31fbba5cac5312fe
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Använd Workfront Fusion för att konvertera ett Workfront-problem till ett projekt som innehåller Adobe Experience Manager-arbetsflöden

Om du skapar ett projekt via Workfront Fusion och vill inkludera Adobe Experience Manager-arbetsflöden i projektet måste du använda en specifik konfiguration för Fusion-modulen som beskrivs i den här artikeln.

>[!NOTE]
>
>Arbetsflöden är bara tillgängliga i en Adobe Experience Manager as a Cloud Service-integrering. De är inte tillgängliga i integreringar med Adobe Experience Manager Assets Essentials.


## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>Adobe Workfront-plan*</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenser*</strong>
   </td>
   <td>Begäran eller senare
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td><b>Adobe Experience Manager<b>:<ul><li><p>Du måste ha Experience Manager Assets as a Cloud Service eller Assets Essentials, och du måste läggas till som användare i Admin Console.</p></li><li><p>Du måste ha skrivåtkomst till databasen i Adobe Experience Manager.</p></li></ul>
  <b>Workfront Fusion</b>:<p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ingår.</li></ul>   <p>eller</p>
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p>
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationer på åtkomstnivå*</strong>
   </td>
   <td>Redigera åtkomst till dokument
<p>
<strong>Obs! </strong>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <strong>Skapa eller ändra anpassade åtkomstnivåer</strong>.
   </td>
  </tr>
</table>

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera arbetsflöden i en Adobe Experience Manager-integrering. Mer information finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Du måste ha en projektmall konfigurerad med ett arbetsflöde för länkade mappar för Adobe Experience Manager-integrering.
* Du måste ha skapat ett OAuth-program i Workfront för att kunna konfigurera anslutningen för den här modulen.

  Instruktioner finns i [Skapa ett OAuth-program](#create-an-oauth-application) i den här artikeln.

## Modulkonfiguration

Om du vill skapa ett projekt som innehåller Adobe Experience Manager-arbetsflöden i Workfront Fusion måste du använda modulen Workfront > Div-åtgärd.

1. Lägg till **Workfront** > **Div-åtgärd** till ditt scenario.
1. I **Anslutning** markerar du den Workfront-anslutning som ansluter till det konto som modulen ska använda.

   Instruktioner om hur du skapar en anslutning finns i [Anslut [!DNL Workfront] till [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) i artikeln Workfront-moduler.

   Instruktioner om hur du skapar klient-ID och klienthemlighet som du måste skapa en anslutning finns i [Skapa ett OAuth-program](#create-an-oauth-application) i den här artikeln.

1. I **Posttyp** fält, markera `Issue`.
1. I **Åtgärd** fält, markera `convertToProject`.
1. I **ID** ska du ange eller mappa ID:t för problemet som du konverterar till ett projekt.
1. Aktivera **Visa avancerade inställningar**.
1. Rulla längst ned i modulen och leta upp **Projekt (avancerad samling)** fält.
1. Klistra in följande text i **Projekt (avancerad samling)** fält.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Ersätt `Folder tree ID here` med mapp-ID:n.

   Information om hur du hittar mappträds-ID finns i [Leta rätt på mappträds-ID:n](#locate-folder-tree-ids) i den här artikeln.

   Om du vill använda mer än ett mappträd avgränsar du ID:n med kommatecken:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Ersätt `New project name here` med namnet som det nya projektet kommer att ha.
1. Ersätt `Template ID here` med ID:t för mallen som du använder för det nya projektet.

   Du kan mappa mall-ID från en tidigare modul (till exempel en Workfront > Sökmodul) eller leta reda på det i URL:en till mallsidan i Workfront.

1. Klicka **OK** för att spara modulkonfigurationen.

## Leta rätt på mappträds-ID:n

Så här hittar du mappträds-ID:n:

>[!NOTE]
>
>De här instruktionerna använder webbläsaren Chrome.

1. Öppna den mall som du vill använda för det här projektet i Workfront. Den här mallen måste innehålla den Adobe Experience Manager-konfiguration som du vill använda för projektet.
1. Öppna utvecklarverktygen för webbläsaren.
1. Öppna **Nätverk** i utvecklingsverktygen.
1. I **Filter** ruta, ange `object-workflow`.
1. Klicka på det alfanumeriska ID:t som visas i kolumnen Namn.

   ![Söker efter mapp-ID 1](assets/finding-folder-id-1.png)

1. Klicka på **Förhandsgranska** till höger om det alfanumeriska ID:t.
1. Öppna följande komprimerade avsnitt:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Varje mappträd representeras av en siffra. 0 (noll) representerar den första mappen i listan, 1 representerar den andra och så vidare. Om mallen bara innehåller ett mappträd är det 0.

1. Öppna mappträdet som du vill använda för det nya projektet. Anteckna `_id` fältvärde. Om du vill använda mer än ett mappträd bör du tänka på alla `_id` fältvärden för de mappträd som du vill använda.

   ![Söker efter mapp-ID 2](assets/finding-folder-id-2.png)

   De här är `aemNativeFolderTreeIDs`  värden som du anger i **Projekt (avancerad samling)** fältet i **Workfront** > **Diverse åtgärder** Fusion-modul.

## Skapa ett OAuth-program

Du måste konfigurera ett OAuth-program i Workfront för den här modulens anslutning. Du behöver bara göra detta en gång för en viss Workfront-anslutning i Fusion.

1. I Workfront börjar du skapa ett OAuth-program enligt beskrivningen i [Skapa ett OAuth2-program med användarens inloggningsuppgifter (kodflöde för auktorisering)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) i artikeln Create OAuth2 applications for [!DNL Workfront] integreringar.
1. Kopiera klient-ID och klienthemlighet till en säker plats.
1. I **Omdirigera URI:er** anger du följande:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Klicka **Spara**.

Du använder detta klient-ID och klienthemlighet när du konfigurerar modulens anslutning i Fusion.

Instruktioner om hur du skapar en anslutning finns i [Anslut [!DNL Workfront] till [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) i artikeln Workfront-moduler.





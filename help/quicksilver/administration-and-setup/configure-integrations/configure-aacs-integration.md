---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integreringar med Adobe Experience Manager Assets
description: Du kan koppla ditt arbete till följande Adobe Experience Manager Assets Integrations.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Experience Manager Assets as a Cloud Service] integration

Du kan koppla ditt arbete till ditt innehåll i [!DNL Experience Manager Assets]&#x200B;:

* Överför resurser och metadata från [!DNL Adobe Workfront] till [!DNL Experience Manager Assets]&#x200B;
* Länka resurser från [!DNL Experience Manager Assets] till dina projekt och uppgifter i [!DNL Workfront&#x200B;]
* Underlätta versionsanvändning
* Skapa mappar länkade till [!DNL Experience Manager Assets]
* Spåra metadata för resurser och mappar
* Synkronisera projektmetadata mellan [!DNL Workfront] och [!DNL Experience Manager Assets]


## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan*</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenser*</strong>
   </td>
   <td>[!UICONTROL Plan]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] licens</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td>Du måste ha [!DNL Experience Manager Assets as a Cloud Service]och du måste läggas till som användare i produkten.
   </td>
  </tr>
  <tr>
   <td>Konfigurationer på åtkomstnivå*
   </td>
   <td>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <strong>Bevilja användaren fullständig administrativ åtkomst</strong>.
   </td>
  </tr>
</table>


*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.


## Förutsättningar

Innan du börjar,

* Du måste ha [!DNL Workfront] och [!DNL Adobe Experience Manager Assets] associeras med ett organisations-ID i [!DNL Adobe Admin Consol]e. Mer information finns i [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Ställ in integreringsinformation

1. Klicka på **[!UICONTROL Main Menu]** ikonen i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** .
1. Välj **[!UICONTROL Documents]** i den vänstra panelen väljer **[!UICONTROL [!DNL Experience Manager] Integration]**.
   >[!NOTE]
   >
   >Det här konfigurationsområdet visas bara om [!DNL Workfront] miljö ingår under en [!DNL Adobe Admin Console].

1. Välj **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. I **[!UICONTROL Name]** anger du det namn som du vill att användare ska se när de interagerar med integreringen i Workfront och Experience Manager Assets.
1. I **[!UICONTROL Navigation URL]** fyller systemet automatiskt i navigerings-URL:en. Den här skrivskyddade URL:en används för att länka till din organisations [!DNL Experience Manager] -instans från [!UICONTROL Main Menu] för snabb åtkomst.
1. Välj en databas på menyn **[!UICONTROL [!DNL Experience Manager] Assets repository]** nedrullningsbar meny. Systemet fyller automatiskt i alla [!DNL Experience Manager] databaser som är associerade med det organisations-ID som din användarprofil är tilldelad till.
   ![välj Experience Manager-databas](assets/setup-information.png)

1. Klicka **[!UICONTROL Save]** eller gå vidare till [Konfigurera metadata (valfritt)](#set-up-metadata-optional) i den här artikeln.

   >[!NOTE]
   >
   >På grund av integreringens komplexitet kan du inte ändra databasen efter att du har sparat den ursprungliga konfigurationen.

## Konfigurera metadata (valfritt)

Du kan mappa [!DNL Workfront] objektdata till objektmediefält i [!DNL Experience Manager] Resurser.

>[!IMPORTANT]
>
>Du kan bara mappa metadata i en riktning: från [!DNL Workfront] till [!DNL Experience Manager]. Metadata för dokument som är länkade till [!DNL Workfront] från [!DNL Experience Manager] kan inte överföras till [!DNL Workfront].



### Konfigurera metadatafält

1. Konfigurera ett metadataschema i [!DNL Experience Manager Assets] enligt [Konfigurera metadatamappning för resurser mellan Adobe [!DNL Workfront] och [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Konfigurera anpassade formulärfält i Workfront. [!DNL Workfront] har många inbyggda anpassade fält som du kan använda. Du kan även skapa egna anpassade fält enligt anvisningarna i [Skapa eller redigera ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Resurser

Metadata mappas när en resurs överförs från [!DNL Workfront] för första gången. Dokument med inbyggda eller anpassade fält mappas automatiskt till de angivna fälten första gången en resurs skickas till [!DNL Experience Manager Assets].

>[!NOTE]
>
>Den här integreringen stöder inte anpassade metadata från [!DNL Adobe Experience Manager].

Så här mappar du metadata för resurser:

1. Välj **[!UICONTROL Assets]** ovanför metadatatabellen.
1. I **[!UICONTROL [!DNL Workfront] field]** väljer du ett inbyggt eller anpassat Workfront-fält.

   >[!NOTE]
   >
   >Du kan mappa en enda [!DNL Workfront] fält till flera [!UICONTROL Experience Manager Assets] fält. Du kan inte mappa flera [!DNL Workfront] fält till ett enda [!DNL Experience Manager Assets] fält.

1. I [!DNL Experience Manager Assets] -fält, söka igenom de redan ifyllda kategorierna eller ange minst två bokstäver i sökfältet för att få tillgång till ytterligare kategorier.
1. Upprepa steg 2 och 3 efter behov.
   ![metadatafält](assets/asset-metadata.png)
1. Klicka [!UICONTROL Save] eller gå vidare till [Mappar](#folders) i den här artikeln.

### Mappar

När användare skapar en länkad mapp i ett projekt mappas associerade projekt-, portfölj- och programdata till mappmetadatafält i [!DNL Experience Manager Assets].

>[!NOTE]
>
>Den här integreringen stöder inte anpassade metadata från [!DNL Adobe Experience Manager].

Så här mappar du metadata för mappar:

1. Välj **[!UICONTROL Folders]** ovanför metadatatabellen.
1. I **[!UICONTROL [!DNL Workfront] field]** väljer du ett inbyggt eller anpassat Workfront-fält.

   >[!NOTE]
   >
   >Du kan mappa ett enstaka Workfront-fält till flera Experience Manager Assets-fält. Du kan inte mappa flera [!DNL Workfront] fält till ett enda [!DNL Experience Manager Assets] fält.

1. I **[!DNL Experience Manager Assets]** -fält, söka igenom de redan ifyllda kategorierna eller ange minst två bokstäver i sökfältet för att få tillgång till ytterligare kategorier.
1. Upprepa steg 2 och 3 efter behov.
   ![mappmetadata](assets/folder-metadata.png)
1. Klicka **[!UICONTROL Save]** eller gå vidare till [Synkronisering av projektmetadata](#project-metadata-sync) i den här artikeln.


### Synkronisering av objektmetadata

An [!DNL Experience Manager] fält som mappas till [!DNL Workfront] portfölj, program, projekt, uppgift, utgåva och dokumentfält uppdateras automatiskt när fältet ändras i [!DNL Workfront].

>[!IMPORTANT]
>
>Användarna måste ha skrivåtkomst i [!DNL Experience Manager] för resurser som finns i objektet för att metadata ska kunna synkroniseras när de uppdateras.

1. Aktivera **[!UICONTROL Sync object metadata]** fält.
1. Klicka på Spara eller gå vidare till [Konfigurera länkade mappar (valfritt)](#set-up-linked-folders-optional) i den här artikeln.

## Konfigurera länkade mappar (valfritt)

Du kan tillåta användare att skapa mappar som är länkade till [!DNL Experience Manager] när du befinner dig i [!DNL Workfront] projekt. När en mapp är länkad visas alla resurser som läggs till i mappen automatiskt i båda [!DNL Workfront] och [!DNL Experience Manager]. När en resurs läggs till i den länkade mappen i [!DNL Workfront] för första gången skickas resursens metadata till [!DNL Experience Manager Assets].

I stegen nedan anger du var du vill att de länkade mapparna ska skapas. Varje integrering kan bara ha en plats för alla länkade mappar.

Så här konfigurerar du länkade mappar:

1. Växla **[!UICONTROL Enable Linked folder]** på.
1. Välj en mappsökväg för att ange var du vill att alla länkade mappar som är associerade med den här integreringen ska vara.

   >[!NOTE]
   >
   >Användare behöver skrivåtkomst i [!DNL Adobe Experience Manager Assets] till den mapp som har angetts för att skapa en länkad mapp.

1. Klicka på **[!UICONTROL Save]**.

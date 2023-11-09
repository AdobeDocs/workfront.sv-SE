---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Konfigurera [!UICONTROL Experience Manager Assets as a Cloud Service] integration
description: Du kan koppla ditt arbete till innehållet i [!DNL Experience Manager Assets].
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 0f625e7d058c6d3ccbfd9dbb12175ad3e2797911
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Experience Manager Assets as a Cloud Service] integration

>[!IMPORTANT]
>
>Den här funktionen är bara tillgänglig för organisationer som har anslutit sig till [!DNL Adobe Admin Console].

Du kan koppla ditt arbete till innehållet i [!DNL Experience Manager Assets]&#x200B;:

* Överför resurser och metadata från [!DNL Adobe Workfront] till [!DNL Experience Manager Assets]&#x200B;
* Länka resurser från [!DNL Experience Manager Assets] till dina projekt och uppgifter i [!DNL Workfront&#x200B;]
* Underlätta versionsanvändning
* Skapa mappar länkade till [!DNL Experience Manager Assets]
* Spåra metadata för resurser och mappar
* Synkronisera projektmetadata mellan [!DNL Workfront] och [!DNL Experience Manager Assets]

>[!NOTE]
>
>Du kan också ansluta flera [!DNL Experience Manager Assets] databaser till en [!UICONTROL Workfront] miljö, eller flera [!DNL Workfront] miljöer till en [!DNL Experience Manager Assets] databas över organisationsnummer. Följ konfigurationsinstruktionerna i den här artikeln för varje integrering som du vill konfigurera.

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

1. Klicka på **[!UICONTROL Main Menu]** i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** .
1. Välj **[!UICONTROL Documents]** i den vänstra panelen väljer **[!UICONTROL [!DNL Experience Manager] Integration]**.

   >[!NOTE]
   >
   >Det här konfigurationsområdet visas bara om [!DNL Workfront] miljö ingår under en [!DNL Adobe Admin Console].

1. Välj **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. I **[!UICONTROL Name]** anger du det namn som du vill att användare ska se när de interagerar med integreringen i Workfront och Experience Manager Assets.
1. I **[!UICONTROL Navigation URL]** fyller systemet automatiskt i navigerings-URL:en. Denna skrivskyddade URL används för att länka till organisationens [!DNL Experience Manager] -instans från [!UICONTROL Main Menu] för snabb åtkomst.
1. Välj en databas på menyn **[!UICONTROL [!DNL Experience Manager] Assets repository]** listruta. Systemet fyller automatiskt i [!DNL Experience Manager] databaser som är associerade med det organisations-ID som din användarprofil är tilldelad till.
   ![välj Experience Manager-databas](assets/setup-information.png)

1. Klicka **[!UICONTROL Save]** eller gå vidare till [Konfigurera metadata (valfritt)](#set-up-metadata-optional) i den här artikeln.

   >[!NOTE]
   >
   >På grund av integreringens komplexitet kan du inte ändra databasen efter att du har sparat den ursprungliga konfigurationen.

## Konfigurera metadata (valfritt)

Du kan mappa [!DNL Workfront] objektdata till objektmediefält i [!DNL Experience Manager] Resurser.

>[!IMPORTANT]
>
>Du kan bara mappa metadata i en riktning: från [!DNL Workfront] till [!DNL Experience Manager]. Metadata för dokument länkade till [!DNL Workfront] från [!DNL Experience Manager] kan inte överföras till [!DNL Workfront].

### Konfigurera metadatafält

Innan du börjar mappa metadatafält måste du konfigurera metadatafält i både Workfront och Experience Manager Assets.

Konfigurera metadatafält:

1. Konfigurera ett metadataschema i [!DNL Experience Manager Assets] som förklaras i [Konfigurera metadatamappning för resurser mellan Adobe [!DNL Workfront] och [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Konfigurera anpassade formulärfält i Workfront. [!DNL Workfront] har många inbyggda anpassade fält som du kan använda. Du kan även skapa egna anpassade fält enligt anvisningarna i [Skapa eller redigera ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Expandera om du vill ha mer information om vilka Workfront- och Experience Manager Assets-fält som stöds**

**Experience Manager Assets-taggar**

Du kan mappa ett fält som stöds av Workfront till en tagg i Experience Manager Assets. För att göra detta måste du se till att taggvärdena i Experience Manager Assets matchar Workfront.

* Taggar och Workfront-fältvärden måste överensstämma exakt med stavning och format.
* Workfront-fältvärden som mappas till Experience Manager-resurstaggar måste vara gemener, även om taggen i Experience Manager Assets verkar ha versaler.
* Workfront fältvärden får inte innehålla blanksteg.
* Fältvärdet i Workfront måste även innehålla mappstrukturen för Experience Manager Assets-taggen.
* Om du vill mappa flera enkelradiga textfält till taggar anger du en kommaseparerad lista över taggvärdena i Workfront-sidan av metadatamappningen och `xcm:keywords` på Experience Manager Assets sida. Varje fältvärde mappas till en separat tagg. Du kan använda ett beräkningsfält för att kombinera flera Workfront-fält till ett enda kommaseparerat textfält.
* Du kan mappa värden från nedrullningsbara listor, alternativknappar och kryssrutefält genom att ange en kommaavgränsad lista med tillgängliga värden i det fältet.


>[!INFO]
>
>**Exempel**: För att matcha taggen som visas i mappstrukturen här är fältvärdet i Workfront `landscapes:trees/spruce`. Lägg märke till de gemena bokstäverna i fältvärdet för Workfront.
>
>Om du vill att taggen ska vara objektet längst till vänster i taggträdet måste den följas av ett kolon. I det här exemplet skulle fältvärdet i Workfront vara `landscapes:`.
>
>![Mappstruktur i AEM](assets/aem-folder-structure-with-red-boxes.png)


När du har skapat taggarna i Experience Manager Assets visas de i listrutan Taggar i avsnittet Metadata. Om du vill länka ett fält till en tagg väljer du `xcm:keywords` i listrutan för Experience Manager Assets i metadatamappningsområdet.

Mer information om taggar i Experience Manager Assets, inklusive hur du skapar och hanterar taggar, finns i [Administrera taggar](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Anpassade metadatafält för Experience Manager Assets**

Du kan mappa både inbyggda och anpassade Workfront-fält till anpassade metadatamatafält i Experience Manager Assets.

Anpassade metadatafält som skapas i Experience Manager Assets ordnas i sina egna avsnitt i området för metadatainställningar.

![anpassad metadatasektion](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront**

Du kan mappa både inbyggda och anpassade Workfront-fält till Experience Manager Assets. Följande fältvärden måste matcha i både fall och stavning mellan Workfront och Experience Manager Assets:

* Nedrullningsbara fält
* Markera flera fält

>[!TIP]
>
> Om du vill kontrollera om fältvärdena matchar exakt går du till
>
> * Inställningar > Anpassad Forms i Workfront eller fältet i objektet
> * Assets > metadata schemas in Experience Manager Assets

+++

### Mappa metadata för resurser

Metadata mappas när en resurs överförs från [!DNL Workfront] för första gången. Dokument med inbyggda eller anpassade fält mappas automatiskt till de angivna fälten första gången en resurs skickas till [!DNL Experience Manager Assets].

Så här mappar du metadata för resurser:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. I **[!UICONTROL [!DNL Workfront] field]** väljer du ett inbyggt eller anpassat Workfront-fält.

   >[!NOTE]
   >
   >Du kan mappa en enda [!DNL Workfront] fält till flera [!UICONTROL Experience Manager Assets] fält. Du kan inte mappa flera [!DNL Workfront] fält till ett enda [!DNL Experience Manager Assets] fält.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. I [!DNL Experience Manager Assets] -fält, söka igenom de redan ifyllda kategorierna eller ange minst två bokstäver i sökfältet för att få tillgång till ytterligare kategorier.
1. Upprepa steg 2 och 3 efter behov.
   ![metadatafält](assets/metadata-no-asset-toggle.png)
1. Klicka [!UICONTROL Save] eller gå vidare till [Ställ in arbetsflöden](#set-up-workflows-optional) i den här artikeln.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## Ställa in arbetsflöden (valfritt)

Ett arbetsflöde är en uppsättning åtgärder som kopplar Workfront till Adobe Experience Manager as a Cloud Service. Som Workfront-administratör kan du konfigurera arbetsflöden i Workfront och sedan tilldela dem till Projektmallar. När ett projekt skapas med en projektmall som ett arbetsflöde är tilldelat till, aktiveras de åtgärder som definieras i arbetsflödet.

De standardvärden för arbetsflöde som du anger i integreringen kan åsidosättas på projektmalls- och projektnivå.

Följande arbetsflöden är tillgängliga i Adobe Experience Manager-integreringen:

* [Skapa länkade Adobe Experience Manager-mappar](#create-adobe-experience-manager-linked-folders)
* [Publicera resurser som skickas till Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Skapa länkade Adobe Experience Manager-mappar

1. Växla **[!UICONTROL Create Linked folder]** på.
1. Välj en mappsökväg för att ange var du vill att alla länkade mappar som är associerade med den här integreringen ska vara.
   ![Navigering för länkad mapp](assets/select-folder-aem-integration.png)
1. Aktivera **[!UICONTROL Append Portfolio and Program Names]** om du vill att Portfolio och programnamn ska inkluderas automatiskt i slutet av den länkade mappens namn.
1. Klicka **[!UICONTROL Save]** eller gå vidare till [Publicera resurser som skickas till Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) i den här artikeln.

### Publicera resurser som skickas till Adobe Experience Manager Assets

1. Växla på **[!UICONTROL Publish assets automatically]**.
1. Markera rutan bredvid den plats där du vill publicera resurser som skickats till Adobe Experience Manager-resurser. Du kan aktivera ett eller båda alternativen.
1. (Villkorligt) Om du har aktiverat alternativet Brand Portal väljer du den Brand Portal där du vill publicera resurser.
1. Klicka **[!UICONTROL Save]** eller gå vidare till [Konfigurera länkade mappar (valfritt)](#set-up-linked-folders-optional) i den här artikeln.

## Konfigurera länkade mappar (valfritt)

Du kan tillåta användare att skapa mappar länkade till [!DNL Experience Manager] när du befinner dig i [!DNL Workfront] projekt. När en mapp är länkad visas alla resurser som läggs till i mappen automatiskt i båda [!DNL Workfront] och [!DNL Experience Manager]. När en resurs läggs till i den länkade mappen i [!DNL Workfront] för första gången skickas resursens metadata till [!DNL Experience Manager Assets].

I stegen nedan anger du var du vill att de länkade mapparna ska skapas. Varje integrering kan bara ha en plats för alla länkade mappar.

Så här konfigurerar du länkade mappar:

1. Växla **[!UICONTROL Enable Linked folder]** på.
1. Välj en mappsökväg för att ange var du vill att alla länkade mappar som är associerade med den här integreringen ska vara.

   >[!NOTE]
   >
   >Användare behöver skrivåtkomst i [!DNL Adobe Experience Manager Assets] till den mapp som har angetts för att skapa en länkad mapp.

1. Klicka på **[!UICONTROL Save]**.

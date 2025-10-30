---
product-area: documents
navigation-topic: approvals
title: Använda Adobe Experience Manager med Frame.io-integrering
description: Använda Adobe Experience Manager med Frame.io-integrering
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cb2a17991a5562c6e734eaa0ada781d706dc5a77
workflow-type: tm+mt
source-wordcount: '1594'
ht-degree: 0%

---


# Använda Adobe Experience Manager med Frame.io-integrering

Du kan använda &#x200B; [!DNL Experience Manager Assets] för att hantera och lagra dina digitala resurser som har gått igenom gransknings- och godkännandecykeln. Tack vare integreringen kan ni utnyttja funktionerna i Adobe Experience Manager, Frame.io och Workfront för att effektivisera innehållshanteringen och samarbetet.

## Konfigurera Experience Manager Assets-integrering

Du kan koppla ditt arbete till ditt innehåll i [!DNL Experience Manager Assets] &#x200B;:

* Överför resurser och metadata från [!DNL Adobe Workfront] till [!DNL Experience Manager Assets]-&#x200B;
* Underlätta versionsanvändning
* Spåra metadata för resurser
* Synkronisera projektmetadata mellan [!DNL Workfront] och [!DNL Experience Manager Assets]

>[!NOTE]
>
>Du kan också ansluta flera [!DNL Experience Manager Assets]-databaser till en [!UICONTROL Workfront] -miljö, eller flera [!DNL Workfront] -miljöer till en [!DNL Experience Manager Assets] -databas över olika organisations-ID:n. Följ konfigurationsinstruktionerna i den här artikeln för varje integrering som du vill konfigurera.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table>
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Prime eller Ultimate</p>
    <p>Arbetsflöde Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront-licenser
   </td>
   <td>
  <p>Så här konfigurerar du integrationen:</p>
   <p>Standard</p>
   <p>Plan</p>

<p>Skicka dokument till Experience Manager Assets:</p>
   <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Adobe Experience Manager-licenser
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td>Ytterligare produkter
   </td>
   <td>Du måste ha [!DNL Experience Manager Assets as a Cloud Service] och du måste läggas till i produkten som en användare.
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar,

* Du måste ha [!DNL Workfront] och [!DNL Adobe Experience Manager Assets] kopplade till ett organisations-ID i [!DNL Adobe Admin Console]. Mer information finns i [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
* Din Workfront-instans måste använda Adobe Enterprise Storage.


## Ställ in integreringsinformation

{{step-1-to-setup}}

1. Välj **[!UICONTROL Documents]** i den vänstra panelen och välj sedan **[!UICONTROL [!DNL Experience Manager] Integration]**.
1. Välj **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. I fältet **[!UICONTROL Name]** anger du det namn som du vill att användare ska se när de interagerar med den här integreringen i Workfront och Experience Manager Assets.
1. I fältet **[!UICONTROL Navigation URL]** fyller systemet automatiskt i navigerings-URL:en. Den här skrivskyddade URL:en används för att länka till din organisations [!DNL Experience Manager]-instans från [!UICONTROL Main Menu] för snabb åtkomst.
1. Välj en databas i listrutan **[!UICONTROL [!DNL Experience Manager] Assets repository]**. Systemet fyller automatiskt i alla [!DNL Experience Manager]-databaser som är associerade med det organisations-ID som din användarprofil är tilldelad till.
   ![välj Experience Manager-databas](assets/setup-information.png)

1. Klicka på **[!UICONTROL Save]** eller gå vidare till avsnittet [Konfigurera metadata (valfritt)](#set-up-metadata-optional) i den här artikeln.

   >[!IMPORTANT]
   >
   >På grund av integreringens komplexitet kan du inte ändra databasen efter att du har sparat den ursprungliga konfigurationen.


## Konfigurera metadata (valfritt)

Du kan mappa [!DNL Workfront] objektdata till resursmediefält i [!DNL Experience Manager] Assets.

>[!NOTE]
>
>Du kan bara mappa metadata i en riktning: från [!DNL Workfront] till [!DNL Experience Manager]. Metadata för dokument som är länkade till [!DNL Workfront] från [!DNL Experience Manager] kan inte överföras till [!DNL Workfront].

### Konfigurera metadatafält

Innan du börjar mappa metadatafält måste du konfigurera metadatafält i både Workfront och Experience Manager Assets.

Konfigurera metadatafält:

1. Konfigurera ett metadataschema i [!DNL Experience Manager Assets] enligt beskrivningen i [Konfigurera metadatamappning för resurser mellan Adobe [!DNL Workfront]  och [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. Konfigurera anpassade formulärfält i Workfront. [!DNL Workfront] har många inbyggda anpassade fält som du kan använda. Du kan även skapa egna anpassade fält enligt beskrivningen i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

+++ **Expandera om du vill visa mer information om Workfront- och Experience Manager Assets-fält som stöds** 

**Experience Manager Assets-taggar**

Du kan mappa ett fält som stöds av Workfront till en tagg i Experience Manager Assets. För att göra detta måste du se till att taggvärdena i Experience Manager Assets matchar Workfront.

* Taggar och Workfront-fältvärden måste överensstämma exakt med stavning och format.
* Workfront-fältvärden som mappas till Experience Manager-resurstaggar måste vara gemener, även om taggen i Experience Manager Assets verkar ha versaler.
* Workfront fältvärden får inte innehålla blanksteg.
* Fältvärdet i Workfront måste även innehålla mappstrukturen för Experience Manager Assets-taggen.
* Om du vill mappa flera enkelradiga textfält till taggar anger du en kommaseparerad lista över taggvärdena i Workfront-sidan av metadatamappningen och `xcm:keywords` på Experience Manager Assets-sidan. Varje fältvärde mappas till en separat tagg. Du kan använda ett beräkningsfält för att kombinera flera Workfront-fält till ett enda kommaseparerat textfält.
* Du kan mappa värden från nedrullningsbara listor, alternativknappar och kryssrutefält genom att ange en kommaavgränsad lista med tillgängliga värden i det fältet.


>[!INFO]
>
>**Exempel**: För att matcha taggen som visas i mappstrukturen här är fältvärdet i Workfront `landscapes:trees/spruce`. Lägg märke till de gemena bokstäverna i fältvärdet för Workfront.
>
>Om du vill att taggen ska vara objektet längst till vänster i taggträdet måste den följas av ett kolon. I det här exemplet skulle fältvärdet i Workfront vara `landscapes:` för att mappa till taggen landscapes.
>
>![Mappstruktur i AEM](assets/aem-folder-structure-with-red-boxes.png)


När du har skapat taggarna i Experience Manager Assets visas de i listrutan Taggar i avsnittet Metadata. Om du vill länka ett fält till en tagg väljer du `xcm:keywords` i listrutan Experience Manager Assets i metadatamappningsområdet.

Mer information om taggar i Experience Manager Assets, inklusive hur du skapar och hanterar taggar, finns i [Administrera taggar](https://experienceleague.adobe.com/en/docs/experience-manager-64/administering/contentmanagement/tags).

**Anpassade metadataschfält för Experience Manager Assets**

Du kan mappa både inbyggda och anpassade Workfront-fält till anpassade metadatamatafält i Experience Manager Assets.

Anpassade metadatafält som skapas i Experience Manager Assets ordnas i sina egna avsnitt i området för metadatainställningar.

![anpassad metadatasektion](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront-fält**

Du kan mappa både inbyggda och anpassade Workfront-fält till Experience Manager Assets. Följande fältvärden måste matcha i både fall och stavning mellan Workfront och Experience Manager Assets:

* Nedrullningsbara fält
* Markera flera fält

>[!TIP]
>
> Om du vill kontrollera om fältvärdena matchar exakt går du till
>
> * Inställningar > Anpassad Forms i Workfront eller fältet i objektet
> * Assets > metadatamaterial i Experience Manager Assets

+++

### Mappa metadata för resurser

Metadata mappas när en resurs överförs från [!DNL Workfront] för första gången. Dokument med inbyggda eller anpassade fält mappas automatiskt till angivna fält första gången en resurs skickas till [!DNL Experience Manager Assets].

Så här mappar du metadata för resurser:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. I kolumnen **[!UICONTROL [!DNL Workfront] field]** väljer du ett inbyggt eller anpassat Workfront-fält.

   >[!NOTE]
   >
   >Du kan mappa ett enskilt [!DNL Workfront]-fält till flera [!UICONTROL Experience Manager Assets]-fält. Du kan inte mappa flera [!DNL Workfront]-fält till ett enskilt [!DNL Experience Manager Assets]-fält.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. I fältet [!DNL Experience Manager Assets] kan du söka igenom de förifyllda kategorierna eller ange minst två bokstäver i sökfältet för att få åtkomst till ytterligare kategorier.
1. Upprepa steg 2 och 3 efter behov.
   ![metadatafält](assets/metadata-no-asset-toggle.png)
1. Klicka på [!UICONTROL **Spara**] eller gå till avsnittet [Synkronisering av objektmetadata](#object-metadata-sync) i den här artikeln.



### Synkronisering av objektmetadata

Ett [!DNL Experience Manager]-fält som mappas till [!DNL Workfront] portfölj-, program-, projekt-, uppgifts-, utgåva- och dokumentfält uppdateras automatiskt när fältet ändras i [!DNL Workfront].

När det här alternativet är aktiverat visar alla resurser som har överförts till Adobe Experience Manager en realtidsvy över dokumentets Adobe Experience Manager-metadata på dokumentinformationssidan i Workfront.

1. Aktivera fältet **[!UICONTROL Sync object metadata]** och klicka sedan på **Spara**.

>[!IMPORTANT]
>
>Användare måste ha skrivåtkomst i [!DNL Experience Manager] för resurser som finns i objektet för att metadata ska kunna synkroniseras när det uppdateras.


## Skicka ett dokument till Experience Manager Assets eller Assets Essentials

Du kan skicka dokument från Workfront till Experience Manager Assets eller Assets Essentials. Dokument som överförts och skickats från Workfront till Assets Essentials räknas fortfarande av mot den totala dokumentlagringen.

Assets som skickas till Experience Manager via den här integreringen har en storleksgräns på **5 GB**.

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Alla metadata som har konfigurerats för att mappa för överordnade objekt skickas också. Mer information om hur du konfigurerar metadatamappning finns i [Konfigurera Experience Manager Assets as a Cloud Service-integreringen](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera Experience Manager Assets Essentials-integreringen](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exempel** När du först skickar en resurs som är kopplad till ett projekt mappas metadata till Experience Manager Assets eller Assets Essentials samt alla mappade metadata från överordnade objekt som en portfölj och ett program.



### Skicka ett dokument från Workfront

När en användare skickar ett dokument från Workfront till Experience Manager Assets eller Assets Essentials överförs mappade metadata längs dokumentet. När dokumentet har skickats återspeglas inte ändringar som görs i dokumentets metadata i Workfront i Assets eller Resurser Essentials. Om ett mappat fält i Workfront ändras måste du skicka en ny version av dokumentet med de uppdaterade metadata till Assets eller Assets Essentials.

Skicka ett dokument:

1. Gå till området **Dokument** i Workfront och markera det dokument som du vill skicka.
1. Klicka på **Skicka till** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för den här integreringen, så den får inte särskilt nämna Assets eller Assets Essentials.

   ![Skicka till](assets/send-to-aem.png)

1. Välj vart du vill att resursen ska gå och klicka sedan på **Välj mapp**.
1. Klicka på **Spara** när du har hittat önskat mål.

### Skicka en ny version

Du kan lägga till en ny version i ett dokument som du tidigare har överfört till Workfront. Mer information finns i [Överföra en ny version av ett dokument](/help/quicksilver/documents/managing-documents/upload-new-document-version.md). När den senaste versionen har överförts kan du skicka den till Assets Essentials. Om ett mappat fält i Workfront har ändrats uppdateras metadata i Assets Essentials när den skickas.

>[!IMPORTANT]
>
>Innan du överför en ny version till Workfront rekommenderar vi att du byter namn på filen. Om du överför en ny version med exakt samma filnamn som en tidigare version kan du bara hämta den senaste versionen från Workfront. Alla versioner kan laddas ned från Experience Manager Assets eller Assets Essentials oavsett filnamn. <!--Is this still a thing with ESM?-->

Så här skickar du den senaste versionen:

1. Gå till området **Dokument** i Workfront och leta upp dokumentet.
1. Välj **Skicka till** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Assets eller Assets Essentials.

   ![Skicka till](assets/send-to-aem.png)

1. Klicka på **Spara**. Den nya versionen sparas på samma plats som den tidigare versionen.

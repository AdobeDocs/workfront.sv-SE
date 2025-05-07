---
title: Konfigurera dokumentintegreringar
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Som Adobe Workfront-administratör kan du konfigurera dokumentintegreringar för att hantera dokument i Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ec0e2be036ce1298e285ce85cdeddae97cd1f144
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 0%

---

# Konfigurera dokumentintegreringar

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Som [!DNL Adobe Workfront]-administratör kan du konfigurera dokumentintegreringar för att hantera dokument i [!UICONTROL Workfront]. Du kan också konfigurera [!UICONTROL Workfront] så att dokument bara lagras i Document Services-program och inte i själva [!UICONTROL Workfront]. Mer information finns i [Uppdatera och länka ett dokument från [!UICONTROL Workfront] till en extern molnleverantör](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Om du vill tillåta öppen kommunikation mellan [!DNL Workfront Proof] och [!DNL Workfront]-servrarna kan du behöva lägga till vissa IP-adresser i tillåtelselista. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: [!UICONTROL Standard]</p>
       <p>eller</p>
       <p>Aktuell: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrationer som stöds

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Du kan konfigurera följande integreringar för hantering av dokument:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Genom att länka korrektur från [!DNL Workfront Proof] kan du göra korrektur som ursprungligen skapades i [!DNL Workfront Proof] tillgängliga i [!DNL Workfront]. För de aktuella planerna krävs en [!UICONTROL Pro] [!DNL Workfront]-plan eller högre för att den här funktionen ska kunna användas. Den här funktionen är tillgänglig för alla planer för nya planer. Mer information om olika tillgängliga planer finns i [Workfront-planer](https://business.adobe.com/products/workfront/pricing.html).

* [!DNL Microsoft SharePoint]

  Mer information om integrering med [!DNL SharePoint] finns i [Konfigurera  [!DNL SharePoint] integreringen](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Tredjepartsleverantörer av molndokument:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]
   * Snabbhet

  >[!TIP]
  >
  >Du kan granska och godkänna dokument som är länkade från en extern molnleverantör på samma sätt som du granskar och godkänner dokument som överförts direkt till [!DNL Workfront].

* Andra dokumentleverantörer (via anpassade dokumentintegreringar).

  För de aktuella planerna krävs en [!UICONTROL Pro] [!DNL Workfront]-plan eller högre för att den här funktionen ska kunna användas. Den här funktionen är tillgänglig för alla planer för nya planer. Mer information om olika tillgängliga planer finns i [Workfront-planer](https://business.adobe.com/products/workfront/pricing.html).

Dessutom kan du förbättra dokumentupplevelsen av [!DNL Workfront] med en DAM-integrering från tredje part. Administratörer måste aktivera de här funktionerna för att användare ska kunna länka tjänsten till sitt [!DNL Workfront]-konto.

## Konfigurera integreringar för att hantera dokument

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]i den vänstra panelen.**

1. (Valfritt) Om du vill lagra dokument i ett Document Services-program och inte i [!DNL Workfront] väljer du **[!UICONTROL Prevent Users From Storing Documents in [!DNL Workfront]].**

1. Välj de integreringar du vill aktivera.
1. Klicka på **[!UICONTROL Save]**.

Om du konfigurerar integreringar med [!DNL Workfront DAM] kan du aktivera [!DNL Workfront] för att inkludera metadata med dokument. Mer information om att mappa metadata finns i [Konfigurera metadatamappning](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Konfigurera anpassade dokumentintegreringar

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Med en anpassad dokumentintegrering kan [!DNL Workfront]-användare länka filer till [!DNL Workfront] från praktiskt taget vilket system som helst, förutsatt att systemet är gjort för att fungera med [!DNL Workfront].

För att göra den anpassade integrationen tillgänglig för användarna måste du först skapa integreringen. Mer information om hur du skapar integreringar som ska användas med [!DNL Workfront] finns i [API:t för dokumentwebbhooks](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

När den anpassade dokumentintegreringen har skapats kan du göra den tillgänglig för användare på din webbplats.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]** i den vänstra panelen.

1. Klicka på **[!UICONTROL Add Custom integration]**.
1. Ange följande information för att konfigurera integreringen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Namnet på den anpassade integrationen. Detta är det namn som användare ser när de använder integreringen i Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>Den grundläggande HTTP- eller säkra HTTP-URL:en för API-anrop. Exempel: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>Den autentiseringsmetod som ska användas när auktoriserade API-anrop görs till den anpassade integreringen.</p> 
       <ul> 
        <li>Om du väljer <strong>[!UICONTROL OAuth]</strong> fortsätter du med steg 5.</li> 
        <li>Om du väljer <strong>[!UICONTROL ApiKey]</strong> fortsätter du med steg 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du valde **[!UICONTROL OAuth]**-autentisering för **[!UICONTROL Authentication Type]** anger du följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>Den fullständiga URL som används för användarautentisering. [!DNL Workfront] navigerar användare till den här adressen som en del av OAuth-etableringsprocessen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>Den fullständiga API-URL som används för att hämta OAuth-tokens.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>OAut-klient-ID för den här integreringen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>OAut-klienthemligheten för den här integreringen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Parameters]</td> 
      <td> <p>Ange valfria värden som ska läggas till i frågesträngen för varje API-anrop. Till exempel access_type=offline.</p> <p>Om du vill lägga till flera begärandeparametrar klickar du på <strong>+Lägg till begärandeparameter</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Den omdirigerings-URI [!DNL Workfront] som visas längst ned på sidan [!UICONTROL Custom Integration] listar den URI som används för att registrera den här integreringen med den externa dokumentprovidern.

1. (Villkorligt) Om du valde **[!UICONTROL ApiKey]**-autentisering för **[!UICONTROL Authentication Type]** anger du API-nyckeln som utfärdades av den anpassade dokumentprovidern.

   [!DNL Workfront] använder den här API-nyckeln för att göra auktoriserade API-anrop till dokumentprovidern.

1. Klicka på **[!UICONTROL Save]** för att skapa integreringen.

## Använd dokumentintegreringar

Mer information om hur användare kan använda korrektur finns i [Skapa korrektur](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Mer information om hur användare kan använda dokumentintegreringar från tredje part efter att du har konfigurerat dem finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Konfigurera [!DNL Workfront] att skicka metadata till [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

När du skickar ett dokument från [!DNL Workfront] till [!DNL Workfront DAM] kan du även skicka information som är kopplad till det dokumentet. Information om dokumentet mappas till [!DNL Workfront DAM] som metadata.

Informationen mappas endast en gång, från [!DNL Workfront] till [!DNL Workfront DAM], och överförs endast när dokumentet överförs till [!DNL Workfront DAM]. Eventuella framtida ändringar i Workfront-fälten kommer inte att uppdatera metadatafält i [!DNL Workfront DAM] efter att dokumentet redan har överförts.\
Du kan mappa samma [!DNL Workfront]-fält till olika [!DNL Workfront DAM]-fält, men du kan inte använda samma [!DNL Workfront DAM]-fält för flera [!DNL Workfront]-fält.

Om du måste konfigurera flera [!DNL Workfront]-fält för export till ett [!DNL Workfront DAM]-fält måste du först skapa ett beräknat anpassat fält i [!DNL Workfront] för att visa alla enskilda anpassade fält för ett objekt. Mappa sedan det beräknade [!DNL Workfront]-fältet till ett [!DNL Workfront DAM]-fält.\
Mer information om beräknade anpassade fält finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Mappningen påverkar alla dokument som överförts av användare från [!DNL Workfront] till [!UICONTROL Workfront] DAM.

Som [!DNL Workfront]-administratör måste du aktivera [!DNL Workfront DAM] i Workfront innan du kan mappa fälten för metadatamappningsprocessen.

Så här konfigurerar du [!DNL Workfront] att skicka metadata till [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. I fältet **[!UICONTROL Select Source Field for Mapping]** börjar du skriva namnet på det Workfront-fält som du vill mappa till [!DNL Workfront DAM] och markerar det sedan när du ser det i listan.
1. I **[!UICONTROL Select Target Field for Mapping]** markerar du det [!DNL Workfront DAM]-fält som du vill fylla i med informationen i det markerade [!DNL Workfront]-fältet.

   >[!NOTE]
   >
   > Alla dokument som skickas till [!DNL Workfront DAM] av användare som har behörighet att göra det har sina metadata uppdaterade med [!DNL Workfront]-fälten mappade här, när de överförs till [!DNL Workfront DAM].

1. Klicka på **[!UICONTROL Add Mapping]**.

1. Fortsätt lägga till fler [!UICONTROL Workfront] fält och motsvarande [!DNL Workfront DAM] fält.

### Ta bort mappade fält

{{step-1-to-setup}}

1. Expandera **[!UICONTROL Documents]** och klicka sedan på **[!UICONTROL Metadata Mapping]**.

1. I listan med fält väljer du något av de fält som du vill ta bort från metadatamappningen.
1. Klicka på **[!UICONTROL Delete]**.

   Fälten tas bort från metadatamappningen och informationen i dem överförs inte till [!DNL Workfront DAM] med de överförda dokumenten.


## Begränsningar

### Integrering med Google Drive

* När en länkad mapp läggs till i Workfront läggs filerna i mappen inte längre till automatiskt.
   * Du kan lägga till Google-mappen i Workfront utan filerna och sedan lägga till de enskilda filerna i Workfront. Filerna läggs automatiskt till i Google-mappen i Workfront.
eller
   * Du kan skapa en dokumentmapp i Workfront, sedan markera alla filer i Google-mappen och lägga till dem i Workfront-mappen.


* Integreringen av Google Drive-dokumentet har stöd för att lägga till filer från My Drive-området på din Google Drive. Du kan inte lägga till mappar eller bilder från en delad enhet. Läs mer om [Google delade enheter](https://support.google.com/a/users/answer/7212025?hl=en).

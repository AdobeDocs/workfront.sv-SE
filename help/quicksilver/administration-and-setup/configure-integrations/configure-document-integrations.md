---
title: Konfigurera dokumentintegreringar
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Konfigurera dokumentintegreringar
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 456c7b21835c96912e8974063f7797283dcb4e6d
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Konfigurera dokumentintegreringar

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Som en [!DNL Adobe Workfront] kan du konfigurera dokumentintegreringar för att hantera dokument i [!UICONTROL Workfront]. Du kan också konfigurera [!UICONTROL Workfront] så att dokument bara lagras i Document Services-program och inte i [!UICONTROL Workfront] själv. Mer information finns i [Uppdatera och länka ett dokument från [!UICONTROL Workfront] till en extern molnleverantör](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Tillåt öppen kommunikation mellan [!DNL Workfront Proof] och [!DNL Workfront] -servrar kan du behöva lägga till vissa IP-adresser i tillåtelselista. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Åtkomstkrav

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Integrationer som stöds

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Du kan konfigurera följande integreringar för hantering av dokument:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Länka korrektur från [!DNL Workfront Proof] gör att du kan skapa korrektur som ursprungligen skapades i [!DNL Workfront Proof] finns inom [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] Plan eller högre krävs för att den här funktionen ska kunna användas. Mer information om olika planer finns i [Workfront Planer.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   Mer information om integrering med [!DNL SharePoint], se [Konfigurera [!DNL SharePoint] integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Tredjepartsleverantörer av molndokument:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >Du kan granska och godkänna dokument som är länkade från en extern molnleverantör på samma sätt som du granskar och godkänner dokument som överförs direkt till [!DNL Workfront].

* Andra dokumentleverantörer (via anpassade dokumentintegreringar).

   A [!UICONTROL Pro] [!DNL Workfront] Plan eller högre krävs för att den här funktionen ska kunna användas. Mer information om olika planer finns i [[!DNL Workfront] Planer.](https://www.workfront.com/plans)

Dessutom kan du förbättra [!DNL Workfront] dokumentupplevelse med ett DAM-system (Digital Asset Management) eller med DAM-integreringar från tredje part. Administratörer måste aktivera de här funktionerna för att användarna ska kunna länka tjänsten till sina [!DNL Workfront] konto. Mer information om Workfront DAM finns i [Hantera dokument med [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Konfigurera integreringar för att hantera dokument

1. Logga in på [!DNL Workfront] som administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers].**

1. (Valfritt) Lagrade dokument i ett Document Services-program och inte i [!DNL Workfront], markera **[!UICONTROL Prevent Users From Storing Documents in [!DNL Workfront]].**

1. Välj de integreringar du vill aktivera.
1. Klicka på **[!UICONTROL Save]**.

Om du skapar integreringar med [!DNL Workfront DAM]kan du aktivera [!DNL Workfront] för att inkludera metadata i dokument. Mer information om att mappa metadata finns i [Ställ in metadatamappning](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Konfigurera anpassade dokumentintegreringar

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Anpassad dokumentintegrering tillåter [!DNL Workfront] användare länka filer till [!DNL Workfront] från praktiskt taget vilket system som helst, förutsatt att systemet är utformat för att fungera med [!DNL Workfront].

För att göra den anpassade integrationen tillgänglig för användarna måste du först skapa integreringen. Mer information om hur du skapar integreringar som ska användas med [!DNL Workfront], se [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

När den anpassade dokumentintegreringen har skapats kan du göra den tillgänglig för användare på din webbplats.

1. Logga in på [!DNL Workfront] som administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration].**

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
      <td>Den grundläggande HTTP- eller säkra HTTP-URL:en för API-anrop. Till exempel: <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>Den autentiseringsmetod som ska användas när auktoriserade API-anrop görs till den anpassade integreringen.</p> 
       <ul> 
        <li>Om du väljer <strong>[!UICONTROL OAuth]</strong>fortsätter du med steg 6.</li> 
        <li>Om du väljer <strong>[!UICONTROL ApiKey]</strong>fortsätter du med steg 7.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du har valt **[!UICONTROL OAuth]** autentisering för **[!UICONTROL Authentication Type]**, ange följande information:

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
      <td> <p>Ange valfria värden som ska läggas till i frågesträngen för varje API-anrop. Till exempel access_type=offline.</p> <p>Om du vill lägga till flera frågeparametrar klickar du på <strong>+Lägg till begärandeparameter</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >The [!DNL Workfront] Omdirigerings-URI som visas längst ned [!UICONTROL Custom Integration] På sidan visas den URI som används för att registrera integreringen med den externa dokumentprovidern.

1. (Villkorligt) Om du har valt **[!UICONTROL ApiKey]** autentisering för **[!UICONTROL Authentication Type]** anger du API-nyckeln som utfärdades av den anpassade dokumentprovidern.

   [!DNL Workfront] använder den här API-nyckeln för att göra auktoriserade API-anrop till dokumentprovidern.

1. Klicka **[!UICONTROL Save]** för att skapa integreringen.

## Använd dokumentintegreringar

Mer information om hur användare kan använda [!DNL Workfront DAM], se [Hantera dokument med [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Mer information om hur användare kan använda korrektur finns i [Skapa korrektur](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Information om hur användare kan använda dokumentintegreringar från tredje part efter att du har konfigurerat dem finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Konfigurera [!DNL Workfront] för att skicka metadata till [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

När ett dokument skickas från [!DNL Workfront] till [!DNL Workfront DAM]kan du också skicka information som är kopplad till det dokumentet. Information om dokumentet mappas till [!DNL Workfront DAM] som metadata.

Informationen mappas endast en gång, från [!DNL Workfront] till [!DNL Workfront DAM] och överförs bara när dokumentet överförs till [!DNL Workfront DAM]. Eventuella framtida ändringar i Workfront-fälten kommer inte att uppdatera metadatafälten i [!DNL Workfront DAM] när dokumentet redan har överförts.\
Du kan mappa samma [!DNL Workfront] fält till olika [!DNL Workfront DAM] fält, men du kan inte använda samma [!DNL Workfront DAM] fält för flera [!DNL Workfront] fält.

Om du måste konfigurera flera [!DNL Workfront] fält att exportera till ett [!DNL Workfront DAM] fält, skapa först ett beräknat anpassat fält i [!DNL Workfront] om du vill visa alla enskilda anpassade fält för ett objekt. Mappa sedan den beräknade [!DNL Workfront] fält till ett [!DNL Workfront DAM] fält.\
Mer information om beräknade anpassade fält finns i [Lägga till beräknade data i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Mappningen påverkar alla dokument som överförts av en användare från [!DNL Workfront] till [!UICONTROL Workfront] DAM.

Som [!DNL Workfront] administratör måste du aktivera [!DNL Workfront DAM] i Workfront innan du kan mappa fälten för metadatamappningsprocessen. Mer information om hur du aktiverar [!DNL Workfront DAM], se [Konfigurera Workfront att skicka metadata till [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

Konfigurera [!DNL Workfront] för att skicka metadata till [!DNL Workfront DAM]:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. I **[!UICONTROL Select Source Field for Mapping]** börjar du skriva in namnet på det Workfront-fält som du vill mappa till [!DNL Workfront DAM]markerar du den när du ser den i listan.
1. I **[!UICONTROL Select Target Field for Mapping]** väljer du [!DNL Workfront DAM] fält som du vill fylla i med informationen i det markerade [!DNL Workfront] fält.

   >[!NOTE]
   >
   > Alla dokument skickade till [!DNL Workfront DAM] av användare som har behörighet att göra detta, får sina metadata uppdaterade med [!DNL Workfront] fält mappas här, när de överförs till [!DNL Workfront DAM].

1. Klicka på **[!UICONTROL Add Mapping]**.

1. Fortsätt lägga till mer [!UICONTROL Workfront] fält och motsvarande [!DNL Workfront DAM] fält.

### Ta bort mappade fält

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Expandera **[!UICONTROL Documents]** och sedan klicka **[!UICONTROL Metadata Mapping]**.

1. I listan med fält väljer du något av de fält som du vill ta bort från metadatamappningen.
1. Klicka på **[!UICONTROL Delete]**.

   Fälten tas bort från metadatamappningen och informationen i dem överförs inte till [!DNL Workfront DAM] med de överförda dokumenten.

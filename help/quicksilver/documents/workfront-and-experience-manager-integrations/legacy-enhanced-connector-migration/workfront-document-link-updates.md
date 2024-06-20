---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrera länkade mappar och dokument
description: Du kan använda API:t för att migrera länkade mappar och dokument till Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Migrera länkade mappar och dokument

Du kan använda API:t för att migrera länkade mappar och dokument till Adobe Experience Manager Assets.

## Förfarande

1. Identifiera alla dokument och mappar som är länkade till den tidigare externa dokumentlagringsleverantören och notera deras interna dokument- eller mappidentifierare i Workfront samt mapp-ID:t för eventuella mappar.

   >[!NOTE]
   >
   > Du bör söka efter alla identifierade mappar eller dokument för att kontrollera att de inte redan har skapat en länk för dem med den nya providern.

1. Leta reda på dokumenten och mapparna i den nya databasen efter sökväg och slå sedan upp deras identitet i det externa systemet.

1. Skapa en mappning av det interna Workfront-id:t till ID:t i den nya externa butiken. Du behöver det här för att skapa en ny länk i följande steg.

1. Skapa en länk till ett nytt dokument eller en ny dokumentmapp i Workfront som pekar på resursen på dess nya plats via dess nya externa ID.

   1. **Dokument**: Lägg till en ny version av det befintliga dokumentet med den nya externa dokumentprovidern.
   1. **Mappar**: Skapa en ny mapp på samma plats med samma namn.

>[!CAUTION]
>
>   Ta inte bort befintliga länkade mappar. Detta kan leda till dataförlust. Om du vill ta bort gamla mapplänkar från Workfront-programmet inaktiverar du den anpassade dokumentintegreringen under Konfigurera.


## Exempelprocess för att migrera länkar

![simplified-link-flow](assets/links-flow-simplified.png)

## API-information

Mer information om Workfront API:er finns i det här avsnittet [dokumentation för utvecklare:dokument](https://developer.workfront.com/documents.html).

### Sök efter alla dokument

Sök alla **Dokument (DOCU)** Länkad till **Dokumentleverantör** av **providerType** med **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API DOCS-referens](https://developer.workfront.com/documents.html#get-/docu/search)

### Söka efter alla mappar

Sök alla **Dokumentmappar (DOCFDR)** Länkat till dokumentprovidern för **providerType** med **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API DOCS: (Slutpunkter för dokumentmapp som för närvarande inte omfattas på developer.workfront.com)

### Länka dokument

Länk **Dokument (DOCU)** från **Extern dokumentprovider** av **providerType** med **documentProviderID**.

>[!IMPORTANT]
>
>Dokument lagras tillfälligt. Det innebär att du har tillgång till alla versioner av dokumentet. När du skapar länken kan du ange det befintliga dokument-ID:t, så du skriver bara en ny version till det dokumentet, där data lagras externt i den nya providern. Detta dokument-ID är samma som det dokument-ID som finns på dokumentlänken som du ersätter. Det är samma konceptuella dokument. Du anger bara att byten för den nya versionen lagras hos en annan leverantör.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API DOCS: (interna länkslutpunkter som för närvarande inte omfattas på developer.workfront.com)

### Länka mappar

Länk **Dokumentmappar (DOCFDR)** från **Extern dokumentprovider** av **providerType** med **documentProviderID**.

>[!IMPORTANT]
>
>För mapplänkar behöver du, till skillnad från dokumentlänkar, &#39;documentFolderId&#39; för den mapp i Workfront som du vill placera den nya länken i. Detta är samma överordnade mapp, troligtvis, som den länkade mappen som vi kopierar.

>[!CAUTION]
>
>Mappar lagras inte temporärt. Ta inte bort gamla mappar. Inaktivera den anpassade dokumentintegreringen i inställningsområdet för att ta bort gamla mappar.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API DOCS: (interna länkslutpunkter som för närvarande inte omfattas på developer.workfront.com)

## Viktiga termer

* **Dokument**: En digital resurs inom Workfront

* **Dokumentmapp**: En behållare för digitala resurser i Workfront

* **Dokument-ID**: Workfront internt ID för en digital resurs

* **Dokumentmapp-ID**: Workfront internt ID för en digital resursmapp

* **Dokumentleverantörs-ID**: ID kopplat till specifika dokumentleverantörer

>[!IMPORTANT]
>
> För varje given dokumentprovidertyp kan kunden ha flera anslutna instanser. De kan till exempel ha flera AEM databaser länkade. Eller flera länkade Google Drive-instanser. Dokumentleverantörens ID anger den specifika instansen av anslutningstypen som du vill ersätta eller växla till.

* **Typ av dokumentlagringsprovider (även &quot;extern integreringstyp&quot;)**: Den typ av dokumentlagringsleverantörsintegrering som Workfront stöder. Antingen via en dedikerad integrering eller en&quot;anpassad integrering&quot;.

* **Aktuella dokumentlagringsprovidertyper (providerType)**:

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **Länkat dokument**: En digital resurs som lagras hos en extern dokumentlagringsleverantör. Workfront har ett internt&quot;dokument-ID&quot; för resursen, men byten lagras externt. För att underlätta detta lagrar Workfront även ett &quot;externt dokument-ID&quot; som hjälp att hitta den externt refererade resursen i fjärrdatabasen eller fjärrbutiken.

* **Mappen Länkat dokument**: En behållare för digitala resurser som lagras hos en extern dokumentlagringsleverantör. Workfront kommer att ha ett internt &quot;dokumentmapp-ID&quot; för resursen, men byten lagras externt. För att underlätta detta lagrar Workfront även ett &quot;externt dokument-ID&quot; som hjälp att hitta den externt refererade resursen i fjärrdatabasen eller fjärrbutiken.

* **Externt dokument-ID**: ID tilldelas när resurser lagras utanför Workfront. Workfront mappar sin interna identifierare till den identifierare som används för att hitta resursen i det externa systemet via detta&quot;externa dokumentidentifierarfält&quot;. När du länkar ett dokument eller en mapp från en ny extern lagringsplats måste därför en ny extern dokumentidentifierare sättas samman i lämpligt format för att den externa dokumentleverantören ska kunna identifiera dokumentet i den nya databasen eller arkivet.

  >[!NOTE]
  >
  > Workfront har ännu ingen standard för externa dokumentidentifierare. En ny specifikation används för AEM ID, men för andra ID kan det externa dokument-ID:t ha olika former beroende på providertypen.


* **Objekttyp**: Detta är endast en API-term för det här dokumentet. Det är en typ av generiskt objekt inom Workfront som du vill interagera med. I så fall interagerar du med dokument och mappar som har typerna &quot;DOCU&quot; respektive &quot;DOCFDR&quot;.

* **Objekt-ID**: Den interna Workfront-identifieraren för det generiska objekt som du vill interagera med. Du kommer att interagera med dokument och mappar så att det blir antingen dokument-ID:t eller dokumentmapp-ID:t.

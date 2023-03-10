---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webbhooks - översikt
description: Webbhooks - översikt
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Webbhooks - översikt

Adobe Workfront Document Webhooks definierar en uppsättning API-slutpunkter genom vilka Workfront gör auktoriserade API-anrop till en extern dokumentleverantör. På så sätt kan vem som helst skapa ett plugin-program för mellanvara för vilken dokumentlagringsleverantör som helst.

![](assets/mceclip0-350x262.png)

Användarupplevelsen för webkrosbaserade integreringar liknar den för befintliga dokumentintegreringar, som Google Drive, Box och Dropbox. En Workfront-användare kan till exempel utföra följande åtgärder:

* Navigera i mappstrukturen för den externa dokumentprovidern
* Sök efter filer
* Länka filer till Workfront
* Överför filer till den externa dokumentleverantören
* Visa en miniatyrbild för dokumentet

**Referensimplementering**

Workfront tillhandahåller en referensimplementering som hjälper dig att snabbt komma igång med utvecklingen av en ny webbhooksimplementering. Kod för detta finns på [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . Implementeringen är Java-baserad och gör att Workfront kan ansluta dokument i ett nätverksfilsystem. 

## Versioner

* Version 1.0 (Releasedatum - maj 2015): Inledande specifikation

* Version 1.1 (Releasedatum - juni 2015). Uppdaterat /uploadInit - Added documentId och documentVersionId

* Version 1.2 (Releasedatum - oktober 2015): Lagt till /createFolder

* Kommande versioner (Releasedatum - TBD):

   * Lagt till/ta bort
   * Lagt till/byt namn
   * Tillagd /serviceInfo
   * Tillagd /customAction
   * Lägg till sidnumrering och parentId i /search

---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhooks API
description: Document Webhooks API
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 0%

---


# Document Webhooks API

Adobe Workfront Document Webhooks definierar en uppsättning API-slutpunkter genom vilka Workfront gör auktoriserade API-anrop till en extern dokumentleverantör. På så sätt kan vem som helst skapa ett plugin-program för mellanvara för alla dokumentlagringsleverantörer.

Användarupplevelsen för webkrosbaserade integreringar liknar den för befintliga dokumentintegreringar, som Google Drive, Box och Dropbox. En Workfront-användare kan till exempel utföra följande åtgärder:

* Navigera i mappstrukturen för den externa dokumentprovidern
* Sök efter filer
* Länka filer till Workfront
* Överför filer till den externa dokumentleverantören
* Visa en miniatyrbild för dokumentet

## Referenskörning

Workfront tillhandahåller en referensimplementering som hjälper dig att snabbt komma igång med utvecklingen av en ny webbhooksimplementering. Kod för detta finns på [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Implementeringen är Java-baserad och gör att Workfront kan ansluta dokument i ett nätverksfilsystem.

## Registrera en Webkroks-integrering

Workfront-administratörer kan lägga till en anpassad webbkrokintegrering för sitt företag genom att gå till Inställningar > Dokument > Anpassade integreringar i Workfront. På sidan Anpassad integrering i installationsprogrammet kan administratörer visa en lista över befintliga webkrok-integreringar för dokument. Från den här sidan kan integreringar läggas till, redigeras, aktiveras och inaktiveras. Om du vill lägga till en integrering klickar du på knappen &quot;Lägg till integrering&quot;.

### Tillgängliga fält

När du lägger till en integrering anger administratören värden för följande fält:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Fältnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Namn</td> 
   <td>Namnet på den här integreringen.</td> 
  </tr> 
  <tr> 
   <td>Bas-API-URL</td> 
   <td> <p>Plats för återanrops-API:t. När du anropar det externa systemet lägger Workfront bara till slutpunktsnamnet till den här adressen. Om administratören t.ex. angav Bas-API-URL:en, https://www.mycompany.com/api/v1, använder Workfront följande URL för att hämta ett dokuments metadata: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Begär parametrar</td> 
   <td> <p>Valfria värden som ska läggas till i frågesträngen för varje API-anrop. Till exempel access_type=offline.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Autentiseringstyp</td> 
   <td>OAuth2 eller ApiKey</td> 
  </tr> 
  <tr> 
   <td>Autentiserings-URL</td> 
   <td> <p>(Endast OAuth2) Den fullständiga URL som används för användarautentisering. Workfront kommer att navigera användare till den här adressen som en del av OAuth-etableringsprocessen. Obs! Workfront lägger till en state-parameter i frågesträngen. Providern måste skicka tillbaka detta till Workfront genom att lägga till det till Workfront omdirigerings-URI.</p> </td> 
  </tr> 
  <tr> 
   <td>URL för tokenslutpunkt</td> 
   <td> <p>(Endast OAuth2) Den fullständiga API-URL som används för att hämta OAuth2-token. Detta hanteras av webbkrokprovidern eller den externa dokumentprovidern</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Klient-ID</td> 
   <td>(Endast OAuth2) Klient-ID för OAuth2 för den här integreringen</td> 
  </tr> 
  <tr> 
   <td>Klienthemlighet</td> 
   <td> <p>(Endast OAuth2) OAuth2-klienthemlighet för den här integreringen</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront Omdirigerings-URI</td> 
   <td>  <p>(Endast OAuth2) Detta är ett skrivskyddat fält som genereras av Workfront. Det här värdet används för att registrera integreringen med den externa dokumentprovidern. Obs! Som beskrivs ovan för autentiserings-URL måste providern lägga till parametern "state" och dess värde i frågesträngen när den utför omdirigeringen.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Endast ApiKey) Används för att göra auktoriserade API-anrop till webbkrokprovidern. Den API-nyckel som utfärdas av webbkrokprovidern.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Autentisering

Workfront dokumentwebhooks stöder två olika typer av autentisering: OAuth2 och ApiKey. I båda fallen skickar Workfront autentiseringstoken i huvudet när ett API-anrop görs.

### OAuth2

Med OAuth2 kan Workfront göra auktoriserade API-anrop till en webkrok-leverantör för en användares räkning. Innan du gör det måste användaren ansluta sitt externa dokumentleverantörskonto till Workfront och bevilja Workfront

behörighet att agera å deras vägnar. Den här handskakningsprocessen utförs bara en gång för varje användare. Så här fungerar det:

1. Användaren börjar ansluta webbkrokintegreringen till sitt konto. För närvarande gör du detta genom att klicka på listrutan Lägg till dokument > Lägg till tjänst > Anpassat integrationsnamn.
1. Workfront navigerar till användaren via autentiserings-URL:en, som kan uppmana användaren att logga in på den externa dokumentleverantören. Den här sidan hanteras av webbkrokprovidern eller det externa dokumenthanteringssystemet. När du gör det lägger Workfront till en state-parameter i autentiserings-URL:en. Detta värde måste skickas tillbaka till Workfront genom att samma värde läggs till i Workfront Retur-URI i steget nedan.
1. När användaren har loggat in på det externa systemet (eller om användaren redan är inloggad) visas sidan Autentisering, som förklarar att Workfront begär åtkomst för att utföra en uppsättning åtgärder för användarens räkning.
1. Om användaren klickar på Tillåt omdirigeras webbläsaren till Workfront omdirigerings-URI och&quot;code=`<code>`&quot; läggs till i frågesträngen. Enligt specifikationen OAuth2 är denna token kortlivad. Frågesträngen måste också ha följande, &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront behandlar denna begäran och gör ett API-anrop till Token Endpoint URL med auktoriseringskoden.
1. Token Endpoint URL returnerar en uppdateringstoken och åtkomsttoken.
1. Workfront lagrar en sådan token och tillhandahåller webbkrokintegreringen för den här användaren.
1. Från och med nu kan Workfront göra auktoriserade API-anrop till webkrok-providern. När du ringer dessa samtal skickar Workfront åtkomsttoken i HTTP-begärandehuvudet enligt nedan:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Om åtkomsttoken har upphört att gälla, kommer Workfront att anropa tokens slutpunkts-URL för att hämta en ny åtkomsttoken och sedan försöka med det auktoriserade API-anropet igen med den nya åtkomsttoken.

### ApiKey

Det är mycket enklare än OAuth2 att göra auktoriserade API-anrop till en webbkrokleverantör med en ApiKey. När du gör ett API-anrop skickar Workfront bara ApiKey och Workfront-användarnamn i HTTP-begärandehuvudet:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webkrockprovidern kan använda användarnamnet för att tillämpa användarspecifika behörigheter. Detta fungerar bäst när båda systemen ansluter till LDAP med enkel inloggning (SSO).

### Lägga till begäranderubriker (valfritt)

Förutom att använda antingen OAuth2-token eller en ApiKey för autentisering, kan Workfront skicka en fördefinierad uppsättning huvuden till webbkrokprovidern för varje API-anrop. En Workfront-administratör kan konfigurera detta när en Webook-integrering registreras eller redigeras, vilket beskrivs i avsnittet ovan. Mer information finns i Registrera en webbkrokintegrering.

Detta kan till exempel användas för grundläggande autentisering. För att göra detta lägger Workfront-administratören till följande information om begärandehuvud i dialogrutan Anpassad integrering:

   Grundläggande behörighet QWxhZGRpbjpvcGVuIHNlc2FtZQ==

där QWxhZGRpbjpvcGVuIHNlc2FtZQ=== är en base-64-kodad sträng med &quot;username:password&quot;. Se Grundläggande autentisering. Under förutsättning att detta läggs till, skickar Workfront detta i HTTP-begärandehuvudet, förutom andra begäranrubriker:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API-specifikation

Nedan finns en lista med API:er som webkrockprovidern ska implementera för att dokumentwebbhooks ska fungera.

### Hämtar OAuth2-token (endast nödvändig OAuth2-autentisering)

Returnerar OAuth2-uppdateringstoken och åtkomsttoken för en autentiserad användare. Detta anropas en gång när användaren tillhandahåller en dokumentleverantör. Efterföljande anrop görs för att få en uppdaterad åtkomsttoken.

POST för HTTP-begäran /any/url

URL:en är konfigurerbar och motsvarar värdet för Token Endpoint URL på sidan Anpassade integrationsinställningar.

**Frågeparametrar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn</th> 
   <th>Obligatoriskt</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>ja</td> 
   <td> <p>Du kan ange värdena "authentication_code" eller "refresh_token". Det angivna värdet anger vilken av de två parametrarna som skickas till det här API-anropet: code eller refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>kod</td> 
   <td>beroende</td> 
   <td> <p>Auktoriseringskoden som skickas till Workfront strax efter att användaren har klickat på knappen "Bevilja". Detta är endast obligatoriskt när anslagstypen är "permission_code". Auktoriseringskoden ska vara kortvarig och i allmänhet upphöra om 10 minuter eller mindre.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>beroende</td> 
   <td> <p>Detta krävs endast vid efterföljande anrop för att hämta en ny access_token, eftersom föregående access_token har upphört att gälla. När du skickar det här värdet anger du parametern grant_type till "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>ja</td> 
   <td>Klient-ID som konfigurerats i Workfront för den här anpassade integreringen.</td> 
  </tr> 
  <tr> 
   <td>client_secrets</td> 
   <td>ja</td> 
   <td> Klienthemlighet som konfigurerats i Workfront för den här anpassade integreringen.</td> 
  </tr> 
 </tbody> 
</table>

 

**Svar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn</th> 
   <th>Typ </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Sträng</td> 
   <td> <p>En token som används för att göra auktoriserade API-anrop för användarens räkning. Detta bör upphöra att gälla för att förhindra otillåtna API-anrop.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Sträng</td> 
   <td> <p>En långvarig token som används för att hämta en ny access_token genom att anropa den här API-metoden.</p> </td> 
  </tr> 
  <tr> 
   <td>förfaller_in </td> 
   <td>long</td> 
   <td>  <p>(valfritt) Tiden (i sekunder) innan åtkomsttoken upphör att gälla, vanligtvis 3 600.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Exempel**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**Svar**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Hämta metadata för fil eller mapp

Returnerar metadata för den angivna filen eller mappen.

**URL**

GET /metadata?id=[dokument- eller mapp-ID]

**Frågeparametrar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>Fil- eller mappens ID, som webbkrokprovidern refererar till. Detta skiljer sig från Workfront dokument-ID. Använd värdet '/' för att hämta metadata för rotkatalogen.</p><p>Obs! Den maximala längden för ID:t är 255 tecken.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Svar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Typ </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Sträng </td> 
   <td>Namnet på dokumentet eller mappen</td> 
  </tr> 
  <tr> 
   <td>sort </td> 
   <td>Sträng </td> 
   <td>Anger om det här objektet är en fil eller mapp ('fil' eller 'mapp')</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Sträng </td> 
   <td>ID för filen eller mappen.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Sträng </td> 
   <td> <p>Den URL-sökväg som en användare använder för att visa dokumentet i ett webbläsarfönster. URL:en kan finnas hos antingen dokumentprovidern eller den interna externa lagringsprovidern.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Sträng </td> 
   <td> <p>Den URL-sökväg som en användare använder för att hämta dokumentet i ett webbläsarfönster. URL:en kan finnas hos antingen dokumentprovidern eller den interna externa lagringsprovidern.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Sträng </td> 
   <td>Filens MIME-typ. (valfritt)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Sträng </td> 
   <td>Senaste gången den här filen ändrades (RFC 339-tidsstämpel formateras)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Lång</td> 
   <td>  Filens storlek i byte. (valfritt)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolean</td> 
   <td>  <p> Anger om den här filen eller mappen är skrivskyddad för den autentiserade användaren.(valfritt)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Exempel:** `https://www.acme.com/api/metadata?id=12345`

**Svar**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>Felhanteringen bör vara konsekvent för alla API-anrop. Mer information finns i avsnittet Felhantering nedan.

### Hämta en lista med objekt i en mapp

Returnerar metadata för filer och mappar för en viss mapp.

**URL**

GET/filer

**Frågeparametrar**

| Namn  | Beskrivning |
|---|---|
| parentId  | Mappens ID. Använd värdet &#39;/&#39; för att hämta metadata för rotkatalogen. |

{style="table-layout:auto"}

Dokumentets webhooks-API har för närvarande inte stöd för sidnumrering.

**Svar**

JSON som innehåller en lista med filer och mappar. Metadata för varje objekt är samma som returneras av /metadata-slutpunkten.

**Exempel:** `https://www.acme.com/api/files?parentId=123456`

**Svar**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Gör en sökning

Returnerar metadata för de filer och mappar som returneras från en sökning. Detta kan implementeras som en fulltextsökning eller som en vanlig databasfråga. Workfront anropar slutpunkten /search när användaren utför en sökning från den externa filläsaren.

**URL**

GET/sökning

**Frågeparametrar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>fråga</td> 
   <td>Sökordet eller frasen.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(valfritt) Mappens ID som sökningen utfördes från. Obs! Detta är en platshållare för en framtida funktion i Workfront. För närvarande skickas inte den här parametern av arbetsfronten. </p> </td> 
  </tr> 
  </tbody> 
</table>

Dokumentets webhooks-API har för närvarande inte stöd för sidnumrering.

 

**Svar**

JSON innehåller en lista med metadata för filer och mappar som matchar frågan. Vad som utgör en matchning bestäms av webbkrokleverantören. Helst ska det göras en textsökning. Det går också att göra en filnamnsbaserad sökning.

**Exempel:** `https://www.acme.com/api/search?query=test-query`

**Svar**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Hämta innehållet i ett dokument

Returnerar oformaterade byte för ett dokument

**URL**

GET/nedladdning

**Frågeparametrar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> Dokument-ID.</td> 
  </tr> 
 </tbody> 
</table>

 

**Svar**

Dokumentets raw-byte.

**Exempel:** `https://www.acme.com/api/download?id=123456`

### Hämta en miniatyrbild för ett dokument

Returnerar byte för miniatyrbilder i Raw-format för ett dokument.

**URL**

GET/miniatyrbild

**Frågeparametrar**

| Namn  | Beskrivning |
|---|---|
| id  | Dokument-ID. |
| size  |  Miniatyrbildens bredd |

{style="table-layout:auto"}

 

**Svar**

Byte till miniatyrbilden för Raw.

**Exempel:** `https://www.acme.com/api/thumbnail?id=123456`

### Överför en fil - del 1 av 2

Att överföra en fil till en dokumentlagringsleverantör är en tvåstegsprocess som kräver två separata API-slutpunkter. Workfront påbörjar överföringen genom att anropa /uploadInit. Den här slutpunkten returnerar ett dokument-ID som sedan skickas till /upload när dokumentbyte överförs. Beroende på det underliggande dokumentlagringssystemet kan det vara nödvändigt att skapa ett dokument med längden noll och sedan uppdatera innehållet i dokumentet senare.

Dokument-ID och dokumentversions-ID kan läggas till i version 1.1 av den här specifikationen för att hämta extra information från Workfront. Om dokumenthanteringssystemet till exempel vill ha extra information om dokumentet, kan webhochimplementeringskoden använda dokument-ID:t för att hämta informationen med Workfront RESTful API. Som en god vana kan den här informationen komma från anpassade datafält i dokumentet och innehålla uppgifter, problem eller projekt.

**URL**

POST /uploadInit

**Frågeparametrar**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>Det överordnade mapp-ID:t som webbkrokprovidern refererar till.</td> 
  </tr> 
  <tr> 
   <td>filnamn </td> 
   <td>Dokumentets namn</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront dokument-ID (lades till i version 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Version-ID för Workfront-dokument (lades till i version 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Svar**

Metadata för filen, enligt definitionen i /metadata-slutpunkten.

**Exempel:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Svar**

`[file_metadata]` innehåller det nya dokument-ID som används av dokumentprovidern.

### Överför en fil - del 2 av 2

Överför byte i ett dokument till webbholleverantören.

**URL**

PUT /upload

**Frågeparametrar**

| Namn  | Beskrivning |
|---|---|
| id  |  Dokument-ID, som precis skapades. |


 

**Begär brödtext**

Dokumentets byte med Raw-innehåll.

**Svar**

```
{
"result": "success"
}
```

eller

```
{
"result": "fail"
}
```

**Exempel:** `https://www.acme.com/api/upload?id=1234` *[dokumentbyte ingår i uppdateringsströmmen]*

**Svar**

```
{
"result":"success"
}
```

### Hämta information om tjänsten 

(Releasedatum - TBD) Returnerar information om tjänsten, t.ex. funktioner. Workfront använder den här informationen för att anpassa användargränssnittet i Workfront. Om webkromimplementeringen till exempel innehåller vissa anpassade åtgärder, ska JSON visa dessa åtgärder i JSON. Användarna kan sedan aktivera dessa åtgärder från Workfront.

**URL**

GET /serviceInfo

Frågeparametrar

Ingen. Dessutom ska anrop till den här slutpunkten inte kräva autentisering.

**Svar**

JSON som innehåller information om den här tjänsten

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn</th> 
   <th>Typ </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webkrokVersion </td> 
   <td>Sträng </td> 
   <td>Den webkrosversion som implementeras av den här tjänsten. Det här är versionsnumret som visas högst upp i den här specifikationen.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Sträng </td> 
   <td>Tjänstens interna versionsnummer. Detta nummer bestäms av webbkroktjänstleverantören och används endast i informationssyfte.<br><br></td> 
  </tr> 
  <tr> 
   <td>utgivare </td> 
   <td>Sträng </td> 
   <td>Namnet på det företag som tillhandahåller webbkrokimplementeringen.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Sträng </td> 
   <td>En lista som innehåller API-slutpunkterna som implementeras av den här tjänsten. Detta kan användas för att säkerställa att användargränssnittet i Workfront återspeglar funktionerna som erbjuds av webkrokprovidern. Varje objekt i listan måste innehålla slutpunktens namn (till exempel "sök").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Sträng</td> 
   <td>  <p>En lista som innehåller de anpassade åtgärder som implementeras av den här webbocken. Varje listobjekt innehåller ett namn och ett visningsnamn. Visningsnamnet visas i listrutan Dokumentåtgärder i Workfront. Om du klickar på objektet i listrutan anropas åtgärden i webkroken genom att slutpunkten /customAction anropas.</p></td> 
  </tr> 
 </tbody> 
</table>

**Exempel:** https://www.acme.com/api/serviceInfo

**Returnerar**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Skapa en mapp

(Tillagt i version 1.2) Skapar en mapp i en angiven katalog.
URL

POST /createFolder

**Frågeparametrar**

| Namn  | Beskrivning |
|---|---|
| parentId  | Mappens ID som mappen ska skapas i |
| name  | Namnet på den nya mappen |

{style="table-layout:auto"}

 

**Svar**

Metadata för den nyligen skapade mappen, enligt definitionen i /metadata-slutpunkten.

**Exempel:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

returnerar

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Ta bort dokument eller mappar

(Releasedatum - TBD) Tar bort ett dokument eller en mapp med det angivna ID:t i det externa systemet. Om du tar bort en mapp tas även dess innehåll bort.

URL

PUT /delete

**Frågeparametrar**

| Namn  | Beskrivning |
|---|---|
| documentId  | Dokument-ID som ska tas bort |
| folderId  |  Mappens ID som ska tas bort |

{style="table-layout:auto"}

Besvara en JSON-sträng som anger om åtgärden lyckades eller misslyckades, enligt avsnittet Felhantering nedan.

**Exempel:** PUT https://www.acme.com/api/delete id=1234

returnerar

```
{
"status": "success" 
}
```

returnerar

```
{
"status": "failure", "error": "File not found"
}
```


### Byta namn på ett dokument eller en mapp

(Releasedatum - TBD) Byter namn på ett dokument eller en mapp med det angivna ID:t i det externa systemet.

URL

PUT /rename

**Frågeparametrar**

| Namn  | Beskrivning |
|---|---|
| id | Dokument- eller mapp-ID att byta namn på |
| name  | Det nya namnet på dokumentet eller mappen |

{style="table-layout:auto"}

 

Svar

En JSON-sträng som anger om åtgärden lyckades eller misslyckades, vilket anges i felhanteringsavsnittet nedan.

**Exempel:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Utför en anpassad åtgärd

(Releasedatum - TBD) Den här slutpunkten gör att en Workfront-användare (eller kanske en automatiserad arbetsflödeshändelse) kan utföra en åtgärd i det externa systemet. Slutpunkten /customAction accepterar en name-parameter, som gör att webkrok-providern kan implementera flera anpassade åtgärder.

Webbholleverantören registrerar anpassade åtgärder med Workfront genom att inkludera åtgärderna i svaret /serviceInfo under customActions. Workfront läser in den här listan när du konfigurerar eller uppdaterar webkrokprovidern under Inställningar > Dokument > Anpassade integreringar.\
![Utför en anpassad åtgärd](assets/mceclip0-350x262.png)

Användarna kan aktivera den anpassade åtgärden genom att markera avsnittet under Dokumentåtgärder\
![Utlös anpassade åtgärder](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Frågeparametrar**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Namn </th>
   <th>Beskrivning</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Identifieraren som anger vilken typ av åtgärd som ska utföras. Det här värdet motsvarar ett av de customAction-värden som anges av slutpunkten /serviceInfo.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>Det dokument-ID för arbetsytan som åtgärden utförs för.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> Version-ID för arbetsfrontdokumentet som åtgärden utförs för.</td>
  </tr>
 </tbody>
</table>

 

**Svar**

En JSON-sträng som anger om åtgärden lyckades eller misslyckades, vilket anges i felhanteringsavsnittet nedan. Vid fel (d.v.s. status = &quot;error&quot;) visas det angivna felmeddelandet för användaren.

**Exempel:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

svar

```
{
"status": "success" 
}
```


## Felhantering

Det kan uppstå problem när API-begäranden behandlas. Detta bör hanteras på ett konsekvent sätt över alla API-slutpunkter. När ett fel inträffar gör webbkrokprovidern följande:

* Ta med en felkod i svarshuvudet. Felkoder:

   * 403 - Ej tillåtet. Anger att tokens för begäran saknas eller är ogiltiga, eller att autentiseringsuppgifterna som är associerade med tokens inte har åtkomst till den angivna resursen. För OAuth-baserade webbhotell försöker Workfront hämta nya åtkomsttokens.
   * 404 - Hittades inte. Anger att den angivna filen eller mappen inte finns.
   * 500 - Internt serverfel. Alla andra typer av fel.

* Beskriv felet i svarstexten i följande format:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Testning

Kör följande tester för att kontrollera att implementeringen av dokumentwebkroken fungerar som den ska. Det här är manuella tester som går igenom Workfront webbgränssnitt och indirekt når slutpunkterna för webkromimplementeringen.

### Förutsättningar

För att köra dessa tester behöver du följande:

* Ett Workfront-konto med ADM (Advanced Document Management) aktiverat
* En Workfront-användare för det här kontot med systemadministratörsbehörighet
* En webkroch-instans för dokument, som har HTTP-slutpunkter tillgängliga för Workfront

Dessa tester förutsätter också att du redan har registrerat din Document Webkroch-instans i Workfront under Konfigurera > Dokument > Anpassade integreringar.

### Test 1: Tillhandahåll Document Webkroch-tjänsten för en användare

Testar autentiserings-URL:en och tokens slutpunkts-URL:en för OAuth-baserade webkrockproviders.

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Klicka på listrutan Lägg till dokument och välj webbkroktjänsten för dokument under Lägg till tjänst.
1. (Endast OAuth-tjänster) När du har slutfört föregående steg läses tjänstens OAuth2-autentiseringssida in i ett popup-fönster. (Obs! Du kan uppmanas att logga in på tjänsten först.) Från autentiseringssidan ger du Workfront åtkomst till användarens konto genom att klicka på knappen Lita på eller Tillåt.
1. Kontrollera att tjänsten har lagts till i listrutan Lägg till dokument. Om du inte ser den från början kan du försöka med att uppdatera webbläsaren.

### Test 2: Länka ett dokument till Workfront Testar följande slutpunkter: /files, /metadata

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Välj webbkroktjänsten för dokument under Lägg till dokument.
1. Navigera i mappstrukturen från modala medier.
1. Kontrollera att du kan navigera i mappstrukturen på rätt sätt.
1. Markera och länka ett dokument till Workfront

### Test 3: Navigera till ett dokument i innehållshanteringssystemet

Testar följande slutpunkter: /metadata (särskilt viewLink)

1. Länka ett dokument till Workfront
1. Markera dokumentet och klicka på länken Öppna.
1. Kontrollera att dokumentet öppnas på en ny flik.

### Test 4: Navigera till ett dokument i innehållshanteringssystemet (med inloggning)

Testar följande slutpunkter: /metadata (särskilt viewLink)

1. Se till att du är utloggad från innehållshanteringssystemet.
1. Länka ett dokument till Workfront.
1. Markera dokumentet och klicka på länken Öppna.
1. Verifiera att inloggningsskärmen för innehållshanteringssystemet läses in på en ny flik.
1. Logga in och verifiera att du kommer till dokumentet

### Test 5: Hämta dokumentet från innehållshanteringssystemet

Testar följande slutpunkter: /metadata (speciellt downloadLink)

1. Länka ett dokument till Workfront.
1. Markera dokumentet och klicka på länken Hämta.
1. Kontrollera att hämtningen börjar.

### Test 6: Sök efter innehåll

Testar följande slutpunkter: /search

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Välj webbkroktjänsten för dokument under Lägg till dokument.
1. Utför en sökning från modal.
1. Kontrollera att sökresultaten är korrekta.

### Test 7: Skicka dokument från Workfront till content management-systemet

Testar följande slutpunkter: /files, /uploadInit, /upload

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Överföra ett dokument till Workfront från datorn
1. Gå till sidan med dokumentinformation
1. I listrutan Dokumentåtgärder väljer du webbkroktjänsten för dokument under Skicka till...
1. Gå till önskad målmapp och klicka på knappen Spara.
1. Kontrollera att dokumentet har överförts till rätt plats i innehållshanteringssystemet.

### Test 8: Visa miniatyrbilder i Workfront

Testar följande slutpunkter: /miniatyrbild

1. Länka ett dokument till Workfront.
1. Markera dokumentet i listan.
1. Kontrollera att miniatyrbilden visas på den högra panelen.

### Test 9: Hämta innehållets byte

Testar följande slutpunkter: /download

1. Länka ett dokument till Workfront.
1. Gå till dokumentinformationssidan.
1. Skicka dokumentet till Workfront genom att välja Dokumentåtgärder > Skicka till.. > Workfront. Då skapas en ny dokumentversion i Workfront.
1. Hämta dokumentet från Workfront genom att klicka på länken Hämta.

### Test 10: Uppdatera åtkomsttoken (endast OAuth2 Webkrok providers)

Testar följande slutpunkter: Token Endpoint URL

1. Tillhandahålla en webbkroktjänst för dokument för en användare
1. Invalidera användarens åtkomsttoken genom att antingen 1 ) vänta på timeout eller 2) ogiltigförklara den manuellt i det externa systemet.
1. Uppdatera åtkomsttoken i Workfront. Du kan göra detta t.ex. genom att länka ett dokument till Workfront. Du kommer att känna till att åtkomsttoken uppdaterades korrekt om du kunde navigera till och länka ett dokument.

>[!NOTE]
>
>För närvarande är Skicka till inte tillgängligt för länkade dokument. Detta läggs till av Workfront. Du kan testa slutpunkten för /download genom att trycka på slutpunkten manuellt med en REST-klient, till exempel Postman. Alternativt kan du testa slutpunkten för /download genom att generera ett digitalt korrektur. Om du vill aktivera korrektur på webben kontaktar du Workfront.

## Versioner

* Version 1.0 (Releasedatum - maj 2015)

   * Inledande specifikation

* Version 1.1 (Releasedatum - juni 2015)

   * Uppdaterat /uploadInit - Added documentId och documentVersionId

* Version 1.2 (Releasedatum - oktober 2015)

   * Lagt till /createFolder


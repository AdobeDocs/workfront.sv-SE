---
content-type: api
navigation-topic: general-api
title: Grunderna i API
description: Grunderna i API
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 7a1df83c0dd7ddf7dd6cf41643ba65c5903d6eba
workflow-type: tm+mt
source-wordcount: '4419'
ht-degree: 0%

---


# Grunderna i API

Målet för Adobe Workfront API är att förenkla byggintegreringen med Workfront genom att införa en REST-full arkitektur som fungerar över HTTP. I det här dokumentet förutsätts att du känner till REST- och JSON-svar och beskriver hur Workfront API fungerar.

Tack vare att du känner till Workfront-schemat kan du förstå de databasrelationer som kan användas för att hämta data från Workfront i integrationssyfte.

## Begränsningar och riktlinjer

För att Workfront on demand-system ska fungera på ett konsekvent sätt begränsar Workfront API-trådar samtidigt. Detta skyddsräcke förhindrar systemproblem som orsakas av felaktiga API-anrop. Sandlådemiljön har samma samtidiga API-trådgräns, vilket gör att kunder och partner kan testa API-anrop korrekt innan kod släpps i produktionen.

I produktions-, förhandsgransknings- och testmiljöer har slutanvändarförfrågningar en maximal URI-längd på 8 892 byte eftersom de dirigeras via Workfront CDN (Akamai). Denna gräns gäller endast URI:er som dirigeras genom CDN.

>[!NOTE]
>
>denna gräns gäller inte för sandlådemiljöer eftersom sandlådemiljöer inte dirigeras via CDN.

### Ansvarsfriskrivning

All användning av API:t bör testas i Workfront beta-miljö innan den körs i produktionsmiljön. Om någon kund använder API för en process som Workfront rimligen anser vara betungande för on-demand-programvaran (dvs. processen orsakar en i hög grad negativ effekt på programvarans prestanda för andra kunder), förbehåller sig Workfront rätten att begära att kunden avbryter denna process. Om kunden inte rättar sig efter detta och problemet kvarstår förbehåller sig Workfront rätten att avsluta processen.

## Workfront API-URL

Mer information om den URL som du kommer att använda för att anropa Workfront API finns i [Domänformat för Adobe Workfront API-anrop](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Grundläggande om REST

I det här avsnittet ges en introduktion på hög nivå om hur du interagerar med Workfront REST API för följande REST-principer:

### Objekt-URI

Varje objekt i systemet får en unik URI som består av objekttypen och ID:t. I följande exempel visas URI:er som beskriver tre unika objekt:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Objekttypen är skiftlägeskänslig och kan vara antingen den förkortade ObjCode (till exempel proj) eller det alternativa objektnamnet (projekt).

En lista över objekt, giltiga ObjCodes-fält och objektfält finns på  [API Explorer](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>I Workfront API är ett anpassat formulär ett `Category`-objekt och ett anpassat fält är ett `Parameter`-objekt.

### Operationer

Objekten ändras genom att en HTTP-begäran skickas till deras unika URI. Den åtgärd som ska utföras anges av HTTP-metoden.

Standardmetoderna för HTTP motsvarar följande åtgärder:

* **GET** - Hämtar ett objekt efter ID, söker efter alla objekt efter en fråga, kör rapporter eller kör namngivna frågor
* **POST** - Infogar ett nytt objekt
* **PUT** - Redigerar ett befintligt objekt
* **DELETE** - Tar bort ett objekt

För att undvika klientbrister eller protokolllängdsbegränsningar kan parametern method användas för att åsidosätta HTTP-beteendet. En GET-åtgärd kan till exempel implementeras genom följande URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Svar

Varje begäran besvaras i JSON-format. Svaret har antingen ett dataattribut om begäran lyckades eller ett felattribut om ett problem uppstod. Till exempel begäran

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

returnerar ett JSON-svar som liknar följande:


<pre>{<br>}    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br></pre>

>[!NOTE]
>
>När du kör en GET-begäran via webbläsarens adressfält behöver du inte inkludera sessions-ID som en del av begäran.

Särskild säkerhet har lagts till runt förfrågningar från PUT, POST och DELETE. Alla förfrågningar som resulterar i att data skrivs till eller tas bort från databasen kan bara köras om **sessionID=abc123** ingår i URI:n. I följande exempel visas hur detta skulle söka efter en DELETE-begäran:
<pre>GET /attask/api/v15.0/project?id=4c78..54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78..54d0?method=delete&amp;sessionID=abc 123</pre>

### Autentisering

API:t autentiserar varje begäran för att säkerställa att klienten har åtkomst att visa eller ändra ett begärt objekt.

Autentisering utförs genom att ett sessions-ID skickas som kan ges på något av följande sätt:

#### Autentisering av begärandehuvud

Den autentiseringsmetod som rekommenderas är att skicka ett begärandehuvud med namnet SessionID som innehåller sessionstoken. Fördelen med detta är att det är säkert mot [CSRF-attacker (Cross-site Request Forgery)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) och att det inte stör URI:n för cachelagring.

Följande är ett exempel på en begäranderubrik:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Begär parameterautentisering

Du kan autentisera genom att skicka en request-parameter med namnet sessionID, vilket visas i följande exempel: 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Cookie-baserad autentisering

API:t använder samma cookie-baserade autentisering som används av webbgränssnittet i systemet. Om en klient loggar in på Workfront med webbgränssnittet används samma autentisering för alla AJAX anrop som görs i samma webbläsare.

>[!NOTE]
>
>För att skydda mot risken för CSRF-attacker (Cross Site Request Falery) är den här autentiseringsmetoden endast tillgänglig för skrivskyddade åtgärder.

## Inloggning

>[!IMPORTANT]
>
>Workfront rekommenderar inte längre att du använder `/login`-slutpunkten eller API-nycklarna. Använd i stället någon av följande autentiseringsmetoder:
>
>* Serverautentisering med JWT
>* Användarautentisering med OAuth2
>
>Instruktioner om hur du konfigurerar dessa autentiseringsmetoder finns i [Skapa OAuth2-program för Workfront-integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Instruktioner om hur du använder serverautentisering i Workfront finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Instruktioner om hur du använder användarautentisering i Workfront finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med hjälp av auktoriseringskodflöde](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>Det förfarande som beskrivs i detta avsnitt gäller endast organisationer som ännu inte har anslutit sig till Adobe Business Platform. Det går inte att logga in på Workfront via Workfront API om din organisation har anslutit sig till Adobe Business Platform.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Med ett giltigt användarnamn och lösenord kan du använda följande begäran för att få ett sessions-ID:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Detta ställer in en cookie för att autentisera framtida begäranden samt returnera ett JSON-svar med det nyligen skapade sessions-ID:t, användar-ID:t för den inloggade användaren och andra sessionsattribut.

>[!NOTE]
>
>Om du har en angiven API-användare som även är administratör rekommenderar Workfront att du loggar in med en API-nyckel.

**Genererar en API-nyckel**

Du kan generera en API-nyckel när du loggar in på systemet som den användaren, vilket visas i följande exempel:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Hämtar en tidigare genererad API-nyckel**

Du kan också hämta en API-nyckel som tidigare har genererats för en viss användare genom att köra getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Du kan sedan använda det här resultatet för att autentisera API-anrop genom att lägga till &quot;apiKey&quot; som en begärandeparameter med det här värdet i stället för ett sessions-ID eller användarnamn och lösenord. Detta är fördelaktigt ur ett säkerhetsperspektiv.

Följande begäran är ett exempel på hur du hämtar data från ett projekt med apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invaliderar en API-nyckel**

Om apiKey-värdet har komprometterats kan du köra clearApiKey som gör den aktuella API-nyckeln ogiltig, vilket visas i följande exempel:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

När detta är klart kan du köra getApiKey igen för att generera en ny API-nyckel.

### Utloggning

När en session är klar kan du använda följande begäran för att logga ut användaren och förhindra ytterligare åtkomst med sessions-ID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

Det sessions-ID som ska loggas ut kan anges antingen som en cookie, begäranhuvud eller begärandeparameter.

Logga ut en användare:

1. Navigera till inloggningsskärmen, men logga inte in.
1. Ändra URL:en till /attask/api/v15.0/project/search.\
   Observera att sidan inte kan hittas.
1. Ersätt ordet *search* med login?username=admin&amp;password=user och ersätt ditt användarnamn och lösenord för *admin* och *user\
   *Den här sessionen lagras i webbläsaren som en cookie och behöver inte anges om i varje efterföljande begäran om GET.

1. Ändra URL:en tillbaka till **/attask/api/v15.0/project/search**.
1. Lägg märke till det svar som lämnats.

Du måste alltid inkludera det sessions-ID som anges efter inloggning när du gör PUT, POST och DELETE.

## GET

Använd HTTP GET-metoden för att hämta ett eller flera objekt och för att köra rapporter.

### Hämtar objekt

Du kan förbättra en sökning efter objekt med modifierare och filter.

#### Hämta ett objekt med objekt-ID

Om du känner till ett objekts ID kan du hämta objektet genom att komma åt dess unika URI. Till exempel begäran

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

returnerar ett svar som liknar följande:

<pre>{<br>}    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b2000002de5ca1ebc19edf2d5" <br></pre>


Du kan hämta flera objekt i samma begäran genom att ange parametern id request och ange en kommaseparerad lista med ID:n, vilket visas i följande exempel:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Observera att begäran /attask/api/v15.0/project?id=.. är densamma som begäran `/attask/api/v15.0/project/...`.

#### Hämta ett objekt med URI:n

Om du vill hämta ett objekt efter andra villkor än ID:t kan du söka efter URI:n.

Du kan till exempel använda följande begäran för att returnera en lista över alla projekt i systemet:

```
GET /attask/api/v15.0/project/search
```

Du kan ange filter med parametrarna för begäran som namnvärdespar. I följande exempel visas en begäran som skulle hitta alla aktuella projekt:

```
GET /attask/api/v15.0/project/search?status=CUR
```

Följande begäran hittar alla uppgifter som ännu inte är slutförda och som tilldelats en användare som heter John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Använda sökmodifierare

I följande tabell visas några modifierare som du kan använda med Workfront API.

| **Modifierare** | **Beskrivning** | **Exempel** |
|---|---|---|
| eq | returnerar resultat som har statusen stängd | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | returnerar resultat som inte har statusen stängd | <pre>...status=cls&amp;status_Mod=ne..</pre> |
| gte | returnerar resultat som har en procentandel färdig som är större än eller lika med 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=get...</pre> |
| lte | returnerar resultat som har en procentandel färdig som är mindre än eller lika med 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte..</pre> |
| är null | returnerar resultat där beskrivningen är Null | <pre>...description_Mod=är null...</pre> |
| notnull | returnerar resultat där beskrivningen inte är Null | <pre>...description_Mod=not null..</pre> |
| innehåller | returnerar resultat där namnet innehåller &quot;Workfront&quot; | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| mellan | returnerar resultat som har ett anmälningsdatum inom de senaste 7 dagarna | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Sökbegäranden är skiftlägeskänsliga. Om du får ett felmeddelande bör du kontrollera  **_Mod** och **_Range** har rätt skiftläge.

#### Använda ELLER-satser

Du kan förbättra en sökning genom att lägga till en parameter som innehåller &quot;OR&quot; samt en siffra som anger nivån på ett filter eller en serie filter.

En OR-programsats returnerar bara poster i API-anropet som uppfyller OR-programsatsens filtervillkor. Filter är inte underförstådda över OR-satsnivåer.

Om du till exempel vill filtrera efter

* Uppgifter som har ett namn som innehåller &quot;Planning&quot; ELLER
* Uppgifter i en portfölj med namnet&quot;FixedAssets&quot; OCH tilldelade till någon med namnet&quot;Steve&quot; OR
* Uppgifter som har en överordnad aktivitet med namnet &quot;Slutlig aktivitet&quot;

Använd sedan följande API-anrop med dess flera OR-satser:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:tilldeladTill:name=Steve<br>&amp;OR:1:tilldeladTill:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Använda filterparametrar

En potentiell fördel med att använda URL-parametrar för sökfilter är att Workfront tolkar vissa parametrar innan de kontrollerar olika autentiseringsmetoder (t.ex. användarnamn, lösenord, apiKey, cookie). När detta inträffar används inte parametrarna som filter i anropet. 

Du kan undvika det här problemet genom att placera dessa värden i filterparametrar med JSON-formatering. Om du till exempel vill filtrera efter användarnamnet som testanvändare, i stället för att använda 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>skicka URL-parametern i ett filter, vilket visas i följande exempel:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Använda parametern för kartbegäran

Som standard är data som returneras från en sökning en JSON-array. Beroende på ditt sätt att arbeta kan det vara mer effektivt att få resultatet som ett JSON-objekt indexerat med ID. Detta kan du göra genom att använda parametern för mappningsbegäran. Till exempel begäran 
<pre>/attask/api/v15.0/task/search?map=true</pre>returnerar ett svar som indexerats med ett ID som liknar följande:
<pre>{<br>}    "data": {<br>        "4c9a97db000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "first task",<br>            "ID": "4c9a97db000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba60002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "second task", <br>            "ID": "4ca28ba60002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br></pre>

#### Använda parametern Fältbegäran

Som standard returneras bara den mest använda delmängden av fält när du hämtar ett objekt.

Du kan använda fältparametern request för att ange att en kommaavgränsad lista med specifika fält returneras. Till exempel begäran
<pre>/attask/api/v15.0/task/search?fields=planningStartDate,priority</pre>returnerar ett svar som liknar följande:
<pre>{<br>}    "priority": 2,<br>    "name": "first task", <br>    "ID": "4c7c08fa000002ff924e298ee148df4",<br>    "planningStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>Dessa fältnamn är skiftlägeskänsliga.

En lista över möjliga fältreferenser finns i  [API-utforskaren](../../wf-api/general/api-explorer.md)

#### Söker efter kapslade objekt

Du kan söka efter kapslade objekt. Som standard returneras kapslade objekt med endast namn och ID. Om du till exempel vill hämta alla problem tillsammans med deras ägare använder du följande begäran:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Om mer information krävs kan du begära ett kapslat fält med kolonsyntax. Följande begäran söker till exempel efter alla problem tillsammans med ägarens namn, ID, titel och telefonnummer
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>och returnerar följande: 
<pre>{<br>}    "name": "an important issue",<br>    "ID": "4c78285f0000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist", <br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a000054c172b2c2d9f7f81c3" <br>    } <br></pre>

#### Hämtar kapslade samlingar

Du kan hämta kapslade objektsamlingar. Om du till exempel vill hämta ett projekt med alla dess uppgifter använder du följande begäran:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>Följande begäran hämtar aktivitetstilldelningar:
<pre>/attask/api/v15.0/task/search?fields=tilldelningar</pre>

#### Söker efter flera kapslade fält

Som standard returneras bara namnet och ID för varje uppgift, men ytterligare kapslade fält kan anges med kolonsyntax. Om du vill visa alla tillgängliga fält för ett relaterat objekt eller en relaterad samling lägger du bara till ett kolon och en asterisk till objektet/samlingsreferensen.
<pre>/attask/api/v15.0/task/search?fields=tilldelningar:*</pre>

#### Hämtar anpassade data

Du kan hämta anpassade datafält med prefixet&quot;DE:&quot;. Om du till exempel vill begära ett projekt med en parameter som heter&quot;CustomText&quot; använder du följande begäran:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>som skulle returnera
<pre>{<br>}    "name": "custom data project",<br>    "ID": "4c9a954f000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br></pre>Du kan också hämta alla anpassade data för ett objekt genom att begära fältet parameterValues. Till exempel: 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>returnerar liknande data som följande:
<pre>{<br>}    "name": "custom data project",<br>    "ID": "4c9a954f000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br></pre>

#### Använda namngivna frågor

Vissa objekttyper har namngivna sökningar som vanligtvis utförs och som är tillgängliga genom att lägga till frågans namn i slutet av objekttypen URI. Följande begäran hämtar till exempel arbetsobjekten (uppgifter och ärenden) som användaren är tilldelad till:
<pre>/attask/api/v15.0/work/myWork</pre>Namngivna frågor har stöd för att begära att parametern fields hämtar ytterligare fält. Vissa namngivna frågor accepterar även ytterligare filter. En lista över tillåtna namngivna frågor för ett objekt finns på fliken Åtgärd för objektet i  [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Använder `Count`

Du kan använda `count` för att returnera antalet resultat som matchar din fråga. Detta kan vara användbart när du inte behöver data i resultaten. Genom att bara returnera antalet kan servern behandla begäran snabbare och spara bandbredd. Till exempel begäran
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>returnerar antalet resultat i följande format:
<pre>{<br>}    "count": 3 <br></pre>Att returnera ett antal är en mycket mindre dataöverföring än om de fullständiga objekten returneras. Syntaxen är identisk med sökkommandot.

### Begär en rapport

Du kan utföra en rapportbegäran där bara sammanställningen av vissa fält är önskvärd med en eller flera grupperingar. Som visas i följande exempel är rapportsyntaxen densamma som syntaxen för SOAP API:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>som returnerar följande resultat
<pre>{<br>}    "Första projektet": <br>        "sum_hours": 15 <br>    }, <br>     "Andra projektet": <br>        "sum_hours": 30 <br>    } <br></pre>Om du lägger till parametern $$ROLLUP=true inkluderas en summa på varje grupperingsnivå:
<pre>{<br>}    "Första projektet": <br>        "sum_hours": 15 <br>    }, <br>    "Andra projektet": <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br></pre>

### Sortering av frågeresultat i API

Du kan sortera resultatet efter vilket fält som helst om du lägger till följande i ditt API-anrop:

&amp;entryDate_Sort=asc

Om du till exempel vill sortera efter planerad startdatum för aktiviteten tar du bort entryDate och ersätter det med planeradCompletionDate.

Detta fungerar för de flesta fält i Workfront.

### Beaktar frågegränser

När du frågar efter ett objekt bör särskild hänsyn tas till förhållandet mellan relaterade objekt och sökbegränsningar. Som framgår av följande tabell kan en projektfråga inte returnera fler än 2 000 projekt. Dessa 2 000 projekt betraktas som&quot;primära objekt&quot;. Om du frågar efter aktivitetsfältet i projekten blir aktivitetsfältet, som är en samling, ett sekundärt objekt till det primära objektet Projekt. En fråga för aktivitetsfältet kan innehålla tusentals uppgifter i projekt. Totalt får det sammanlagda antalet returnerade objekt (projekt och uppgifter) inte överskrida det maximala antalet 50 000.

För att få optimala prestanda visas i följande tabell de begränsningar som finns för sökbegäranden. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Frågeresultat</th> 
   <th>Begränsning</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Standardantal resultat</td> 
   <td>100</td> 
   <td> Om ingen gräns har angetts i frågefiltret (d.v.s. $$LIMIT) kan resultatet inte innehålla fler än 100 primära objekt. <br>Se <a href="#using-paginated-responses" class="MCXref xref">Använda sidnumrerade svar</a> för instruktioner om hur du åsidosätter den här begränsningen. </td> 
  </tr> 
  <tr> 
   <td>Maximalt antal resultat</td> 
   <td>2 000</td> 
   <td>Frågefiltret (dvs. $$LIMIT) kan inte returnera fler än 2 000 resultat. Mer information finns i"Sidnumrerade svar".</td> 
  </tr> 
  <tr> 
   <td>Maximalt fältdjup</td> 
   <td>4</td> 
   <td>När du identifierar de fält som du vill visa kan du inte gå mer än fyra nivåer bort från objektet som efterfrågas.</td> 
  </tr> 
  <tr> 
   <td>Maximalt antal objekt</td> 
   <td>50 000</td> 
   <td>Resultatuppsättningen får inte innehålla 50000 primära och sekundära objekt.</td> 
  </tr> 
  <tr> 
   <td>Maximalt antal fält</td> 
   <td nowrap>1 000 000</td> 
   <td>När resultatmängden är mindre än 50 000 objekt kan resultatet innehålla högst 1 000 000 fält.</td> 
  </tr> 
  <tr> 
   <td>Maximalt antal grupparbeten som skapats/uppdaterats</td> 
   <td>100</td> 
   <td>Den maximala gränsen för att skapa eller uppdatera grupper är 100.</td> 
  </tr> 
 </tbody> 
</table>

### Använda sidnumrerade svar {#using-paginated-responses}

Om du vill åsidosätta standardfrågebegränsningen för antal resultat och tillåta 200 resultat, kan du inkludera filtret `$$LIMIT=200` i din fråga, vilket visas i följande exempel:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

För att säkerställa tillförlitlighet och prestanda för andra klientorganisationer i systemet är den högsta tillåtna resultatgränsen per fråga 2 000 objekt. Om du försöker ange en större gräns visas ett `IllegalArgumentException`-felmeddelande. 

Därför rekommenderar vi att du använder sidnumrerade svar för stora datamängder. Om du vill ange det första resultatet som ska returneras lägger du till filtret `$$FIRST`. Följande begäran returnerar till exempel resultatet 201-250 för en fråga:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Observera att i ovanstående exempel returnerar `$$FIRST=200` det 201:a resultatet. `$$FIRST=0` returnerar det första resultatet. Det kan hjälpa att tänka på $$FIRST-värdet som antalet resultat som du vill hoppa över innan du returnerar resultaten.

Använd en sorteringsparameter för att försäkra dig om att resultatet är rätt sidnumrerat. Detta gör att resultaten kan returneras i samma ordning, så att sidnumreringen inte upprepas eller hoppar över resultat. Om du till exempel vill sortera med objekt-ID använder du `ID_Sort=asc`.

### Skapa en åtkomstregel

Du kan skapa en åtkomstregel som avgör vem som får åtkomst till ett objekt. Nedan följer exempel på åtkomstregler som du kan ange:

Om du vill ställa in ett projekt så att det bara delas med en användare med ID &quot;abc123&quot; använder du följande begäran:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Om du bara vill dela med en ny person och behålla befintliga behörigheter intakta:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Så här hämtar du befintliga åtkomstregler:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST

POST infogar ett nytt objekt. Syntaxen är identisk med PUT, men med några få undantag. Eftersom det nya objektet inte finns än har det inget ID. Därför innehåller URI:n inte ID:t.

### Skapa ett objekt

Nedan följer ett exempel på en begäran om att skapa ett nytt projekt:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>Svaret innehåller det nyskapade projektet tillsammans med dess nya ID och alla andra fält som anges.

### Kopiera ett objekt

Vissa objekt kan kopieras. För dessa objekttyper kan du skapa nya objekt genom att publicera med en copySourceID-parameter. Följande begäran kopierar till exempel det aktuella projektet och ger det ett nytt namn:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Överför dokument

Du kan överföra dokument via följande API-URL:
<pre>POST /attask/api/v15.0/upload</pre>API förväntar sig att innehållstypen ska vara multipart/form-data. Filens parameternamn måste vara uploadedFile. Servern returnerar följande JSON-data:
<pre>{<br>}    "handle": "4c7c08fa000002ff924e298ee148df4" <br>}</pre>Du kan använda handtaget och skicka till följande URL när du skapar ett Workfront-dokument:
<pre>POST /attask/api/v15.0/document?updates={<br>}    name: aFileName, <br>    handle: abc...123, (handle from the file upload) <br>    docObjCode: PROJ, (eller TASK, OPTASK osv.) <br>    objID: abc...123,<br>    currentVersion:{version:v1.0,filnamn:aFilnamn}<br>}</pre>

## PUT

PUT används för att uppdatera ett befintligt objekt.

Svaret för PUT är identiskt med ett GET. I båda fallen returnerar servern objektets nya läge efter uppdateringen. Alla regler som används för att ändra ett svar på en GET-begäran fungerar också med PUT, som att ange ytterligare fält som ska returneras, anpassade data och så vidare.

### Redigera objekt

Objekten uppdateras alltid med ID:t med objektets unika URI. Fält som ska uppdateras anges som begärandeparametrar. Om du till exempel vill ändra namnet på ett projekt kan du skicka en begäran som ser ut så här:
<pre>PUT /attask/api/v15.0/project/4c7..?name=Nytt projektnamn <br>PUT /attask/api/v15.0/project?id=4c7..&amp;name=Nytt projektnamn</pre>Eftersom uppdateringen kräver ett ID misslyckas den här åtgärden (utan infogning) om objektet inte finns på servern.

### Ange JSON-redigeringar

Som visas i följande exempel kan du använda parametern för uppdateringsbegäran för att ange de fält som ska uppdateras med JSON-syntax:
<pre>PUT /attask/api/v15.0/project/4c7..?updates= <br>{<br>}     name: "New Project Name", <br>     status: "CUR", <br>     ... <br></pre>

### Skapa kapslade uppdateringar

Vissa objekt har privatägda samlingar som kan uppdateras. I följande exempel visas hur du skriver över befintliga tilldelningar för en viss uppgift:
<pre>PUT /attask/api/v15.0/task/4c7..?updates= <br>{<br>}    tilldelningar: [ <br>        <br>            assignToID: "2222...54d0, <br>            assignPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br></pre>

>[!NOTE]
>
>Uppdateringar som görs på den översta nivån är små, men uppdateringar av en samling eller ett kapslat objekt ersätter den befintliga samlingen. Om du vill redigera ett enstaka uppdrag i en uppgift utan att påverka objekten använder du PUT i uppdraget i stället för i uppgiften.

I följande exempel blir ett projekt en offentlig helpdesk-kö. Observera att de befintliga köegenskaperna ersätts.
<pre>PUT /attask/api/v15.0/project/4c7..?updates= <br>{ <br>    queueDef: <br>        isPublic: 1 <br>    } <br></pre>

### Använda parametern Åtgärdsbegäran

Vissa objekt har stöd för ytterligare åtgärder som kan utföras utöver enkla redigeringar. Du kan ange dessa åtgärder med parametern för åtgärdsbegäran. Följande begäran beräknar till exempel om tidslinjen för ett givet projekt:
<pre>PUT /attask/api/v15.0/project/4c7..?action=calculateTimeline<br><br>eller<br><br>PUT /attask/api/v15.0/project/4c7../calculateTimeline </pre>

### Flytta objekt

I följande exempel visas syntaxen för att flytta en uppgift från ett projekt till ett annat:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8..</pre>Ett exempel för varje åtgärdstyp finns här: (??)
<pre>PUT /attask/api/v15.0/project/1234/acceptableApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculate<br><br>2} PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/revgApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval{4 5}PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed<br><br></pre>Det är bara flyttåtgärden som kräver att du identifierar ytterligare attribut för att ange vilket projekt som arbetsposten ska flyttas till.

Följande är ett exempel på varje åtgärdstyp: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Dela objekt

I följande exempel visas syntaxen för att dela ett projekt med ett team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>När du redigerar ett objekt kan du ersätta alla åtkomstregler för ett objekt genom att göra ett PUT och skicka uppdateringar som liknar följande exempel:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',core Åtgärd:'VIEW'}]}</pre>I följande exempel visas syntaxen för att flytta en uppgift från ett projekt till ett annat:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8..</pre>

## DELETE

DELETE tar bort ett objekt. I samtliga fall kan URI:n innehålla parametern force=true, vilket gör att servern tar bort angivna data och dess underordnade. I följande exempel tas en uppgift bort genom att metoden HTTP DELETE körs på en URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c7882 1c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d5 4d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Massuppdateringar

En satsvisa uppdateringssats uppdaterar flera objekt samtidigt i ett enda API-anrop. Ett API-anrop för att skapa satsvis byggs på liknande sätt som ett vanligt uppdateringsanrop, vilket visas i följande exempel:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>vilket ger en avkastning som liknar följande:
<pre>data: [{<br>}    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    namn: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planningStartDate: "2014-08-28T11:00:00:000-0400",<br>    prioritet: 0,<br>    selectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    namn: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planningStartDate: "2014-08-28T11:00:00:000-0400",<br>    prioritet: 0,<br>    selectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>]</pre>Du kan också göra en gruppuppdatering som liknar följande:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>vilket ger en avkastning som liknar följande:
<pre>data: [ {<br>}     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     planningStartDate: "2014-08-28T11:00:00:000-0400",<br>     prioritet: 0,<br>     selectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    namn: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planningStartDate: "2014-08-28T11:00:00:000-0400",<br>    prioritet: 0,<br>    selectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>]</pre>Om du vill att alla åtgärder ska utföras i samma transaktion lägger du till"atomic=true" i ditt batch-API-anrop som en request-parameter. På så sätt återställs alla åtgärder om någon av åtgärderna misslyckas.

>[!NOTE]
>
>Atombatchåtgärder kan bara returnera &quot;success: true&quot; eller ett fel.


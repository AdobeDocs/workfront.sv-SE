---
title: Vanliga frågor om SOAP API
description: Vanliga frågor om SOAP API
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 79b6370ec3283922a16435e8eb8069f7f9560c55
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Vanliga frågor om SOAP API

## Hur skapar jag mitt första dokumentbevis?

Det krävs tre enkla steg:

**Steg 1**: Överför filen till Workfront Proof genom att skicka den via en efterbeställning till  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php) . Vi skickar tillbaka hash-filen till dig - det här är mycket viktigt! Observera att i det här skedet kommer du inte att se något på ditt konto. Det enda du har gjort hittills är att skicka filen till oss, men inte berätta vad du ska göra med den.

**Steg 2**: Om du inte har något sessions-ID kan du hämta ett med metoderna doLogin() eller getSessionID(). Använd den första för att&quot;logga in&quot; med en användares e-postadress och lösenord eller den senare metoden om du har användarens e-postadress och autentiseringstoken.

**Steg 3:** Nu är det dags att skapa ett korrektur. Använd metoden createProof() och skicka minst de obligatoriska fälten (för närvarande finns det bara 5). Se till att du ställer in hash-parametern på den filhash som returneras under&quot;Steg 1&quot; eftersom det gör att vi kan avgöra vilken fil som ska användas när korrekturet skapas.

Om du loggar in på ditt konto ser du korrekturet.

## Hur skapar jag mitt första korrektur för webbögonblicksbilder?

Det krävs två enkla steg:

**Steg 1**: Om du inte har något sessions-ID kan du hämta ett med metoderna doLogin() eller getSessionID(). Använd den första för att&quot;logga in&quot; med en användares e-postadress och lösenord eller den senare metoden om du har användarens e-postadress och autentiseringstoken.

**Steg 2:**&#x200B;Nu är det dags att skapa ett korrektur. Använd metoden createProof() och skicka minst de obligatoriska fälten (för närvarande finns det bara 5). Se till att du anger parametern Hash som &quot;web&quot; och parametern SourceName som URL för den webbsida som du vill hämta.

Om du loggar in på ditt konto ser du korrekturet.

## Vad är skillnaden mellan ett bevis och en version?

I Workfront Proof-versioner visas som ett enda korrektur. Om du klickar på en specifik version i webbgränssnittet visas information om den versionen. I själva verket är varje version ett separat bevis och webbgränssnittet visar dessa tillsammans.

Ur API:ts perspektiv är varje version ett separat korrektur och korrekturen länkas samman med sina ID:n.

**createProof()** skapar alltid **version 1** av korrekturet. Låt oss anta, som ett exempel, att det ID som returnerades för detta bevis &quot;100&quot;.

När du använder **createProofVersion()** skickas alltid ID:t för den föregående versionen. Om vi vill skapa **version 2** vid korrektur 100, skickar vi **100 för parametern ParentFileID**. Detta anger för systemet att detta korrektur ska vara version 2 av uppsättningen. Metoden returnerar ett unikt korrektur-ID, till exempel &quot;101&quot;.

Om en tredje version, t.ex. **version 3**, krävs, anropar du **createProofVersion()** igen och den här gången **skickar in &quot;101&quot; för ParentFileID** vilket säkerställer att den länkade listan med versioner skapas på rätt sätt.

## Måste jag skaffa ett nytt sessions-ID före varje samtal?

Det är viktigt att understryka att varje sessions-ID i princip är en användare som utför åtgärderna. 

Du behöver inte skaffa något nytt sessions-ID innan varje anrop till API:t. Det gäller i 24 timmar. Förfallotiden återställs varje gång du anropar API:t.

## Vad är ett bevis/en personlig URL?

**Team/Public**: Varje korrekturversion har en unik Team-URL (Public). Om det här alternativet är aktiverat öppnas korrekturet i skrivskyddat läge. Du kan hämta Team-URL:en med metoden [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html).

**Personlig**: En personlig URL är unik för varje granskare och korrekturversion. Om en korrekturuppsättning innehåller tre versioner och en granskare finns i alla versioner har granskaren tre unika personliga URL:er. En personlig URL öppnar korrekturversionen med granskaren som redan är identifierad och som därför ska vara säker och inte delas. Personliga URL:er kan hämtas genom att metoden [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html) anropas och sedan itereras över varje  [&#x200B; SOAPRecepientObject &#x200B;](https://api.proofhq.com/home/objects/soaprecipientobject.html) och hämtar parametern &quot;proof_url&quot;.

## >Hur du inkluderar anpassade parametrar när du öppnar minikorrekturet?

Med minikorrekturet kan du bädda in språkverktyget på en egen sida. En referensparameter kan inkluderas som en del av det minsta korrekturet för att ge en omdirigerings-URL när en användare klickar på stängningsknappen i det lilla korrekturet. Du kan inkludera valfritt antal anpassade parametrar som en del av den här omdirigerings-URL:en genom att lägga till dem med ett &quot;&amp;&quot;-tecken, t.ex. %26.

Exempelvis en URL för minikorrektur
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` måste kodas som 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` för att de anpassade parametrarna ska skickas igenom.



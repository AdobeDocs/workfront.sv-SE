---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Snabba upp problem i [!DNL Workfront Proof]
description: Den här hjälpsidan kan hjälpa dig att avgöra om det finns några hastighetsproblem som du kan uppleva när du använder [!DNL Workfront Proof] är relaterade till din internetleverantör eller [!DNL Workfront Proof]dess leveransnätverk.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# Snabba upp problem i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Den här hjälpsidan kan hjälpa dig att avgöra om det finns några hastighetsproblem som du kan uppleva när du använder [!DNL Workfront Proof] är relaterade till din internetleverantör eller [!DNL Workfront Proof]dess leveransnätverk.

Hastighetsproblem beror i allmänhet på den lokala Internet-anslutningen eller lokala Internet-åtkomstinställningar (t.ex. där en proxyserver används) och därför ligger de tyvärr utanför kontrollen över [!DNL Workfront Proof].

Det finns dock några steg du kan ta för att kontrollera din anslutningshastighet, vilket gör att grundorsaken till de problem du upplever kan fastställas. Alla dessa steg är lika viktiga för felsökningsprocessen och vi rekommenderar att du tar dig tid att samla in information om alla steg i listan för att få den mest korrekta diagnosen av problemet.

När du har samlat in alla uppgifter rekommenderar vi att du rådfrågar din lokala IT-avdelning för att identifiera eventuella lokala problem. Om du behöver mer hjälp kan du kontakta [Supportteam](https://support.workfront.com/hc/en-us/requests/new).

## Fastställ vilken del av systemet som är långsam

När du använder [!DNL Workfront Proof]kan du arbeta med kontrollpanelen, till exempel för att hantera mappinnehåll och användare eller med [!DNL Workfront Proof] Visningsprogram: genomföra en korrekturgranskning, kontrollera de kommentarer som redan gjorts och så vidare.

Att avgöra vilken del av systemet som är långsam är det första steget när det gäller att felsöka hastighetsproblem. När du rapporterar [!DNL Workfront Proof] Om du är långsam bör du beskriva följande:

* Har du långsam användning av andra webbsidor?
* Inträffar problemet på kontrollpanelen eller [!DNL Workfront Proof] Visningsprogram?
* Vilken exakt del av systemet är långsam? (t.ex. bearbeta ett nytt korrektur eller öppna en kommentar i [!DNL Workfront Proof] Viewer)

## Köra spårvägs- och pingtester

När du får prestandaproblem är det viktigt att du kör kommandot traceroute för att verifiera anslutningen. Det gör du genom att öppna kommandotolken i datorn (Terminal i Mac/Linux) och utföra följande steg:

1. Skriv något av följande och vänta sedan tills spårningen är klar:

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Endast Windows) Typ **ping app.proofhq.com**.
1. När ping-åtgärden är klar högerklickar du i kommandotolken och väljer Alla.
1. Kopiera och klistra in resultaten i svaret på ditt e-postmeddelande.
Se till att du tillåter att kalkering och ping slutförs innan du skickar resultaten till supportteamet.

## Testa anslutningshastigheten med Speedtest.net

1. Klicka [här](http://www.speedtest.net/) för att få tillgång till Speedtest.net.
1. Följ instruktionerna i kunskapsbasen Speedtest för att testa hastigheten på din internetanslutning.
1. Kopiera och klistra in resultaten i ett e-postmeddelande till vårt supportteam.

## Kontrollera nätverksfliken i webbläsarkonsolen

Webbkonsolen som finns i de moderna webbläsarna samlar in användbar information om eventuella fördröjningar i nätverket, vilket kan vara bra för oss att fastställa grundorsaken till de problem du upplever.

Så här kontrollerar du inläsningstiderna för en webbsida:

1. Öppna webbläsarens konsol och fliken Nätverk.
1. Läs in sidan igen.
1. Ta skärmdumpar eller spela in en skärmdump av resultatet.
1. Dela resultaten med supportteamet.

Kontrollera att skärmbilden visar alla data. Du kan expandera konsolfönstret när du tar en skärmbild eller rulla nedåt i en skärmdump.

Om du inte vet hur du öppnar konsolen i webbläsaren kan du läsa följande inspelade steg:

* [Krom](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

Du kan även läsa webbläsarens dokumentation för mer detaljerade anvisningar.

## Kontrollera anslutningen på ett annat nätverk och på en annan dator

Att kontrollera om du upplever samma problem med anslutningshastigheten genom att använda en annan enhet eller ett annat nätverk är ett viktigt steg i felsökningsprocessen. Försök att byta till en annan dator eller mobil enhet, och försök använda ett annat nätverk (t.ex. mobildata).

Jämför anslutningen i olika kombinationer: använda en annan dator i samma nätverk, använda samma dator i ett annat nätverk och använda både en alternativ dator och ett annat nätverk, och sedan dela resultaten med supportteamet.

---
title: Fjärde kvartersversionen 2025 - översikt
description: Den här sidan innehåller information om funktioner som ingår i den fjärde utgåvan av kvartalet 2025. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
source-git-commit: cbdc60db525dabb93e984dff7787a83edceb6c8c
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 0%

---

# Fjärde kvartersversionen 2025 - översikt

Den här sidan innehåller information om de funktioner som ingår i den fjärde utgåvan av kvartalet 2025, som är planerad till oktober 2025.

Förbättringarna på den här sidan är tillgängliga i förhandsvisningsmiljön. Den här sidan uppdateras med ytterligare förbättringar eftersom den fjärde utgåvan av kvartal 2025 närmar sig den planerade produktionsutgåvan.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Månads- och kvartalsvisa releaser planeras vara tillgängliga torsdagen den andra hela veckan i månaden, om inte annat anges.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>25.8 (augusti 2025)</li><li>25.9 (september 2025)</li><li>25.10 (oktober 2025)</li></ul> | <ul><li>25.10 (oktober 2025)</li></ul> |
>
>Observera att för den sista utgåvan av varje kvartal (25.10 i kvartal) kommer användare med fast releaseschema att få releasen en dag i förtid.
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättringar av dokument och korrektur](#document-and-proofing-enhancements)
  <!--* [Home enhancements](#home-enhancements)-->
* [Projektförbättringar](#project-enhancements)
  <!--* [Requests enhancements](#requests-enhancements)-->
* [Förbättrad resurshantering](#resource-management-enhancements)
* [Andra förbättringar](#other-enhancements)

### Administratörsförbättringar

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Lägg till flera värdealternativ från ett externt API till ett anpassat formulär</a><p></p>
            <p>En ny fälttyp, Flerval extern sökning, är nu tillgänglig för den anpassade formulärdesignern. När du har data lagrade på ett externt system kan du med den här fälttypen läsa in alternativ från ett externt API och filtrera baserat på andra fältvärden i det anpassade formuläret. Det här är samma som en extern sökning med ett enda val.</p>
            <p>När formuläret läggs till i ett objekt visas de värden som returneras från API:t i ett listrutefält och användaren kan välja flera värden.</p>
        </td>
        <td>31 juli 2025</td>
        <td>14 augusti 2025</td>
        <td>16 oktober 2025</td>
    </tr>     
  </tbody>
</table>


### Förbättringar av dokument och korrektur

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Ny korrekturintegrering för Adobe Express</a><p></p>
            <p>Vi är glada över att kunna presentera en ny integrering mellan Adobe Express och Workfront Proof.</p>
            <ul>
            <li>Effektivisera samarbetet mellan kreatörer, jurister och grupper som arbetar med regelefterlevnad och minska tiden för publicering samtidigt som ni upprätthåller tillsyn</li>
            <li>Genomför djupgående granskningar med ritmarkeringar, kommentarer och kommentarer i Workfront korrekturläsare</li>
            <li>Följ standarderna med elektroniska signaturer och fullständiga granskningsloggar</li>
            <li>Kräv godkännande av ommixade filer från en Express-mall</li>
            <li>Mappa en Express-mall till ett arbetsflöde för granskning och godkännande i flera steg med avancerade korrekturmallar</li>
            </ul>
        </td>
        <td>28 juli 2025</td>
        <td>28 juli 2025</td>
        <td>28 juli 2025</td>
    </tr>     
  </tbody>
</table>

<!--### Home enhancements

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}">Updates to the My Requests widget in Home</a><p></p>
            <p>To create a more seamless experience between Workfront and Workfront Planning, we've redesigned the My Requests widget in Home. The new widget features the following changes:
            <ul>
                <li>Improved layout and organization of request information</li>
                <li>Enhanced filtering and sorting options</li>
                <li>Integration with Workfront Planning for better visibility into resource allocation</li>
            </ul>
            </p>
        </td>
        <td>July 31, 2025</td>
        <td>August 14, 2025</td>
        <td>October 16, 2025</td>
    </tr>     
  </tbody>
</table> 

### Requests enhancements

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Updates to Requesting experience</a><p></p>
            <p>To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:
            <ul>
                <li>View Workfront and Workfront Planning requests in a single list.</li>
                <li>Filter submitted requests based on criteria you specify.</li>
                <li>Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.</li>
                <li>Hide and reorder columns in the submitted requests list.</li>
            </ul>
            </p>
        </td>
        <td>July 31, 2025</td>
        <td>August 14, 2025</td>
        <td>October 16, 2025</td>
    </tr>     
  </tbody>
</table> -->

### Projektförbättringar

<table style="table-layout:auto">
  <tbody>
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Nya uttryck har lagts till i formelfält i Planning och beräknade anpassade fält i Workfront</a><p><p>[!BADGE Off schema]{type=Neutral}</p></p>
            <p>Vi har lagt till nya uttryck med följande användning i formelfält i Workfront Planning och i beräknade anpassade fält i Workfront:</p>
            <ul>
            <li>REMOVEACCENTS(sträng): Tar bort diakritiska tecken från alla tecken med accent i indatasträngen.</li>
            <li>REPLACEPATTERN(sträng, mönster, ersättningssträng): Ersätter matchningarna för det angivna mönstret med ersättningssträngen.</li>
            <li>PASCAL(string): Konverterar indatasträngen till PascalCase genom att ändra den första bokstaven i varje ord till versal och ta bort alla blanksteg.</li>
            </ul>
        </td>
        <td>7 augusti 2025</td>
        <td>7 augusti 2025</td>
        <td>7 augusti 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Ytterligare sätt att komma åt avancerade tilldelningar från listor</a><p></p>
            <p>En <b>avancerad</b>-knapp är nu tillgänglig för tilldelningar i listor, vilket gör det snabbare för dig att komma åt sidan Avancerade tilldelningar. Ikonen <b>Personer</b> för att komma åt avancerade tilldelningar är också tillgänglig för tilldelningar i listor.</p>
        </td>
        <td>7 augusti 2025</td>
        <td>11 september 2025</td>
        <td>16 oktober 2025</td>
    </tr> 
  </tbody>
  </table>

### Förbättrad resurshantering

<table style="table-layout:auto">
  <tbody>
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">Utjämning av arbetsbelastning är nu tillgängligt för din användarprofil</a><p></p>
            <p>Alla användare kan nu visa sina egna data om efterfrågan och kapacitet i arbetsbelastningsutjämnaren från sin profil, oavsett åtkomstnivå. När du öppnar din Workfront-användarprofil visas belastningsutjämnaren i den vänstra navigeringspanelen.</p>
            <p>Utjämningsdata för arbetsbelastning för en användare är skrivskyddade. Du kan inte tilldela arbete, ta bort tilldelning av arbete eller justera allokeringar på användarnivå.</p>
        </td>
        <td>31 juli 2025</td>
        <td>14 augusti 2025</td>
        <td>16 oktober 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">Rolltilldelningar visas i arbetsbelastningsutjämnaren </a><p></p>
            <p>Resurshanterare kan nu granska jobbrolltilldelningar i arbetsbelastningsutjämnaren. Tilldelningarna visas i området Ej tilldelat arbete, under de uppgifter eller utgåvor som rollerna är tilldelade till. Endast arbetsobjekt som är tilldelade användare visas i området Tilldelad arbetsyta. </p>
            <p>En ny inställning för Utjämning av arbetsbelastning, Visa rolltilldelningar, avgör om rolltilldelningar visas eller inte. Inställningen är aktiverad som standard.</p>
        </td>
        <td>31 juli 2025</td>
        <td>14 augusti 2025</td>
        <td>16 oktober 2025</td>
    </tr>     
  </tbody>
</table>

### Andra förbättringar

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funktion</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatum</span>
                        </p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Uppdateringar av utseende och känsla under den fjärde kvartersutgåvan 2025 </a></p>
                        <p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för den fjärde utgåvan, kvartal 2025. </p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsgranskningsversion: Under den fjärde kvartersutgåvan 2025<br /></p>
                            </li>
                            <li>
                                <p>Produktionsrelease: Minst två veckor efter lanseringen till Förhandsgranska (om inget annat anges)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernisering av gränssnitt

Vi uppdaterar gränssnittet i hela Adobe Workfront för att förbättra användarupplevelsen och sammanföra det med andra Adobe-program. Dessa ändringar släpps utanför standardreleaseplanen. En lista över de här ändringarna finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Versionsinformation för andra områden

### Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production på en cadence som ligger utanför standardreleaseprogrammet. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Förbättringar av Workfront Planning

Nya funktioner i Workfront Planning finns i Production. Mer information om de senaste funktionerna finns i [Fjärde utgåvan av kvartal 2025 för Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

Det finns inga uppdateringar för följande i den här versionen:

* Scenarioplan
* Korrektur
* Mål

## Uppdateringar för korrekturläsare för datorer

### Version 2.1.52

**Produktionsrelease för alla kunder: 31 juli 2025**

Desktop Proofing Viewer har uppdaterats till version 2.1.52 som åtgärdar felkorrigeringar.

2.1.51-uppdateringen inkluderade interna verktygsuppdateringar och påverkade inte slutanvändarnas funktioner.

Uppdateringen gäller både Mac och Windows.

## Meddelanden

### Ny version av Workfront för Microsoft Teams

När [Microsoft övergår till New Teams-klienten](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) är Classic Teams-klienten inte längre tillgänglig efter 1 juli 2025. För att kunna fortsätta använda Microsoft Teams och integrerade program som Workfront måste kunderna gå över till nya Teams-klienten före detta datum.

Den uppdaterade Workfront-integreringen är nu tillgänglig och helt kompatibel med New Teams. I de flesta fall visas Workfront automatiskt när användaren har gått över. Om så inte är fallet kan integreringen installeras manuellt från Microsoft Teams App Store. Information om hur du installerar eller verifierar Workfront-integreringen i klienten New Teams finns i [Installera [!DNL Adobe Workfront] för Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront för Microsoft Outlook

[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.

* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**

Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**

### Andra integreringsövergångar för Workfront

För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen är följande integreringar inte tillgängliga efter **28 februari 2026**:

* Workfront for G Suite
* Workfront för Jira
* Workfront för Salesforce.

Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Google Workspace.
En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

### API version 20

Workfront API version 20 släpptes den 4 maj 2025. För API-version 20 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 20](/help/quicksilver/wf-api/api/new-api-version-19.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes under den första utgåvan av kvartal 2025 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=sv-SE).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront-sidan ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=sv-SE).

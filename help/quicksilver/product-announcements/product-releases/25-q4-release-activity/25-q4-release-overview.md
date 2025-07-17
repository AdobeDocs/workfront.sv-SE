---
title: Fjärde kvartersversionen 2025 - översikt
description: Den här sidan innehåller information om funktioner som ingår i den fjärde utgåvan av kvartalet 2025. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b495399ff6375eae222b9a15538c52ae3c73f6bb
workflow-type: tm+mt
source-wordcount: '712'
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
>| <ul><li>25.9 (september 2025)</li><li>25.10 (oktober 2025)</li><li>25.11 (november 2025)</li></ul> | <ul><li>25.10 (oktober 2025)</li></ul> |
>
>Observera att för den sista utgåvan av varje kvartal (25.10 i kvartal) kommer användare med fast releaseschema att få releasen en dag i förtid.
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Andra förbättringar](#other-enhancements)

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

Nya funktioner i Workfront Fusion finns i Production på en cadence som ligger utanför standardreleaseprogrammet. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Förbättringar av Workfront Planning

Nya funktioner i Workfront Planning finns i Production. Mer information om de senaste funktionerna finns i [Fjärde utgåvan av kvartal 2025 för Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

Det finns inga uppdateringar för följande i den här versionen:

* Scenarioplan
* Korrektur
* Mål

## Meddelanden

### Ny version av Workfront för Microsoft Teams

När [Microsoft övergår till New Teams-klienten](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) är Classic Teams-klienten inte längre tillgänglig efter 1 juli 2025. För att kunna fortsätta använda Microsoft Teams och integrerade program som Workfront måste kunderna gå över till nya Teams-klienten före detta datum.

Den uppdaterade Workfront-integreringen är nu tillgänglig och helt kompatibel med New Teams. I de flesta fall visas Workfront automatiskt när användaren har gått över. Om så inte är fallet kan integreringen installeras manuellt från Microsoft Teams App Store. Information om hur du installerar eller verifierar Workfront-integreringen i klienten New Teams finns i [Installera [!DNL Adobe Workfront] för Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront för Microsoft Outlook

[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.

* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**

Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**

### API version 20

Workfront API version 20 släpptes den 4 maj 2024. För API-version 20 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 20](/help/quicksilver/wf-api/api/new-api-version-19.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes under den första utgåvan av kvartal 2025 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront-sidan ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
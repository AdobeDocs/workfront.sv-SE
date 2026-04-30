---
title: Översikt över utgåvan för tredje kvartalet 2026
description: Den här sidan innehåller information om funktioner som ingår i utgåvan för tredje kvartalet 2026. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8ca50590-ef6a-44b1-a856-9821bdafbc1c
source-git-commit: 1a498abcf4a9ef8940eb2da09da42636253e557a
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Översikt över utgåvan för tredje kvartalet 2026

Den här sidan innehåller information om de funktioner som ingår i den tredje utgåvan av kvartal 2026 som planeras släppas i juli 2026.

Förbättringarna på den här sidan är tillgängliga i förhandsvisningsmiljön. Den här sidan kommer att uppdateras med ytterligare förbättringar eftersom utgåvan för tredje kvartalet 2026 närmar sig den planerade produktionsutgåvan.

Live-webbinarier hålls för varje kvartalsrelease - där de nya funktionerna markeras och detaljerad information presenteras. Registrera dig på [eventsidan](https://experienceleague.adobe.com/sv/events?filters=Workfront) och filtrera efter Workfront.

>[!IMPORTANT]
>
>
>Månads- och kvartalsvisa releaser planeras vara tillgängliga torsdagen den andra hela veckan i månaden, om inte annat anges.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>26.5 (14 maj 2026)</li><li>26.6 (11 juni 2026)</li><li>26.7 (16 juli 2026)</li></ul> | <ul><li>26.7 (16 juli 15, 2026)</li></ul> |
>
>Observera att för den slutliga utgåvan av varje kvartal (26,7 i det här kvartalet) kommer användare som har den snabba releasen att få den en dag i början (15 juli 2026).
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Förbättrade dokument](#documents-enhancements)
* [Förbättrade begäranden](#requesting-enhancements)

### Förbättrade dokument

<table>
    <col style="width: 50%;" />
    <col style="width: 25%;" />
    <tbody>
        <tr>
            <td><strong>Funktion</strong>
            </td>
            <td><strong>Förhandsgranskning</strong></td>
            <td><strong>Snabb release</strong></td>
            <td><strong>kvartalsvis</strong></td>
        <tr>
            <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md" class="MCXref xref" xrefformat="{para}">Visa Adobe användning av företagslagring</a>
                <p>Sidan Kundinformation i installationsprogrammet innehåller nu ett nytt lagringsöversiktsavsnitt med användningsmätare för Adobe Enterprise-lagring.</p>
            </td>
            <td><p>30 april 2026</p></td>
            <td><p>14 maj 2026</p></td>
            <td><p>16 juli 2026</p></td>
        </tr>
    </tbody>
</table>

### Förbättrade begäranden

<table>
    <col style="width: 50%;" />
    <col style="width: 25%;" />
    <tbody>
        <tr>
            <td><strong>Funktion</strong>
            </td>
            <td><strong>Förhandsgranskning</strong></td>
            <td><strong>Snabb release</strong></td>
            <td><strong>kvartalsvis</strong></td>
        <tr>
            <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">Fördefinierade vyer har lagts till i listan över förfrågningar i området Förfrågningar och i widgeten Mina förfrågningar</a><p>[!BADGE Off schema]{type=Neutral}</p>
                <p>För att hjälpa dig att organisera din begärandelista bättre har vi lagt till de fördefinierade vyerna i listan över förfrågningar i området Begäranden och widgeten Mina förfrågningar i Hem.</p>
            </td>
            <td><p>23 april 2026</p></td>
            <td><p>23 april 2026</p></td>
            <td><p>23 april 2026</p></td>
        </tr>
    </tbody>
</table>

## Versionsinformation för andra områden

### Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production på en cadence som ligger utanför standardreleaseprogrammet. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Förbättringar av Workfront Planning

Det finns inga förbättringar av Workfront Planning i den här versionen.

<!--

New features in Workfront Planning are available in Production. For more information about the latest features, see [Third Quarter 2026 release activity for Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q3.md).

-->

### Andra Workfront-förbättringar

Det finns inga uppdateringar för följande i den här versionen:

* Workfront Planning
* Scenarioplan
* Korrektur
* Mål

## Uppdateringar för korrekturläsare för datorer

### Version 2.1.55

Produktionsrelease för alla kunder: 19 mars 2025

Desktop Proofing Viewer har uppdaterats till 2.1.54 till 2.1.55. Uppdateringen innehöll interna verktygsuppdateringar och påverkade inte slutanvändarnas funktioner.

Uppdateringen gäller både Mac och Windows.

## Meddelanden

### API version 21

Workfront API version 21 släpptes 23 oktober 2025. För API-version 21 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

>[!IMPORTANT]
>
>Denna API-version innehåller en brytningsändring som kan påverka dina befintliga API-anrop. Detta beror på att API version 21 använder Event Subscriptions version 2.
>
> För flervalsfält skickas alltid Event Subscriptions version 2 som en array. Version 1 skickade en array om mer än ett värde har valts. Om bara ett värde valdes, skickades en sträng.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 21](/help/quicksilver/wf-api/api/new-api-version-21.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the Third Quarter 2026 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=sv-SE).

-->

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront-sidan &#x200B;](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=sv-SE).

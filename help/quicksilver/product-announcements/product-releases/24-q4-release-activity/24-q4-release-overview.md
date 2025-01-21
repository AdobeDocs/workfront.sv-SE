---
title: Fjärde kvartersversionen 2024 - översikt
description: Den här sidan innehåller information om funktioner som ingår i den fjärde utgåvan av kvartalet 2024. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: e620074ab0509e3052678e8c7e46e9629f3b34f2
workflow-type: tm+mt
source-wordcount: '2193'
ht-degree: 0%

---

# Fjärde kvartersversionen 2024 - översikt

Den här sidan innehåller information om funktioner som ingår i den fjärde utgåvan av kvartalet 2024. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.

<span class="preview">Funktioner utanför cykeln (de som lanserades till Produktion före fjärde utgåvan av kvartal 2024) är markerade i gult.</span>

>[!IMPORTANT]
>
>23.3-versionen innehåller ett alternativ för att flytta organisationen till månatliga releaser. Därför har Workfront ändrat numreringsschemat för releaser så att det tar hänsyn till både månads- och kvartalsversionerna. Det första numret anger året och det andra numret anger månaden för releasen. Exempel: Versionen för april 2024 är 24.4.
>
>Månads- och kvartalsvisa releaser planeras vara tillgängliga torsdagen den andra hela veckan i månaden, om inte annat anges.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>24.8 (15 augusti 2024)</li><li>24.9 (12 september 2024)</li><li>24.10 (17 oktober 2024)</li></ul> | <ul><li>24.10 (17 oktober 2024)</li></ul> |
>
>Observera att för den sista utgåvan av varje kvartal (24.10 i kvartal) kommer användare med fast releaseschema att få releasen en dag i förtid.
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättrad dokumenthantering](#document-management-enhancements)
* [Hemförbättringar](#home-enhancements)
* [Integration enhancements](#integration-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Förbättringar av korrektur](#proofing-enhancements)
* [Förbättringar av rapporter och kontrollpaneler](#report-and-dashboard-enhancements)
* [Andra förbättringar](#other-enhancements)
* [Funktioner som snart ska tas bort från Workfront](#functionality-soon-to-be-removed-from-workfront)

### Administratörsförbättringar

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Åtkomstnivån är nu tillgänglig i miljökampanjen</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Vi har lagt till möjligheten att inkludera åtkomstnivåer för att utöka funktionerna för miljömarknadsföring. Nu kan du konfigurera en åtkomstnivå i en sandlådemiljö och sedan höja den åtkomstnivån till din produktionsmiljö.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 17 oktober 2024</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">En räknare i anpassade formulär visar antalet fält</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Anpassade formulär är begränsade till 500 fält. I lång form kan det vara svårt att veta hur många fält som finns i formuläret och om du närmar dig gränsen. En räknare har lagts till i anpassade formulär längst ned till vänster. Räknaren visar hur många fält som används i formuläret och den visas alltid när du rullar i formulärdesignern.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 1 oktober 2024</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Alternativet Markera alla är nu tillgängligt i layoutmallar</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>För att du enklare ska kunna visa och dölja fält med layoutmallar har kryssrutan Markera alla lagts till under Översikt och Ekonomi i detaljvyn i en layoutmall. Det här alternativet är tillgängligt när du har valt Projekt, Aktivitet, Utgåva, Portfolio eller Program under Anpassa vad användare ser.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 29 augusti 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 29 augusti 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Återställa kampanjer för miljöförbättringar</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>För att göra miljökampanjen mer flexibel och enklare att använda har vi aktiverat återställningsfunktionen. Nu kan du återställa paket inom 24 timmar, så att du enklare kan återställa tidigare konfigurationer som har påverkats av ett paket för miljöbefordran.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 29 augusti 2024</p>
                        </li>
                        <li>
                            <p>Production for fast release: Med version 24.9 (12 september 2024)</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Layoutknappen i den anpassade formulärdesignern tillåter två eller tre kolumner</a></p>
                    <p>Med en layoutknapp i den anpassade formulärdesignern kan du välja mellan två- eller trekolumnsarbetsytor. Den ursprungliga formulärdesignern använder tre kolumner och fältinställningarna visas i kolumnen längst till höger. Om du markerar två kolumner visas fältinställningarna intill fältbiblioteket i kolumnen längst till vänster.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p><s>Förhandsversion: 12 augusti 2024</s></p>
                        </li>
                        <li>
                            <p>Production for fast release: Ej tillämpligt</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Ej tillämpligt</p>
                        </li>
                    </ul>
                    <p><i>Den här funktionen har tagits bort från förhandsgranskningen och kommer inte att släppas i framtida versioner.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Förbättrad dokumenthantering

>[!IMPORTANT]
>
>De funktioner som listas i **Förbättringar av dokumenthanteringen** ingår i en fasversion och är bara tillgängliga för specifika kunder.

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Visa dokumentets beslutsstatus direkt i dokumentlistan</a></p>
                    <p>Nu kan du visa ett dokuments beslutsstatus direkt i dokumentlistan.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p><s>Förhandsversion: 3 oktober 2024</s></p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Lägg snabbt till tidigare granskare och godkännare i nya dokumentversioner</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Nu kan du snabbt lägga till granskare och godkännare från tidigare dokumentversioner.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 3 oktober 2024</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Hemförbättringar

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Uppdateringar av widgeten Väntar på mitt godkännande i nytt hem</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Vi har gjort följande ändringar i widgeten Väntar på mitt godkännande:</p>
                        <ul>
                            <li>Widgetens nya namn: Widgetens namn är nu Mitt godkännande.</li>
                            <li>Tillagda godkännanden som jag har skickat in som ett filteralternativ: Nu kan du visa godkännanden som du har skickat in i den nya Hem-widgeten.</li>
                            <li>Deadline: Du kan nu se korrekturdeadline om en sådan har angetts. Om ingen deadline anges används som standard datumet då filen skapades.</li>
                        </ul>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 10 oktober 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 10 oktober 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Prioriteringar: en enklare, smidigare och intuitiv Workfront-upplevelse för uppgiftsägare</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Prioriteringarna ökar fokus och produktivitet och hjälper kunderna att uppnå mer på kortare tid.</p>
                    <p>Med Prioriteringar får du:</p>
                        <ul>
                            <li>Hantera och prioritera rutinuppgifter: Organisera din dag eller vecka med konsoliderad navigering för bättre tydlighet.</li>
                            <li>Större produktivitet: Kom åt projektsammanhang och utför uppgifter snabbare med färre klick.</li>
                            <li>Personaliserade funktioner: Dra nytta av funktioner som är unika för uppgiftsägare.</li>
                        </ul>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 3 oktober 2024</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Integration enhancements

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Förbättringar av inloggningsfunktionen för Outlook-integrering</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Inloggningen för Outlook-integrering har strömlinjeformats så att alla kunder ser samma knapp för att logga in på Workfront oavsett om de är IMS-aktiverade eller inte. De efterföljande inloggningsstegen skiljer sig åt för IMS- och icke-IMS-instanser, men den inledande sidan är densamma för alla användare.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 6 augusti 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 6 augusti 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Projektförbättringar

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Fler relevanta tilldelningar har lagts till i arbetsflödet Ny uppgift</a></p>
                    [!BADGE In production for Fast Release ]{type=Positive}
                    <p>Vi har lagt till samma funktioner för mer relevanta smarta tilldelningar i fältet Uppdrag i rutan Ny uppgift när en uppgift läggs till i ett projekt och i en projektuppgiftslista.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 13 februari 2024</p>
                        </li>
                        <li>
                            <p>Produktion för snabb lansering: Med version 24.5 (16 maj 2024)</p>
                        </li>
                    </ul>
                <p><i>Den här funktionen har tagits bort från Förhandsgranska och snabb produktion.</i></p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mer relevanta smarta tilldelningar</a></p>
                    [!BADGE In production for Fast Release ]{type=Positive}
                    <p>Vi har ändrat den algoritm som Workfront använder för att beräkna och föreslå smarta tilldelningar för uppgifter. Den nya algoritmen används i följande områden i Workfront där du tilldelar en uppgift: uppgiftslistor, uppdragsområdet i uppgiftshuvudet, Hem och sammanfattningspanelen.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 21 december 2023</p>
                        </li>
                        <li>
                            <p>Produktion för snabb lansering: Med version 24.5 (16 maj 2024)</p>
                        </li>
                    </ul>
                <p><i>Den här funktionen har tagits bort från Förhandsgranska och snabb produktion.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Förbättringar av korrektur

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Korrigera problem med kopiera/klistra in för Desktop Proofing Viewer</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Vi har åtgärdat ett problem där innehåll klistras in felaktigt i uppdateringsavsnittet i Desktop Proofing Viewer.</p>
                    <p>Ny version: 2.1.39</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 2 oktober 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 2 oktober 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Tom skärmkorrigering för Windows-användare med Desktop Proofing Viewer</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Ett problem med den nya versionen av 2.1.36 Desktop Proofing Viewer som gjorde att vissa Windows-användare såg en tom skärm när de öppnade visningsprogrammet har åtgärdats. </p>
                    <p>Ny version för Windows-användare: 2.1.37</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 30 augusti 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 30 augusti 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Kromiumuppdatering för Desktop Proofing Viewer</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Vi uppgraderar Desktop Proofing Viewer till stöd för Chromium 126.0.6478.127 som löser problem med gränssnittselement i interaktiva korrektur.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 29 augusti 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 29 augusti 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Förbättringar av rapporter och kontrollpaneler

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect finns för nya planer</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Workfront Data Connect kommer att bli tillgängligt för företag som har en av de nya Workfront-planerna. Data Connect gör det möjligt för organisationer att få tillgång till sina data som en säker och skalbar datalinje, som kan analyseras och visualiseras med hjälp av verktyg för affärsintelligens eller lagras externt. Dessutom kan organisationer använda Data Connect för att visa dataanalyser som tidigare inte fanns tillgängliga, som tidsbaserad trendanalys, variabelmappning och analys av externa systemdata i kombination med Workfront-data.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                    <p><i>Endast tillgängligt för organisationer som har en av de nya Adobe Workfront-planerna. Data Connect ingår i Ultimate-planen och kan köpas som tillägg till Prime- och Select-planerna under första halvåret 2025.</i></p>
                </td>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Sammanfatta projekt eller uppdateringar med ett klick</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>För att det ska bli enklare att snabbt se högdagrar i ett projekt eller en uppdateringsström har vi lagt till knapparna Sammanfatta i dessa delar av Workfront. Nu kan du klicka på knappen för att generera en sammanfattning i AI-assistenten.</p><p>Tidigare användare kunde öppna AI Assistant och skriva in en uppmaning om att skapa en sammanfattning av projektet eller uppdateringsströmmen.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 3 oktober 2024</p>
                        </li>
                        <li>
                            <p>Produktionsrelease för alla kunder: Med version 24.10 (17 oktober 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Allmän tillgänglighet för Adobe Workfront Planning</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Workfront Planning är tillgängligt för alla kunder som har köpt en Workfront Planning-licens, utöver Workfront-licensen. Kontakta din kontorepresentant om du vill ha mer information om Workfront Planning.</p>
                    <p>Information om den senaste utgåvan av Workfront Planning varje kvartal finns i avsnittet <a href="#workfront-planning-enhancements">Förbättringar av Workfront Planning</a> nedan.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p><span class="preview">Produktionsrelease för alla kunder: 28 augusti 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe AI Assistant finns i Workfront</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Vi har lagt till Adobe AI Assistant till Workfront så att du enklare kan utföra ditt arbete. AI Assistant kan hjälpa dig genom att:</p>
                    <ul>
                        <li>Sammanfatta arbetsobjekt och dokument så att du snabbt kan få en allmän förståelse för uppgifter, projekt och resurser.</li>
                        <li>Tillhandahålla information från Experience League-dokumentation, föra in instruktioner och referensmaterial i Workfront och länka till mer ingående dokumentation.</li>
                        <li>Skapa och förfina formler för beräknade anpassade formulärfält, generera formler från textmeddelanden eller hitta fel i befintliga formler.</li>
                        </ul>
                        <p>Din Workfront-administratör kan aktivera eller inaktivera AI Assistant för din organisation. AI-assistenten är tillgänglig för instanser med planerna Select, Prime och Ultimate.</p>
                    </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsversion: 28 augusti 2024</p>
                        </li>
                        <li>
                            <p class="preview">Produktionsrelease: 28 augusti 2024</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Uppdateringar av utseende och känsla under den fjärde perioden i kvartalet 2024 </a></p>
                    <p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för det fjärde kvartalet 2024. Granska de enskilda versionsinformationen för specifika releasedatum.</p>
                </td>
                <td><p><b>Tillgängligt på följande datum:</b></p>
                    <ul>
                        <li>
                            <p>Förhandsgranskningsversion: Under den fjärde kvartersutgåvan 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Produktionsrelease: Granska versionsinformationen för specifika datum</span></p>
                        </li>
                    </ul>
                </td>
            </tr>                            
        </tbody>
</table>

### Funktioner som snart ska tas bort från Workfront

Följande funktioner kommer snart att tas bort från Workfront:

#### Borttagning av den gamla hemupplevelsen med 24.10

Vi kommer officiellt att ta bort den gamla hemupplevelsen med version 24.10. Vi rekommenderar att du börjar använda nya Home, som även i fortsättningen kommer att utökas med ytterligare funktioner innan borttagningen.

## Meddelanden

### Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än den fjärde utgåvan av kvartal 2024. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Förbättringar av Workfront Planning

Nya funktioner i Workfront Planning finns i Production. Mer information om de senaste funktionerna finns i [Versionsaktiviteten för Adobe Workfront Planning Fjärde kvartalet 2024](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Förbättringar av Workfront Scenario Planner

Det finns för närvarande inga uppdateringar av scenarioplanen i den här versionen. Det här området uppdateras när det finns uppdateringar.

### Workfront Proof-förbättringar

Det finns inga Workfront Proof-uppdateringar just nu. Det här området uppdateras när det finns uppdateringar.

### Förbättringar av Workfront-mål

Det finns inga Workfront Goals-uppdateringar just nu i den här versionen. Det här området uppdateras när det finns uppdateringar.

### API-version 19

För API-version 19 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 19](/help/quicksilver/wf-api/api/new-api-version-19.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes i den fjärde utgåvan av kvartal 2024 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

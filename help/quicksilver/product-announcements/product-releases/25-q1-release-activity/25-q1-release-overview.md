---
title: Första utgåvan, kvartal 2025, översikt
description: Den här sidan innehåller information om de funktioner som ingår i den första utgåvan av kvartalet 2025. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: ec74d34bc69f2f1424414453f9fdf94e539a75fd
workflow-type: tm+mt
source-wordcount: '2786'
ht-degree: 0%

---

# Första utgåvan, kvartal 2025, översikt

Den här sidan innehåller information om de funktioner som ingår i den första utgåvan av kvartalet 2025. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.

<span class="preview">Funktioner utanför cykeln (de som lanserades till Produktion före första utgåvan av kvartal 2025) är markerade i gult.</span>

>[!IMPORTANT]
>
>23.3-versionen innehåller ett alternativ för att flytta organisationen till månatliga releaser. Därför har Workfront ändrat numreringsschemat för releaser så att det tar hänsyn till både månads- och kvartalsversionerna. Det första numret anger året och det andra numret anger månaden för releasen. Exempel: Versionen för april 2025 är 25,4.
>
>Månads- och kvartalsvisa releaser planeras vara tillgängliga torsdagen den andra hela veckan i månaden, om inte annat anges.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>24.11 (14 november 2024)</li><li>24.12 (12 december 2024)</li><li>25.1 (15 januari 2025)</li></ul> | <ul><li>25.1 (16 januari 2025)</li></ul> |
>
>Observera att för den sista utgåvan av varje kvartal (25.1 detta kvartal) kommer användare med fast releaseschema att få releasen en dag i förtid.
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättringar av anslagstavlor](#boards-enhancements)
* [Förbättrad dokumenthantering](#document-management-enhancements)
* [Prioriterade förbättringar](#priorities-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Förbättringar av korrektur](#proofing-enhancements)
* [Förbättringar av rapporter och kontrollpaneler](#report-and-dashboard-enhancements)
* [Förbättrad uppdateringsström](#update-stream-enhancements)
* [Andra förbättringar](#other-enhancements)

### Administratörsförbättringar

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Affärsregler stöds nu för fler objekt</a></p>
           [!BADGE In production &#x200B;]{type=Informative}
            <p>Nu kan du skapa affärsregler och tillämpa validering på ytterligare objekt: Företag, Iteration, Resurskategori som inte är arbetsplats, Jobbroll, Användare, Tilldelning, Resurspool, Tid av, Dokument och Timme.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsgranskningsversion: 16 januari 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Jämför objekt mellan miljöer för att förbättra miljön</a></p>
           [!BADGE In production &#x200B;]{type=Informative}
            <p>För att det ska bli enklare att avgöra vilket objekt som ska ingå i ett miljöbefordringspaket har vi lagt till möjligheten att jämföra objekt i olika miljöer. Du kan sedan lägga till objekt i ett paket direkt från jämförelsen.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsgranskningsversion: 6 januari 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Fler tillgängliga objekt för miljöbefordran</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi har lagt till fler objekt för att utöka funktionerna för miljöbefordran.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsgranskningsversion: 6 januari 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>  
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Förhindra att uppgifter flyttas när det finns timmar loggade</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Eftersom flyttningar av uppgifter eller problem som har loggade timmar ibland kan orsaka problem med regelefterlevnad eller revision, har vi lagt till en inställning under Inställningar för Aktivitet och problem i installationsprogrammet som gör att du kan förhindra användare från att flytta uppgifter och problem om det finns timmar inloggade.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 19 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Inställning för att använda projekt eller användarschema för uppgifter med enkel tilldelning</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Som system- eller gruppadministratör har du nu en ny inställning som anger om Workfront ska använda projektets eller användarens schema för att beräkna tidslinjen för projektet när du tilldelar en användare till en aktivitet och både projektet och användaren är associerade med ett schema.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 21 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.12 (12 december 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Affärsreglerna stöder nu hyperlänkar</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Nu kan du inkludera hyperlänkar i det anpassade felmeddelandet för en affärsregel, som vägleder användaren om hur de kan ändra sin åtgärd inom regelbegränsningen. Den statiska URL:en kan länka till dokumentation eller andra sidor som skulle vara till hjälp för användaren.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 21 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.12 (12 december 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Det finns nu möjlighet att filtrera på inbyggda typsnittsfält</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>När du lägger till en intern fältreferens i ett anpassat formulär och den refererar till ett typsnittsfält (som Portfolio, Company eller Owner), är nu ett filteralternativ tillgängligt. Med filtret kan du begränsa vilka objekt som användare kan välja när de använder fältet. Det här anpassade filtret fungerar på samma sätt som ett filter i ett anpassat typsnittsfält, där textläget används för att definiera filtret.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 21 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.12 (12 december 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ikonen "Flytta till" har lagts till i anpassade fält</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>När ett anpassat formulär innehåller flera avsnitt med många fält kan det vara svårt att flytta ett fält från ett avsnitt till ett annat genom att dra och släppa. En"flytta till"-ikon har lagts till i varje fält, så att du kan markera det avsnitt som fältet placeras i.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 29 oktober 2024</li>
                <li>Produktion för snabb lansering: Med version 24.11 (14 november 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Förbättringar av anslagstavlor

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ändra ägare till en styrelse</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Den som har skapat en styrelse är som standard ägare. Styrelseledamot är den enda person som kan ta bort eller uppdatera brädans filter på panelen Konfigurera.</p>
            <p>Funktioner har lagts till så att Workfront systemadministratörer kan ändra ägare till en styrelse. Den nuvarande ägaren av en styrelse kan också ändra ägaren till den specifika styrelsen. Den här funktionaliteten finns för enkla, retrospektiva och Kanban-tavlor, men inte dynamiska.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 18 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Förbättrad dokumenthantering

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Redigera flera dokument samtidigt</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Nu kan du redigera flera dokument samtidigt. Du kan redigera beskrivningarna och uppdatera anpassade formulär.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 21 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.12 (12 december 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ny återkallad status tillgänglig för godkännande av dokumentversioner</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>När en ny version läggs till i ett dokument med väntande godkännanden visas nu godkännandet för den tidigare versionen som "Återkallad", vilket anger att den tidigare godkännandeprocessen har stängts på grund av att den nya versionen har lagts till.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 7 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.11 (14 november 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
            <p><i>Den här funktionen ingår i en fasad version och är endast tillgänglig för vissa kunder.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Prioriterade förbättringar

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Använd smarta filter för att hitta ditt material i prioriteter</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Använd naturligt språk för att snabbt filtrera arbetet i prioriteringslistan. Du kan skriva saker som </p>
            <ul>
                <li>Visa mig sena uppgifter</li>
                <li>Visa uppgifter som förfaller den här veckan</li>
                <li>Visa topprioriteringar</li>
            </ul>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsgranskningsversion: 9 januari 2025</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Fånga upp arbetet i prioriteringar</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Du kan använda Fånga upp mig för att minska tiden när du söker information om aktiva projekt.</p>
            <p>Med Workfront AI Assistant kan jag göra en sammanfattning av uppdateringar, överförda dokument och andra betydande ändringar av dina projekt inom följande tidsramar: 24 timmar, 3 dagar eller 7 dagar.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 20 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Visa ändringar direkt på detaljsidan i Prioriteter</a></p>
            <p>Du kan nu visa uppdateringar i realtid på informationssidan för en uppgift eller ett problem. Du kan också se om andra tittar på sidan samtidigt som du med visningsindikatorer i realtid.</p>
        </td>
        [!BADGE In production &#x200B;]{type=Informative}
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 19 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Överför och visa dokument och korrektur i prioriteter</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Nu kan du interagera med dokument och korrektur för uppgifter och utgåvor i arbetslistan och kalendern. På fliken Nya dokument kan du</p>
            <ul>
                <li>Överföra ett dokument</li>
                <li>Skapa ett korrektur</li>
                <li>Starta korrekturläsaren</li>
                <li>Och mer</li>
            </ul>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 19 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Kalendervyn är nu tillgänglig i Prioriteringar</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Du kan spåra ditt arbete med en tydlig, visuell månadskalender. Med Prioritetskalendern kan du</p>
            <ul>
                <li>Använd filter för att hitta ditt material</li>
                <li>Använd anpassade fält som status och fokusnivå för att identifiera högprioriterat arbete</li>
                <li>Använd färger för snabb sortering</li>
                <li>Och mer</li>
            </ul>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 19 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Uppdateringar i prioriteringslistan</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi har uppdaterat prioriteringslistan för att förbättra funktionerna och anpassa dem till andra områden i programmet.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 12 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Navigera till informationssidan för ett projekt från Prioriteringar</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Du kan nu navigera direkt till ett projekt i Workfront från listan Prioriteter.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 5 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Uppdaterade alternativ i kolumnen Mitt fokus i Prioriteringar</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi har uppdaterat alternativen i kolumnen Mitt fokus så att du kan prioritera och sortera ditt arbete på ett mer intuitivt sätt. De nya etiketterna innehåller</p>
            <ul>
                <li>Urgent</li>
                <li>Hög</li>
                <li>Normal</li>
                <li>Låg</li>
            </ul>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 14 november 2024</li>
                <li><span class="preview">Produktionsrelease för alla kunder: 14 november 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Visa projektinformation i Prioriteringar</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Nu kan du visa projektinformation och kommentarer från arbetslistan i Prioriteringar.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 6 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.11 (14 november 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
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
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mer relevanta tilldelningar har tagits bort från förhandsgranskning och produktion för snabbversionsmiljöer</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>En funktion som har funnits i förhandsvisningsmiljön sedan december 2023 och i den snabba produktionsmiljön sedan mars 2024 har nu tagits bort. Funktionerna lade till mer relevanta förslag på smarta uppdrag när uppgifter tilldelas.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 19 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
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
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Uppgradering av Desktop Proofing Viewer</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi har uppdaterat Desktop Viewer med den senaste versionen av Electron 3.3.0 som använder Chromium 130.0.6723.152. </p>
            <p>Senaste version: 2.1.44 </p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsgranskningsversion: 2 januari 2024</li>
                <li><span class="preview">Produktionsrelease för alla kunder: 9 januari 2025</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nytt webbläsartillägg för interaktiv granskning finns i betaversion</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi introducerar ett nytt webbläsartillägg, Adobe Workfront granskningsverktyg, som ersätter det äldre webbläsartillägget för granskning av interaktivt ZIP-innehåll. Det nya granskningsverktyget i Adobe Workfront har stöd för granskning av ZIP-innehåll i alla vanliga webbläsare.</p>
            <p>Det äldre webbläsartillägget tas bort den 28 februari 2025.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 7 november 2024</li>
                <li><span class="preview">Produktionsrelease för alla kunder: 7 november 2024</span></li>
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
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nya entiteter tillgängliga i Data Connect</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi har lagt till stöd för ett antal nya enheter i Data Connect, inklusive vissa byråspecifika enheter.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 15 januari 2025</li>
                <li>Produktionsrelease för alla kunder: 15 januari 2025</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Gräns för 25 rapporter, externa sidor eller kalendrar i kontrollpaneler</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>För att behålla kontrollpanelens prestanda har vi implementerat en gräns för det totala antalet rapporter, externa sidor eller kalendrar som kan placeras på en kontrollpanel. När du skapar en ny kontrollpanel kan högst 25 objekt läggas till.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 16 december 2024</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Knapp för att skapa konto för förstagångsläsare för dataanslutning</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Administratörer som använder Data Connect för första gången kan nu skapa ett nytt Snowflake Reader-konto genom att klicka på en enda knapp. Processen tar några minuter, men kräver ingen ytterligare åtgärd.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 14 november 2024</li>
                <li><span class="preview">Produktionsrelease för alla kunder: 14 november 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Förbättrad uppdateringsström

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Releasedatum</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Uppdaterad kommentarsfunktion i widgeten Mentions i området Home och My Updates</a></p>
            <p>Vi uppdaterar kommentarsfunktionerna i widgeten Meningar i Hem och i avsnittet Meningar i området Mina uppdateringar. Nu finns samma upplevelse i uppdateringsområdet för de flesta Workfront-objekt även i widgeten Mentions och i avsnittet Mentions i Mina uppdateringar.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 19 december 2024</li>
                <li>Produktionsrelease för alla hemanvändare: Ska tillkännages</li>
                <li>Produktionsrelease för alla kunder för Mina uppdateringar: 19 juni 2025</li>
            </ul>
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
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Uppdatera hur flyttade eller borttagna resurser i länkade mappar hanteras</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Vi har ändrat det sätt på vilket flyttade och borttagna resurser hanteras när vi använder Adobe Workfront-integreringen med Experience Manager Assets och Assets Essentials:</p>
            <ul>
                <li>Borttagna resurser: När en resurs tas bort inuti en länkad mapp i Assets eller Resurser Essentials behålls den borttagna resursen i området Projektdokument.</li>
                <li>Flyttade resurser: När en resurs flyttas utanför en länkad mapp i Assets eller Assets Essentials behålls den flyttade resursen i området Projektdokument.</li>
            </ul>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 21 november 2024</li>
                <li><span class="preview">Produktionsrelease för alla kunder: 5 december 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Avsnitt i ett anpassat formulär kan nu komprimeras och utökas</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>När ett anpassat formulär med flera avsnitt är kopplat till ett objekt kan du nu komprimera och expandera alla avsnitt utom standardavsnittet högst upp i formuläret. Administratören kan även se den här funktionen när formuläret förhandsgranskas i formulärdesignern.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 11 november 2024</li>
                <li>Produktion för snabb lansering: Med version 24.12 (12 december 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            AI Assistant kan nu arbeta med projekt, uppgifter och problem</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>För att göra det enklare att hantera dina arbetsuppgifter i Workfront har vi uppdaterat AI Assistant för att arbeta med projekt, uppgifter och problem. Nu kan AI Assistant hitta projekt, uppgifter och problem baserat på kriterier som du anger.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsversion: 31 oktober 2024</li>
                <li>Produktion för snabb lansering: Med version 24.11 (14 november 2024)</li>
                <li>Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Uppdateringar av utseende och känsla under första kvartalet 2025</a></p>
            <p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för första kvartalet 2025. Granska de enskilda versionsinformationen för specifika releasedatum.</p>
        </td>
        <td>
            <p><b>Tillgängligt på följande datum:</b></p>
            <ul>
                <li>Förhandsgranskningsversion: Under den första kvartersreleasen 2025</li>
                <li><span class="preview">Produktionsrelease: Granska versionsinformationen för specifika datum</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## Meddelanden

### Workfront Fusion-förbättringar

>[!IMPORTANT]
>
>Workfront Fusion-dokumentationen har flyttats till en ny plats. Mer information, instruktioner och releaser för Fusion finns i [Workfront Fusion-dokumentationen](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/home).
>
>Varje aktuell Fusion-dokumentationsartikel innehåller en länk till motsvarande artikel på den nya platsen. Uppdatera bokmärkena.
>
>Den aktuella Fusion-dokumentationsuppsättningen uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än den första utgåvan av kvartal 2025. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Förbättringar av Workfront Planning

Nya funktioner i Workfront Planning finns i Production. Mer information om de senaste funktionerna finns i [Adobe Workfront Planning First Quarter 2025 Release Activity](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

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

Mer information om underhållsuppdateringar som gjordes under den första utgåvan av kvartal 2025 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront-sidan ](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).

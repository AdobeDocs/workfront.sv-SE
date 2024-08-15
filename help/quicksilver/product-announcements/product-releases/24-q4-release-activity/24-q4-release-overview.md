---
title: Fjärde kvartersversionen 2024 - översikt
description: Den här sidan innehåller information om funktioner som ingår i den fjärde utgåvan av kvartalet 2024. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 5138321543175cac3e51cc21c8309cbefd8bc1e8
workflow-type: tm+mt
source-wordcount: '1072'
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
>| <ul><li>24.8 (augusti 2024)</li><li>24.9 (september 2024)</li><li>24.10 (oktober 2024)</li></ul> | <ul><li>24.10 (oktober 2024)</li></ul> |
>
>Observera att för den sista utgåvan av varje kvartal (24.10 i kvartal) kommer användare med fast releaseschema att få releasen en dag i förtid.
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar]
* [Projektförbättringar](#project-enhancements)
* [Integration enhancements](#integration-enhancements)
* [Andra förbättringar](#other-enhancements)

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Layoutknappen i den anpassade formulärdesignern tillåter två eller tre kolumner</a></p>
                        <p>Med en layoutknapp i den anpassade formulärdesignern kan du välja mellan två- eller trekolumnsarbetsytor. Den ursprungliga formulärdesignern använder tre kolumner och fältinställningarna visas i kolumnen längst till höger. Om du markerar två kolumner visas fältinställningarna intill fältbiblioteket i kolumnen längst till vänster.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 augusti 2024</p>
                            </li>
                            <li>
                                <p>Production for fast release: Med version 24.9 (september 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: TBD</p>
                            </li>
                        </ul>
                        <p><i>Den här funktionen ingår i en fasad version och kommer att vara tillgänglig för ett begränsat antal kunder i september.</i></p>
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
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.10 (oktober 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mer relevanta smarta tilldelningar</a></p>
                        [!BADGE In production ]{type=Informative}
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
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.10 (oktober 2024)</p>
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


### Andra förbättringar

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
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
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe AI Assistant finns i Workfront</a></p>
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
           </tbody>
        </table>

## Meddelanden

### Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än den fjärde utgåvan av kvartal 2024. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Förbättringar av Workfront Scenario Planner

Det finns för närvarande inga uppdateringar av scenarioplanen i den här versionen. Det här området uppdateras när det finns uppdateringar.

### Workfront Proof-förbättringar

Det finns inga Workfront Proof-uppdateringar just nu. Det här området uppdateras när det finns uppdateringar.

### Förbättringar av Workfront-mål

Det finns inga Workfront Goals-uppdateringar just nu i den här versionen. Det här området uppdateras när det finns uppdateringar.

### API-version 18

För API-version 18 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes i den fjärde utgåvan av kvartal 2024 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Funktioner som snart ska tas bort från Workfront

Följande funktioner kommer snart att tas bort från Workfront:

#### Borttagning av den gamla hemupplevelsen med 24.10

Vi kommer officiellt att ta bort den gamla hemupplevelsen med version 24.10. Vi rekommenderar att du börjar använda nya Home, som även i fortsättningen kommer att utökas med ytterligare funktioner innan borttagningen. Mer information om övergången, inklusive vad användare och administratörer kan göra för att förbereda, kommer.

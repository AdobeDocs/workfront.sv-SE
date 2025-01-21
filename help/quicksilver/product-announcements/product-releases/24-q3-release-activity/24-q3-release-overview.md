---
title: Översikt över utgåvan för tredje kvartalet 2024
description: Den här sidan innehåller information om funktioner som ingår i utgåvan för tredje kvartalet 2024. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: e620074ab0509e3052678e8c7e46e9629f3b34f2
workflow-type: tm+mt
source-wordcount: '1830'
ht-degree: 0%

---

# Översikt över utgåvan för tredje kvartalet 2024

Den här sidan innehåller information om funktioner som ingår i utgåvan för tredje kvartalet 2024. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.

Webbseminariet live 24.7 avbröts, men du kan fortfarande [se en videodemonstration om 24.7-funktioner här](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Funktioner utanför cykeln (de som lanserades till Produktion före tredje kvartalet 2024-utgåvan) är markerade i gult.</span>

>[!IMPORTANT]
>
>23.3-versionen innehåller ett alternativ för att flytta organisationen till månatliga releaser. Därför har Workfront ändrat numreringsschemat för releaser så att det tar hänsyn till både månads- och kvartalsversionerna. Det första numret anger året och det andra numret anger månaden för releasen. Exempel: Versionen för april 2024 är 24.4.
>
>Månads- och kvartalsvisa releaser planeras vara tillgängliga torsdagen den andra hela veckan i månaden, om inte annat anges.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>24.5 (16 maj 2024)</li><li>24.6 (13 juni 2024)</li><li>24.7 (18 juli 2024)</li></ul> | <ul><li>24.7 (18 juli 2024)</li></ul> |
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättrad ekonomisk förvaltning](#financial-management-enhancements)
* [Integration enhancements](#integration-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Förbättringar av korrektur](#proofing-enhancements)
* [Förbättrad resurshantering](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Affärsregler är nu tillgängliga</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Administratörer kan nu lägga till affärsregler under Konfigurera i Workfront.</p>
                        <p>Med en affärsregel kan du validera Workfront-objekt och hindra användare från att skapa, redigera eller ta bort ett objekt när vissa villkor är uppfyllda. Reglerna byggs med en formel som liknar beräkningsfält i anpassade formulär.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 4 juli 2024</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.7 (18 juli 2024)</p>
                            </li>
                        </ul>
                        <p><i>Gäller endast för organisationer som har den nya Ultimate-planen.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Anpassad formulärdesigner är vanligtvis tillgänglig i Adobe Workfront</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Med version 24.7 blir blankettkonstruktören allmänt tillgänglig och blir standardupplevelsen när man skapar och redigerar anpassade blanketter i Adobe Workfront. När du skapar ett nytt anpassat formulär eller öppnar ett befintligt, visas formulärdesignerns arbetsyta i arbetsytan.</p>
                        <p>Efter den här versionen har du inte längre möjlighet att återgå till det tidigare formulärverktyget.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 19 juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Flytta objekt mellan Workfront-miljöer med miljöbefordran</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Med miljöfrämjande funktioner kan du flytta objekt från en Workfront-miljö till en annan, till exempel från en sandlådemiljö till en produktionsmiljö. Du kan konfigurera och testa objekt utan risk för organisationens data och poster. Du kan sedan flytta dessa objekt till produktion utan att behöva konfigurera om dem, vilket sparar tid och arbete.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.6 (13 juni 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Dela anpassade formulär och anpassade fält i den anpassade formulärdesignern</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Nu kan du dela både anpassade formulär och anpassade fält i den nya formulärdesignern. Detta möjliggör bättre samarbete mellan användare i anpassade formulär.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 6 juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsrelease för alla kunder: 13 juni</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Lägg till ett nytt anpassat fält från fältområdet</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Nu kan du lägga till ett nytt anpassat fält eller en ny widget direkt från fältområdet i Workfront, utan att öppna ett anpassat formulär för att skapa fältet. På så sätt kan du snabbt skapa återanvändbara anpassade fält.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 6 juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Flervalsfälttyp som är tillgänglig i formulärdesignern</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>För att du enklare ska kunna definiera listrutefält har vi lagt till flervalsfältet i den anpassade formulärdesignern. Med den här fälttypen kan användare välja mer än ett alternativ i en listruta.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 4 juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 4 juni 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Förbättrad ekonomisk förvaltning

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Fakturerbara och ej fakturerbara utgiftsfält tillgängliga för projekt och uppgifter</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>För att du enklare ska kunna visa utgiftstyper har utgifterna delats upp i fakturerbara och icke-fakturerbara utgifter för projekt och uppgifter. Följande fält är tillgängliga för att du ska kunna lägga till i vyer och rapporter:</p>
                        <ul>
                            <li><p>Planerad fakturerbar utgift</p></li>
                            <li><p>Planerad icke-fakturerbar utgift</p></li>
                            <li><p>Faktisk icke-fakturerbar utgift</p></li>
                            <li><p>Faktisk icke-fakturerbar utgift</p></li>
                        </ul>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 10 maj 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 10 maj 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Förbättringar av Workfront för Experience Manager Assets och Assets Essentials</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Vi har gjort följande förbättringar för integreringen av Workfront för Experience Manager Assets och Assets Essentials:</p>
                        <ul>
                            <li><p>Integreringen har nu stöd för GCP som molntjänstleverantör. AWS och Azure stöddes tidigare.</p></li>
                            <li><p>Storleksgränsen för filer som skickas till Experience Manager via integreringen har ökat till 30 GB. Tidigare var gränsen 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 27 juni 2024</p>
                            </li>
                            <li>
                                <p>Produktion för alla kunder: Med version 24.7 (18 juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Redigera aktiviteten och skicka bekräftelsedatum och villkor från huvud- eller detaljavsnittet</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>För att göra det enklare för dig att uppdatera uppgifter och ärenden har vi nu lagt till fälten Genomför datum och villkor som alternativ att lägga till i åtgärdshuvuden och utgivningsrubriker och Detaljer i en layoutmall. Användarna kan nu uppdatera dessa fält från sidhuvudet eller detaljavsnittet på en sida när de tilldelas den ändrade layoutmallen.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 30 maj 2024</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 24.6 (13 juni 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Fler relevanta tilldelningar har lagts till i arbetsflödet Ny uppgift</a></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mer relevanta smarta tilldelningar</a></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Säkerhetsuppdateringar för Desktop Proofing Viewer</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Säkerhetsuppdateringen Workfront Proof Desktop Proofing Viewer 2.1.35 innehåller säkerhetsfelkorrigeringar för säkerhetsluckor som har identifierats i tidigare versioner.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 4 juli 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 4 juli 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Förbättrad resurshantering

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Ledig tid återspeglas nu i arbetsbelastningsutjämnaren</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>För att smidigt justera arbete när den primära tilldelaren för en aktivitet har en schemalagd tid inaktiverad, omfördelar nu arbetsbelastningsutjämnaren timmar till både den primära och den sekundära användaren när projekttidslinjen beräknas om.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 6 juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.7 (18 juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Byt bakgrund till produktguider</a></p>
                        <p>Vi implementerar en teknikförändring för våra produktguider under de kommande veckorna. Vi har försökt minimera effekten av den här övergången, men vissa användare kan stöta på guider som de tidigare har sett.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Produktion för alla kunder: Inkrementellt till mitten av augusti 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience finns nu för fler Workfront-organisationer</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>För att ge företag och organisationer tillgång till fördelarna med Adobe Unified Experience har vi börjat göra den tillgänglig för befintliga Workfront-kunder. </p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 20 juni 2024</p>
                            </li>
                            <li>
                                <p>Produktion för angivna kunder: Med version 24.7 (18 juli 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Det enhetliga Adobe-skalet görs tillgängligt i en fasad utrullning. Ytterligare organisationer kommer att ingå i Adobe Unified Shell med versionerna 24.10 och 25.1. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Hjälpknappen har tagits bort från navigeringsfältet</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Hjälpknappen i huvudnavigeringsfältet har tagits bort för att ge en enhetlig upplevelse för användare som inte använder det enhetliga gränssnittet. Den här knappen, som inte finns för användare i Unified Shell, är länkad till Workfront-dokumentationen och överflödig med en liknande hjälpknapp tillgänglig för alla användare på huvudmenyn.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 6 juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsrelease för alla kunder: Med version 24.7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Förbättrat användargränssnitt för användare med begränsad objektåtkomst</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>När en användare inte har åtkomst till ett objekt visas"Ingen åtkomst" var som helst där objektnamnet visas i Workfront. Den här förbättrade upplevelsen gäller även Workfront API.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 27 mars 2024</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 24.5 (16 maj 2024)</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 24.7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Uppdateringar av utseende och känsla under tredje kvartalet 2024 </a></p>
                        <p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för tredje kvartalet 2024. Granska de enskilda versionsinformationen för specifika releasedatum.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsgranskningsversion: Under den tredje kvartersversionen 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsrelease: Granska versionsinformationen för specifika datum</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## Meddelanden

### Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production på en cadence som ligger utanför den tredje utgåvan av kvartal 2024. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

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

Mer information om underhållsuppdateringar som gjordes under tredje kvartersversionen 2024 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

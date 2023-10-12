---
title: Versionsöversikt för fjärde kvartalet 2023
description: Versionsöversikt för fjärde kvartalet 2023
author: Becky
feature: Product Announcements
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: cc7e0d3a44d81149cd691332821df016b9e57419
workflow-type: tm+mt
source-wordcount: '2528'
ht-degree: 0%

---

# Versionsöversikt för fjärde kvartalet 2023

Den här sidan innehåller information om funktioner som ingår i den fjärde utgåvan av kvartalet 2023. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön för alla kunder med 23.10-utgåvan den 26 och 27 oktober 2023.

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

Webbseminariet 23.10 släpptes den 5 oktober 2023. Du kan [registrera dig för webbinariet för att visa en on-demand-inspelning här](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">Funktioner utanför cykeln (de som lanserades till Production före fjärde utgåvan av kvartal 2023) markeras med gult.</span>

>[!IMPORTANT]
>
>23.3-versionen innehåller ett alternativ för att flytta organisationen till månatliga releaser. Därför ändrar Workfront numreringsschemat för releaser så att det tar hänsyn till både månads- och kvartalsvisa versionsspår.
>
>* Om du är på **snabb release (månadsvis)** track, the release after 23.3 is **23.8**, den 31 augusti 2023.
> * Om du är på **kvartalsvis** release track, the release after 23.3 is **23.10**, i veckan den 26 oktober 2023.
> 
> Kvartalsvisa releaser kommer att innehålla funktionalitet från tre månadsversioner. Den 23.10 kvartalsversionen kommer till exempel att innehålla funktioner som släpptes i månadsversionerna 23.8, 23.9 och 23.10.
>
>Månads- och kvartalsvisa releaser planeras bli tillgängliga den sista torsdagen i månaden.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>23.8 (31 augusti 2023)</li><li>23.9 (28 september 2023)</li><li>23.10 (26 oktober 2023)</li></ul> | <ul><li>23.10 (vecka 26 oktober 2023)</li></ul> |
>| <ul><li>Ingen release (november 2023)</li><li>Ingen release (december 2023)</li><li>24.1 (januari 2024)</li></ul> | <ul><li>24.1 (januari 2024)</li></ul> |
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättringar av anslagstavlor](#boards-enhancements)
* [Förbättrad finansiell hantering](#financial-management-enhancements)
* [Hemförbättringar](#home-enhancements)
* [Integration enhancements](#integration-enhancements)
* [Projektförbättringar](#project-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Beräknade fält i anpassade formulär kan nu använda jokertecknet $$USER</a></p>
                        <p>Jokertecknet $$USER är nu tillgängligt i beräknade anpassade fält och externa sökfält i den nya formulärdesignern.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 5 oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Lägg till värdealternativ från ett externt API till ett anpassat formulär</a></p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>En ny fälttyp, <strong>Extern sökning</strong>finns nu på den anpassade formulärdesignern. När du har data lagrade på ett externt system kan du med den här fälttypen läsa in alternativ från ett externt API och filtrera baserat på andra fältvärden i det anpassade formuläret.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 14 september 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.9</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Underuppgifter finns nu på Adobe Workfront Boards</a></p><span style="color: #ff0000;"> Nyheter i förhandsvisning!</span><p>När du lägger till ett anslutet kort till en anslagstavla för en Workfront-uppgift importeras alla befintliga underaktiviteter till kortet. När du skapar en underaktivitet på ett anslutet kort läggs en underaktivitet till i Workfront-aktiviteten.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion för tidig åtkomst till styrelser: Ej tillämpligt</p>
                            </li>
                            <li>
                                <p>Production for fast release: Ej tillämpligt</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Förbättringar av användartilldelningar på kort och kort</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Nu finns det förbättringar som ger större flexibilitet när du lägger till användare på kort och kort i Adobe Workfront Boards.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 21 augusti 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 24 augusti 2023</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Lägga till dokument på anslutna kort</a></p><p>Nu kan du bifoga dokument på anslutna kort på Adobe Workfront Boards. Alla dokument som du lägger till på kortet blir tillgängliga på fliken Dokument i den anslutna uppgiften eller utgåvan, och samma filtyper stöds i båda områdena.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 21 augusti 2023</p>
                            </li>
                            <li>
                                <p>Production for Boards tidig åtkomst: 24 augusti 2023</p>
                            </li>
                            <li>
                                <p>Production for fast release: Ej tillämpligt</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Dokument som är tillgängliga på anslutna kort är skrivskyddade</a></p><p>För anslutna kort på Adobe Workfront Boards kan du nu visa dokument som bilder och PDF. Du kan antingen förhandsgranska ett dokument i webbläsaren eller hämta det till datorn. </p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 3 augusti 2023</p>
                            </li>
                            <li>
                                <p>Production for Boards tidig åtkomst: 10 augusti 2023</p>
                            </li>
                            <li>
                                <p>Production for fast release: Ej tillämpligt</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Styrelsevy för ett projekt som nu är tillgängligt för frågor</a></p><p>Du kan nu få åtkomst till en vy över en projektutgåva. Kanban-panelen kan hjälpa dig att spåra problemets förlopp på ett mer visuellt sätt än att visa dem i listan. </p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 3 augusti 2023</p>
                            </li>
                            <li>
                                <p>Produktion för tidig åtkomst till styrelser: Ej tillämpligt</p>
                            </li>
                             <li>
                                <p>Production for fast release: Ej tillämpligt</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>    
           </tbody>
        </table>

### Förbättrad finansiell hantering

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Datum för gällande kostnad och faktureringstariffer</a></p>
                        <p>Giltig kostnad och faktureringstariffer är nu tillgängliga för företagets, användarens och jobbrollens objekt i Workfront. När gällande datumsatser tillämpas på ett projekt, och timmar loggas på projektuppgifter, beräknas kostnader och intäkter med hjälp av de angivna tarifferna för varje tidsperiod.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 29 juni 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Ny widget för bokrutor för nytt hem</a> <span style="color: #ff0000;"> Nyheter i förhandsvisning!</span></p>
                        <p>Förutom de nya arbetshanteringsalternativen i Nytt hem kan du nu visa en anslagstavla på startsidan!</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Ny startsida för medverkande: Ny startsida</a> <span style="color: #ff0000;"> Nyheter i förhandsvisning!</span> </p>
                        <p>Ny startsida är nu standardstartsida för medverkarkonton. Den nya standardstartsidan innehåller ett antal widgetar som är särskilt valda för att hjälpa medarbetarna att hantera sitt arbete direkt.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Ändringar i arbetsspårning i Nytt hem </a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Baserat på användarfeedback har vi tagit bort det sidomfattande tidsintervallfiltret och sammanfattningsfältet som justerade uppgifter som förfaller och slutförs. Widgetarna Projekt, Uppgift och Utgåva har inbyggda filtreringsfunktioner som gör att du kan anpassa deras omfång individuellt.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 13 september 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.9</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nya snabbåtkomstknappar för widgetarna Projekt, Uppgift och Ärendespårning</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Ytterligare utökade möjligheter att hantera material direkt från Nytt hem, nya snabbåtkomstknappar har lagts till i widgetarna Projekt, Aktivitet och Ärendespårning.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 13 september 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.9</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nya filteralternativ för Nytt hem</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Nya filteralternativ är nu tillgängliga för widgeten Mitt arbete i Nytt hem. Alternativen är filter för objekttyper (uppgifter, problem och begäranden) och status (inte redo, klar att börja, arbeta med och slutförd).</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 17 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Stöd för anpassad terminologi i Nytt hem</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>För att bättre kunna tillgodose organisationernas unika behov använder Nytt hem nu anpassad terminologi för objekt som definieras i en förekomsts layoutmallar. Om till exempel"Projekt"-objekt har omdöpts till"Kampanjer" i din Workfront-instans visas widgeten Mina projekt som Mina kampanjer i Nytt hem.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 17 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 31 augusti 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Knappen Ny startsida har tagits bort för konton som har inaktiverat Ny startsida</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Knappen Testa ny startsida finns inte längre för konton där Ny startsida har inaktiverats. Nytt hem måste aktiveras på nytt av systemadministratören innan enskilda användare kan använda knappen för att prova Nytt hem.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 17 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Växla till Ny standardwidget för hem</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Widgeten Att göra, som kräver behörighet att skapa uppgifter, finns nu bara i standardwidgetuppsättningen för användare med licenstyperna Standard, Plan och Work. Dessutom har widgeten automatiskt tagits bort från startsidorna för användare med alla andra licenstyper.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 17 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p>Production for fast release: 17 augusti 2023</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis utgivning: 17 augusti 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Förbättrade upplevelser när du skickar dokument till SharePoint (GraphAPI)</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Vi har gjort några ändringar som gör det enklare att hitta mappar när du skickar dokument till dina SharePoint-mappar (GraphAPI)</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 24 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 31 augusti 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Uppgraderingar för att dra och släppa för dokumentintegreringar</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Vi har gjort några förbättringar för att lägga till tydlighet och ta bort användarfel när en fil dras och släpps till en länkad mapp.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 24 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion för alla kunder: 31 augusti 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Godkännanden av nya dokument</a> <span style="color: #ff0000;"> Nyheter i förhandsvisning!</span></p>
                        <p>I den här versionen har godkännandeprocessen effektiviserats både för att skapa godkännanden och för att godkänna/granska dokument, utöver den nya funktionen.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 oktober 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Den här funktionen ingår i en fasad version och är för närvarande endast tillgänglig för vissa kunder.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Uppdaterad design när en ny utgåva läggs till i ett projekt</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Den här uppdateringen har annonserats med version 23.3.</p>
                        <p>Vi har uppdaterat rutan Nytt problem som visas när du skickar in en ny utgåva till ett projekt. Nu matchar gränssnittet rutan Ny begäran som visas när en ny begäran skickas till en begärandekö.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 26 juli 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Dynamisk omberäkning av beräknade fält i formulär</a></p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Beräknade fält i ett formulär som är kopplat till ett objekt omberäknas nu dynamiskt i realtid när beroende värden på något formulär på sidan ändras. På så sätt kan du se de uppdaterade resultaten utan att spara formuläret.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 17 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Ange planerade timmar för återkommande underordnade uppgifter med enkel varaktighet utan tilldelningar</a></p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Vi har gjort en ändring i hur Planerade timmar tilldelas återkommande uppgifter utan tilldelningar och med en typ av enkel varaktighet. När du nu anger Planerade timmar för en ny återkommande aktivitet med enkel varaktighetstyp och utan tilldelningar, tilldelas även timmarna till de enskilda perioderna. Före den här ändringen sparades inte timmarna för enskilda återkommande aktiviteter när de överordnade aktiviteterna inte tilldelades.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 17 augusti 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Uppdaterade e-postmallar</a> <span style="color: #ff0000;"> Nyheter i förhandsvisning!</span></p>
                        <p>Vi har uppdaterat två av de vanligaste e-postmeddelandena som utgör början på ett nytt initiativ för att uppdatera våra e-postmeddelanden om evenemang: dokumentgodkännande och objektdelning.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Ändringar på huvudmenyn för Contributor</a> <span style="color: #ff0000;"> Nyheter i förhandsvisning!</span></p>
                        <p>Om du vill informera medarbetarna bättre om vilka funktioner som är tillgängliga med en betald Workfront-licenstyp kan de nu se alla alternativ som finns på huvudmenyn.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsversion: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Med version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis lansering: Med version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Förbättringar av kommentarupplevelsen</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Förbättringar av uppdateringsavsnittet görs tillgängliga inom tidsramen för den fjärde utgåvan av kvartal 2023 för betaversionen av kommentarsfunktionen. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön för alla kunder med den fjärde utgåvan av kvartal 2023 (oktober 2023).</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsgranskningsversion: Under den fjärde kvartersversionen 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Från och med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis utgivning: Med version 23.10 (om inget annat anges)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nya betaversioner av Canvas Dashboards</a> </p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
                        <p>Förbättringar av arbetsytans kontrollpaneler görs tillgängliga inom tidsramen för den fjärde utgåvan av kvartal 2023 som en del av den pågående betaversionen. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön för alla kunder med den fjärde utgåvan av kvartal 2023 (oktober 2023).</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsgranskningsversion: Under den fjärde kvartersversionen 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion för snabb lansering: Från och med version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion för kvartalsvis utgivning: Med version 23.10 (om inget annat anges)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Uppdateringar av utseende och känsla under fjärde kvartalet 2023</a></p><p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för det fjärde kvartalet 2023. Granska de enskilda versionsinformationen för specifika releasedatum.</p>
                    </td>
                    <td><p><b>Tillgängligt på följande datum:</b></p>
                        <ul>
                            <li>
                                <p>Förhandsgranskningsversion: Under den fjärde kvartersversionen 2023</p>
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

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än den fjärde utgåvan av kvartal 2023. Mer information om de senaste funktionerna finns i [Versionsaktivitet för Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Förbättringar av Workfront Scenario Planner

Det finns för närvarande inga uppdateringar av scenarioplanen i den här versionen. Det här området uppdateras när det finns uppdateringar.

### Förbättringar av Workfront-korrektur

Det finns för närvarande inga Workfront Proof-uppdateringar. Det här området uppdateras när det finns uppdateringar.

### Förbättringar av Workfront-mål

Det finns inga Workfront Goals-uppdateringar just nu i den här versionen. Det här området uppdateras när det finns uppdateringar.

### API-version 17

API version 17 släpptes 12 oktober 2023. För API-version 17 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns på [Nyheter i API-version 17](/help/quicksilver/wf-api/api/new-api-version-17.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes i version 2.3 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet &quot;Nyheter&quot; i [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Funktioner som snart ska tas bort från Workfront

Följande funktioner kommer snart att tas bort från Workfront:

#### Borttagning av mobilappen Proof med 23.10

Vi kommer officiellt att ta bort mobilappen Proof i version 23.10. Den allmänna Workfront-mobilappen har förbättrats med nya korrekturfunktioner (mer information finns i versionsinformationen under Workfront Mobile-förbättringarna) och användare rekommenderas att börja använda den för korrekturläsning så snart som möjligt.

Observera att Workfront mobilapp kräver en Workfront-inloggning. Externa användare och gäster kan fortsätta att använda Korrektur-appen för korrekturarbete, men det stöds inte längre och kommer inte att vara tillgängligt med version 23.10.

#### Arbetsflöden som tagits bort för konton som inte använder dem

För konton som aldrig har skapat ett arbetsflöde i Adobe Workfront Boards har Workstreams-området tagits bort från instrumentpanelen för paneler den 11 oktober 2023. Konton som använder arbetsflöden har fortfarande tillgång till dem. Förbättrade trumfunktioner kommer att åtgärdas i framtida versioner.

<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->

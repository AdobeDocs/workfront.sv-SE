---
product-area: home
navigation-topic: use-the-home-area
title: Gå från äldre startsida till ny startsida
description: Äldre startsida tas bort från Workfront den 10/17 med Q4-versionen. Den här artikeln innehåller information om vilka funktioner som kommer att vara tillgängliga i det nya hemmet samt rekommendationer om hur du flyttar användare till det nya hemmet.
author: Courtney
feature: Get Started with Workfront
source-git-commit: b34de7dc66d69b030e313ee891a7404e1d5470e8
workflow-type: tm+mt
source-wordcount: '1596'
ht-degree: 0%

---


# Gå från äldre startsida till ny startsida

Äldre startsida tas bort från Workfront den 10/17 med Q4-versionen. Den här artikeln innehåller information om vilka funktioner som kommer att vara tillgängliga i det nya hemmet samt rekommendationer för Workfront-administratörer som flyttar användare till den nya hemupplevelsen.

Mer information om borttagning av äldre hemsidor finns i [guiden för äldre hemborttagning](/help/quicksilver/product-announcements/announcements/legacy-home-deprecation.md).


## Förstå vad som ändras från äldre startsida till nya startsidor

### Arbetslista

#### Ordna arbetet med widgeten Mitt arbete

Widgeten Mitt arbete har skapats i widgetform för att spegla den äldre hemarbetslista så nära som möjligt. Användare kan gruppera och filtrera sin arbetslista i widgeten Mitt arbete med liknande filter och grupperingar:

| **Filter** | **Gruppering** |
|------------|-----------|
| - Arbetar på <br> - Klar att starta <br> - Inte klar <br> - Begärd <br> - Delegerad <br> - Slutförd | - Projekt <br> - status <br> - Förfallodatum <br> - ingenting |


**Äldre hemgrupperingar är inte tillgängliga i Nytt hem**

* Planerat slutförandedatum - ändrat namn till förfallodatum i nytt hem
* Planerad start
* Bekräftelsedatum
* Min prioritet

| **Äldre startsida** | **Nytt hem** |
|------------|-----------|
| ![](assets/filter-list-legacy.png) | ![](assets/filter-list-my-work.png) |

#### Delegera arbete

Användare kan fortfarande delegera arbete från Nytt hem i följande widgetar:

* Mitt arbete
* Mina uppgifter
* Mina problem
* Väntar på mina godkännanden

Användare kan hitta arbete som delegerats till dem i följande widgetar:

* Min arbetswidget använder filtret Delegerat till mig
* Väntar på mina godkännanden med hjälp av filtret för delegerade godkännanden

| **Äldre startsida** | **Nytt hem** |
|------------|-----------|
| ![](assets/delegate-legacy.png) | ![](assets/delegate-my-work.png) |

#### Använda kalendervyn

Kalendervyn är inte längre tillgänglig i Nytt hem, men en kalenderersättning finns på färdplanen för prioriteringar.

#### Skapa en personlig uppgift

Användare kan inte längre skapa en personlig uppgift på samma sätt som i den äldre hemsidan, utan användare kan i stället skapa att göra-uppgifter.

#### Visa godkännanden som jag har skickat in

Användarna kan inte visa godkännanden som de har skickat in i Nytt hem. Om användare i din organisation behöver den här funktionen kan du skapa en godkännanderapport som en tillfällig lösning eller lägga upp en kommentar här i följande communityinlägg:

* [Lägg till widgeten&quot;Godkännanden jag har skickat&quot; i nytt hem](https://experienceleaguecommunities.adobe.com/t5/workfront-ideas/add-quot-approvals-i-submitted-quot-widget-to-new-home/idc-p/704664#M25269)
* [Lägg till&quot;Godkännanden som jag har skickat&quot; i det nya startfönstret](https://experienceleaguecommunities.adobe.com/t5/workfront-ideas/add-quot-approvals-i-submitted-quot-widget-to-new-home/idc-p/704664#M25269)

#### Lägg till objekt i Min prioritet

Användare har inte längre tillgång till funktionen Min prioritet i Nytt hem. Vi introducerar en ny kolumn för Mitt fokus med prioriteringar som kommer att ersätta detta.

Användare kan använda widgeten för att spåra objekt med hög prioritet om så önskas.

### Uppdatera arbetsuppgifter

I det äldre hemmet kan användarna använda den högra panelen för att uppdatera sitt arbete. I Nytt hem använder användarna nu panelen Sammanfattning för att uppdatera arbetet. Det här är samma sammanfattningspanel som finns i Projekt, Åtgärder, Problem och Dokument.

#### Använda panelen Sammanfattning

I Sammanfattningen kan användarna

* Uppdatera procent färdigt
* Lägg till en uppdatering
* Navigera till området Dokument för att överföra ett dokument
* Visa information om arbetsuppgift och uppdatera anpassade fält
Workfront-administratörer kan anpassa vilka fält som ska visas i sammanfattningen i layoutmallen. Mer information finns i [Anpassa hem och sammanfattning med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Ändra arbetsuppgiftens status
* Visa underaktiviteter
* Loggtid
* Visa bifogade godkännandeprocesser
* Överför filer - Den här funktionen är ny

| **Äldre startsida** | **Nytt hem** |
|------------|-----------|
| ![](assets/right-panel-legacy.png) | ![](assets/summary-new-home.png) |


#### Öppna sammanfattningspanelen

Användarna kan öppna panelen Sammanfattning genom att hålla markören över arbetsposten och sedan klicka på ikonen **Sammanfattning** ![](assets/open-summary-new-home.png) .

Mer information om hur du använder panelen Sammanfattning finns i [Översikt över sammanfattning](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

#### Använd snabbåtgärder

Förutom sammanfattningspanelen kan användare även använda snabbåtgärder för att

* Loggtid
* Lägg till en uppdatering
* Uppdatera ett anpassat formulär
* Överföra en fil

Håll markören över arbetsobjektet för att hitta snabbåtgärdsmenyn. Listan med snabbåtgärder visas nära knappen **Arbeta med den** eller **Klar**.

![](assets/quick-actions-new-home.png)


### Visa godkännanden och teamförfrågningar

Användare kan fortfarande hantera godkännanden och teamförfrågningar i Nytt hem med följande widgetar:

* Väntar på mitt godkännande
* Alla godkännanden
* Teamförfrågningar

Mer information om hur du lägger till widgetar på din nya hemsida finns i [Lägg till, redigera eller ta bort widgetar i Nytt hem](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).

## Läs om tillgängliga widgetar

Widgets är grunden för New Home. Genom att lägga till widgetar på hemsidan kan användarna välja vilken typ av information som ska visas så att de bäst uppfyller sina behov. Vissa widgetar är bara tillgängliga för specifika licenstyper, eftersom de objekt de spårar bara är tillgängliga för dessa licenser.

Workfront-administratörer kan anpassa vilka widgetar som är tillgängliga i Nytt hem med hjälp av en layoutmall. Mer information finns i [Anpassa nytt hem med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md).

+++ Expandera om du vill visa en detaljerad lista över tillgängliga widgetar
Nedan finns de 11 widgetarna som du kan välja bland, samt en sammanfattning av den information de visar:

* **Mitt arbete**\
   Visar alla dina tilldelade uppgifter, utgåvor och förfrågningar på ett och samma ställe. Du kan klicka på knappen Arbeta på för att börja arbeta med ett objekt eller på knappen Klar för att markera det som färdigt. Du kan också uppdatera information (Status, Villkor, Procent färdigt) om uppgifter och problem, logga tid och lägga till uppdateringar från widgeten Mitt arbete.

* **Vandrar**\
    Visar alla ritytor som du har skapat eller har bjudits in att använda. Du kan också skapa en ny styrelse baserat på följande mallar: Grundläggande styrelse, Kanban-tavla, Perspektivpanel, Dynamisk styrelse.

* **Mina projekt**\
    Visar _projekt som du äger_ eller _projekt som du är på_ i en lista. Du kan använda befintliga filter, vyer eller grupperingar för att anpassa listan eller skapa ett projekt direkt från widgeten.

* **Mina uppgifter**\
    Visar uppgifter som du har tilldelats i en lista. Du kan använda befintliga filter, vyer eller grupperingar för att anpassa listan eller skapa en uppgift direkt från widgeten. Du kan även delegera dina uppgifter medan du inte är på kontoret.

* **Mina problem**\
    Visar problem som du har tilldelats i en lista. Du kan använda befintliga filter, vyer eller grupperingar för att anpassa listan eller skapa ett problem direkt från widgeten. Den här widgeten innehåller endast problem vars associerade projekt är inställda på Aktuell och inte slutförda projekt. Du kan även delegera dina ärenden medan du inte är på kontoret.

* **Mina förfrågningar**\
    Visar alla begäranden som du har skickat, ett filter som bara visar öppna begäranden och en knapp som öppnar sammanfattningspanelen för en begäran.

* **Teamförfrågningar**\
    Visar alla väntande begäranden för team som du är i sorterad efter team, samt knappar som du kan använda för att tilldela en användare en förfrågan direkt eller för att arbeta med den själv.

* **Väntar på mitt godkännande**\
    Visar alla väntande tilldelade eller delegerade godkännanden, en knapp för att delegera godkännanden och knappar för att fatta godkännandebeslut direkt i widgeten.

* **Alla godkännanden**\
        Visar 2 diagram med information om genomsnittlig godkännandetid och beslut samt en lista över väntande och försenade godkännanden. <span style="color: #ff0000;">Den här funktionen är en del av en fasversion och är för närvarande endast tillgänglig för vissa kunder.</span>

* **Meningar**\
    Visar senaste kommentarstrådar från hela Workfront, som liknar sidan Mina uppdateringar. Du kan använda svarsknappen för att skapa ett svar i widgeten. Den här widgeten visar också kommentarer som gjorts för uppgifter och problem som du har tilldelats, som du har tilldelat en annan användare, som du äger, som du är den primära kontakten för eller som du har skapat, så länge som uppgiften eller utgåvan har uppdaterats de senaste 30 dagarna.

* **Att göra**\
    Med den här unika widgeten kan du lägga till objekt i en personlig checklista som du kan redigera fritt. Att göra-uppgifter spåras som uppgifter i ditt personliga projekt och stannar i upp till två veckor efter att de har slutförts.

  >[!NOTE]
  >
  >Du måste ha behörighet att skapa uppgifter för att kunna skapa uppgifter i Att göra-widgeten, och bara personliga uppgifter som anges av den aktuella användaren visas i widgeten.

+++

  ![](assets/widgets-menu.png)

### Visa widgetar tillgängliga för varje licenstyp

Som standard innehåller startsidan några specifika widgetar baserat på din licenstyp. Tabellerna nedan visar vilka widgetar användare av varje licenstyp ser när de först navigerar till Nytt hem.

<table border="1" class="inlineTable">
    <tr>
        <td><b>Ny licenstyp</b></td>
        <td><b>Standardwidgetar</b></td>
    </tr>
    <tr>
        <td>Standard</td>
        <td>Mina projekt, mitt arbete, omnämnanden, uppgifter</td>
    </tr>
    <tr>
        <td>Ljus</td>
        <td>Mitt arbete, väntar på mitt godkännande</td>
    </tr>
    <tr>
        <td>Medarbetare</td>
        <td>Mina förfrågningar, omnämnanden, väntar på mitt godkännande, anslagstavlor</td>
    </tr>
    <tr>
        <td>Extern</td>
        <td>Väntar på mitt godkännande</td>
    </tr>
</table>

<table border="1" class="inlineTable">
    <tr>
        <td><b>Aktuell licenstyp</b></td>
        <td><b>Standardwidgetar</b></td>
    </tr>
    <tr>
        <td>Plan</td>
        <td>Mina projekt, omnämnanden, uppgifter</td>
    </tr>
    <tr>
        <td>Arbete</td>
        <td>Mitt arbete, omnämnanden, att göra</td>
    </tr>
    <tr>
        <td>Granska</td>
        <td>Mitt arbete, omnämnanden</td>
    </tr>
    <tr>
        <td>Begäran</td>
        <td>Mina projekt, väntar på mitt godkännande</td>
    </tr>
    <tr>
        <td>Contribute</td>
        <td>Mitt arbete, omnämnanden</td>
    </tr>
    <tr>
        <td>Extern</td>
        <td>Väntar på mitt godkännande</td>
    </tr>
</table>

## Förbered för borttagning

Nedan följer några rekommendationer som hjälper dig att underlätta övergången för att minimera störningarna för dig och din organisation.

### Börja med övergången till Nytt hem

Vår primära rekommendation är att börja gå över till nya Home så fort som möjligt. Organisativt innebär det att administratören anpassar användarnas upplevelser med hjälp av layoutmallar - som liknar dem i äldre versioner - för att säkerställa att alla användare har det de behöver.

Vi rekommenderar administratörer:

1. Skapa en standardlayout för nya startsidor med layoutmallar (eller, om du vill, skapa en för varje användare, team, grupp eller jobbroll som behöver en unik layout). Mer information finns i [Anpassa nytt hem med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md).

1. Tilldela ett litet antal testanvändare dina nya layoutmallar och kontrollera att deras widgetar och allmänna inställningar uppfyller deras behov.

1. Tilldela om de andra användarna till layouten Ny hemsida.

Om du gör detta så snart som möjligt får användarna tid att anpassa sig till den nya upplevelsen och anpassa sina nya hemsidor efter sina egna behov. Se [Ta bort, lägga till och ordna om widgetar i nya Hem](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md) för information om hur en användare kan anpassa widgetarna på sin egen nya Hem-sida.
---
navigation-topic: search
title: Sök [!DNL Adobe Workfront]
description: Du kan enkelt hitta objekt i [!DNL Adobe Workfront] genom att söka efter dem när du inte kommer ihåg deras exakta plats.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: b04d09d1244a7d7abef8aaddb62dbdf7124bfde8
workflow-type: tm+mt
source-wordcount: '1580'
ht-degree: 0%

---

# Sök [!DNL Adobe Workfront]

Du kan enkelt hitta objekt i [!DNL Adobe Workfront] genom att söka efter dem när du inte kommer ihåg deras exakta plats.

Du kan se rutan [!UICONTROL Search] i det övre högra hörnet på en sida i [!DNL Workfront].

![Ikonen Sök i navigeringsfältet](assets/search-globalnavigationbar-350x62.png)

Du måste ha behörighet att visa ett objekt innan du kan hitta det i en sökning. Därför varierar sökresultaten från användare till användare.

## Åtkomstkrav

+++ Expandera det här avsnittet om du vill visa den åtkomst som behövs för att utföra stegen i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] åtkomst till objekttypen </p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Du måste ha behörighet att visa ett objekt innan du kan hitta det i en sökning.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Förstå sökning

* [[!UICONTROL Objects available for search]](#objects-available-for-search)
* [[!UICONTROL Fields available for search]](#fields-available-for-search)

### Objekt som är tillgängliga för sökning

Du kan söka efter följande objekt i Workfront:

* Projekt
* Uppgifter
* Problem
* Rapporter
* Användare
* Mallar
* Dokument
* Portföljer
* Program
* Kontrollpaneler
* Företag
* Anteckningar

### Fält som är tillgängliga för sökning

De fält som är tillgängliga för sökning baseras på typen av sökning: Grundläggande eller [!UICONTROL Advanced Search].

* **Grundläggande sökning**: När du söker efter objekt i en grundsökning söker [!DNL Workfront] efter text som kan innehålla dina nyckelord i följande fält:

   * Objektnamn
   * Beskrivning
   * Anpassade datafält
   * Uppdateringar
   * Dokumentnamn (i specifika dokumentsökningar och i en grundläggande sökning)

  Mer information om grundläggande sökning i [!DNL Workfront] finns i [Grundläggande sökning](#basic-search) i den här artikeln.

* **[!UICONTROL Advanced Search]**: I en [!UICONTROL Advanced Search] kan du konfigurera filter för att söka efter fält som inte är tillgängliga i den grundläggande sökningen. Därför kan du i [!UICONTROL Advanced Search] söka efter alla fält i objektet.

  Mer information om [!UICONTROL Advanced Search] finns i [Avancerad sökning](#advanced-search) i den här artikeln.

>[!NOTE]
>
>Om du vill utföra en [!UICONTROL Advanced Search] måste du markera alternativet [!UICONTROL Advanced Search] när sökningen börjar. Du kan inte förfina en grundläggande sökning till en [!UICONTROL Advanced Search].

## Förstå begränsningar för [!DNL Workfront]-sökningar

Tänk på följande begränsningar när du använder [!UICONTROL Search] i [!DNL Workfront]:

* Sökningar är inte skiftlägeskänsliga
* [!DNL Workfront] rättar inte eller förstår inte stavfel
* Sökning i [!DNL Workfront] stöder inte jokertecken
* Sökning i [!DNL Workfront] stöder partiella ordsökningar, men stöder inte delsträngssökningar.\
   Söknyckelordet &quot;ställ&quot; returnerar till exempel resultat som innehåller ordet &quot;standard&quot;, men returnerar inte resultat som innehåller ordet &quot;förstå&quot;.

## Sök efter flera ord

När du tar med flera ord i en sökning och bara vill söka efter objekt som matchar alla ord i sökrutan, kan du skriva orden i valfri ordning.

Om du till exempel söker efter&quot;Marknadsföringsdemo&quot; (utan citattecken) hittas objekt med följande namn:

* Marknadsföringsdemo
* Demonstrationsmarknadsföring
* Marknadsanalysdemo för januari

Den hittar även objekt som kan ha &quot;Marknadsföring&quot; i namnet och &quot;Demo&quot; i beskrivningen.

Du kan dock göra följande i rutan [!UICONTROL Search] för att justera sökresultaten som visas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Inkludera citattecken</td> 
   <td> <p>Om du anger ord i rätt ordning inom citattecken kan du bara söka efter objekt som är exakt likadana.<br>Om du till exempel söker efter"Marknadsföringsdemo" (med citattecken) hittas objekt med följande namn:</p> 
    <ul> 
     <li> Marknadsföringsdemo</li> 
     <li> Marknadsföringsdemo i januari</li> 
     <li>Marknadsföringsdemoplan</li> 
    </ul> <p>Den här sökningen hittar dock inte något objekt med namnet"Demomarknadsföring".</p> </td> 
  </tr> 
  <tr> 
   <td>Inkludera ELLER</td> 
   <td> <p>Om du kopplar ord med "OR" (utan citattecken) kan du bara söka efter objekt som matchar minst ett av orden i rutan [!UICONTROL Search]. Dessa ord kan anges i valfri ordning.<br>Om du till exempel söker efter"Marknadsföring ELLER demo" (utan citattecken) hittas objekt med följande namn:</p> 
    <ul> 
     <li> Marknadsanalysdemo</li> 
     <li>Marknadsanalysdemo för januari</li> 
     <li>Demo</li> 
     <li>Marknadsanalys</li> 
    </ul> <p>Obs! "OR" måste finnas i versaler. Annars tolkas det som ett annat ord i den fras du söker efter.</p> </td> 
  </tr> 
  <tr> 
   <td>Inkludera OCH</td> 
   <td> <p>Om du kopplar ord med"AND" (utan citattecken) kan du bara söka efter objekt som matchar alla ord i rutan [!UICONTROL Search]. Dessa ord kan anges i valfri ordning.<br>Om du till exempel söker efter"Marknadsföring och demo" (utan citattecken) hittas objekt med följande namn:</p> 
    <ul> 
     <li>Marknadsföringsdemo</li> 
     <li>Demonstrationsmarknadsföring</li> 
     <li>Marknadsanalysdemo för januari</li> 
    </ul> <p>Obs!"AND" måste finnas i versaler. Annars tolkas det som ett annat ord i den fras du söker efter. Om du tar med "&amp;" (utan citattecken) söker du bara efter objekt som innehåller et-tecknet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Använd sökning i [!DNL Workfront]

[!DNL Workfront] innehåller två typer av sökningar: Grundläggande och avancerad. Använd Grundläggande sökning om du vill söka efter nyckelord i vanliga objektfält som namn eller beskrivning. Använd [!UICONTROL Advanced Search] om du vill använda filter för att söka efter andra objektfält.

* [Grundläggande sökning](#basic-search)
* [Avancerad sökning](#advanced-search)

### Grundläggande sökning

Med en grundläggande sökning kan du söka efter nyckelord i alla objekt i systemet eller i endast ett objekt i taget (till exempel projekt). [!DNL Workfront] söker sedan efter nyckelorden i några specifika fält. Du kan sedan förfina sökresultaten baserat på andra objektspecifika fält som markerats av [!DNL Workfront].

En lista över de specifika fält som har genomsökts i Grundläggande sökning finns i [Fält som är tillgängliga för sökning](#fields-available-for-search) i den här artikeln.

>[!NOTE]
>
>Om du vill utföra en [!UICONTROL Advanced Search] måste du markera alternativet [!UICONTROL Advanced Search] när sökningen börjar. Du kan inte förfina en grundläggande sökning till en [!UICONTROL Advanced Search].

* [Utför en grundläggande sökning](#perform-a-basic-search)
* [Förfina en grundläggande sökning](#refine-a-basic-search)

#### Utför en grundläggande sökning

Du kan göra en grundläggande sökning på något av följande sätt:

* För alla objekt i systemet (allmän sökning).
* Endast ett objekt i taget (objektspecifik sökning).

Så här utför du en grundläggande sökning:

1. Klicka på förstoringsglaset ![Sökikonen](assets/search-icon.png) i det övre högra hörnet på sidan. Du kan också skriva **[!UICONTROL ALT + /]** eller **[!UICONTROL Option + /]** för att öppna menyn [!UICONTROL Search].

1. (Valfritt) Om du vill söka efter ett specifikt objekt klickar du på den nedrullningsbara menyn **[!UICONTROL All]** och markerar det objekt som du vill söka efter.

   ![Sök efter objekttyp](assets/search-objecttype.png)

1. I rutan **[!UICONTROL Search]** börjar du skriva den information du söker efter.
Mer information om vilka fält som söks igenom i [!DNL Workfront] finns i [Förstå sökning](#understand-search).
   ![Listrutan Sök](assets/qs-search-drop-down-highlighted-350x234.png)

   När du börjar skriva i sökfältet gör [!DNL Workfront] rekommendationer baserat på din visningshistorik och det nyckelord du söker efter markeras med blått.

1. Om det objekt du söker efter visas på menyn [!UICONTROL typeahead] klickar du på det.

   eller

   Tryck på **[!UICONTROL Enter]** för att utföra en omfattande sökning. Med den här sökningen söks hela databasen igenom i stället för de senast visade objekten.

   Sidan [!UICONTROL Search Results] öppnas från vänster och täcker det mesta av föregående sida.

   Om du utförde en allmän sökning returnerar [!DNL Workfront] resultat för alla objekt som matchar söktermen i något av de sökta fälten, vilket beskrivs i [Förstå sökning](#understand-search). De objekt som matchar sökningen visas i en lista.

   >[!NOTE]
   >
   >Ibland kan varianter av ett ord visas i listan med hittade objekt.\
   >Om du till exempel söker efter&quot;marknadsföring&quot; visas objekt som innehåller antingen&quot;marknadsföring&quot; eller&quot;marknad&quot; i namnet.

1. (Valfritt) Om sökningen genererade för många resultat kan du förfina sökningen enligt beskrivningen i [Förfina en grundläggande sökning](#refine-a-basic-search).
1. (Valfritt) Om du vill gå tillbaka till sidan som du var på innan sökningen klickar du på **[!UICONTROL Close]** i det övre högra hörnet.

>[!NOTE]
>
>Sidan [!UICONTROL Search Results] förblir bara öppen när den är i fokus. Om du klickar utanför sidan eller öppnar en annan sida stängs sidan [!UICONTROL Search Results].

#### Förfina en grundläggande sökning

När du har utfört en grundläggande sökning, enligt beskrivningen i [[!UICONTROL Perform a Basic Search]](#perform-a-basic-search), kan du förfina sökningen.

Använd verktygsfältet till vänster om sökresultaten för att begränsa den information du letar efter.

Så här förfinar du en sökning:

1. (Villkorligt) Om du utförde en allmän sökning markerar du det objekt du sökte efter i objektlistan längst upp till vänster i resultatet.
1. Leta upp fälten som är tillgängliga för de objekt som visas i sökningen i verktygsfältet till vänster om resultatet.
Värdena för varje fält visas, sorterade efter antal, upp till 10 värden för varje fält.
1. Klicka i något av de tillgängliga fälten för att förkorta resultatlistan.
De markeringar du gör markeras med blått och de fältvärden du inte markerar döljs.
När du har valt varje nytt värde uppdateras resultatet till höger dynamiskt.

   ![Fliken Grundläggande sökning](assets/basic-search.png)

1. (Valfritt) Klicka på de markerade värdena för att avmarkera dem och visa alla värden för varje fält igen.

### [!UICONTROL Advanced Search]

Med [!UICONTROL Advanced Search] kan du söka med hjälp av fält och filter som inte är tillgängliga för grundläggande sökning. Du kan till exempel söka efter projekt med en viss prioritet eller dokumentägarnamn.

>[!NOTE]
>
>Om du vill utföra en [!UICONTROL Advanced Search] måste du markera alternativet [!UICONTROL Advanced Search] när sökningen börjar. Du kan inte förfina en grundläggande sökning till en [!UICONTROL Advanced Search].

* [Använd [!UICONTROL Advanced Search]](#use-advanced-search)

#### Använd [!UICONTROL Advanced Search]

Du kan använda [!UICONTROL Advanced Search] för att filtrera din sökning baserat på specifika villkor.\
Den här typen av sökning är användbar när du inte kommer ihåg ett nyckelord som är associerat med ett objekt, men du känner till viss specifik information om det objektet (till exempel Projektprioritet, Dokumentägarnamn).

Så här utför du en avancerad sökning:

1. Klicka på ikonen **[!UICONTROL Search]** ![Sök ](assets/search-icon.png) i det övre högra hörnet på en sida i [!DNL Workfront]. Menyn [!DNL Search] visas.

1. Klicka på **[!UICONTROL Advanced Search]** längst ned på menyn [!UICONTROL Search].\
   ![Avancerad sökning](assets/qs-advanced-search-350x224.png)\
   Sidan [!UICONTROL Advanced Search] öppnas från höger och täcker det mesta av föregående sida.

1. Välj den typ av objekt du söker efter.\
   **[!UICONTROL Tasks]** är markerat som standard.

   ![Avancerade sökobjekt](assets/advanced-search.png)

1. (Valfritt) Skriv ett nyckelord i fältet högst upp i listan.
1. (Valfritt) Aktivera **[!UICONTROL Filter your results]** om du vill skapa ett filter för att begränsa sökningen. Klicka på **Använd** när du är klar.

1. Klicka på **[!UICONTROL Search]**.\
   En lista med objekt som matchar sökningen visas till höger om verktygsfältet [!UICONTROL Advanced Search].

1. (Valfritt) Om du vill gå tillbaka till sidan som du var på innan sökningen klickar du på **[!UICONTROL Close]** i det övre högra hörnet.

>[!NOTE]
>
>Sidan [!UICONTROL Search Results] förblir bara öppen när den är i fokus. Om du klickar utanför sidan eller öppnar en annan sida stängs sidan [!UICONTROL Search Results].

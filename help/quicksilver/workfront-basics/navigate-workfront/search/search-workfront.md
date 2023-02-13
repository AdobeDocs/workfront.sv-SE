---
navigation-topic: search
title: Sök [!DNL Adobe Workfront]
description: Du kan enkelt hitta objekt i [!DNL Adobe Workfront] genom att söka efter dem när du inte kommer ihåg deras exakta plats.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 0%

---

# Sök [!DNL Adobe Workfront]

Du kan enkelt hitta objekt i [!DNL Adobe Workfront] genom att söka efter dem när du inte kommer ihåg deras exakta plats.

Du kan se [!UICONTROL Search] i det övre högra hörnet på en sida i [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

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
   <td> <p>[!UICONTROL View] åtkomst till objekttypen </p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Du måste ha behörighet att visa ett objekt innan du kan hitta det i en sökning.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

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
* Portfolio
* Program
* Kontrollpaneler
* Företag
* Anteckningar

### Fält som är tillgängliga för sökning

De fält som är tillgängliga för sökning baseras på typen av sökning: Grundläggande eller [!UICONTROL Advanced Search].

* **Grundläggande sökning**: När du söker efter objekt i en grundsökning [!DNL Workfront] söker efter text som kan innehålla dina nyckelord i följande fält:

   * Objektnamn
   * Beskrivningar
   * Anpassade datafält
   * Uppdateringar
   * Dokumentnamn (i specifika dokumentsökningar och i en grundläggande sökning)

   Mer information om grundläggande sökning i [!DNL Workfront], se [Grundläggande sökning](#basic-search) i den här artikeln.

* **[!UICONTROL Advanced Search]**: I en [!UICONTROL Advanced Search]kan du ställa in filter för att söka efter fält som inte är tillgängliga i den grundläggande sökningen. Därför [!UICONTROL Advanced Search] gör att du kan söka i alla fält i objektet.

   Mer information om [!UICONTROL Advanced Search], se [Avancerad sökning](#advanced-search) i den här artikeln.

>[!NOTE]
>
>Så här utför du en [!UICONTROL Advanced Search]måste du välja [!UICONTROL Advanced Search] när sökningen börjar. Du kan inte begränsa en grundläggande sökning till en [!UICONTROL Advanced Search].

## Förstå begränsningar för [!DNL Workfront] sökningar

Tänk på följande begränsningar när du använder [!UICONTROL Search] in [!DNL Workfront]:

* Sökningar är inte skiftlägeskänsliga
* [!DNL Workfront] rättar inte eller förstår inte stavfel
* Söker i [!DNL Workfront] stöder inte jokertecken
* Söker i [!DNL Workfront] stöder delvis ordsökning, men inte delsträngssökningar.\
   Söknyckelordet &quot;ställ&quot; returnerar till exempel resultat som innehåller ordet &quot;standard&quot;, men returnerar inte resultat som innehåller ordet &quot;förstå&quot;.

## Sök efter flera ord

När du tar med flera ord i en sökning och bara vill söka efter objekt som matchar alla ord i sökrutan, kan du skriva orden i valfri ordning.

Om du till exempel söker efter&quot;Marknadsföringsdemo&quot; (utan citattecken) hittas objekt med följande namn:

* Marknadsföringsdemo
* Demonstrationsmarknadsföring
* Marknadsanalysdemo för januari

Den hittar även objekt som kan ha &quot;Marknadsföring&quot; i namnet och &quot;Demo&quot; i beskrivningen.

Du kan dock göra följande i [!UICONTROL Search] för att justera sökresultaten som visas:

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
   <td> <p>Om du kopplar ord med "OR" (utan citattecken) kan du bara söka efter objekt som matchar minst ett av orden i [!UICONTROL Search] box. Dessa ord kan anges i valfri ordning.<br>Om du till exempel söker efter"Marknadsföring ELLER demo" (utan citattecken) hittas objekt med följande namn:</p> 
    <ul> 
     <li> Marknadsanalysdemo</li> 
     <li>Marknadsanalysdemo för januari</li> 
     <li>Demo</li> 
     <li>Marknadsanalys</li> 
    </ul> <p>Obs! "OR" måste vara i versaler. I annat fall tolkas det som ett annat ord i den fras du söker efter.</p> </td> 
  </tr> 
  <tr> 
   <td>Inkludera OCH</td> 
   <td> <p>Om du kopplar ord efter "AND" (utan citattecken) kan du bara söka efter objekt som matchar alla ord i [!UICONTROL Search] box. Dessa ord kan anges i valfri ordning.<br>Om du till exempel söker efter"Marknadsföring och demo" (utan citattecken) hittas objekt med följande namn:</p> 
    <ul> 
     <li>Marknadsföringsdemo</li> 
     <li>Demonstrationsmarknadsföring</li> 
     <li>Marknadsanalysdemo för januari</li> 
    </ul> <p>Obs! "AND" måste vara i versaler. I annat fall tolkas det som ett annat ord i den fras du söker efter. Om du tar med "&amp;" (utan citattecken) söker du bara efter objekt som innehåller et-tecknet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Använd Sök i [!DNL Workfront]

[!DNL Workfront] har två typer av sökningar: Grundläggande och avancerad. Använd grundläggande sökning om du vill söka efter nyckelord i vanliga objektfält som namn eller beskrivning. Använd [!UICONTROL Advanced Search] om du vill använda filter för att söka i andra objektfält.

* [Grundläggande sökning](#basic-search)
* [Avancerad sökning](#advanced-search)

### Grundläggande sökning

Med en enkel sökning kan du söka efter nyckelord i alla objekt i systemet eller i endast ett objekt i taget (till exempel projekt). [!DNL Workfront] söker sedan efter nyckelorden i några specifika fält. Du kan sedan förfina sökresultaten baserat på andra objektspecifika fält som markerats av [!DNL Workfront].

En lista med de specifika fält som har genomsökts i grundläggande sökning finns i [Fält som är tillgängliga för sökning](#fields-available-for-search) i den här artikeln.

>[!NOTE]
>
>Så här utför du en [!UICONTROL Advanced Search]måste du välja [!UICONTROL Advanced Search] när sökningen börjar. Du kan inte begränsa en grundläggande sökning till en [!UICONTROL Advanced Search].

* [Utför en grundläggande sökning](#perform-a-basic-search)
* [Förfina en grundläggande sökning](#refine-a-basic-search)

#### Utför en grundläggande sökning

Du kan göra en grundläggande sökning på något av följande sätt:

* För alla objekt i systemet (allmän sökning).
* Endast ett objekt i taget (objektspecifik sökning).

Så här utför du en grundläggande sökning:

1. Klicka på förstoringsglaset ![](assets/search-icon.png) i det övre högra hörnet på sidan. Du kan också skriva **[!UICONTROL ALT + /]** eller **[!UICONTROL Option + /]** för att öppna [!UICONTROL Search] -menyn.

1. (Valfritt) Om du vill söka efter ett visst objekt klickar du på **[!UICONTROL All]** och markera det objekt som du vill söka efter.

   ![](assets/search-objecttype.png)

1. I **[!UICONTROL Search]** börjar du skriva den information du söker efter.\
   För information om vilka fält som söks i [!DNL Workfront], se [Förstå sökning](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   När du börjar skriva i sökfältet [!DNL Workfront] ger rekommendationer baserat på din visningshistorik och markerar det nyckelord du söker efter i blått.

1. Om objektet du söker efter visas i [!UICONTROL typeahead] klickar du på den.

   eller

   Tryck **[!UICONTROL Enter]** för att göra en omfattande sökning. Med den här sökningen söks hela databasen igenom i stället för de senast visade objekten.

   The [!UICONTROL Search Results] sidbilder öppnas från vänster och täcker större delen av föregående sida.

   Om du gjorde en allmän sökning [!DNL Workfront] returnerar resultat för alla objekt som matchar söktermen i något av de sökta fälten, enligt beskrivningen i [Förstå sökning](#understand-search). De objekt som matchar sökningen visas i en lista.

   >[!NOTE]
   >
   >Ibland kan varianter av ett ord visas i listan med hittade objekt.\
   >Om du till exempel söker efter&quot;marknadsföring&quot; visas objekt som innehåller antingen&quot;marknadsföring&quot; eller&quot;marknad&quot; i namnet.

1. (Valfritt) Om sökningen genererade för många resultat kan du förfina sökningen enligt beskrivningen i [Förfina en grundläggande sökning](#refine-a-basic-search).
1. (Valfritt) Om du vill gå tillbaka till sidan som du var på innan sökningen klickar du på **[!UICONTROL Close]** i det övre högra hörnet.

>[!NOTE]
>
>The [!UICONTROL Search Results] sidan är bara öppen när den är i fokus. När du klickar utanför sidan eller öppnar en annan sida stängs [!UICONTROL Search Results] sida.

#### Förfina en grundläggande sökning

Efter en grundsökning enligt beskrivningen i [[!UICONTROL Perform a basic search]](#perform-a-basic-search)- du kan förfina sökningen.

Använd verktygsfältet till vänster om sökresultaten för att begränsa den information du letar efter.

Förfina en sökning:

1. (Villkorligt) Om du utförde en allmän sökning markerar du det objekt du sökte efter i objektlistan längst upp till vänster i resultatet.
1. Leta upp fälten som är tillgängliga för de objekt som visas i sökningen i verktygsfältet till vänster om resultatet.\
   Värdena för varje fält visas, sorterade efter antal, upp till 10 värden för varje fält.
1. Klicka i något av de tillgängliga fälten för att förkorta resultatlistan.\
   De markeringar du gör markeras med blått och de fältvärden du inte markerar döljs.\
   När du har valt varje nytt värde uppdateras resultatet till höger dynamiskt.\
   ![](assets/qs-refine-search-350x175.png)

1. (Valfritt) Klicka på de markerade värdena för att avmarkera dem och visa alla värden för varje fält igen.

### [!UICONTROL Advanced Search]

[!UICONTROL Advanced Search] gör att du kan söka med hjälp av fält och filter som inte är tillgängliga för grundläggande sökning. Du kan till exempel söka efter projekt med en viss prioritet eller dokumentägarnamn.

>[!NOTE]
>
>Så här utför du en [!UICONTROL Advanced Search]måste du välja [!UICONTROL Advanced Search] när sökningen börjar. Du kan inte begränsa en grundläggande sökning till en [!UICONTROL Advanced Search].

* [Använd [!UICONTROL Advanced Search]](#use-advanced-search)

#### Använd [!UICONTROL Advanced Search]

Du kan använda [!UICONTROL Advanced Search] om du vill filtrera sökningen baserat på specifika villkor.\
Den här typen av sökning är användbar när du inte kommer ihåg ett nyckelord som är associerat med ett objekt, men du känner till viss specifik information om det objektet (exempel: Projektprioritet, dokumentägarnamn osv.).

Så här utför du en avancerad sökning:

1. I det övre högra hörnet på en sida i [!DNL Workfront]klickar du på **[!UICONTROL Search]** icon ![](assets/search-icon.png). The [!DNL Search] visas.

1. Längst ned på [!UICONTROL Search] meny, klicka **[!UICONTROL Advanced Search]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   The [!UICONTROL Advanced Search] sidbilder öppnas från höger och täcker större delen av föregående sida.

1. Välj den typ av objekt du söker efter.\
   **[!UICONTROL Projects]** är markerat som standard.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Valfritt) Skriv ett nyckelord i fältet högst upp i listan.
1. (Valfritt) Klicka på **[!UICONTROL Filter your results]** Om du vill filtrera sökresultaten baserat på specifika fälttyper väljer du ett fält i listan. Välj ett värde för fältet om det behövs.\
   eller\
   Lägg till ett nytt filter.

1. Klicka på **[!UICONTROL Search]**.\
   En lista med objekt som matchar sökningen visas till höger om [!UICONTROL Advanced Search] verktygsfält.

1. (Valfritt) Om du vill gå tillbaka till sidan som du var på innan sökningen klickar du på **[!UICONTROL Close]** i det övre högra hörnet.

>[!NOTE]
>
>The [!UICONTROL Search Results] sidan är bara öppen när den är i fokus. När du klickar utanför sidan eller öppnar en annan sida stängs [!UICONTROL Search Results] sida.

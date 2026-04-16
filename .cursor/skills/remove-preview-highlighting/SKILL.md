---
name: remove-preview-highlighting
description: ""
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---


# Ta bort markering av förhandsgranskning (Workfront)

## Omfång

Använd bara när **all** är true:

1. Användaren anropade det här arbetsflödet (t.ex. **&quot;ta bort markering av förhandsgranskning&quot;** eller tydligt samma återgivning).
2. Markdown-filens sökväg innehåller **inte** **`product-announcements`** (utelämna hela mappträdet, t.ex. versionsinformation, betaversioner, meddelanden under `help/quicksilver/product-announcements/`).
3. Markeringsfilen **visas inte** under **[Uteslutna sökvägar](#excluded-paths)** nedan.
4. Markup-filens främsta komponent är **`Courtney`** på raden `author:` (den enda författaren eller medförfattaren).
5. Artikeln har **minst en** av:
   - Förhandsgranskningsmiljö **språk i textutkast eller i riktiga textutdrag** (typiska mönster: &quot;markerad information&quot;, &quot;förhandsvisningsmiljö&quot;, &quot;ännu inte tillgänglig&quot;, snabbversionsinformation)—**inte** en matchning från **enbart länktext** på en innehållsförteckning/indexsida (se nedan); eller
   - Alla HTML-element med **`class="preview"`** (t.ex. `<span class="preview">`, `<div class="preview">`) eller
   - Ett förhandsvisningsfragment **variabel**, till exempel **`{{highlighted-preview}}`** eller **`{{highlighted-preview-article-level}}`**.

Om omfånget är oklart bekräftar du det innan du redigerar.

**Innehållsförteckning/indexsidor - hoppa alltid över det här fallet:** **Aldrig** placera en fil i inventeringen när den **endast** förhandsvisningsrelaterade ordalydelsen är **inuti** en markeringslänks visningstext som pekar på **en annan** artikel (t.ex. *Skicka en rapport i förhandsgranskningssandlådemiljön*) **)** 2&rbrace;och **filen innehåller** no`class="preview"` **,** no **kodfragmentvariabler och** no **förhandsvisningsmallarna i** prose utanför länkarna. Det här är inte en markering av förhandsvisningen på den sidan, utan bara ett omnämnande av innehållsförteckningen. Gäller alla index/innehållsförteckningar, inte bara en fil.

### Exkluderade banor

Lägg aldrig till dessa i lagret eller redigera dem i det här arbetsflödet såvida inte användaren uttryckligen åsidosätter:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md` - parallell förhandsgranskning jämfört med produktionsbegränsningar kräver ett avsiktligt redaktionellt beslut utanför automatisering.
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md` - Rapporterar innehållsförteckning. Den enda förhandsgranskningssignalen är länken till leveransartikeln i sandlådan för förhandsgranskning.

## Nödvändigt arbetsflöde (människa i slingan)

Redigera **inte** gruppvis svaret utan godkännande.

1. **Lager**\
   Skapa en sorterad lista med sökvägar som uppfyller omfångsreglerna ovan (sök i svaret; använd `help/` träd). **Utelämna** alla sökvägar under **`product-announcements`**, alla sökvägar under **[Uteslutna sökvägar](#excluded-paths)** och alla **TOC-/indexsidor** som matchar **TOC-/indexsidor** under Omfång. Om användaren säger att en listad fil inte har någon markering för förhandsgranskning tar du bort den från körningen och justerar villkoren i stället för att framtvinga redigeringar.

2. **Start**\
   Fråga om du vill börja med den **första** artikeln i listan (eller en sökväg till användarnamnen).

3. **Per artikel - visa först, redigera efter OK**
   - Läs filen.
   - Föreslå redigeringar tydligt: **före/efter utdrag** eller en fokuserad beskrivning av vad som ska ändras.
   - **Vänta** på explicit godkännande (t.ex. &quot;OK&quot;, &quot;apply&quot;, &quot;yes&quot;) innan du skriver filen.

4. **Efter varje fil**\
   Fråga om du vill gå till artikeln **nästa** (eller stoppa/hoppa över).

## Innehållsregler (GA: Förhandsgranska innehåll blir dokumentet)

När du tar bort markering av förhandsgranskning för **allmän tillgänglighet** är målet: **Behåll beteendet som dokumenterades för förhandsgranskning**, släpp **föråldrade grenar av typen&quot;i produktion&quot;/gammal process** och **ta bort etiketter och wrappers som endast är för förhandsgranskning** så att avsnittet läses som aktuellt för alla kunder.

### Parallella steg

- Om artikeln har ett steg (eller ett numrerat objekt) **inramat som&quot;i produktion&quot;** (eller motsvarande: aktuell produktion/befintlig produktionsfunktion) **och** ett **parallellt** steg inramat som **&quot;i förhandsgranskning&quot;** (eller i förhandsvisningsmiljön):
   - **Ta bort** steget i produktionen (den gamla sökvägen).
   - **Behåll** förhandsgranskningens **substans**, men **omord** så att den **inte** är förhandsvisningsspecifik (ta bort &quot;i förhandsgranskning&quot;, &quot;Förhandsvisningsmiljö&quot; osv.). Justera numreringen så att listan förblir konsekvent.

Om strukturen är tvetydig (ingen klar parallell struktur) **stop** och visar båda kandidaterna. Fråga användaren vilket block som ska behållas.

### Parallella avsnitt

- Om ett **avsnitt** (rubrik + brödtext) är **om &quot;i produktionsmiljön&quot;** och det finns ett **parallellt avsnitt** **om &quot;i förhandsgranskningsmiljön&quot;**:
   - **Ta bort** avsnittet för produktionsmiljö (det ersatta innehållet).
   - **Ersätt** med förhandsvisningsavsnittets innehåll och **ta sedan bort** förhandsvisningsmiljöns ordalydelse och eventuella **`class="preview"`**-omslag så att avsnittet är neutralt (GA-klart).

### Kodavsnitt och meddelanden om artikeltoppar

- Ta bort block av typen **med enbart förhandsgranskning** (omfång/divar eller stycken som bara förklarar att markerat innehåll är enbart förhandsgranskning, snabb release, sandlåda osv.) när funktionen är GA.
- Ta bort länkar eller meningar vars **endast**-syfte är förhandsvisningstillgänglighet, såvida inte användaren säger att ett annat meddelande ska visas.

### HTML `class="preview"`

- Ta bort de **inledande och avslutande taggarna** för element som använder **`class="preview"`**, **behåller det inre innehållet** (markdown/HTML inuti taggen).
- Hantera både **`<span class="preview">`** och **`<div class="preview">`**, och samma mönster för andra taggar (t.ex. **`<p class="preview">`**, **`<li class="preview">`**) när de visas i brödtextinnehållet **visible** (ej kommenterat).
- Bevara list-/tabellstruktur; korrigera brutna listor eller tomt utrymme efter uppackning.

### Utkommenterade avsnitt (HTML kommentarer)

- **Ta inte** bort, dela upp eller på annat sätt **ändra** innehåll i **`<!-- … -->`** HTML-kommentarer **om inte användaren uttryckligen anger** vad som ska göras (t.ex. ta bort hela kommentaren, ta bort förhandsgranskningsklasser inuti enbart kommentaren, ta bort kommentar för GA).
- Om förhandsgranskningsrelaterat innehåll eller **`class="preview"`** visas **endast** inuti kommentarer, **anropar du den** när du granskar artikeln: säg vad som finns i kommentaren och **frågar** vad du ska göra. **Standard: låt de kommenterade avsnitten vara oförändrade.**

### Vad du inte ska göra

- Kör inte det här arbetsflödet på sökvägar under **`product-announcements`** (versionsinformation och relaterade). Lagret måste exkludera dem.
- Inventera eller redigera inte sökvägar som listas under **[Exkluderade sökvägar](#excluded-paths)** såvida inte användaren uttryckligen ber att inkludera en sådan.
- **Ta inte** bort eller redigera **kommenterade-utkommenterade** (`<!-- … -->`) block automatiskt. Följ **Utkommenterade avsnitt** ovan.
- Ta inte bort Förhandsgranska när det **inte** handlar om det här mönstret för funktionstillgänglighet (t.ex. [Förhandsgranska sandlådemiljö] (·) som ett **produktnamn** i ett orelaterat sammanhang). Använd ett omdöme och fråga om det är osäkert.
- Ändra inte `author:` eller icke-relaterade fronter såvida inte användaren frågar.
- Hoppa inte över steget **visa → godkänn**.

## Kvalitetskontroller innan redigeringar presenteras

- Det finns inga återstående **`class="preview"`** i det avtalade ändringsintervallet.
- Inga överblivna dubblettrubriker eller brutna stegnummer.
- Introduktionen läses **korrekt utan** motsägande GA (ingen&quot;endast i förhandsvisning&quot; för levererade funktioner).

## Referenser

- Matcha **[dokumentationsformat för Workfront](https://experienceleague.adobe.com/?lang=sv#home)** och repo-konventioner (implementerings-/PR-regler om användaren implementerar).

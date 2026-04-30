---
name: release-notes-formatter
description: Formatera och validera Workfront versionsinformation för enhetlighet, korrekt struktur och korrekt länkning. Använd endast för versionsfakturafiler i produktreleasekataloger eller när användaren anger versionsinformation, produktreleaser eller kvartalsvisa releaser. Använd inte artiklar som visar hur man gör eller allmän dokumentation.
source-git-commit: 1a498abcf4a9ef8940eb2da09da42636253e557a
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---


# Utgivningsanteckningsformat

Formaterar och validerar versionsinformation för Adobe Workfront i katalogen `help/quicksilver/product-announcements/product-releases/`.

## Sidtyper

Identifiera sidtypen från filens sökväg och innehåll:

| Sidtyp | Filmönster | Mall |
|-----------|-------------|----------|
| **Översikt** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **Del av programmet** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **Planerar** | `planning-release-activity-{YY}-q{N}.md` | Liknar produktområdet |
| **Utseende och känsla** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#look-and-feel](reference.md#look-and-feel-page-template) |

## Formateringsarbetsflöde

### Steg 1: Validera innehåll

Obligatoriska fält för alla versionsfakturasidor:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Regler:
- `feature` måste vara exakt `Product Announcements`
- `recommendations` måste vara exakt `noDisplay, noCatalog`
- Uppfinna aldrig en `exl-id` - inkludera bara om det redan finns en
- Lägg inte till `draft: Probably` på riktiga sidor (endast mallar)

### Steg 2: Validera struktur efter sidtyp

#### Produktområdessidor

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Exempel: `# Second Quarter 2026 Administrator enhancements`
   - Kvartal måste skrivas ut: &quot;Första kvartalet&quot;, &quot;andra kvartalet&quot;, &quot;tredje kvartalet&quot;, &quot;fjärde kvartalet&quot;

2. **Intro paragraph**: Beskriver området och länkar till översikten
   - Måste länka till översiktsfilen **för det** korrekta kvartalet
   - Vanligt fel: länka till föregående kvartal (t.ex. `26-q1` i stället för `26-q2`)

3. **H2 per funktion**: Funktionstitel som rubrik
   - **De senaste funktionerna först** - den senaste versionsinformationen måste visas som den första H2 efter det inledande stycket
   - Äldre funktioner följer i omvänd kronologisk ordning

4. **Bildtextblock för datum** efter varje H2:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **Brödtext**: Funktionsbeskrivning och länka sedan till hjälpdokumentationen

#### Översikt över sidor

1. **H1**: `{Written Quarter} release overview`

2. **Intro paragraph** med schemalagd frisläppningsmånad

3. **`>[!IMPORTANT]`block** med versionsschematabell

4. **H2`Adobe Workfront enhancements`** med punktlista över ankarlänkar:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. **H3 per produktområde** med HTML-funktionstabell (se [reference.md](reference.md#overview-feature-table))
   - I varje tabell visas **de senaste funktionerna först** - den senaste raden visas högst upp i tabellen (efter rubrikraden)

&#x200B;6. **Avslutande avsnitt** (H2): Versionsinformation om andra områden, uppdateringar för Desktop Proofing Viewer, meddelanden, API-version, underhållsuppdateringar, utbildningsuppdateringar

### Steg 3: Validera länkar

- **Översiktslänk på produktområdessidor**: Måste peka på samma kvartal
   - Korrekt: `26-q2-release-activity/26-q2-release-overview.md`
   - Fel: `26-q1-release-activity/26-q1-release-overview.md`
- **Ankarlänkar i översikt**: Måste matcha H3-ID:n (gemener, bindestreck)
- **Funktionslänkar i översiktstabeller**: Måste använda `class="MCXref xref" xrefformat="{para}"`
- **Länkar till hjälpdokument**: Måste börja med `/help/quicksilver/`

### Steg 4: Validera datum

- Format: `{Month} {Day}, {Year}` (t.ex. &quot;12 mars 2026&quot;)
- Använd `TBD` för okända datum
- Datum på produktområdessidan `>[!NOTE]` måste matcha motsvarande översiktstabellrad
- Förhandsgranskningsdatum bör ligga före produktionsdatum

### Steg 5: Vanliga korrigeringar

Använd följande korrigeringar vid formatering:

| Problem | Korrigera |
|-------|-----|
| Fel översiktslänkkvartal | Uppdatera för att matcha filens eget kvartal |
| `>[!NOTE]`-datumblock saknas | Lägg till block efter H2-funktionens rubrik |
| Inkonsekvent datumformat | Standardisera till `Month Day, Year` |
| En tom rad saknas före `>[!NOTE]` | Lägg till tom rad |
| Extra blanksteg i bildtextrader | Trimma avslutande blanksteg |
| HTML på produktområdessidor | Behåll som markering (HTML är endast för översiktstabeller) |
| `exl-id` saknas | Låt det vara - generera ingen |

### Steg 6: Uppdatera innehållsförteckningen

När du skapar en **ny** versionsanteckningssida (översikt eller produktområde) lägger du till den i `help/quicksilver/TOC.md` i samma ändring. En sida som inte finns i innehållsförteckningen visas inte i den publicerade navigeringen, även om länkar i översiktstabellen pekar på den.

Var ska den läggas till:

- Innehållsförteckningen har ett avsnitt per kvartal under en rubrik som `* 2026 Q3 Release {#release-26-q3}`. Om kvartalsrubriken inte finns än (första sidan i ett nytt kvartal) lägger du till den ovanför föregående kvartal så att det senaste kvartalet ligger överst.
- Under den kvartalsrubriken anger du sidorna i den här ordningen:
   1. **Översikt** först (`Third Quarter 2026 release overview`).
   2. **Product-area-sidor** i bokstavsordning efter områdesnamn (Administratör, Dokument, Företagsåtgärder, Projekt, Rapportering, Begär).
   3. **Andra förbättringar** är sista (alltid efter de alfabetiska produktområdena).

Varje post i innehållsförteckningen är en markeringslänk med hjälp av sidrubriken och den absoluta rapportsökvägen:

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Matcha indrag (sex blanksteg) med de omgivande posterna. Använd sidans H1-ordlista som länktext - till exempel `Documents enhancements`, `Requesting enhancements` (inte `Requests`) - så att innehållsförteckningsetiketterna matchar föregående kvartal.

Vanliga misstag att undvika:

- Skapa en produktområdessida utan att lägga till den i innehållsförteckningen.
- Länkar till en översikt för ett annat kvartal från den nya produktsidan (steg 3).
- Infoga ett nytt kvarts sidor under föregående kvarts rubrik.

## Namngivningskonventioner

| Typ | Mönster | Exempel |
|------|---------|---------|
| Ökning | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Produktområde | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Katalog | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Instruktioner för standardområde: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Kvartsmappning

| Kvartal | Skrivna formulär | Månader |
|---------|-------------|--------|
| Q1 | Första kvartalet | Jan-Mar |
| Q2 | Andra kvartalet | Apr-Jun |
| Q3 | Tredje kvartalet | Jul-sep |
| Q4 | Fjärde kvartalet | okt-dec |

Den kvartalsvisa produktionsreleasen landar vanligtvis på torsdagen den andra hela veckan i den sista månaden i kvartalet.

## Checklista för validering

Kontrollera följande när du granskar en versionsinformation:

- [ ] Frontmatter har alla obligatoriska fält med korrekta värden
- [ ] H1 matchar sidtypsformatet
- [ ] Översikt länkar till rätt kvartal
- [ ] Varje funktion har ett `>[!NOTE]` datumblock (produktområdessidor)
- [ ] Datumformatet är konsekvent (`Month Day, Year`)
- [ ] Funktionstabellrader i översikt matchar innehållet på produktområdessidan
- [ ] inga brutna interna länkar
- [ ] ankarlänkar i översikt matchar H3-avsnitts-ID
- [ ] Funktioner ordnas för det senaste först (både produktområdessidor och översiktstabeller)
- [ ] Nya versionsanteckningssidor visas i `help/quicksilver/TOC.md` under rätt kvartal, med översikten först och produktområden i alfabetisk ordning (övrigt senast)

## Ytterligare resurser

- Fullständiga HTML-mallar och exempel finns i [reference.md](reference.md)

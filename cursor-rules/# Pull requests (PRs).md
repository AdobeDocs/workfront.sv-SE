---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Dragningsbegäranden (PR)

Följ de här konventionerna när du skapar eller granskar en titel eller beskrivning för en pull-begäran (t.ex. i GitHub/GitLab eller när du tillfrågas i Agent chat).

## Deriving the Jira issue

- **Source av sanningen:** Hämta Jira-utgivar-ID från det **aktuella Git-grennamnet** (till exempel ett segment som matchar ditt projektnyckelmönster, till exempel `FFENT-8796`).
- **Om filialnamnet innehåller ett Jira-ID:** Använd det ID:t i PR-titeln (se nedan) och länka det i `# Context` → `## Jira`.
- **Om filialnamnet inte innehåller något Jira-ID:** Behandla PR som inte associerat med en biljett. **Utelämna** Jira-nyckeln från PR-titeln (uppfinna inte en biljett). Inkludera fortfarande `# Context` → `## Jira`, med innehållet exakt: `No ticket` (ingen länk).

## PR-titel

**När filialnamnet innehåller ett Jira-problem-ID** inkluderar du **båda**:

1. **Jira-utgåva-ID** (t.ex. `FFENT-8001`).
2. **implementeringstypen** (se listan nedan), med det här mönstret:

`{type}/{JIRA-ID}- {short task description}`

Exempel:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Använd en kortfattad beskrivning av tvingande stil efter ID:t. Matcha det visade avståndsmönstret: type, slash, Jira key with trailing hyphen, space, then the description.

**När filialnamnet inte innehåller ett Jira-problem-ID** utelämnar du biljetten från titeln och använder:

`{type}- {short task description}`

Exempel:

`docs- Refresh Object Composite API changelog`

### Godtagbara implementeringstyper (använd exakt dessa etiketter före `/`)

- **feat** - lägger till en ny funktion. När ett nytt innehållsförteckningsobjekt läggs till eller JIRA ansluts till ett annat `feat`-märkt Jira.
- **fix** - korrigerar ett fel
- **refactor** - skriver om/omstrukturerar kod utan att ändra beteende
- **perf** - förbättrar prestanda (särskild refaktor)
- **style** - endast formatering/blanksteg; ingen meningsändring. Endast redigeringar
- **test** - lägger till eller korrigerar tester
- **docs** - Nytt innehåll har lagts till. endast dokumentation
- **build** - byggverktyg, CI, beroenden, projektversion osv.
- **ops** - infrastruktur, distribution, säkerhetskopiering, återställning osv.
- **kedja** - övrig (t.ex. `.gitignore`)

## PR-organ - obligatoriska avsnitt

Använd **exakt dessa toppnivåavsnitt** (markeringsrubriker):

### 1. `# Summary`

Kort översikt över **vad** har ändrats och **varför** (affärs- eller teknikåtergivning).

### 2. `# Changes`

Ordna efter **fil**. Använd en nivå 2-rubrik för varje berörd fil med banan i backticks och sedan punkter som beskriver redigeringarna.

Format:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Inkludera alltid ett **Jira**-underavsnitt under `# Context`.

**När filialnamnet innehåller ett Jira-ID:** Använd en klickbar länk till problemet (härleda nyckeln från filialnamnet).

Format:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Ersätt nyckeln och URL:en med den faktiska biljetten. Om det finns flera biljetter, ange var och en på sin egen rad i samma underavsnitt.

**När filialnamnet inte innehåller något Jira-ID:** Behåll `## Jira` och använd exakt:

```markdown
# Context

## Jira
No ticket
```

## Exempel (fullständig PR-beskrivning)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Exempel (fullständig PR-beskrivning, förgrening utan Jira-ID)

**Titel:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```

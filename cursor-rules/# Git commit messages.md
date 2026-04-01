---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---
# Git-implementeringsmeddelanden

Använd alltid den här regeln. Följ det här formatet när du skapar ett utkast eller genererar ett implementeringsmeddelande för Git (till exempel i rutan Bekräfta för Source Control eller när du tillfrågas i Agentchatt).

## Subject line (first line only)

- Cirka **50 tecken eller färre**.
- Sammanfatta ändringen i **tvingande stämning** (t.ex. &quot;Lägg till..&quot;, &quot;Korrigera..&quot;, &quot;Reaktor..&quot;).

## Tom rad

Lämna en **tom rad** efter ämnet före brödtexten.

## Brödtext (detaljerad beskrivning)

- Radbryt vid cirka **72 tecken** (inklusive punktprefix och mellanslag).
- Använd **punktlinjer** för förklaringen. Varje punkt måste börja med exakt ett av följande:
   - **📖** - använd när ändringen **lägger till** något nytt: nya filer, nya avsnitt, nya funktioner, nya rubriker, nya rader eller annat grönfältsinnehåll.
   - **✏️** - använd när ändringen **ändrar** befintligt arbete: redigerar befintliga rader, uppdaterar befintliga avsnitt, omberäknar befintlig kod eller ändrar aktuellt innehåll.

Använd **📖** eller **✏️** för alla punkter så att det är tydligt vad som introducerades jämfört med vad som ändrades.

## Mall

Fyll i platshållarna (lämna inte vinkelparenteser i det slutliga meddelandet):

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Exempel

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

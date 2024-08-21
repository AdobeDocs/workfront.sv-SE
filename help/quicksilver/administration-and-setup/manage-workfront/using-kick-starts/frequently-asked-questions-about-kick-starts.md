---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,sparkstart,kickstarter,sparkstarter
navigation-topic: use-kick-starts
title: Vanliga frågor om snabbstart
description: Hitta svar på vanliga frågor om import och export av Workfront-data med Quick-Starts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Frågor och svar om snabbstart

Nedan följer vanliga frågor och svar om hur du kommer igång:

## Varför får jag det här felet när jag försöker importera en snabbstartsfil:&quot;Filen var korrekt, men inget importerades?&quot;

### Svar

En av följande tre saker kan saknas i filen Kickstart:

1. Kolumnen **isNew** måste anges till **TRUE** för alla objekt som du vill importera. **isNew** måste vara **TRUE** eftersom du bara kan importera nya data med Spark-Start. Du kan inte ändra befintliga data via Snabbstart. Du kan ha andra rader i kalkylbladet med **isNew = FALSE**, men dessa rader importeras inte.

1. &#x200B; Filen måste ha en tom rad innan datarubrikerna börjar.
1. &#x200B; Excel-bladen måste ha rätt namn.

När du arbetar med Spark-Starts rekommenderar vi att du först hämtar snabbstartmallen, fyller i den manuellt med rätt data och sedan importerar tillbaka den till Adobe Workfront.

Mer information om hur du importerar data korrekt i Workfront med Quick-Starts finns i [Importera data till Adobe Workfront med en Quick-Start-mall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Varför får jag det här felet när jag försöker importera timmar till Workfront med hjälp av en snabbstartsfil: &quot;Användare med primärnyckelvärden &quot;null&quot; hittades inte?&quot;

### Svar

Felet refererar till GUID för användaren som är associerad med timmarna.

För att åtgärda detta:

1. Exportera en tom snabbstartmall endast för objektet **Timmar**.\
   Mer information om hur du exporterar en tom snabbstartfil finns i&quot;Exportera snabbstartmallen&quot; i [Importera data till Adobe Workfront med en snabbstartmall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Kopiera data manuellt från den ursprungliga snabbstarten och klistra in dem i den tomma filen.\
   Gör detta för varje kolumn.
1. Försök importera den nya filen igen.\
   Quick-Start bör importeras korrekt.

## Varför fylls inte landfältet i i användarprofilen i en snabbstartimport?

### Problem

När du importerar en nyckelstart för användare med fältet **setCountry**, kommer dessa data inte till landet i användarprofilen.

### Svar

Om användaren har aktiverats för Unified User Management (UUM) eller Adobe Identity Management System (IMS), godtar fältet **Country** bara landskodsvärden (till exempel USA, GB, IN). Kontrollera att fältet **setCountry** i din snabbstartmall använder landskodsvärden innan du importerar.

Mer information om hur du importerar data korrekt i Workfront med Quick-Starts finns i [Importera data till Adobe Workfront med en Quick-Start-mall](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

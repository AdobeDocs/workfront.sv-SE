---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Flytta objekt från en miljö till en annan i Workfront
description: Funktionen för miljömarknadsföring är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Det stöder inte möjligheten att flytta transaktionsobjekt (med begränsade undantag).
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 4c5a9705cf90498b08b45d85e0b4f571dc2e30f2
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# Översikt över rörliga objekt mellan Workfront-miljöer (miljöfrämjande)

Med funktionen för miljöfrämjande åtgärder kan du flytta objekt från en Workfront-miljö till en annan. Du kan t.ex. skapa en mall och konfigurera den i sandlådemiljön, i vetskap om att alla tester du gör inte kommer att påverka organisationens faktiska data. När mallen har konfigurerats och testats kan du flytta den till produktionsmiljön, klar att använda.

Denna process kallas för&quot;miljöfrämjande&quot;.

Du kan utföra den här processen i Workfront genom att skapa ett paket med objekt som ska flyttas och sedan installera paketet i den nya miljön.

* Specifika anvisningar om hur du utför den här processen i Workfront finns i:

   * [Skapa eller redigera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Instruktioner om hur du utför den här processen via Workfront API finns i [Flytta objekt mellan [!DNL Workfront] miljöer som använder [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3429735/){target=_blank}

## Objekt som stöds för miljöbefordran

Funktionen för miljöfrämjande åtgärder är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Detta är objekt som kan konfigureras, till exempel projekt, team eller anpassade formulär.

Eftersom miljöbefordran hanterar objektkonfiguration inkluderas inte transaktionsobjekt (objekt som ändras ofta eller som är mycket beroende av användningsfall). Exempel på transaktionsobjekt är dokument, utgåvor, förfrågningar, uppdateringar och korrekturbeslut.

* [Arbetsobjekt](#work-objects)
* [Rapporteringsobjekt](#reporting-objects)
* [Anpassade dataobjekt](#custom-data-objects)
* [Organisationsobjekt](#organization-objects)
* [Andra konfigurationsobjekt](#other-configuration-objects)


### Arbetsobjekt

| Upphöjt objekt | Inkluderade länkade objekt som kan höjas |
| --- | --- |
| Projekt (PROJ) | Projekt<br>Uppgift<br>Tilldelning<br>Föregående<br>Företag<br>Åsidosätt hastighet<br>Grupp<br>Roll<br>Team<br>Godkännandeprocess<br>Godkännandesökväg<br>Godkännandesteg<br>Steggodkännare<br>Schema<br>Ledig arbetsdag<br>Ködefinition<br>Köämnesgrupp<br>Köämne<br>Cirkulationsregel<br>Sökväg för milstolpe<br>Milstolpe<br>Timtyp<br>Resurspool<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |
| Mall (TMPL) | Mall<br>Malluppgift<br>Mallaktivitetstilldelning<br>Föregångare för mallaktivitet<br>Företag<br>Åsidosätt hastighet<br>Grupp<br>Roll<br>Team<br>Godkännandeprocess<br>Godkännandesökväg<br>Godkännandesteg<br>Steggodkännare<br>Schema<br>Ledig arbetsdag<br>Ködefinition<br>Köämnesgrupp<br>Köämne<br>Cirkulationsregel<br>Sökväg för milstolpe<br>Milstolpe<br>Timtyp<br>Resurspool<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |

### Rapporteringsobjekt

| Upphöjt objekt | Inkluderade länkade objekt som kan höjas |
| --- | --- |
| Layoutmall (UITMPL) | Layoutmall<br>Kontrollpanel<br>Kalender<br>Kalenderavsnitt<br>Extern sida<br>Rapport<br>Filter<br>Gruppering<br>Visa<br>Parameter |
| Kontrollpanel (PTLTAB) | Kontrollpanel<br>Kalender<br>Kalenderavsnitt<br>Extern sida<br>Rapport<br>Filter<br>Gruppering<br>Visa<br>Parameter |
| Kalender (KALEND) | Kalender<br>Kalenderavsnitt |
| Extern sida (EXTSEC) | Extern sida |
| Rapport (PTLSEC) | Rapport<br>Filter<br>Gruppering<br>Visa<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Gruppering (UIGB) | Gruppering<br>Parameter |
| Visa (UIVW) | Visa<br>Parameter |

### Anpassade dataobjekt

| Upphöjt objekt | Inkluderade länkade objekt som kan höjas |
| --- | --- |
| Kategori (CTGY) | Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik<br>Grupp |
| Parameter (PARAM) | Parameter<br>Parameteralternativ |
| Parametergrupp (PGRP) | Parametergrupp |

### Organisationsobjekt

| Upphöjt objekt | Inkluderade länkade objekt som kan höjas |
| --- | --- |
| Grupp (GRUPP) | Grupp <br>Undergrupper (upp till 5 nivåer) *<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |
| Roll (ROLE) | Roll |
| Team (TEAM) | Team<br>Grupp |
| Företag (CMPY) | Företag<br>Åsidosätt hastighet<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameter <br>Kategorivisningslogik<br>Grupp |
| Portfolio (PORT) | Portfolio<br>Program<br>Grupp<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |
| Program (PRGM) | Program<br>Portfolio<br>Grupp<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |

### Andra konfigurationsobjekt

| Upphöjt objekt | Inkluderade länkade objekt som kan höjas |
| --- | --- |
| Godkännandeprocess (ARVPRC) | Godkännandeprocess<br>Godkännandesökväg<br>Godkännandesteg<br>Steggodkännare<br>Roll<br>Team<br>Grupp |
| Schema (SCHED) | Schema<br>Ledig arbetsdag<br>Grupp |
| Sökväg för milstolpe (MPATH) | Sökväg för milstolpe<br>Milstolpe |
| Tidrapportprofil (TSPRO) | Tidrapportprofil<br>Timtyp |
| Timtyp (HOURT) | Timtyp |
| Utgiftstyp (EXPTYP) | Utgiftstyp |
| Risktyp (risktyp) | Risktyp |
| Resurspool (RSPL) | Resurspool |

\* Inte tillgängligt för tillfället

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## Status för miljöbefordran

Paket för miljöbefordran går igenom flera statusar när de skapas och är förberedda för att växla mellan miljöer. Du kan se dessa statusvärden i din paketlista i Workfront, eller i API-svaren om du använder Workfront API.

Dessa statusvärden är följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>OMONTERAD</td> 
   <td><p>Den här statusen tilldelas automatiskt och representerar ett paket som har sparats men ännu inte monterats. </p><p>Den här statusen kan inte anges direkt av en användare.</p></td> 
  </tr> 
  <tr> 
   <td>SAMMANSÄTTNING</td> 
   <td><p>Den här statusen tilldelas automatiskt medan objekt monteras. </p><p>Sammanfogning avser den automatiska processen att identifiera objekt och underobjekt som ska ingå i ett paket och lägga till dessa objekt och deras data i paketet.</p><p>Den här statusen kan inte anges direkt av en användare.</p></td> 
  </tr> 
  <tr> 
   <td>UTKAST</td> 
   <td><p>Den här statusen tilldelas när en sammansättningsprocess avslutas eller när ett tomt kampanjpaket skapas.</p><p>Användaren kan flytta erbjudandepaketet tillbaka till den här statusen.</p><p>I den här statusen kan erbjudandepaketet inte installeras i någon miljö.</p></td> 
  </tr> 
  <tr> 
   <td>TESTNING</td> 
   <td><p>Den här statusen tillåter att ett kampanjpaket installeras i alla sandlådor av typerna Förhandsgranska eller Anpassad uppdatering. I den här statusen kan paketet inte installeras i Production.</p></td> 
  </tr> 
  <tr> 
   <td>AKTIV</td> 
   <td><p>Denna status tillåter att ett kampanjpaket installeras i alla miljöer, inklusive Production.</p><p>När en paketstatus är inställd på AKTIV <code>publishedAt</code> datumet anges automatiskt till den aktuella tidsstämpeln för begäran.</p></td> 
  </tr> 
  <tr> 
   <td>INAKTIVERAT</td> 
   <td><p>Den här statusen används för att dölja tidigare använda erbjudandepaket som inte kommer att installeras i någon miljö i framtiden.</p><p>När ett paket har den här statusen kan det inte installeras i någon miljö.</p><p>När paketstatusen är INAKTIVERAD visas <code>retiredAt</code> datumet anges automatiskt till den aktuella tidsstämpeln för begäran.</p><p>Vi rekommenderar att du använder den här statusen framför <code>DELETE /package</code> slutpunkten eftersom den kan hämtas och installationshistoriken sparas för alla distributioner som görs med det här paketet.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Kampanjpaketet får automatiskt denna status om ASSEMBLING-fasen misslyckas.</p><p>Om du vill returnera paketet till ASSEMBLING-scenen måste du starta monteringsprocessen igen.</p><p>Mer information om hur du sammanställer ett paket finns i avsnittet <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">Redigera eller sätta ihop ett befintligt paket</a> i artikeln Skapa eller redigera ett paket med miljökampanjer.</td> 
  </tr> 
  </tbody> 
</table>


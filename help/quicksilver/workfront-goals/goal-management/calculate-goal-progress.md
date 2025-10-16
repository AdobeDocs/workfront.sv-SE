---
product-previous: workfront-goals
navigation-topic: goal-management
title: Översikt över målstatus och villkor i Adobe Workfront-mål
description: Målutvecklingen styrs av förloppsindikatorer som aktiviteter, resultat eller barnmål. Målvillkoret avgörs av målets förlopp vid den aktuella tidpunkten.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Översikt över målets förlopp och villkor i Adobe Workfront-mål

<!--Audited for P&P only: 4/2025-->

>[!NOTE]
>
>Ditt företag kan välja att fortsätta använda Adobe Workfront-mål om de tidigare har köpt det här paketet. Du måste prata med din kontorepresentant för mer information.
>
>Adobe Workfront-mål går inte längre att köpa.
>
>Mer information om åtkomst till Workfront-mål finns i [Krav för att använda Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--Old:
>[!IMPORTANT]
>
>Your organization must have the following to use the functionality described in this article:
>
>
>* For the new plan and license structure:
>
>   * An Ultimate plan 
>    
>* For the current plan and license structure: 
>
>   * A Pro or higher 
>   * An Adobe Workfront Goals license in addition to a Workfront license.
>
> Contact your Workfront account manager to learn about a Workfront Goals license.-->


Adobe Workfront beräknar automatiskt målutvecklingen baserat på förloppet för sina förloppsindikatorer.

## Översikt över målets förlopp och tröskelvärde

När du har aktiverat ett mål börjar Workfront Target beräkna dess förlopp och villkor och visar följande indikatorer när du hovrar över förloppsfältet:

| Indikator | Indikatorbeskrivning |
|---|---|
| Faktisk procent slutförd | Hur mycket av målet som faktiskt har uppnåtts hittills. Workfront Target beräknar det här värdet genom att beräkna det genomsnittliga antalet procent slutförda av alla förloppsindikatorer som är associerade med målet. |
| Förväntad procent slutfört | Hur mycket av målet som ska vara slutfört i tid ska vara slutfört. Workfront Target beräknar detta värde genom att titta på målets varaktighet och den aktuella tidpunkten. Målet ska visa det här värdet vid den aktuella tidpunkten om det skulle slutföras i tid. |
| Förlopp | En etikett som anger om målet är på väg att slutföras i tid eller om det är i fara eller om det är i problem att inte slutföras. |

![I problem](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Faktisk procent slutförd](#actual-percent-complete)
* [Förväntad procent slutförd](#expected-percent-complete)
* [Förlopp och villkor](#progress)

### Faktisk procent slutförd {#actual-percent-complete}

Workfront Goals beräknar automatiskt hur stor procentandel av ett mål som faktiskt har slutförts baserat på det genomsnittliga antalet målförloppsindikatorer som har uppnåtts.

Följande punkter betraktas som förloppsindikatorer för målen:

* Resultat

  Mer information om hur du lägger till resultat i mål finns i [Lägga till resultat i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Aktiviteter

  Mer information om hur du lägger till aktiviteter, inklusive projekt, till mål finns i [Lägg till aktiviteter i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Justerade underordnade mål

  Mer information om mål för överordnade och underordnade finns i [Justera mål genom att ansluta dem i Adobe Workfront-mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  Workfront Target beräknar den faktiska procentandelen som slutförs med följande formel:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Om ett mål till exempel har ett resultat som är 20 % färdigt, ett manuellt förloppsindikator som är 30 % färdigt, ett projekt som är 10 % färdigt och ett mål för barn som är 40 % färdigt, är målprocenten 25 %.

### Förväntad procent slutfört {#expected-percent-complete}

Workfront Target beräknar automatiskt den förväntade procentandelen av ett mål baserat på det totala antalet dagar i målets varaktighet samt på antalet dagar som har passerat sedan målets startdatum.

Workfront Target beräknar den förväntade procentandelen som slutförs med följande formel:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Om ett mål t.ex. ska vara klart inom 90 dagar, och idag är den 45:e dagen i den perioden, är den förväntade andelen färdigt 50 %.

### Förlopp och villkor {#progress}

Workfront Target beräknar en förloppsprocent och tilldelar en förloppsetikett till målen baserat på hur stor procentandel av den förväntade procentandelen som har uppnåtts vid den aktuella tidpunkten. Färgen på målprocentets fält för slutförande ändras för att visa målets förlopp.

Målets villkor uppdateras också i enlighet med detta för att ange om målet är på väg att slutföras i tid eller om det ligger efter.

Workfront Target beräknar förloppsprocenten för ett mål med hjälp av följande formel:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Om den förväntade andelen slutförd till exempel är 53 % vid den aktuella tidpunkten och den faktiska andelen slutfört är 30 %, är målförloppet 56 %. Workfront Goals etiketterar det här målet med villkoret&quot;I problem&quot;.

I följande diagram visas förhållandet mellan villkorsetiketterna och förloppsprocenten:

![Statusetiketter för förlopp har diagram](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

Tabellen nedan visar målvillkorsetiketterna och målförloppsprocenten som är associerade med varje etikett.

>[!TIP]
>
>Målvillkorsetiketterna matchar Workfront-projektvillkorsnamn och -färg.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Namn på målförlopp</b></td> 
   <td><b>Definition av målförlopp</b></td> 
   <td><b>Procent av målförlopp</b></td> 
   <td><b>Färg på procent färdigt fält</b></td> 
   <td><b>Ikon för villkorsindikator</b></td> 
  </tr> 
  <tr> 
   <td>Nyhet</td> 
   <td> <p>Målet är nyskapat och har ännu inte registrerats. Ett målförlopp visas som Nytt tills någon uppdaterar förloppet för första gången. </p> <p>Information om hur du uppdaterar målförloppet finns i <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Uppdatera målförloppet i Adobe Workfront-mål</a>.</p> </td> 
   <td>Ingen procent</td> 
   <td>Inget fält</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>På mål</span> </p> </td> 
   <td>Målet fungerar som förväntat och det är mycket sannolikt att det kommer att vara färdigt i tid. </td> 
   <td>90-100 %</td> 
   <td>Grön</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Vid risk</span> </p> </td> 
   <td>Målet släpar efter, men det kan fortfarande vara möjligt att slutföra det i tid. </td> 
   <td>70-89,99 %</td> 
   <td>Gul</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>I problem</span> </p> </td> 
   <td> <p>Det är mycket troligt att målet inte kommer att bli färdigt i tid. </p> </td> 
   <td>0-69,99 %</td> 
   <td>Röd</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>

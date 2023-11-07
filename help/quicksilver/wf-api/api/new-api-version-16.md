---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 16
description: Adobe Workfront släppte API-version 16 den 6 april 2022. API-version 16 innehåller följande ändringar från version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Nyheter i API-version 16

Adobe Workfront släppte API-version 16 den 6 april 2023. API-version 16 innehåller följande ändringar från version 15.

## Tillagda resurser

Inga resurser har lagts till för API-version 16.

## Borttagna resurser

Inga resurser togs bort för API-version 16

## Ändrade resurser

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Godkännande (GODKÄNNANDE)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Timme (TIMME)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Obs!](#note-note)
* [OpTask/Issue (OPTASK)](#note-note)
* [Projekt (PROJ)](#project-proj)
* [Hastighet (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Roll/jobbroll (ROLE)](#role--job-role-role)
* [Aktivitet (AKTIVITET)](#task-task)
* [Tidrapport (TSPEN)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Gruppering (UIGB)](#uigroupby--grouping-uigb)
* [UIView / View (UIVW)](#uiview--view-uivw)
* [Användare (ANVÄNDARE)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

### Godkännande (GODKÄNNANDE)

En viss arbetsuppgift, till exempel en uppgift, ett dokument eller en tidrapport, kan kräva att en ansvarig eller annan användare signerar arbetsposten. Ett Approval-objekt representerar åtgärden för signering av en arbetsuppgift.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Det här fältet har lagts till och visar hur många minuter arbete du behöver utföra per dag. Den har formatet <code>YYYY-MM-DD: (number of minutes)</code>och tar hänsyn till tidszonen.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tilldelning (ASSGN)

Ett uppdragsobjekt representerar anslutningen mellan en arbetsuppgift och användaren, teamet eller gruppen som är tilldelad att arbeta med den.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Det här fältet har lagts till och visar hur många minuter arbete du behöver utföra per dag. Den har formatet <code>YYYY-MM-DD: (number of minutes)</code>och tar hänsyn till tidszonen.</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>Det här fältet har lagts till och är ett booleskt värde som anger om uppdraget är innehållt. Om uppdragets minuter per dag har redigerats i Arbetsbelastningsutjämnaren, har uppdraget konturerats.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

CustomEnum-objektet hjälper dig att konvertera statuskoder till läsbar text.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### CustomerPreferences (CUSTPR)

Ett CustomerPreferences-objekt representerar den uppsättning inställningar som en kund har ställt in för sin instans av Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>Den här åtgärden returnerar ett booleskt värde som beskriver om kunden har inaktiverat alternativet att automatiskt uppgradera Contributor-licensinnehavare.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Ett ExternalSection-objekt är en extern webbsida som är inbäddad i en Workfront-rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>Detta lades till och beräknar URL:en för en iFrame som är inbäddad i en rapport.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Detta lades till och beräknar URL:er för iFrames som är inbäddade i en rapport.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Timme (TIMME)

Ett Timobjekt representerar en timme som loggas av en användare på en tidrapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>tidrapportHourIdentifier</b>
            </p>
            <p>Tillagd. Den här parametern används för att identifiera de timmar som skapas med <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Obs!

Ett Note-objekt är en kommentar eller en uppdatering som görs på ett Workfront-objekt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>Det här fältet har lagts till och representerar en lista med dokument som är bifogade kommentaren.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Issue (OPTASK)

Ett OpTask-objekt kallas vanligtvis för ett problem. Ett problem är en arbetsuppgift som vanligtvis anger att det finns ett problem som förhindrar att en uppgift eller ett projekt slutförs. Ett problem kan också vara en Help Desk-begäran. Ändringsorder, begäranden och buggar är också problem.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Det här fältet har lagts till och visar hur många minuter arbete du behöver utföra per dag. Den har formatet <code>YYYY-MM-DD: (number of minutes)</code>och tar hänsyn till tidszonen.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Den här åtgärden har lagt till fältet <code>teamIDs</code> för att ge stöd åt funktionaliteten att tilldela flera team till en uppgift eller ett problem.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Projekt (PROJ)

Projekt är arbetsuppgifter inom Workfront och är en viktig byggsten i det sätt på vilket Workfront hjälper människor att arbeta. Ett Project-objekt representerar en grupp med uppgifter med ett gemensamt, specifikt mål.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
            <p>Det här fältet har lagts till och representerar summan av alla budgeterade timmar för projektet.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hastighet (RATE)

Ett Rate-objekt representerar en faktureringsfrekvens i Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerTimme</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Dessa parametrar har flyttats till objektet Rate från rollobjektet så att Role- och User-objekt kan ha flera värden (för olika datumintervall).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Dessa parametrar representerar ID:t och objektkoden för objektet som hastigheten är kopplad till.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Den här åtgärden har lagts till och kopplar Rate-objekt till det angivna objektet. Den här slutpunkten fungerar för alla objekt som kan kopplas till hastigheten.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Ett RichTextNote-objekt är en kommentar eller en uppdatering som har gjorts på ett Workfront-objekt och som innehåller formaterad text, till exempel fet eller kursiv text.

RichTextNote-objektet tog bort flaggan `REPORTABLE`.

### Roll/jobbroll (ROLE)

Ett rollobjekt (jobbroll) representerar en funktionskapacitet eller en kompetensuppsättning som en användare kan fylla, till exempel Designer eller Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
           <li>
            <p><b>frekvenser</b>
            </p>
            <p>Detta har lagts till och representerar Rate-objekten som är kopplade till den här rollen.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Aktivitet (AKTIVITET)

Ett Task-objekt representerar en arbetsuppgift som måste utföras som ett steg mot att uppnå ett slutligt mål (slutföra ett projekt).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Det här fältet har lagts till och visar hur många minuter arbete du behöver utföra per dag. Den har formatet <code>YYYY-MM-DD: (number of minutes)</code>och tar hänsyn till tidszonen.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Den här åtgärden har lagt till fältet <code>teamIDs</code> för att ge stöd åt funktionaliteten att tilldela flera team till en uppgift eller ett problem.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Tidrapport (TSPEN)

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>Den här parametern tog bort flaggan <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Den här parametern tog bort flaggan <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Den här parametern har lagts till och lagrar tidrapporternas varaktighet i dagar oavsett ändringar i"Motsvarande timmar för fullständig Workday".  Om till exempel Motsvarande timmar är inställt på 6 och en dag är loggad ändras Motsvarande timmar till 8 timmar. <code>totalDays</code> har fortfarande värdet 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>Den här åtgärden har lagts till och tar en filterfrågemappning och lägger till <code>allowingnull</code> join for nullable fields.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Dessa åtgärder har stöd för möjligheten att dela filter, vyer och grupperingar i hela systemet.</p><p>Mer information finns i <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Göra filter, vyer och grupperingar tillgängliga för alla användare</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Gruppering (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Dessa åtgärder har stöd för möjligheten att dela filter, vyer och grupperingar i hela systemet.</p><p>Mer information finns i <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Göra filter, vyer och grupperingar tillgängliga för alla användare</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">funktionsmakron</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Dessa åtgärder har stöd för möjligheten att dela filter, vyer och grupperingar i hela systemet.</p><p>Mer information finns i <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Göra filter, vyer och grupperingar tillgängliga för alla användare</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Användare (ANVÄNDARE)

Ett User-objekt representerar en person med ett konto i Workfront som kan logga in och interagera med systemet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
           <li>
            <p><b>frekvenser</b>
            </p>
            <p>Detta har lagts till och representerar de Rate-objekt som är kopplade till den här användaren.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Ett UserNote-objekt är ett meddelande.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Frågor</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Följande möjliga värde har lagts till:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Arbete (ARBETE)

Ett Work-objekt är ett vanligt gränssnitt som både Task och OpTask ärver och delar gemensam kod mellan de två.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Det här fältet har lagts till och visar hur många minuter arbete du behöver utföra per dag. Den har formatet <code>YYYY-MM-DD: (number of minutes)</code>och tar hänsyn till tidszonen.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

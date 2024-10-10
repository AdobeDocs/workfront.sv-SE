---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 19
description: Adobe Workfront släppte API-version 19 den 6 april 2022. API-version 19 innehåller följande ändringar från version 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 13910328903744aa9bf619e8b4c376520c21b89e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Nyheter i API-version 19

Adobe Workfront släppte API-version 19 den 8 april 2024. API-version 19 innehåller följande ändringar från version 18.

## Tillagda resurser

Inga resurser har lagts till för API-version 19.

## Borttagna resurser

Inga resurser togs bort för API-version 19

## Ändrade resurser

### AccessLevel (ACSLVL)

Ett AccessLevel-objekt är associerat med användare och beskriver uppsättningen AccessLevelPermissions som avgör vad användaren kan komma åt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestritions</b><p>Följande möjliga värden har lagts till:
            </p>
            <ul>
              <li>
                <p>Inaktivera Workfront AI Assistant (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tilldelning (ASSGN)

Ett uppdragsobjekt representerar anslutningen mellan en arbetsuppgift och användaren, teamet eller gruppen som är tilldelad att arbeta med den.

Tilldelningsobjektet lade till flaggan **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>Följande direkta fält har lagts till:
        <ul>
          <li>
            <p><b>categoryID</b><p>En kategori är ett anpassat formulär. Det här fältet har stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
            </p>
          </li>
          <li>
            <p><b>prioritet</b><p>Det här fältet tillåter följande värden:
            <ul>
              <li>0 (ingen)</li>
              <li>1 (låg)</li>
              <li>2 (normal)</li>
              <li>3 (hög)</li>
              <li>4 (Urgent)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>Följande referensfält har lagts till:
        <ul>
          <li>
            <p><b>kategori</b><p>En kategori är ett anpassat formulär. Det här fältet har stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>Följande samlingsfält har lagts till:
        <ul>
          <li>
            <p><b>objectCategories</b><p>En kategori är ett anpassat formulär. Det här fältet har stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Kategori (CTGY)

Ett kategoriobjekt är ett anpassat formulär.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>Följande fält har lagts till som stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
        <ul>
          <li>
            <p><b>catObjCode</b><p>Följande möjliga värden har lagts till:
            </p>
            <ul>
              <li>
                <p>Tilldelning (ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Följande möjliga värden har lagts till:
            </p>
            <ul>
              <li>
                <p>Tilldelning (ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Klassificerare (CLSF)

En klassificerare är en plats.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>Följande åtgärder har lagts till:
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Kund

Ett kundobjekt representerar en organisation som använder en instans av Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Följande möjliga värden har lagts till:
            </p>
            <ul>
              <li>
                <p>Tilldelningsprioriteter (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>CustomEnum-objektet hjälper dig att konvertera statuskoder till läsbar text.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences (CUSTPR)

Ett CustomerPreferences-objekt representerar den uppsättning inställningar som en kund har ställt in för sin instans av Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>Följande möjliga värden har tagits bort:
            </p>
            <ul>
              <li>
                <p>Aktivera zoomintegrering i uppdateringsströmmen (lösenord:zoomIntegrationEnabled)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Dokument (DOCU)

Ett Document-objekt representerar en fil (t.ex. skrivet material, bilder eller andra typer av information).

<table>
  <tbody>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>Fältet <code>folderID</code> har lagts till.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Tillagd.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate (EXRAT)

Ett ExchangeRate-objekt representerar en valutakurs som har ställts in i Workfront. ExchangeRate-objekt är inte dynamiska.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
      <ul>
      <li>Följande fält har lagt till valideraren <code>REQUIRED</code>:
        <ul>
          <li><p><b>valuta</b></li>
          <li><p><b>ränta</b></li></ul>
      <li>Följande fält har lagts till:
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>
      <ul>
        <li>Följande fält har lagts till:
        <ul>
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupp (GRUPP)

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

Group-objektet lade till flaggan **SHARABLE**.

### Timme (TIMME)

Ett Timobjekt representerar en timme som loggas av en användare på en tidrapport.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
      Följande fält har lagts till:
        <ul>
          <li><p><b>assignApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>jectedByID</b></li>
          <li><p><b>jectedOnDate</b></li>
          <li><p><b>refuseringKommentar</b></li>
          <li><p><b>submitByID</b></li>
          </ul>
          <p>Följande ändringar gjordes i fältet <b>hours</b>.</p>
          <ul> 
          <li> Borttagen validerare <b>GREATER_THAN</b></li>
          <li> Valideraren <b>NOT_EQUAL</b> har lagts till</li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
      Följande åtgärder har lagts till:
        <ul>
          <li><p><b>godkänn</b></li>
          <li><p><b>ogodkänna</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

JournalEntry-objektet kan ställas in för att logga information om specifika objektfält när som helst när dessa fält ändras. När ett fält har ställts in för att loggas som en del av journalpostobjektet, skapas en motsvarande journalpost varje gång fältet ändras.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>flaggor</b><p>Följande möjliga värden har lagts till:
            </p>
            <ul>
              <li>
                <p>Är kostnadstariff
                </p>
              </li>
              <li>
                <p>Faktureringsränta (BR)
                </p>
              </li>
              <li>
                <p>Är allmän finansiering
                </p>
              </li>
              <li>
                <p>Är kombinerad finansiering (CF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Parameter (PARAM)

Ett Parameter-objekt är ett anpassat fält.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>Följande möjliga värde har lagts till:
            <ul>
            <li>Varaktighet (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Om du vill skapa ett mer användarvänligt och flexibelt system har fälttypen <b>WIDGET </b> tagits bort och delats upp i följande fälttyper:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Bild (BILD)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Extern sökning (EXTRNL)</li>
            <li>Flerval extern sökning (MULTEXTRNL)</li>
            <li>Native Field (WFNATIVE)</li>
            <li>Planeringsfält (WFPLANNING)</li>
            <li>Tidsfasad KPI (TIMEPHASED)</li>
            <li>Samlad (ROLLUP)</li>
            <li>Dokument (DOKUMENT)</li>
           </ul>
          </li>
          <li>
            <p><b>konfigurationer</b><p>Tillagd.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Roll (ROLE)

Ett rollobjekt (jobbroll) representerar en funktionskapacitet eller en kompetensuppsättning som en användare kan fylla, till exempel Designer eller Product Manager.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
    Följande fält har lagts till:
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>
        Följande fält har lagts till:
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Ett ScoreCardQuestion-objekt representerar en fråga som har lagts till i ett styrkort. Dessa frågor avgörs vanligtvis av Portfolio-förvaltaren och deras svar gör det möjligt för förvaltaren att förstå hur väl ett projekt passar ihop med portföljens mål.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
            <p><b>displayType</b></p><p>Om du vill skapa ett mer användarvänligt och flexibelt system har fälttypen <b>WIDGET </b> tagits bort och delats upp i följande fälttyper:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Bild (BILD)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Extern sökning (EXTRNL)</li>
            <li>Flerval extern sökning (MULTEXTRNL)</li>
            <li>Native Field (WFNATIVE)</li>
            <li>Planeringsfält (WFPLANNING)</li>
            <li>Tidsfasad KPI (TIMEPHASED)</li>
            <li>Samlad (ROLLUP)</li>
            <li>Dokument (DOKUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TASSGN)

Ett TemplateAssignment-objekt representerar anslutningen mellan en malluppgift och användaren, teamet eller gruppen som är tilldelad att arbeta med den. När mallen används för ett projekt tilldelas användaren, teamet eller gruppen uppgiften.

TemplateAssignment-objektet lade till flaggan **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>Följande direkta fält har lagts till:
        <ul>
          <li>
            <p><b>categoryID</b><p>En kategori är ett anpassat formulär. Det här fältet har stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>Följande referensfält har lagts till:
        <ul>
          <li>
            <p><b>kategori</b><p>En kategori är ett anpassat formulär. Det här fältet har stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>Följande samlingsfält har lagts till:
        <ul>
          <li>
            <p><b>objectCategories</b><p>En kategori är ett anpassat formulär. Det här fältet har stöd för möjligheten att lägga till ett anpassat formulär i ett uppdrag.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tidrapport (TSPEN)

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Borttagen.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>



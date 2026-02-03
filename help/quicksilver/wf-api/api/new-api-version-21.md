---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 21
description: Adobe Workfront släppte API-version 21 den 23 oktober 2025. API version 21 innehåller följande ändringar från version 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 7166a6b51a45b744a33df697c2bc8080427908a8
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Nyheter i API-version 21

>[!IMPORTANT]
>
>Denna API-version innehåller en brytningsändring som kan påverka dina befintliga API-anrop. Detta beror på att API version 21 använder Event Subscriptions version 2.
>
> För flervalsfält skickas alltid Event Subscriptions version 2 som en array. Version 1 skickade en array om mer än ett värde har valts. Om bara ett värde valdes, skickades en sträng.

Adobe Workfront släppte API-version 21 den 23 oktober 2025. API version 21 innehåller följande ändringar från version 20.

## Tillagda resurser

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

## Borttagna resurser

### Tilldelningens faktureringsroll (ASBLRL)

AssignmentBillingRole-objektet och alla dess fält har tagits bort.

## Ändrade resurser

### AccessLevelPermissions (ALVPER)

Ett AccessLevelPermissions-objekt representerar en specifik behörighet för att komma åt, skapa eller ändra ett Workfront-objekt. Dessa behörigheter kan sedan kopplas till en åtkomstnivå.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Om en användare inte har åtkomst till ett objekt i Workfront som de behöver kan de begära åtkomst till det objektet. AccessRequest-objektet representerar denna begäran.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>åtgärd</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Ett AccessRule-objekt representerar en regeluppsättning med anpassade åtkomstnivåer som avgör hur användare kan dela projekt som de skapar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AnnouncementAttachment (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Tillagd</p>
          </li>
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
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>tilldelningBillingRoles</b>
            </p>
            <p>Borttagen</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Kategori (CTGY)

Ett kategoriobjekt är ett anpassat formulär.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Kund (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Inaktivera användning av ett Java-miniprogram för tidslinjeberäkningar)
            </p>
            <p>Tillagd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Dokument (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Tillagd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

DocumentFolder-objektet lade till flaggan `RESTORABLE`.

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
            <p><b>getTerejectionCommentmodernCloudURL</b>
            </p>
            <p>Valideraren har lagts till <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Tillagd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Parameter (PARAM)

Ett Parameter-objekt är ett anpassat fält.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (Lexikalisk RTF)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Enkelradssammanslagning)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Tillagd</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfält</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Tillagd</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORT)

Ett Portfolio-objekt är en samling projekt som konkurrerar om samma resurser, vanligtvis pengar eller personer som ska slutföra dem.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Tillagd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Program (PRGM)

Ett Program-objekt är en delmängd av projekt i en portfölj, där liknande projekt kan grupperas tillsammans.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>valuta</b>
            </p>
            <p>Tillagd</p>
              </li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Tillagd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats i Help Desk-området där användarna kan skicka utgåvor till den.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>requestedCoreAction</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestedForbiddenActions</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Redigera kontaktinformation)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>Tillagd</p>
            </li>
            </ul>
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
            <p><b>localBillingPerHour</b>
            </p>
            <p>Borttagen</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Borttagen</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Roll (ROLE)

Ett rollobjekt (jobbroll) representerar en funktionskapacitet eller en kompetensuppsättning som en användare kan fylla, till exempel Designer eller Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>Åsidosätt valuta</b>
            </p>
            <p>Borttagen</p>
              </li>
          <li>
            <p><b>Åsidosätt kostnadstariff</b>
            </p>
            <p>Borttagen</p>
              </li>
          <li>
            <p><b>Åsidosätt faktureringshastighet</b>
            </p>
            <p>Borttagen</p>
              </li>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport (SCHREP)

Ett ScheduledReport-objekt representerar en rapport som har konfigurerats att schemaläggas för leverans.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Ett ScoreCardQuestion-objekt representerar en fråga som har lagts till i ett styrkort. Dessa frågor avgörs vanligtvis av Portfolio-chefen och deras svar gör det möjligt för den som ansvarar för ledningen att förstå hur väl ett projekt passar in i portfolions mål.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Följande möjliga värde har lagts till:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Enkelradssammanslagning)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Team

Team-objektet lade till flaggorna `DATA_EXTENDIBLE` och `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>
        <ul>
          <li>
            <p><b>kategori</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### TemplateAssignment

TemplateAssignment-objektet lade till flaggan `ATTRIBUTE_ATTACHABLE`.

### Tidrapport (TSPEN)

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>Borttagen</p>
              </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Tillagd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>



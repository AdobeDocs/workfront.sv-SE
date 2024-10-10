---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 18
description: Adobe Workfront släppte API-version 18 den 6 april 2022. API-version 18 innehåller följande ändringar från version 17.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Nyheter i API-version 18

Adobe Workfront släppte API-version 18 den 8 april 2024. API-version 18 innehåller följande ändringar från version 17.

## Tillagda resurser

Inga resurser har lagts till för API-version 18.

## Borttagna resurser

Inga resurser togs bort för API-version 18

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
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
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
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
          </li>
        </ul>
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
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
          </li>
        </ul>
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
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Väntar på godkännande (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Operationer</td>
      <td>
        <ul>
          <li>
            <p>Följande åtgärder har lagts till:
            </p>
            <ul>
              <li>
                <p><b>LÄGG TILL</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Baslinje (BLIN)

Baslinjer är bilder på hur ett projekts prestanda ser ut vid en viss tidpunkt. De lagrar viktig information om projektet, t.ex. nyckeldatum, förlopp, kostnad och intäktsvärden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Originalaktivitet (BSTSK)

Baslinjer är bilder på hur ett projekts prestanda ser ut vid en viss tidpunkt. De lagrar viktig information om projektet, t.ex. nyckeldatum, förlopp, kostnad och intäktsvärden. När du skapar en baslinje hämtas uppgiftsinformationen också till baslinjeuppgifterna för den baslinjen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
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
            <p><b>catObjCode</b>:
            </p>
            <p>Följande möjliga värden har lagts till:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Resurskategori för annat än arbete)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Timme)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Kreditkort)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Följande möjliga värden har lagts till:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Resurskategori för annat än arbete)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Timme)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Kreditkort)
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Dokument (DOCU)

Ett Document-objekt representerar en fil (t.ex. skrivet material, bilder eller andra typer av information).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>Följande parameter har lagts till:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Tillagd. Den här nya åtgärden har följande parametrar:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
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
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

JournalEntry-objektet kan ställas in för att logga information om specifika objektfält när som helst när dessa fält ändras. När ett fält har ställts in för att loggas som en del av journalpostobjektet, skapas en motsvarande journalpost varje gång fältet ändras.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.Decision.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
              </li>
            </ul>
          </li>
        </ul>
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
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Följande fält har lagts till:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Följande fält har lagts till:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
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
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Tillagd.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
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
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestedForbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visa kostnadstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visa faktureringstariffer)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Se allmän ekonomi)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Redigera kostnadstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Redigera faktureringstariffer)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Redigera allmän ekonomi)</p>
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
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Följande flaggor har lagts till:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DYNAMIC
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Tillagd.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
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
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>Följande fält har lagts till:
             <ul><li><code>copyCategories</code></li></ul>
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Mall (TMPL)

Ett Template-objekt representerar ett mönster för ett projekt. Projekt kan skapas från mallar för att spara tid. En mall innehåller ett team och uppgifter som kopieras till alla projekt som skapas från mallen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

Ett TemplateTask-objekt representerar en aktivitet som är en del av en Template. Malluppgifter blir uppgifter i det projekt där mallen används.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (TTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>Följande fält har tagits bort:
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Uppdatera (UPPDATERA)

Arbetsobjekt i Workfront kan uppdateras för att hålla användarna informerade om den aktuella statusen. Ett Update-objekt representerar en av dessa uppdateringar. Uppdateringar kan anges av användare eller skapas av Workfront-systemet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Ett UserPrefValue-objekt representerar en användarinställning.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>värde</b>
            </p>
            <p>Valideraren har lagts till <code>MAX_LENGTH</code></p>
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
            <p>Följande fält har lagts till:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>planeradFakturerbarUtgiftKostnad</b>
                </p>
              </li>
              <li>
                <p><b>planeradNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


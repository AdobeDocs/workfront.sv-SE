---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 17
description: Adobe Workfront släppte API-version 17 den 6 april 2022. API-version 17 innehåller följande ändringar från version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Nyheter i API-version 17

Adobe Workfront släppte API version 17 den 12 oktober 2023. API-version 17 innehåller följande ändringar från version 16.

## Tillagda resurser

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

Ett ExternalDocument-objekt är ett dokument eller en annan digital resurs som finns i en dokumentlagringsleverantör utanför Workfront. Dessa resurser kan länkas till och från Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>bana</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>bana</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>value</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfält</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Frågor</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operationer</td>
      <td>
        <ul>
          <li><p><b>SÖK</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>
        <ul>
          <li><p><b>kund</b></p></li>
          <li><p><b>användare</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Borttagna resurser

Inga resurser togs bort för API-version 17

## Ändrade resurser

Följande resurser ändrades för API-version 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Baslinje (BLIN)

Baslinjer är bilder på hur ett projekts prestanda ser ut vid en viss tidpunkt. De lagrar viktig information om projektet, t.ex. nyckeldatum, förlopp, kostnad och intäktsvärden.

Baslinjeobjektet tog bort flaggan **INLINE_EDITABLE**.

### Faktureringspost (BILL)

Ett BillingRecord-objekt registrerar intäkter, timmar eller utgifter som kan faktureras. Den här informationen kan användas för att skapa fakturor i ett externt redovisningssystem.

Faktureringsposten-objektet tog bort flaggan **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Företag (CMPY)

Ett företagsobjekt representerar en organisation som består av en samling personer.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Borttagen</p>
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
            <p>Lagt till det möjliga värdet "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)&gt;/p?<p>På så sätt kan en organisation göra den nya hemupplevelsen till standardupplevelsen för sina användare.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Ett DocumentVersion-objekt representerar en specifik version av en fil (t.ex. skrivet material, bilder eller andra typer av information).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Det möjliga värdet "Frame.io" (FRAMEIO) har lagts till</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Det möjliga värdet enum.filetype.site (site) har lagts till</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRAT)

Ett ExchangeRate-objekt representerar en valutakurs som har ställts in i Workfront. ExchangeRate-objekt är inte dynamiska.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>Följande fält har lagts till:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrency</b></p></li>
          <p>Tillagd.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Utgift (EXPNS)

Utgifter är de icke-arbetskostnader som kan uppstå under ett projekts livslängd.

Utgiftsobjektet tog bort flaggan **INLINE_EDITABLE**.

### Grupp (GRUPP)

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Borttagen</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Timme (TIMME)

Ett Timobjekt representerar en timme som loggas av en användare på en tidrapport.

Objektet Timme tog bort flaggan **INLINE_EDITABLE**.

### Iteration (ITRN)

Ett Iteration-objekt representerar en enkel Agile Iteration. Iterationer är diskreta tidsperioder som används för att planera och slutföra Agile-berättelser.

Iteration-objektet tog bort flaggan **INLINE_EDITABLE**.


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
              <li>Tillagd godkännare (AAA)</li>
              <li>Granskare tillagd (AAR)</li>
              <li>Borttagen granskare (ARR)</li>
              <li>Godkännare (ARA) har tagits bort</li>
              <li>Godkänt beslut (ADA)</li>
              <li>Beslut godkänt med ändringar (ADC)</li>
              <li>Beslutsbehov (ADN)</li>
              <li>Beslutet har återkallats (ADR)</li>
              <li>Godkännaren har ändrats (AAC)</li>
              <li>Granskaren har ändrats (ARC)</li>
              <li>Granskningen är klar (RDC)</li>
              <li>Granskningen har återkallats (RDR)</li>
              <li>Publicera (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban Board (KNBNBD)

En Kanban-tavla används för att spåra uppgifter i en Agile-miljö.

Kanban-styrelsobjektet tog bort flaggan **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Ett LinkedFolder-objekt representerar en mapp som är länkad från en extern dokumentleverantör, till exempel Google Drive eller Dropbox.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Tillagt möjligt värde "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Issue (OPTASK)

Ett OpTask-objekt kallas vanligtvis för ett problem. Ett problem är en arbetsuppgift som vanligtvis anger att det finns ett problem som förhindrar att en uppgift eller ett projekt slutförs. Ett problem kan också vara en Help Desk-begäran. Ändringsorder, begäranden och buggar är också problem.

Objektet Issue tog bort flaggan **INLINE_EDITABLE**.

### Projekt (PROJ)

Projekt är arbetsuppgifter inom Workfront och är en viktig byggsten i det sätt på vilket Workfront hjälper människor att arbeta. Ett Project-objekt representerar en grupp med uppgifter med ett gemensamt, specifikt mål.

Project-objektet tog bort flaggan **INLINE_EDITABLE**.

### ProjectUser (PRTU)

Ett ProjectUser-objekt representerar en användare som är associerad med ett visst projekt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Hastighet (RATE)

Ett Rate-objekt representerar en faktureringsfrekvens i Workfront.

Rate-objektet tog bort flaggan **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>Följande åtgärder har lagts till för att stödja funktionen för grafikkort:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>The <b>setRatesForRole</b> åtgärden har ändrats för att lägga till följande fält:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risk (RISK)

Ett Risk-objekt representerar en möjlig händelse som kan hindra ett projekt från att avslutas i tid eller inom budgeten. Risker läggs till projekt i planeringsfasen för att identifiera potentiella hinder innan något arbete godkänns.

Riskobjektet tog bort flaggan **INLINE_EDITABLE**.

### Roll/jobbroll (ROLE)

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
            <p><b>defaultInterface</b>
            </p>
            <p>Borttagen</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aktivitet (AKTIVITET)

Ett Task-objekt representerar en arbetsuppgift som måste utföras som ett steg mot att uppnå ett slutligt mål (slutföra ett projekt).

Aktivitetsobjektet tog bort flaggan **INLINE_EDITABLE**.

### Team (TEAMOB)

Ett Team-objekt är en samling användare som kan tilldelas till ett arbetsobjekt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Borttagen</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMMB)

Ett TeamMember-objekt är en användare som är kopplad till ett specifikt team.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
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
            <p><b>objCode</b>
            </p>
            <p>Borttagen</p>
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
            <p><b>changeType</b>
            </p>
            <p>Följande värden har lagts till:</p>
            <ul>
              <li>Tillagd godkännare (AssetApprovalAddApprover)</li>
              <li>Granskare tillagd (assetapprovalAddReviewer)</li>
              <li>Godkännaren har tagits bort (AssetApprovalRemoveApprover)</li>
              <li>Borttagen granskare (assetapprovalRemoveReviewer)</li>
              <li>Godkänt beslut (godkännandeGodkäntBeslutGodkänt)</li>
              <li>Beslut behöver arbete (assetapprovalDecisionNeedsWork)</li>
              <li>Beslut godkänt med ändringar (assetapprovalDecisionApprovedChanges)</li>
              <li>Beslut återkallat (godkännandeBeslutÅterkallat)</li>
              <li>Godkännaren har ändrats (AssetApprovalApproverChanged)</li>
              <li>Granskaren har ändrats (assetapprovalReviewerChanged)</li>
              <li>Granskningen är klar (assetapprovalReviewerDecisionComplete)</li>
              <li>Granskningen har återkallats (assetapprovalReviewerDecisionRevoked)</li>
              <li>Fel vid sändning av externt dokument (externalDocumentSendError)</li>
              <li>Dokumentversion publicerad (documentVersionPublish)</li>
              <li>Arbetsflöde för länkad mapp (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Användare (ANVÄNDARE)

Ett User-objekt representerar en person med ett konto i Workfront som kan logga in och interagera med systemet.

Användarobjektet tog bort flaggan **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Det här fältet har lagts till och är ett tal mellan 0 och 1 som representerar den procentandel av tiden som en användare kan lägga på projektarbete (icke-overheadarbete) varje dag. Värdet 1 innebär att användaren kan lägga 100 % av sin tid på projektarbete.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserGroups (USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote (USRNOT)

Ett UserNote-objekt är ett meddelande.

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
            <p>Följande värden har lagts till:</p>
            <ul>
              <li>Dokumentet måste godkännas (AAA)</li>
              <li>Dokumentet behöver din granskning (AAR)</li>
              <li>Dokumentet behöver inte längre ditt godkännande (ARA)</li>
              <li>Dokumentet behöver inte längre din granskning (ARR)</li>
              <li>Dokumentet behöver (användarens) godkännande (ATA)</li>
              <li>Dokumentbehov (användare) - granskning (ATR)</li>
              <li>Dokumentet behöver inte längre (användarens) godkännande</li>
              <li>Dokumentet behöver inte längre (RTR)</li>
              <li>Dokumentet har godkänts (ADA)</li>
              <li>Dokumentet har godkänts med ändringar (ADC)</li>
              <li>Dokumentet behöver arbete (ADN)</li>
              <li>(Användare) har markerat (dokument) som godkänt. Ditt godkännande behövs inte längre. (AAN)</li>
              <li>(Användare) har markerat (dokument) som godkänt med ändringar. Ditt godkännande behövs inte längre. (ACN)</li>
              <li>(Användare) har markerat (dokument) som nödvändigt arbete. Ditt godkännande behövs inte längre. (AWN)</li>
              <li>Dokumentet behöver granskas nu istället för godkännande (AAC)</li>
              <li>Dokumentet behöver ditt godkännande nu i stället för en granskning (ADN)</li>
              <li>Dokumentet granskat (RDC)</li>
              <li>Dokument granskat (TRC)</li>
              <li>(Användare) har granskat (dokument) som slutfört. Granskningen behövs inte längre. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 15
description: Adobe Workfront släppte API version 14 den 14 juni 2022. API-version 15 innehåller följande ändringar från version 14.
author: Becky
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 0%

---

# Nyheter i API-version 15

Adobe Workfront släppte API version 15 den 14 juni 2022. API-version 15 innehåller följande ändringar från version 14.

## Tillagda resurser

* [Initiative (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Initiative (INITIV)

Objektet Initiative skapar uppskattningar i Workfront Scenario Planner för typ och antal av jobbroller, fasta kostnader och planerad förmån.

Mer information om Initiativ finns i [Översikt över initiativ i scenarioplaneraren](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Detta är ett internt objekt.</p>
          </li>
          <li>
            <p><b>varaktighet</b>
            </p>
            <p>Tiden mellan endDate och startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Det planerade datumet för slutförandet av initiativet.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>Det ID som är associerat med användaren som skickade begäran.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Det ID som är associerat med åtgärden</p>
          </li>
          <li>
            <p><b>initialID</b>
            </p>
            <p>Det ID som är kopplat till initiativet.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>Det datum då initiativet senast offentliggjordes i Workfront Scenario Planner.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Initiativets namn</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>ID för den plan som är förknippad med initiativet.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>Namnet på den plan som är förknippad med initiativet.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>ID för det projekt som är associerat med initiativet.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>ID:t för scenariot i Workfront Scenario Planner som är kopplat till initiativet.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>Initiativets planerade startdatum.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <ul>
          <li>
            <p><b>kund</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>projekt</b>
            </p>
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
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operationer</td>
      <td>
        <ul>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RAPPORT </b>
            </p>
          </li>
          <li>
            <p><b>SÖK</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

IssueDef-objektet representerar en uppsättning data om problemformatet. Det här objektet kan bifogas till projekt eller mallar och påverkar de problem som läggs till i projektet eller mallen.

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
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

I vissa fall går det att länka Workfront-objekt direkt till objekt i en extern programprodukt. Objektet ObjectIntegration representerar den här länken.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Detta är ett internt objekt.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>Det datum och den tidpunkt då ObjectIntegration angavs i Workfront System.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Unikt Workfront-ID för det specifika ObjectIntegration-objektet.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>Den externa programvara som ObjectIntegration-objektet skapar en länk med. Möjliga värden är:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>Det objekt i Workfront som ObjectIntegration är associerat med.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>Objektkoden för det objekt i Workfront som ObjectIntegration är associerat med.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <ul>
          <li>
            <p><b>kund</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

TaskDef-objektet representerar en uppsättning data om aktiviteternas format. Det här objektet kan bifogas till projekt eller mallar och påverkar de uppgifter som läggs till i projektet eller mallen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält </td>
      <td>
        <ul>
          <li>
            <p><b>godkännareID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <ul>
          <li>
            <p><b>godkännare</b>
            </p>
          </li>
          <li>
            <p><b>kund</b>
            </p>
          </li>
          <li>
            <p><b>begärande</b>
            </p>
          </li>
          <li>
            <p><b>användare</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfält</td>
      <td >
        <ul>
          <li>
            <p><b>godkännareID</b>
            </p>
          </li>
          <li>
            <p><b>requestID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>godkänn</b>
            </p>
          </li>
          <li>
            <p><b>avvisa</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operationer</td>
      <td>
        <ul>
          <li>
            <p><b>LÄGG TILL</b>
            </p>
          </li>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RAPPORT</b>
            </p>
          </li>
          <li>
            <p><b>SÖK</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Borttagna resurser

Inga resurser togs bort för API-version 15.

## Ändrade resurser

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Godkännande (GODKÄNNANDE)](#Approval)

* [Kategori (CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Grupp (GRUPP)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask/Issue (OPTASK)](#OpTask)

* [Parameter (PARAM)](#Paramete)

* [Portfolio (PORT)](#Portfoli)

* [Program (PRGM)](#Program)

* [Projekt (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Aktivitet (AKTIVITET)](#Task)

* [Mall (TMPL)](#Template)

* [Tidrapport (TSPEN)](#Timeshee)

* [Visa (UIVIEW)](#View)

* [Uppdatera (UPPDATERA)](#Update)

* [Användare (ANVÄNDARE)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Arbete (ARBETE)](#Work)

### AccessLevel (ACSLVL)

Ett AccessLevel-objekt är associerat med användare och beskriver uppsättningen AccessLevelPermissions som avgör vad användaren kan komma åt.

Mer information om åtkomstnivåer finns i [Åtkomstnivåer](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>VTMAWMG (Visa team som är associerade med mina grupper)</p>
              </li>
              <li>
                <p>VALLTM (Visa alla team)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>coreAction</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
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
            <p><b>åtgärd</b> (sträng)</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (sträng)</p>
            <p>Följande möjliga värde har lagts till:</p>
            <ul>
              <li>
                <p>WDL</p>
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
            <p><b>coreAction</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (sträng[])</p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
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
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <ul>
          <li>
            <p><b>initiativ</b>
            </p>
            <p>Tillagd.</p>
            <p>Objektet Initiative skapar uppskattningar i Workfront Scenario Planner för typ och antal av jobbroller, fasta kostnader och planerad förmån. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Tillagd.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Tillagd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Tillagd.</p>
            <p>I vissa fall går det att länka Workfront-objekt direkt till objekt i en extern programprodukt. Objektet ObjectIntegration representerar den här länken.</p>
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
            <p><b>catObjCode</b> (sträng)</p>
            <p>Följande möjliga värde har lagts till:</p>
            <ul>
              <li>
                <p>GRUPP (Grupp)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (sträng[])</p>
            <p>Tillagd.</p>
            <p style="font-weight: normal;">Den här parametern är en array med möjliga objekt som det anpassade formuläret kan kopplas till. Den lades till för att ge stöd för möjligheten att bifoga ett anpassat formulär till flera typer av objekt.</p>
            <p>Möjliga värden: </p>
            <p>CMPY, PORT, PRGM, PROJ, AKTIVITET, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (sträng[])</p>
            <p>Tillagd.</p>
            <p style="font-weight: normal;">Den här parametern är en array med möjliga objekt som det anpassade formuläret kan kopplas till. Den lades till för att ge stöd för möjligheten att bifoga ett anpassat formulär till flera typer av objekt.</p>
            <p>Möjliga värden: </p>
            <p>CMPY, PORT, PRGM, PROJ, AKTIVITET, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>Tillagd.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Tillagd.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Tillagd.</p>
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
            <p>Följande värden har lagts till:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint-integrering (Graph API) aktiverad)</p>
                <p>Det här värdet stöder den uppdaterade Sharepoint-integreringen.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Tillåt användare att skapa projekt utan att använda en mall)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Dokument kan ordnas i mappar. Du kan skapa personliga mappar i ditt personliga dokumentområde. DocumentFolder-objektet representerar en av dessa mappar.

DocumentFolder-objektet lade till flaggan `SHARABLE`.

### DocumentVersion (DOCV)

Ett DocumentVersion-objekt representerar en specifik version av en fil (t.ex. skrivet material, bilder eller andra typer av information).

Mer information om dokumentversioner finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>Följande värde har lagts till: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>Det här värdet stöder den uppdaterade Sharepoint-integreringen.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupp (GRUPP)

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

Mer information om grupper finns i Grupper kontra team.

Group-objektet lade till flaggan `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <p>Följande fält har lagts till:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>En kategori är ett eget formulär. Den här parametern har lagts till för att ge stöd för möjligheten att lägga till anpassad Forms till gruppobjekt. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Det här är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <p>Följande fält har lagts till:</p>
        <ul>
          <li>
            <p><b>godkännare</b>
            </p>
          </li>
          <li>
            <p><b>kund</b>
            </p>
          </li>
          <li>
            <p><b>begärande</b>
            </p>
          </li>
          <li>
            <p><b>användare</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <p>Följande fält har lagts till:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>I vissa fall går det att länka Workfront-objekt direkt till objekt i en extern programprodukt. Objektet ObjectIntegration representerar den här länken.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfält</td>
      <td >
        <p>Följande fält har lagts till:</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Det här är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <p>Följande fält har lagts till:</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Den här åtgärden beräknar om uttrycken i anpassade formulärfält.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
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
        <p><b>changeType</b>
        </p>
        <p>Följande värde har lagts till: </p>
        <ul>
          <li>
            <p>DW (hämta)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Ett LinkedFolder-objekt representerar en mapp som är länkad från en extern dokumentleverantör, till exempel Google Drive eller Dropbox.

Mer information om länkade mappar finns i Länka dokument från externa program.

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
            <p>Följande värde har lagts till: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>Det här värdet stöder den uppdaterade Sharepoint-integreringen.</p>
              </li>
            </ul>
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
      <td role="rowheader">Åtgärder</td>
      <td>
        <p>Följande åtgärder har lagts till:</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>Följande åtgärd ändrades:</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Tillagt fält <code>parentID</code></p>
          </li>
        </ul>
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
        <p>Följande fält har lagts till:</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Följande fält har ändrats:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Det möjliga värdet har lagts till <code>WIDGET </code>(Widget) </p>
            <p>Det här värdet stöder användning av bilder i anpassade formulär.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Det möjliga värdet har lagts till <code>WIDGET </code>(Widget)</p>
            <p>Det här värdet stöder användning av bilder i anpassade formulär.</p>
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
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Program (PRGM)

Ett programobjekt är en delmängd av projekt i en portfölj, där liknande projekt kan grupperas tillsammans.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
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
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td >
        <ul>
          <li>
            <p><b>initiativ</b>
            </p>
            <p>Objektet Initiative skapar uppskattningar i Workfront Scenario Planner för typ och antal av jobbroller, fasta kostnader och planerad förmån. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>I vissa fall går det att länka Workfront-objekt direkt till objekt i en extern programprodukt. Objektet ObjectIntegration representerar den här länken.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats i Help Desk-området där användarna kan skicka utgåvor till den.

Mer information om köer finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>requestCoreAction</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestForbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (redigera team jag är på)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Ett ScoreCardQuestion-objekt representerar en fråga som har lagts till i ett styrkort. Dessa frågor avgörs vanligtvis av Portfolio-förvaltaren och deras svar gör det möjligt för förvaltaren att förstå hur väl ett projekt passar ihop med portföljens mål.

Mer information om styrkortsfrågor finns i [Skapa ett styrkort](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
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
            <p>Det möjliga värdet har lagts till <code>WIDGET </code>(Widget)</p>
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
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>I vissa fall går det att länka Workfront-objekt direkt till objekt i en extern programprodukt. Objektet ObjectIntegration representerar den här länken.</p>
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
      <td role="rowheader">Referensfält</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
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
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <p>Följande fält har tagits bort:</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Visa (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>Följande möjliga värden togs bort:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (layout med fyra kolumner)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Uppdateringar)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Uppdateringar)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Arbetar på)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Anpassade data)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Uppdatera anpassade data)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Statusuppdatering)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Statusuppdatering)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Statusuppdatering)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Statusuppdatering)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Detaljlista)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Detaljlistavsnitt)</p>
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
            <p>Det möjliga värdet har lagts till <code>documentVersionDownload </code>(enum.updatetypeenum.documents versiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Användare (ANVÄNDARE)

Ett User-objekt representerar en person med ett konto i Workfront som kan logga in och interagera med systemet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Referensfält</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Åtgärder</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
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
            <p><b>eventType</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Begärt att du korrekturläser ett dokument)</p>
              </li>
              <li>
                <p><code>DUV </code>(Gör att du kan visa ett dokument)</p>
              </li>
            </ul>
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
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>I vissa fall går det att länka Workfront-objekt direkt till objekt i en extern programprodukt. Objektet ObjectIntegration representerar den här länken.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

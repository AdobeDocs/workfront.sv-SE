---
content-type: api
navigation-topic: workfront-objects
title: När APIModel INTERNAL inte har stöd för fältprojekttid (OpTask)Kategori
description: När APIModel INTERNAL inte har stöd för fältprojekttid (OpTask)
author: Becky
feature: Workfront API
exl-id: 24c900ee-a8f1-458e-a18b-c098c6314e0c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---


# Kategori

FileClass: &quot;java.lang.IllegalArgumentException&quot;,\
meddelande: &quot;APIModel INTERNAL stöder inte fältprojekttid (OpTask)&quot;

<table style="table-layout:auto"> 
 <col width="100"> 
 <col width="100"> 
 <col width="100"> 
 <col width="240"> 
 <col width="200"> 
 <col width="100"> 
 <thead> 
  <tr> 
   <th>Namn</th> 
   <th>Etikett</th> 
   <th>Typ</th> 
   <th>Beskrivning</th> 
   <th>Möjliga värden</th> 
   <th>Flaggor</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}"><strong>ID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}">ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Identifying GUID&quot;}">Identifierar GUID</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;accessorIDs&quot;}"><strong>accessorID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;acessorIDs&quot;}">accessorIDs</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String Array&quot;}">Strängarray</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;List of People/Team IDs that can access this object&quot;}">Lista över personer-/team-ID:n som kan komma åt det här objektet</td> 
   <td> </td> 
   <td> <p><span class="dtRead">Skrivskyddad</span> </p> <p><span class="dtLazy">Lazy Read</span> </p> <p><span class="dtDyn">Dynamisk</span> </p> <p><span class="dtGrp">Inte grupperingsbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;catObjCode&quot;}"><strong>catObjCode</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">Typ</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type of Object the Custom form is related to&quot;}">Objekttyp som det anpassade formuläret är relaterat till</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;[{\&quot;label\&quot;:\&quot;Company\&quot;,\&quot;value\&quot;:\&quot;CMPY\&quot;},{\&quot;label\&quot;:\&quot;Task\&quot;,\&quot;value\&quot;:\&quot;TASK\&quot;},{\&quot;label\&quot;:\&quot;Project\&quot;,\&quot;value\&quot;:\&quot;PROJ\&quot;},{\&quot;label\&quot;:\&quot;Portfolio\&quot;,\&quot;value\&quot;:\&quot;PORT\&quot;},{\&quot;label\&quot;:\&quot;Program\&quot;,\&quot;value\&quot;:\&quot;PRGM\&quot;},{\&quot;label\&quot;:\&quot;User\&quot;,\&quot;value\&quot;:\&quot;USER\&quot;},{\&quot;label\&quot;:\&quot;Document\&quot;,\&quot;value\&quot;:\&quot;DOCU\&quot;},{\&quot;label\&quot;:\&quot;Issue\&quot;,\&quot;value\&quot;:\&quot;OPTASK\&quot;},{\&quot;label\&quot;:\&quot;Expense\&quot;,\&quot;value\&quot;:\&quot;EXPNS\&quot;},{\&quot;label\&quot;:\&quot;Iteration\&quot;,\&quot;value\&quot;:\&quot;ITRN\&quot;}]&quot;}"><code>[{"label":"Company","value":"CMPY"},{"label":"Task","value":"TASK"},{"label":"Project","value":"PROJ"},{"label":"Portfolio","value":"PORT"},{"label":"Program","value":"PRGM"},{"label":"User","value":"USER"},{"label":"Document","value":"DOCU"},{"label":"Issue","value":"OPTASK"},{"label":"Expense","value":"EXPNS"},{"label":"Iteration","value":"ITRN"}]</code> </td> 
   <td> <p><span class="dtEdit">Redigerbar</span> </p> <p><span class="dtReq">Obligatoriskt</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;customerID&quot;}"><strong>customerID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Customer ID&quot;}">Kund-ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the Customer&quot;}">Kundens ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Inte grupperingsbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;description&quot;}"><strong>description</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">Beskrivning</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">Beskrivning</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Redigerbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;enteredByID&quot;}"><strong>enteredByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Entered By ID&quot;}">Anges av ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the User that added the Custom Form&quot;}">ID för användaren som lade till det anpassade formuläret</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Inte grupperingsbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;extRefID&quot;}"><strong>extRefID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;External Reference ID&quot;}">Externt referens-ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;User Editable Field inteded to be used a link to an external object&quot;}">Redigerbart fält för användare avsett att användas som länk till ett externt objekt</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Redigerbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;groupID&quot;}"><strong>groupID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Group ID&quot;}">Grupp-ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the first group with access to the custom form&quot;}">ID för den första gruppen som har åtkomst till det anpassade formuläret</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Redigerbar</span> </p> <p><span class="dtGrp">Inte grupperingsbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;hasCalculatedFields&quot;}"><strong>hasCalculatedFields</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Has Calculated Fields&quot;}">Har beräknade fält</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Boolean&quot;}">Boolean</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Does the form have calculated fields associated with it?&quot;}">Har formuläret associerade beräkningsfält?</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Inte grupperingsbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdateDate&quot;}"><strong>lastUpdateDate</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Update Date&quot;}">Senaste uppdateringsdatum</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date/Time&quot;}">Datum/tid</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date of when the object was last modified&quot;}">Datum då objektet senast ändrades</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdatedByID&quot;}"><strong>lastUpdatedByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Updated By ID&quot;}">Senast uppdaterad av ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the last user to Update the object&quot;}">ID för den senaste användaren som ska uppdatera objektet</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Inte grupperingsbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;name&quot;}"><strong>name</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name&quot;}">Namn</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">Sträng</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name of the Object&quot;}">Objektets namn</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Redigerbar</span> </p> <p><span class="dtReq">Obligatoriskt</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Referenser

| Namn | Etikett | Typ | Typobjektkod | URL |
|---|---|---|---|---|
| Kund | kund | Kund | CUST | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Anges av | enteredBy | Användare | ANVÄNDARE | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Grupp | grupp | Grupp | GRUPP | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Senast uppdaterad av | lastUpdatedBy | Användare | ANVÄNDARE | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |


## Samlingar

| Namn | Etikett | Typ | Typobjektkod | URL |
|---|---|---|---|---|
| Åtkomstregler | accessRules | Åtkomstregel | ACSRUL | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Åtkomstregler för kategori | categoryAccessRules | Åtkomstregler för kategori | KATACR | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Överlappande kategoriregler | categoryCascadeRules | Överlappande regler för kataloger | CTCSRL | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Kategoriparametrar | categoryParameters | Kategoriparametrar | CTGYPA | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| Andra grupper | otherGroups | Grupp | GRUPP | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |


## Åtgärder

| Etikett | Namn | Argument |
|---|---|---|
| Tilldela kategorier | assignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| Tilldela kategori | assignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
| Ta bort tilldelning av kategorier | unassignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| Ta bort tilldelning av kategori | unassignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |

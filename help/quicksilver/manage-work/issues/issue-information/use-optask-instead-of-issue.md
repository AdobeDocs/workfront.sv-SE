---
product-area: projects
navigation-topic: issue-information
title: Använd"opTask" och"issue" när du refererar till problem
description: Namnet på ett problem visas som opTask i Adobe Workfront-databasen. Även om det finns tillfällen när du måste använda problemfältnamnet för att referera till problem, måste du för det mesta använda namnet på fältet opTask i stället för ett problem när du refererar till problem.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Använd&quot;opTask&quot; och&quot;issue&quot; när du refererar till problem

Namnet på ett problem visas som `opTask` i Adobe Workfront-databasen. Även om du behöver använda `issue` fältnamn för att hänvisa till problem, oftast måste du använda `opTask` fältnamn i stället för `issue` när du refererar till problem.

Mer information om hur objekt visas i Workfront-databasen finns i [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filnamn

Använd `opTask` fältnamn när du refererar till problem i följande sammanhang:

* När du skapar en anpassad textlägesrapport för problem och vill referera till problem i vyer, filter, grupperingar eller uppmaningar.

   Mer information om hur du använder textläge i en rapport finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* När du uppdaterar utskicksfält i en snabbstartsdatablad.

   Mer information om hur du importerar data i Workfront med Snabbstart finns i [Importera data till Adobe Workfront med en snabbstartsmall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` fältnamn

Använd `issue` fältnamn för att referera till problem i följande sammanhang:

* När du refererar till problem i en samling med textläge i en rapport.
* När du refererar till en problemsamling med Workfront API.

Mer information om rapportering om samlingar finns i [Referenssamlingar i en rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->

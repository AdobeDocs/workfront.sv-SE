---
product-area: projects
navigation-topic: issue-information
title: Använd"opTask" och"issue" när du refererar till problem
description: Namnet på ett problem visas som opTask i Adobe Workfront-databasen. Även om det finns tillfällen när du måste använda problemfältnamnet för att referera till problem, måste du för det mesta använda namnet på fältet opTask i stället för ett problem när du refererar till problem.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Använd&quot;opTask&quot; och&quot;issue&quot; när du refererar till problem

Namnet på ett problem visas som `opTask` i Adobe Workfront-databasen. Det finns tillfällen när du behöver använda fältnamnet `issue` för att referera till problem, men för det mesta måste du använda fältnamnet `opTask` i stället för `issue` för att referera till problem.

Mer information om hur objekt visas i Workfront-databasen finns i [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` fältnamn

Använd fältnamnet `opTask` när du refererar till problem i följande sammanhang:

* När du skapar en anpassad textlägesrapport för problem och vill referera till problem i vyer, filter, grupperingar eller uppmaningar.

  Mer information om hur du använder textläge i en rapport finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* När du uppdaterar utskicksfält i en snabbstartsdatablad.

  Mer information om hur du importerar data i Workfront med Snabbstart finns i [Importera data till Adobe Workfront med en Snabbstart-mall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` fältnamn

Använd fältnamnet `issue` för att referera till problem i följande sammanhang:

* När du refererar till problem i en samling med textläge i en rapport.
* När du refererar till en problemsamling med Workfront API.

Mer information om hur du rapporterar om samlingar finns i [Referenssamlingar i en rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->

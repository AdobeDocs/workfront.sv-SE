---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Hämta valutainformation för ett projekt när valutan är null
description: Hämta valutainformation för ett projekt när valutan är null
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Hämta valutainformation för ett projekt när valutan är null (inte tilldelad)

Projektobjektet med valutafältet kan hämtas med följande begäran:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Detta skulle returnera följande svarstext:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Om valutan inte är inställd för projektet innehåller det här svaret en valuta med värdet `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Om du behöver valutan för projektet (t.ex. för beräkningar) kan du hämta kundens standardvaluta:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

Svaret innehåller den valuta som användaren har angett som standard, vilket skulle användas i alla projekt för den kunden som inte har angett valutan:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```

---
product-area: documents
navigation-topic: approvals
title: Begränsat dokument och bevisbeslut för obetalda användare - översikt 
description: Handläggningsbeslut och dokumentbeslut är begränsade för alla obetalda Workfront-licenser. Begränsningar som återställs per användare och månad.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3e68fd8-723a-4e49-9cf1-823e36d04e55
source-git-commit: 4038180d69d4a8027f33b5bafd2104c7c6916b82
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 2%

---

# Begränsat dokument och bevisbeslut för obetalda användare - översikt

Handläggningsbeslut och dokumentbeslut är begränsade för alla obetalda Workfront-licenser för nya planer. När du tilldelas som godkännare för ett dokument eller ett korrektur måste du fatta ett beslut om att flytta gransknings- och godkännandeprocessen framåt.

Följande beslutstyper räknas in i månadsgränsen:

<table>
  <tr>

<td><strong>Godkännanden av äldre dokument</strong> 
   </td>
   <td><strong>Enhetliga godkännanden</strong> 
   </td>
   <td><strong>Korrektur för godkännanden</strong> 
   </td>
  </tr>
  <tr>
   <td>
   <ul>
   <li>Godkänn</li>
    <li>Godkänn med ändringar</li>
     <li>Avvisa</li>
   </ul>
   </td>
   <td>
      <ul>
   <li>Godkänn</li>
    <li>Godkänn med ändringar</li>
     <li>Behöver göras</li>
   </ul>
   </td>
   <td>
      <ul>
   <li>Godkänn</li>
    <li>Godkänn med ändringar</li>
     <li>Ändringar krävs</li>
   </ul>
   <p><strong>Obs!</strong>: Korrekturgodkännanden kan ha anpassade beslutsetiketter</p>
  </tr>
  </tr>
</table>



## Gränser

Begränsningar som återställs per användare och månad. Beslutsgränsen för respektive licens varierar beroende på vilken plan du har:

<table>
  <tr>
   <td> 
   </td>
   <td><strong>Extern</strong> 
   </td>
   <td><strong>Deltagare</strong> 
   </td>
   <td><strong>Ljus</strong> 
   </td>
   <td><strong>Standard</strong> 
   </td>
  </tr>
  <tr>
   <td><strong>Välj</strong> 
   </td>
   <td>3 
   </td>
   <td>3 
   </td>
   <td rowspan="3" >Obegränsad 
   </td>
   <td rowspan="3" >Obegränsad 
   </td>
  </tr>
  <tr>
   <td><strong>Prime</strong> 
   </td>
   <td>5 
   </td>
   <td>5 
   </td>
  </tr>
  <tr>
   <td><strong>Ultimate</strong> 
   </td>
   <td>7 
   </td>
   <td>7 
   </td>
  </tr>
</table>

Mer information finns i [Översikt över nya licenser](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

## Externa användare

Om en extern användare når sin beslutsgräns förlorar de inte åtkomsten till Workfront och kan fortfarande fatta beslut. Adobe Workfront kommer att utvärdera överskottet.

## Contributor-användare

När en användare med en Contributor-licens når sin beslutsgräns uppgraderas de automatiskt till Light-licensen med obegränsat antal korrektur- och dokumentbeslut. Mer information om Light-licensen finns i avsnittet [Ljusåtkomstnivå](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) i artikeln [Översikt över åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

>[!NOTE]
>
>Workfront-administratören får ett e-postmeddelande om uppgraderingen.


## Visa antalet beslut för en användare

Du kan visa antalet beslut för en användare i området Användare i Workfront. Mer information finns i [Visa antalet beslut för alla användare](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

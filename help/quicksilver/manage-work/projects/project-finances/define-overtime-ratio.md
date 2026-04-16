---
content-type: overview
product-area: projects
navigation-topic: financials
title: Definiera en övertidskvot
description: Du kan definiera en övertidskvot för en uppgift om du vill justera beräkningen av den planerade intäkten för aktivitetstilldelningarna.
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Definiera en övertidskvot

När en övertidskvot läggs till i en uppgift används den på alla tilldelningar i aktiviteten. Den multiplicerar alla planerade timmar för den uppgiften och påverkar beräkningarna av den planerade intäkten.

Övertidskvoten kan inte variera för tilldelningar inom samma uppgift. Om olika övertidsmultiplikatorer krävs måste du skapa separata underaktiviteter under en överordnad uppgift.

>[!NOTE]
>
>Det finns ingen validering som förhindrar att övertidsförhållandet läggs till i en aktivitet som inte är övertidsaktiviteter.

## Övertidsberäkning av planerad intäkt

Systemet bestämmer först faktureringstakten med hjälp av standardhierarkin för faktureringsfrekvens. Mer information finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Om det finns en övertidskvot för aktiviteten är beräkningen:
Planerad intäkt = faktureringsränta × övertidskvot × planerad timme

Om övertidskvoten är tom är beräkningen:
Planerad intäkt = faktureringsränta × planerad timme

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till uppgifter, projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td><p>Hantera behörigheter för en aktivitet som innehåller Redigera faktureringssatser</p>
     <p>Contribute eller högre behörighet för projektet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Aktivitetens intäktstyp måste vara Användare och Roll per timme. Mer information finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Fältet **Övertidsförhållande** måste vara aktiverat i layoutmallen.

1. Klicka på nedåtpilen under **Anpassa det som visas för användarna** i layoutmallen och klicka sedan på **Aktivitet**.
1. I avsnittet **Detaljer** markerar du fältet **Övertidsförhållande** i området **Ekonomi**.

   Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Definiera övertidsförhållandet för en uppgift

1. Gå till uppgiften som du vill redigera.

   Mer information finns i [Hantera aktivitetsfinanser i avsnittet Uppgiftsinformation](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Klicka på **Uppgiftsinformation** i den vänstra panelen.
1. I området **Ekonomi** anger du multiplikatorn för övertid i fältet **Övertidsförhållande**.
1. Klicka på **Spara ändringar**.

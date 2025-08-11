---
title: Fyll i en begäran automatiskt från tidigare data
content-type: reference
description: Du kan använda AI för att autofylla begärandefält med data från tidigare begäranden.
author: Becky
feature: Get Started with Workfront
source-git-commit: cf2ae77ed27b1dd30144f6de31bec474f53f1efb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Fyll i en begäran automatiskt från tidigare data

>[!NOTE]
>
>* Den här funktionen kommer att vara tillgänglig som en öppen betaversion enligt följande schema:
>
>   * Månadsutgåva: 11 september 2025
>   * kvartalsvis version: 16 oktober 2025

AI kan hjälpa dig att fylla i begärandefält automatiskt baserat på tidigare begäranden. Du kan godkänna eller avvisa dessa förslag innan du skickar in begäran.

Autofyll skriver inte över fält som du redan har fyllt i.

Användarna får inga förslag på data som de annars inte har tillgång till.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Medarbetare eller högre</p>
   eller
   <p>Aktuell: Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  </td> 
  </tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td><p>Åtkomst att lägga till begäranden i en begärandekö</p> <p>Visa eller högre behörigheter för den befintliga begäran</p> <p>Mer information om hur du konfigurerar en begärandekö finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Få förslag när du fyller i formulär

Autofyll kan föreslå fältvärden medan du fyller i formuläret. När du anger värden i begärandefälten jämför Workfront dessa värden med tidigare begäranden. Om det angivna värdet har en nära koppling till andra fältvärden i liknande sammanhang i tidigare begäranden föreslår Workfront dessa värden.

Om t.ex. en klinik alltid använder samma faktureringskod föreslår Workfront att faktureringskoden anges i rätt fält när det kliniska namnet anges.

Så här använder du förslag som baseras på tidigare begäranden:

1. Börja skapa en begäran.

   Instruktioner finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Börja fylla i fält.

   När du fyller i fält kan andra fält visa förslag.

1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** för fältet.

   ![Godkänn eller avvisa förslag](assets/accept-reject-suggestion.png)

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

   >[!NOTE]
   >
   >Alla ogranskade förslag godkänns automatiskt när du skickar in begäran.

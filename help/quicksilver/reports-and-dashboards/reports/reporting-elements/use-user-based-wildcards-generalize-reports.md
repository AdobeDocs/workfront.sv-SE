---
product-area: reporting
navigation-topic: reporting-elements
title: Generera rapporter med användarbaserade jokertecken
description: Du kan generera en rapport genom att använda jokertecken i stället för specifik information när du skapar vissa rapportelement.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Generera rapporter med användarbaserade jokertecken

<!-- Audited: 11/2024 -->

Du kan generera en rapport genom att använda jokertecken i stället för specifik information när du skapar vissa rapportelement. Om du till exempel vill skapa en rapport som visar de uppgifter som tilldelats en viss användare, kan du använda användarens namn i fältet Tilldelad till i filtret. Om du vill skapa en rapport som visar uppgifter som tilldelats den inloggade användaren, oavsett vem som är den användaren, kan du använda ett jokertecken som anger att när någon visar rapporten visas endast information som gäller användaren. På så sätt skapar du rapporten en gång, men eftersom du använder ett jokertecken i filtret skapas olika resultat varje gång någon annan läser den.

Du kan använda användarbaserade jokertecken när du skapar följande rapportelement:

* Filter
* Anpassade uppmaningar
* Vyer när regler för kolumner läggs till

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera rapportelement i en rapport</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
    <td> <p>Hantera behörigheter till en rapport för att redigera rapportelement i en rapport</p> <p>Hantera behörigheter till en vy eller ett filter för att redigera dem</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste skapa en rapport innan du kan lägga till en jokervariabel i den.

Instruktioner om hur du skapar rapporter finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Instruktioner

Infoga ett användarbaserat jokertecken i en rapport:

1. Gå till en rapport som du vill infoga ett användarbaserat jokertecken för.
1. Klicka på **Rapportera åtgärder** och sedan på **Redigera**.

1. Klicka på fliken **Filter**.
1. Klicka på **Lägg till en filterregel**.
1. Börja skriva namnet på fältet som du vill filtrera efter.\
   Du måste skriva fält som refererar till användarobjektet eller användarinformation.
1. Välj **Lika med** i listrutan för filtervariabeln.

   >[!TIP]
   >
   >Du måste alltid markera filtervariabeln **Lika med** när du arbetar med jokertecken i Adobe Workfront.

1. I rutan **Börja skriva namn ...** skriver du: `$$USER.ID` eller `$$USER.name` om du vill att rapporten ska visa information om användaren som loggar in, baserat på deras namn. Du kan infoga andra jokertecken som refererar till den inloggade användarens Group, Team, Company eller annan information.

   En fullständig lista över användarbaserade jokertecken finns i [Översikt över variabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicka på **Spara + Stäng**.

## Ytterligare information

Se även:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Översikt över filtervariabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Skapa eller redigera filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Lägg till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

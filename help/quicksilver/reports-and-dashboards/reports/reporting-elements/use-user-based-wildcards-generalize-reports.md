---
product-area: reporting
navigation-topic: reporting-elements
title: Generera rapporter med användarbaserade jokertecken
description: Du kan generera en rapport genom att använda jokertecken i stället för specifik information när du skapar vissa rapportelement.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Generera rapporter med användarbaserade jokertecken

Du kan generera en rapport genom att använda jokertecken i stället för specifik information när du skapar vissa rapportelement. Om du till exempel vill skapa en rapport som visar de uppgifter som tilldelats en viss användare, kan du använda användarens namn i fältet Tilldelad till i filtret. Om du vill skapa en rapport som visar uppgifter som tilldelats den inloggade användaren, oavsett vem som är den användaren, kan du använda ett jokertecken som anger att när någon visar rapporten visas endast information som gäller användaren. På så sätt skapar du rapporten en gång, men eftersom du använder ett jokertecken i filtret skapas olika resultat varje gång någon annan läser den.

Du kan använda användarbaserade jokertecken när du skapar följande rapportelement:

* Filter
* Anpassade uppmaningar
* Vyer när regler för kolumner läggs till

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera rapportelement i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera rapportelement i en rapport</p> <p>Hantera behörigheter till en vy eller ett filter för att redigera dem</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste skapa en rapport innan du kan lägga till en jokervariabel i den.

Instruktioner om hur du skapar rapporter finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Instruktioner

Infoga ett användarbaserat jokertecken i en rapport:

1. Gå till en rapport som du vill infoga ett användarbaserat jokertecken för.
1. Klicka **Rapportåtgärder** sedan **Redigera**.

1. Klicka på **Filter** -fliken.
1. Klicka **Lägg till en filterregel**.
1. Börja skriva namnet på fältet som du vill filtrera efter.\
   Du måste skriva fält som refererar till användarobjektet eller användarinformation.
1. Välj **Jämn** i listrutan för filtervariabeln.

   >[!TIP]
   >
   >Du måste alltid välja **Jämn** filtervariabeln när du arbetar med jokertecken i Adobe Workfront.

1. I **Börja skriva namn ...** ruta, typ: `$$USER.ID` eller `$$USER.name` om du vill att rapporten ska visa information om användaren som loggar in, baserat på deras namn. Du kan infoga andra jokertecken som refererar till den inloggade användarens Group, Team, Company eller annan information.

   En fullständig lista över användarbaserade jokertecken finns i [Översikt över filtervariabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Klicka **Spara + Stäng**.

## Ytterligare information

Se även:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Översikt över filtervariabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Skapa eller redigera filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

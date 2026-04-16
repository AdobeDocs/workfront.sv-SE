---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Ställ in valutakurser
description: Valutakurserna påverkar alla finansiella element i Workfront. Basvalutan är standardvalutan för alla projekt i hela systemet.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc71072107ce80f6cb9033fcb17fe4ac74d5af18
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Ställ in valutakurser

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Som Adobe Workfront-administratör kan du ställa in valutakurser i Workfront. Detta inkluderar följande:

* Ange standardvalutan för Workfront-systemet
* Uppdatera valutakurser i Workfront så att de matchar aktuella valutakurser
* Konfigurera valutakurser för flera valutor (på så sätt kan användarna välja en standardvaluta för enskilda projekt)

Valutakurserna påverkar alla finansiella element i Workfront. Basvalutan är standardvalutan för alla projekt och rapporter i hela systemet, såvida den inte åsidosätts för ett visst projekt eller en viss jobbroll. Den aktuella bas- eller standardvalutan anges med ikonen ![Standardvaluta](assets/default-icon.png) i listan. Du kan också välja att visa ekonomisk information i valutor som är tillgängliga i systemet och som skiljer sig från basvalutan eller från den för projektet när du visar dem i en rapport eller lista. Mer information finns i [Skapa rapporter om finansiella data med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Mer information om hur du åsidosätter basvalutan i Workfront för projekt och jobbroller finns i följande artiklar:

* [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

Hur du ställer in valutakurser påverkar om användare kan ändra valutakurser för ett visst projekt.

>[!IMPORTANT]
>
>Valutakurserna i Workfront är inte dynamiska. Värdet som du anger måste uppdateras när växelkursförändringar inträffar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Så här ställer du in valutakurser: Alla Workfront- eller arbetsflödespaket</p>
       <p>Så här använder du giltighetsdatum för valutakurser: Workflow Ultimate-paket</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ställ in valutakurser

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Exchange-priser**.
1. Klicka på **Lägg till valuta**.
1. I rutan **Lägg till valuta** börjar du skriva namnet på valutan och klickar sedan på den när den visas i listrutan.
1. I fältet **Växelkurs** anger du kursen för den valda valutan, jämfört med valutan som är angiven som basvaluta i systemet.
1. Klicka på **Lägg till** om du vill lägga till den nya valutan och valutakursen.
1. (Valfritt) Gör något av följande om du vill ändra basvalutan (standardvalutan):

   * Markera kryssrutan bredvid valutanamnet och välj **Gör standard** i åtgärdsfältet längst ned på skärmen.
   * Håll markören över valutanamnet och klicka på menyn **Mer** som visas. Välj sedan **Använd som standard**.

     Den nya standardvalutan uppdateras med ikonen ![Standardvaluta](assets/default-icon.png).

     >[!NOTE]
     >
     >Standardvalutan visas alltid först i listan, oavsett hur listan sorteras.

1. (Valfritt) Om du vill ta bort en valuta markerar du kryssrutan bredvid valutanamnet och väljer **Ta bort** i åtgärdsfältet längst ned på skärmen. Du kan inte ta bort standardvalutan.

## Ange giltighetsdatum för valutakurser

Giltiga datum för en valutas valutakurser konfigureras så att ett kursvärde slutar på ett visst datum och en annan kurs börjar. Växelkursen för rätt datum används sedan i finansiella beräkningar.

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Exchange-priser**.
1. Välj en valuta i listan och klicka på **Hantera datum** i åtgärdsfältet.
1. Välj **Slutdatum** för den aktuella valutakursen på dialogrutan **(valutanamn) för gällande valutakurser**.

   eller

   Välj ett **startdatum** för den nya valutakursen.

   Den första valutakursen har inget startdatum och den sista kursen har inget slutdatum. Vissa datum läggs till automatiskt. Om till exempel den första kursen inte har ett slutdatum och du lägger till en valutakurs med startdatumet 1 december 2025, läggs slutdatumet 30 november 2025 till den första kursen så att inga luckor uppstår.

   ![Dialogrutan Datum för gällande valutakurser](assets/euro-date-effective-rates.png)

1. Ange det nya **valutakursen**.
1. (Valfritt) Klicka på **Lägg till giltighetskurs** om du vill lägga till fler valutakurser med giltighetsdatum för den här valutan.
1. Klicka på **Spara**.

## Ge användarna möjlighet att ändra standardvalutan för ett projekt

Användarna kan ändra standardvalutan för ett projekt när följande villkor är uppfyllda:

* Användaren har en Standard- eller Plan-licens med administrativ åtkomst till Exchange Rates.

  Mer information finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mer än en valuta är aktiverad i Workfront.

Mer information om hur användare kan ändra standardvalutan för ett visst projekt finns i [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md).

## Gör det möjligt för användare att ändra standardvalutan för en jobbroll

Användarna kan ändra valutan för en jobbroll när följande villkor är uppfyllda:

* Användaren har en Standard- eller Plan-licens med administrativ åtkomst till jobbroller.

  Mer information finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mer än en valuta är aktiverad i Workfront.

Mer information om hur användare kan ändra standardvalutan för en viss jobbroll finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).




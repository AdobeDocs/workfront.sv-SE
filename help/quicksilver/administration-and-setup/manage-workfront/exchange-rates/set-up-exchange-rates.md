---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Som Adobe Workfront-administratör kan du ställa in valutakurser i Workfront.
description: Ställ in valutakurser
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
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

Valutakurserna påverkar alla finansiella element i Workfront. Basvaluta är standardvaluta för alla projekt i hela systemet, såvida den inte åsidosätts för ett visst projekt eller en viss jobbroll. Du kan också välja att visa ekonomisk information i valutor som är tillgängliga i systemet och som skiljer sig från basvalutan eller från den för projektet när du visar dem i en rapport eller lista. Mer information finns i [Skapa rapporter om finansiella data med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Mer information om hur du åsidosätter basvalutan i Workfront för projekt och jobbroller finns i följande artiklar:

* [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

Hur du ställer in valutakurser påverkar om användare kan ändra valutakurser för ett visst projekt.

>[!IMPORTANT]
>
>Växelkurserna i Workfront är inte dynamiska. värdet som du anger måste uppdateras när växelkursförändringar inträffar.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ställ in valutakurser

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Projektinställningar** > **Växelkurser.**

1. Klicka **Lägg till valuta.**
1. Börja skriva namnet på valutan och klicka sedan på den när den visas i listrutan.

1. I fältet Tillhandahålls anger du kursen för den valda valutan, beroende på vilken valuta som är angiven som basvaluta i systemet.
1. (Valfritt) Ange valutan som basvaluta (standardvaluta) för Workfront.

   Det här är den valuta som används som standard för alla projekt och rapporter i hela systemet.

1. Klicka **Spara** för att spara ändringarna.

## Gör det möjligt för användare att ändra standardvalutan för ett projekt

Användarna kan ändra standardvalutan för ett projekt när följande villkor är uppfyllda:

* Användaren har en planlicens med administrativ åtkomst till Exchange-priser.

   Mer information finns i [Ge användarna administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mer än en valuta är aktiverad i Workfront.

Mer information om hur användare kan ändra standardvalutan för ett visst projekt finns i [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md).

## Gör det möjligt för användare att ändra standardvalutan för en jobbroll

Användarna kan ändra valutan för en jobbroll när följande villkor är uppfyllda:

* Användaren har en planlicens med administrativ åtkomst till jobbroller.

   Mer information finns i [Ge användarna administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mer än en valuta är aktiverad i Workfront.

Mer information om hur användare kan ändra standardvalutan för en viss jobbroll finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

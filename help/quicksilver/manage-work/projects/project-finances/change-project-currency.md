---
product-area: projects
navigation-topic: financials
title: Ändra projektvalutan
description: Som projektledare kan du konfigurera ett projekt så att det använder en annan valuta än standardvalutan för ditt Adobe Workfront-system. På så sätt kan du visa ekonomisk information om projektet i den önskade valutan vid beräkning av arbetskostnader och intäkter.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Ändra projektvalutan

Som projektledare kan du konfigurera ett projekt så att det använder en annan valuta än standardvalutan för ditt Adobe Workfront-system. På så sätt kan du visa ekonomisk information om projektet i den önskade valutan vid beräkning av arbetskostnader och intäkter.

Innan du kan använda alternativa valutor enligt beskrivningen i det här avsnittet måste Workfront-administratören först aktivera och konfigurera flera valutor enligt beskrivningen i artikeln [Ställ in valutakurser](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du ändrar ett projekts valuta i Workfront

* Du kan inte ändra valutan för ett projekt om det finns någon ekonomisk information i projektet.
* Kurser används för arbetskraftskostnader. Intäktsberäkningar och används i framtiden för rapportering.
* Om du inte anger en annan valuta för ett projekt antar Workfront att projektets valuta är systemets standardvaluta. Mer information om standardvaluta på systemnivå finns i [Ställ in valutakurser](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Som standard har alla användare med full licens tillgång till valutor och valutakurser. Workfront-administratören måste bevilja ytterligare administrativ åtkomst för **Växelkurser** för att göra det möjligt för användare att ange specifika satser för projekt.
* Valutakurserna i Workfront är inte dynamiska. Värdet anges av en administratör och måste uppdateras när växelkursändringar inträffar.
* När du skapar en rapport som återspeglar valutan i ett projekt grupperas alla rapporter som standard efter projektets standardvaluta. Om du skapar en rapport med flera projekt som har olika valutakurser, återspeglar alla grupperingar som används i projektet standardväxelkursen på systemnivå. Mer information finns i artikeln [Skapa rapporter om finansiella data med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Konfigurera valutan för ett projekt

1. Gå till det projekt där du vill ändra standardvalutan.

   >[!TIP]
   >
   >Kontrollera att projektet inte redan har någon ekonomisk information. Se till exempel till att inga planerade eller faktiska kostnader är kopplade till projektet.

1. Klicka **Projektinformation** i den vänstra panelen och sedan gå till **Ekonomi** område.
1. Klicka **Lägg till** i **Valuta** och välj den valuta som du vill använda som standardvaluta för projektet. Alla valutor som din Workfront-administratör anger för din Workfront-instans visas.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Villkorligt) Om du väljer en annan valuta än standardvalutan som är inställd för ditt Workfront-system anger du kursen för den valda valutan, i förhållande till den valuta som är inställd som basvaluta i systemet.
1. Klicka **Spara ändringar**.

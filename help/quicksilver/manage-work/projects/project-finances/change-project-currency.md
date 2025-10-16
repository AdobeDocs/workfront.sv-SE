---
product-area: projects
navigation-topic: financials
title: Ändra projektvaluta
description: Som projektledare kan du konfigurera ett projekt så att det använder en annan valuta än standardvalutan för ditt Adobe Workfront-system. På så sätt kan du visa ekonomisk information om projektet i den önskade valutan vid beräkning av arbetskostnader och intäkter.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Ändra projektvalutan

Som projektledare kan du konfigurera ett projekt så att det använder en annan valuta än standardvalutan för ditt Adobe Workfront-system. På så sätt kan du visa ekonomisk information om projektet i den önskade valutan vid beräkning av arbetskostnader och intäkter.

Innan du kan använda alternativa valutor enligt beskrivningen i det här avsnittet måste Workfront-administratören först aktivera och konfigurera flera valutor enligt beskrivningen i artikeln [Konfigurera valutakurser](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för projektet</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du ändrar ett projekts valuta i Workfront

* Du kan inte ändra valutan för ett projekt om det finns någon ekonomisk information i projektet.
* Kurser används för arbetskraftskostnader; intäktsberäkningar och används i framtiden för rapportering.
* Om du inte anger en annan valuta för ett projekt antar Workfront att projektets valuta är systemets standardvaluta. Mer information om standardvaluta på systemnivå finns i [Konfigurera valutakurser](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Som standard har alla användare med full licens tillgång till valutor och valutakurser. Workfront-administratören måste bevilja ytterligare administrativ åtkomst för **valutakurser** för att användare ska kunna ange specifika priser för projekt.
* Valutakurserna i Workfront är inte dynamiska. Värdet anges av en administratör och måste uppdateras när växelkursändringar inträffar.
* När du skapar en rapport som återspeglar valutan i ett projekt grupperas alla rapporter som standard efter projektets standardvaluta. Om du skapar en rapport med flera projekt som har olika valutakurser, återspeglar alla grupperingar som används i projektet standardväxelkursen på systemnivå. Mer information finns i artikeln [Skapa rapporter om finansiella data med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Konfigurera valutan för ett projekt

1. Gå till det projekt där du vill ändra standardvalutan.

   >[!TIP]
   >
   >Kontrollera att projektet inte redan har någon ekonomisk information. Se till exempel till att inga planerade eller faktiska kostnader är kopplade till projektet.

1. Klicka på **Projektinformation** i den vänstra panelen och gå sedan till området **Ekonomi**.
1. Klicka på **Lägg till** i fältet **Valuta** och välj den valuta som du vill använda som standardvaluta för projektet. Alla valutor som din Workfront-administratör anger för din Workfront-instans visas.

   ![Valuta i projekt](assets/currency-on-project-expanded-nwe.png)

1. (Villkorligt) Om du väljer en annan valuta än standardvalutan som är inställd för ditt Workfront-system anger du kursen för den valda valutan, i förhållande till den valuta som är inställd som basvaluta i systemet.
1. Klicka på **Spara ändringar**.

---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Dela arbetsbelastningsutjämnaren med en länk
description: Du kan dela belastningsutjämnaren med andra användare som kanske inte har resursområdet tillgängligt. Mer information om hur du använder arbetsbelastningsutjämnaren finns i Navigera i Arbetsbelastningsutjämnaren.
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Dela arbetsbelastningsutjämnaren med en länk

Du kan dela belastningsutjämnaren med andra användare som kanske inte har resursområdet tillgängligt. Mer information om hur du använder arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

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
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera när du använder belastningsutjämnaren för arbetsbelastning i resursområdet:</br>
       Arbeta, när du använder belastningsutjämnaren för ett team eller projekt</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomsten till följande:</p> 
    <ul> 
     <li>Resurshantering</li> 
     <li>Projekt</li> 
     <li>Uppgifter</li> 
     <li>Problem</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Visa eller högre behörigheter för projekt, uppgifter och ärenden</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Information som ingår i arbetsbelastningsutjämnaren när den visas från en delad länk

När du delar en länk till belastningsutjämnaren för arbetsbelastning med andra användare inkluderas följande information med den delade länken:

* Den tilldelade arbetsytan i Utjämning av arbetsbelastning.
* Projekt, uppgift, användarinformation. Detta inkluderar information om användarallokering.
* Informationen visas enligt det valda filtret.

  >[!IMPORTANT]
  >
  >Om du tar bort filtren när du har delat länken får användarna som visar arbetsbelastningsutjämnaren från länken en varning om att filtren har tagits bort. De visar alla användare på den tilldelade arbetsytan. Det här är standardvyn för Utjämning av arbetsbelastning.

* Antalet veckor som tidigare valts.

Följande alternativ är tillgängliga för användare som visar arbetsbelastningsutjämnaren från en delad länk för att uppdatera sig själva:

* Följande tidslinjeval:

   * Idag
   * Bakåt- och framåtikoner
   * Kalenderval

* Ikonerna Dag, Vecka och Månad
* Ikonen Inställningar
* Ikonen Visa allokeringar

  Mer information om hur du använder dessa alternativ finns i [Navigera i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Ikonen Visa rollallokeringar

  Det här är bara tillgängligt för arbetsbelastningsutjämnaren för ett projekt.

Användaren som tar emot den delade länken kan inte göra följande i arbetsbelastningsutjämnaren via den här länken:

* Tilldela arbetsobjekt till användare
* Hantera användarallokeringar
* Skapa nya eller uppdatera filter som ursprungligen tillämpades

## Åtkomst krävs för att visa information i arbetsbelastningsutjämnaren från en delad länk

Du behöver följande åtkomst för att visa information i arbetsbelastningsutjämnaren från en delad länk:

* En giltig Adobe Workfront-licens och du måste vara inloggad på Workfront.
* Visa minst åtkomst till resurshantering på din åtkomstnivå. Information om hur du beviljar åtkomst till resurshantering finns i [Bevilja åtkomst till resurshantering](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Visa behörigheter för de projekt, uppgifter, utgåvor och användare som visas i Utjämning av arbetsbelastning.

## Dela arbetsbelastningsutjämnaren med andra användare från en länk

1. Gå till Utjämning av arbetsbelastning

   Mer information om hur du får åtkomst till arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Valfritt) Gör något av följande:

   * Uppdatera valet av tidsperiod.
   * Klicka på **Dag, Vecka** eller **Månad** om du vill visa information om dag, vecka eller månad.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Använd filter på områdena Ej tilldelat och Tilldelat arbete.

     Mer information om filtrering av information i arbetsbelastningsutjämnaren finns i [Filtrera information i Arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Klicka på **länkikonen** ![](assets/wb-shearable-link-icon-small.png).

   Då läggs länken till i Urklipp.

1. Gör något av följande om du vill dela länken med andra:

   * Klistra in den i ett e-postmeddelande, chattmeddelande eller något annat program och dela den med andra användare.
   * Lägg till den i ett anpassat avsnitt som en extern sida, lägg till det anpassade avsnittet i en användarprofil eller i en layoutmall och dela sedan layoutmallen med användare, team, jobbroller eller grupper.

     Mer information om hur du skapar en extern sida finns i [Bädda in en extern webbsida i en kontrollpanel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Mer information om hur du lägger till anpassade avsnitt i en layoutmall finns i [Anpassa den vänstra panelen med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >När du lägger till belastningsutjämnaren för arbetsbelastning i ett objekts anpassade avsnitt filtreras inte informationen i belastningsutjämnaren av objektet. I Utjämning av arbetsbelastning visas den information som filtrerats av de filter som ursprungligen tillämpades.

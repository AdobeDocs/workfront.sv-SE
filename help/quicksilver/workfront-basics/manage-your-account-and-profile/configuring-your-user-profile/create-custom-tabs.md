---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Skapa anpassade avsnitt
description: Den information du ser i  [!DNL Workfront] webbprogrammet visas ofta som standard i avsnitten i den vänstra panelen. Varje avsnitt innehåller olika information om ett  [!DNL Workfront] område eller objekt.
author: Becky
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: ccaf637601c53e5d92dd3357fb07e84b5fd69166
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Skapa anpassade avsnitt

## [!DNL Adobe Workfront] avsnitt

Informationen som du ser i webbprogrammet [!DNL Workfront] visas ofta som standard i de vänstra panelavsnitten. Varje avsnitt innehåller olika information om ett [!DNL Workfront]-område eller objekt.\
Mer information om standardområdena för [!DNL Workfront] finns i artikeln [Om standardlayouten [!DNL Adobe Workfront] ](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Förutom de avsnitt som medföljer [!DNL Workfront] som standard kan du lägga till en instrumentpanel där du kan visa information som är relevant för ditt arbetsflöde. Du kan inte lägga till en kontrollpanel till alla områden och objekt.

I följande tabell visas alla [!DNL Workfront] områden och objekt som innehåller avsnitt på den vänstra panelen och vilka av dem som kan anpassas:

| **[!DNL Workfront]område eller objekt** | **Standardsystemavsnitt** | **Anpassade avsnitt** |
|---|---|---|
| [!UICONTROL Projects] område | ✓ | ✓ |
| [!UICONTROL Team] | ✓ |   |
| [!UICONTROL Requests] område | ✓ |   |
| [!UICONTROL Timesheets] område | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Program] | ✓ | ✓ |
| [!UICONTROL Project] | ✓ | ✓ |
| [!UICONTROL Task] | ✓ |  ✓ |
| [!UICONTROL Issue] |  ✓ |  ✓ |
| [!UICONTROL User] |  ✓ |  ✓ |
| [!UICONTROL Document] |  ✓ |  ✓ |
| [!UICONTROL Resourcing] område | ✓ | ✓ |

{style="table-layout:auto"}

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td>[!UICONTROL Reviewer] eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Visa åtkomst till objekttypen</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan eller licenstyp du har.

## Lägg till en instrumentpanel i den vänstra panelen för ett [!DNL Workfront]-objekt eller -område

Innan du kan lägga till en kontrollpanel måste du skapa kontrollpanelen med all information som du vill visa på den. Du kan också skapa en extern sida.\
Mer information om hur du skapar kontrollpaneler finns i artikeln [Skapa en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Mer information om hur du skapar externa sidor finns i artikeln [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

När du har skapat kontrollpanelen eller den externa sidan kan du lägga till dem i den vänstra panelen.

1. Gå till ett av [!DNL Workfront]-områdena eller objekten där du kan lägga till ett anpassat avsnitt i den vänstra panelen.\
   eller
1. Gå till ett objekt där du kan lägga till [!UICONTROL dashboard] i den vänstra panelen.\
   Mer information om vilka områden och objekt du kan lägga till anpassade avsnitt i finns i [[!DNL Adobe Workfront] avsnitt](#adobe-workfront-sections).
1. Klicka på **[!UICONTROL Add dashboard]** i den vänstra panelen.
1. Ange ett namn för instrumentpanelen i fältet **[!UICONTROL Quick link name]**. Detta är bara synligt för dig.
1. Börja skriva namnet på en befintlig instrumentpanel eller extern sida i fältet **[!UICONTROL Choose a dashboard]** och välj sedan instrumentpanelen när den visas i listan.
1. Klicka på **[!UICONTROL Add]**.
1. (Valfritt) Dra och släpp avsnitten i den ordning som du vill visa dem.

   Det övre avsnittet är standardavsnittet för sidan.

   De avsnitt som du har skapat för enskilda objekt visas när du öppnar alla objekt av samma typ och är bara tillgängliga för dig.

## Visa instrumentpaneler på den vänstra panelen med objekt

Mer information om hur du lägger till en kontrollpanel under ett objekt finns i avsnittet [[!UICONTROL Add a dashboard] på den vänstra panelen i ett Workfront-objekt eller -område ](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) i den här artikeln.

När du lägger till en kontrollpanel i ett anpassat avsnitt under ett objekt fungerar objektet som ett filter för kontrollpanelen. Om du till exempel lägger till en uppgiftsrapport på en kontrollpanel och lägger till kontrollpanelen i ett projekt, visas bara uppgifter i det anpassade avsnittet som innehåller kontrollpanelen i projektet i det projekt som du visar.

Följande objekt filtreras efter det objekt som de visas under, om objektet är högre i hierarkin än dem:

* Projekt
* Uppgift
* Problem
* Godkännandeprocess
* Obs
* Dokument

Mer information om objekts hierarki och inbördes beroende finns i avsnittet [Objektens inbördes beroende och hierarki](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Anpassa den vänstra panelen i en layoutmall

När du lägger till instrumentpaneler i din [!DNL Workfront]-instans är de bara synliga för dig.

Du kan anpassa avsnitten i [!DNL Workfront] och dela den nya layouten med flera användare i en layoutmall. Endast system- eller gruppadministratörer kan dela dem med andra användare i en layoutmall. Mer information om hur du anpassar den vänstra panelen med en layoutmall finns i [Anpassa den vänstra panelen med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

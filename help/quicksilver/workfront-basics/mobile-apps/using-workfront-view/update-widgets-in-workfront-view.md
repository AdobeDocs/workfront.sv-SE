---
product-previous: mobile
navigation-topic: use-workfront-view
title: Uppdatera widgetar i projektinformationsvyn
description: Du kan visa ytterligare information om [!UICONTROL project] när du har öppnat den från projektlistan genom att lägga till widgetar på [!UICONTROL Project Details]-skärmen. Varje användare kan anpassa sina egna widgetar.
author: Nolan
feature: Get Started with Workfront
exl-id: 593dc4a2-20aa-44d3-b819-1d4b160095ed
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Uppdatera widgetar i vyn [!UICONTROL Project Details]

Du kan visa ytterligare information om [!UICONTROL project] när du har öppnat den från projektlistan genom att lägga till widgetar på [!UICONTROL Project Details]-skärmen. Varje användare kan anpassa sina egna widgetar.

## Åtkomstkrav

Du måste ha följande åtkomst i [!DNL Workfront] för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Uppdatera widgetarna i vyn [!UICONTROL Project Details]

1. Gå till ett projekt från startsidan för [!DNL Adobe Workfront View] genom att trycka på dess namn.
1. Tryck på fliken längst ned i mitten av skärmen.\
   Området [!UICONTROL widget] visas.\
   Bläddra genom widgetarna genom att svepa från vänster till höger.\
   ![Widgets](assets/screen-shot-2013-009-11-at-8.25.01-am-350x262.png)

1. Dra och släpp en widget för att anpassa layouten på projektsidan.\
   Du kan visa upp till fyra widgetar samtidigt.\
   Du kan ordna om widgetarna genom att dra dem och släppa dem på en annan plats.\
   Widgetordningen sparas när du navigerar mellan projekt.

1. Välj bland följande widgetar:

   * **[!UICONTROL Task Condition]**: Visar alla aktiviteter i projektet efter [!UICONTROL Condition] i ett cirkeldiagram.
   * **[!UICONTROL Issues]**: Visar tidslinjen för alla utgåvor i ett linjediagram. Antalet öppna problem visas inom parentes.
   * **[!UICONTROL Hours]**: Visar [!UICONTROL Actual] och [!UICONTROL Planned Hours] för aktiviteterna i projektet i ett kombinerat linjediagram.
   * **[!UICONTROL Issue]** [!UICONTROL Status]: Visar alla problem efter status i ett cirkeldiagram.
   * **[!UICONTROL Updates]**: Visar alla uppdateringar och kommentarer i projektet.
   * **[!UICONTROL Costs]**: Visar [!UICONTROL Actual] och [!UICONTROL Planned Cost] för projektet i ett kombinerat stapeldiagram.
   * **[!UICONTROL Revenue]**: Visar [!UICONTROL Actual] och [!UICONTROL Planned Revenue] för projektet i ett kombinerat stapeldiagram.
   * **[!UICONTROL Task Progress]**: Visar alla aktiviteter i projektet efter [!UICONTROL Progress Status] i ett cirkeldiagram.
   * **[!UICONTROL Upcoming Tasks]**: Visar upp till 6 kommande aktiviteter. Widgeten sorterar projektuppgifterna i följande ordning:

      * först, av [!UICONTROL Estimated Due Date]
      * sekund, av [!UICONTROL Work Breakdown Structure]

     Här visas de två senaste slutförda uppgifterna (om det är tillämpligt) och de fyra nästa uppgifterna. För att förstå vilka uppgifter som ska visas i mobilappen [!DNL Workfront] View kan du skapa en aktivitetsrapport för det projekt som du visar och sortera den efter beräknat förfallodatum och sedan efter [!DNL Workfront] Brytningsstruktur. De första sex uppgifterna är de uppgifter som listas i Workfront View-mobilappen i [!UICONTROL Upcoming]-widgeten Åtgärder.

   * **[!UICONTROL Remaining Tasks]**: Visar de ofullständiga uppgifterna i ett linjediagram.
   * **[!UICONTROL Documents]**: Visar en lista över dokument som är kopplade till projektet.\

     Du kan öppna följande dokumentformat med [!DNL Workfront View]:

      * alla textfiler
      * PDF
      * bildfiler (.jpg, .jpeg, .png osv.)
      * .xls
   * **[!UICONTROL Details]**: Visar följande information om projektet:

      * Projektnamn
      * Namnet på den som skapat projektet
      * Projektstatus
      * Projektgrupp
      * Projektschema
   * **[!UICONTROL Team]**: Visar namnen på de användare som ingår i projektgruppen.\

     Mer information om projektteam finns i [Översikt över projektteamet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

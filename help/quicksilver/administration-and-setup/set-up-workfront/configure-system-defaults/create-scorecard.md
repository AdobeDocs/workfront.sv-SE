---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa ett styrkort
description: Ett styrkort mäter hur väl ett projekt överensstämmer med de tidigare fastställda kriterierna för en portfölj. Ett styrkort avspeglar ofta en organisations uppdrag, värderingar och strategiska mål. Chefer för Portfolio definierar vanligtvis styrkortsfrågor och svar för att säkerställa att de är meningsfulla och värdefulla vid projektprioritering och urval. An [!DNL Adobe Workfront] administratören bygger styrkort baserat på rekommendationer från portföljförvaltare.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Skapa ett styrkort

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ett styrkort mäter hur väl ett projekt överensstämmer med de tidigare fastställda kriterierna för en portfölj. Ett styrkort avspeglar ofta organisationens uppdrag, värderingar och strategiska mål.

Portfolio chefer definierar vanligtvis styrkortsfrågor och svar för att säkerställa att de är meningsfulla och värdefulla vid projektprioritering och urval. An [!DNL Adobe Workfront] administratören bygger styrkort baserat på rekommendationer från portföljförvaltare.

De frågor och svar som väljs ut för ett styrkort måste vara kvantifierbara för att det ska gå att jämföra olika projekt.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Aktuell: [!UICONTROL Business] eller högre</p> 
   eller
   <p>Nytt: [!UICONTROL Prime] eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   eller
   <p>Nytt: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

## Skapa ett styrkort

{{step-1-to-setup}}

1. Klicka **[!UICONTROL Scorecards]** och sedan klicka **[!UICONTROL New Scorecard]** för att starta styrkortsverktyget och skapa ett styrkort.

1. Ange en **[!UICONTROL Scorecard Name]** och **[!UICONTROL Description]**.

   Namnet visas när du associerar styrkortet med projektet. Beskrivningen visas bredvid styrkortets namn i styrkortslistan.

1. Klicka på **[!UICONTROL Add Question]** nedrullningsbar meny där [!UICONTROL scorecard question] och sedan ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Question]</td> 
      <td>Skriv frågan som du vill ta med i styrkortet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Ange maximalt antal poäng för den här frågan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Negative Points]</td> 
      <td>Välj det här alternativet om du vill ange att [!DNL Workfront] ska subtrahera från de totala möjliga poängen. Negativa poäng kan inte läggas till i maximalt möjliga poäng i ett styrkort.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Välj <strong>[!UICONTROL Value(0-100)]</strong> om du vill visa ett numeriskt fält i styrkortet där användarna kan ange ett värde mellan 0 och 100.<p>Eller markera <strong>[!UICONTROL Drop Down]</strong> eller <strong>[!UICONTROL Radio Buttons]</strong> för att skapa ett svar som användare kan ange med den kontrollen. Klicka <strong>[!UICONTROL Add Answer]</strong>och skriver sedan <strong>[!UICONTROL Value]</strong> i procentenheter för detta svar, om det är uppfyllt. Om du väljer 100 % kommer antalet poäng som tilldelas för den här frågan att uppnås helt. Om du vill ange att svaret bara innehåller en del av det totala poängbeloppet som tilldelats den här frågan väljer du ett lägre procentvärde. Om din fråga till exempel värderas till 10 poäng och du vill att svaret ska innehålla 5 av dessa punkter, väljer du 50 % som värde.</p>
      <p>Välj <strong>[!UICONTROL Default]</strong> om du vill ange att det här svaret är standardsvaret.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Klicka **[!UICONTROL Add Question]** om du vill lägga till fler frågor och svar i styrkortet följer du samma steg.

   >[!NOTE]
   >
   >Du kan ändra ordningen på frågorna i styrkortet genom att dra och släppa frågorna i rätt ordning.

1. Klicka **[!UICONTROL Save]** när du är klar med att ange all information.

   Detta skapar styrkortet och projektledare kan nu bifoga det till projektärendet.

## Tillämpa ett styrkort på ett projekt

En användare med [!UICONTROL manage] behörigheter för ett projekt kan tillämpa ett styrkort på ett projekt efter att styrkortet har skapats av [!DNL Workfront] administratör.

Ett styrkort läggs till i ett projekt som en del av skapandet av ett affärsärende för projektet. Mer information om hur du lägger till ett styrkort i ett projekt finns i [Tillämpa ett styrkort på ett projekt och generera ett justeringsresultat](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Mer information om projektbehörigheter finns i [Dela ett projekt i [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

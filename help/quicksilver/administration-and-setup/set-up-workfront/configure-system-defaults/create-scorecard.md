---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa ett styrkort
description: Ett styrkort mäter hur väl ett projekt överensstämmer med de tidigare fastställda kriterierna för en portfölj. Ett styrkort avspeglar ofta en organisations uppdrag, värderingar och strategiska mål. Chefer för Portfolio definierar vanligtvis styrkortsfrågor och svar för att säkerställa att de är meningsfulla och värdefulla vid projektprioritering och urval. En  [!DNL Adobe Workfront] administratör bygger styrkorten baserat på rekommendationer från portföljförvaltare.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Skapa ett styrkort

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ett styrkort mäter hur väl ett projekt överensstämmer med de tidigare fastställda kriterierna för en portfölj. Ett styrkort avspeglar ofta organisationens uppdrag, värderingar och strategiska mål.

Portfolio chefer definierar vanligtvis styrkortsfrågor och svar för att säkerställa att de är meningsfulla och värdefulla vid projektprioritering och urval. En [!DNL Adobe Workfront]-administratör skapar styrkorten baserat på rekommendationer från portföljförvaltare.

De frågor och svar som väljs ut för ett styrkort måste vara kvantifierbara för att det ska gå att jämföra olika projekt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Aktuell: [!UICONTROL Business] eller högre</p> 
   eller
   <p>Nytt: [!UICONTROL Prime] eller senare</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   eller
   <p>Nytt: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett styrkort

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Scorecards]** och sedan på **[!UICONTROL New Scorecard]** för att starta styrkortsverktyget och skapa ett styrkort.

1. Ange **[!UICONTROL Scorecard Name]** och **[!UICONTROL Description]**.

   Namnet visas när du associerar styrkortet med projektet. Beskrivningen visas bredvid styrkortets namn i styrkortslistan.

1. Klicka på listrutan **[!UICONTROL Add Question]** för att öppna avsnittet [!UICONTROL scorecard question] och ange sedan följande information för din fråga:

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
      <td>Välj det här alternativet om du vill ange att [!DNL Workfront] ska subtrahera från det totala antalet möjliga punkter. Negativa poäng kan inte läggas till i maximalt möjliga poäng i ett styrkort.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Välj <strong>[!UICONTROL Value(0-100)]</strong> om du vill visa ett numeriskt fält i styrkortet där användare kan ange ett värde mellan 0 och 100.<p>Du kan också välja <strong>[!UICONTROL Drop Down]</strong> eller <strong>[!UICONTROL Radio Buttons]</strong> för att skapa ett svar som användare kan ange med den kontrollen. Klicka på <strong>[!UICONTROL Add Answer]</strong> och skriv sedan <strong>[!UICONTROL Value]</strong> i procentenheter för det här svaret om det är uppfyllt. Om du väljer 100 % kommer antalet poäng som tilldelas för den här frågan att uppnås helt. Om du vill ange att svaret bara innehåller en del av det totala poängbeloppet som tilldelats den här frågan väljer du ett lägre procentvärde. Om din fråga till exempel värderas till 10 poäng och du vill att svaret ska innehålla 5 av dessa punkter, väljer du 50 % som värde.</p>
      <p>Välj <strong>[!UICONTROL Default]</strong> om du vill ange att det här svaret är standardsvaret.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Add Question]** om du vill lägga till fler frågor och svar i styrkortet, så följer du samma steg.

   >[!NOTE]
   >
   >Du kan ändra ordningen på frågorna i styrkortet genom att dra och släppa frågorna i rätt ordning.

1. Klicka på **[!UICONTROL Save]** när du är klar med att ange all information.

   Detta skapar styrkortet och projektledare kan nu bifoga det till projektärendet.

## Tillämpa ett styrkort på ett projekt

En användare med [!UICONTROL manage] behörigheter för ett projekt kan använda ett styrkort för ett projekt efter att styrkortet har skapats av administratören för [!DNL Workfront].

Ett styrkort läggs till i ett projekt som en del av skapandet av ett affärsärende för projektet. Mer information om hur du lägger till ett styrkort i ett projekt finns i [Använda ett styrkort i ett projekt och generera ett justeringsresultat](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Mer information om projektbehörigheter finns i [Dela ett projekt i [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

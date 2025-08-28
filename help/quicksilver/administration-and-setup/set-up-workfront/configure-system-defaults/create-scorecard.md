---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa ett styrkort
description: Ett styrkort mäter hur väl ett projekt överensstämmer med de tidigare fastställda kriterierna för en portfölj. Ett styrkort återspeglar ofta organisationens uppdrag, värderingar och strategiska mål.Portfolio-chefer definierar vanligtvis styrkortsfrågor och svar för att säkerställa att de är meningsfulla och värdefulla vid projektprioritering och urval. En  [!DNL Adobe Workfront] administratör bygger styrkorten baserat på rekommendationer från portföljförvaltare.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 7f719c903ad4079470a6dbd046dce445ba227a5b
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Skapa ett styrkort

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

Ett styrkort mäter hur väl ett projekt överensstämmer med de tidigare fastställda kriterierna för en portfölj. Ett styrkort avspeglar ofta organisationens uppdrag, värderingar och strategiska mål.

Som portföljförvaltare kan du definiera styrkortsfrågor och svar för att säkerställa att de är meningsfulla och värdefulla vid projektprioritering och urval.

Som [!DNL Adobe Workfront]-administratör kan du skapa styrkort baserat på rekommendationer från portföljförvaltare.

De frågor och svar som väljs ut för ett styrkort måste vara kvantifierbara för att det ska gå att jämföra olika projekt.

Du kan skapa ett styrkort på följande sätt:

* Från början
* Genom att kopiera en befintlig

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Nytt: Ultimate</p>
   <p>Aktuell: [!UICONTROL Business] eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader"><p>Åtkomstnivå</p></td> 
   <td><p>Systemadministratör</p>
   </td> 
  </tr>
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett styrkort från grunden

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Scorecards]** och sedan på **[!UICONTROL New Scorecard]**.

   Rutan **Nytt styrkort** öppnas.

   ![Ny styrkortsruta](assets/new-scorecard-350x173.png)

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

1. Klicka på **[!UICONTROL Save]**.

   Detta skapar styrkortet och projektledare kan nu bifoga det till projektärendet.

## Kopiera ett befintligt styrkort

Du kan skapa ett styrkort genom att kopiera och redigera ett befintligt.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Scorecards]** i den vänstra panelen.
1. Markera ett styrkort i listan och klicka sedan på ikonen **Kopiera** ![Kopiera styrkort](assets/copy-scorecard-icon.png) högst upp i styrkortslistan.

   Rutan **Kopiera styrkort** öppnas.

   ![Kopiera styrkortsruta](assets/copy-scorecard-box.png)

1. Ange följande information:

   * **Styrkort**: Uppdatera namnet på styrkortet.  Som standard uppdateras namnet automatiskt enligt följande format:

     `Original scorecard name (Copy)`
   * **Beskrivning**: Ange ytterligare information om styrkortet.
1. Klicka på **Spara**.

   Detta skapar ett nytt styrkort med samma information som det ursprungliga. Projektledare kan nu bifoga den till sina projekt.

## Tillämpa ett styrkort på ett projekt

En användare med [!UICONTROL manage] behörigheter för ett projekt kan använda ett styrkort för ett projekt efter att styrkortet har skapats av administratören för [!DNL Workfront].

Ett styrkort läggs till i ett projekt som en del av skapandet av ett affärsärende för projektet. Mer information om hur du lägger till ett styrkort i ett projekt finns i [Använda ett styrkort i ett projekt och generera ett justeringsresultat](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Mer information om projektbehörigheter finns i [Dela ett projekt i [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).



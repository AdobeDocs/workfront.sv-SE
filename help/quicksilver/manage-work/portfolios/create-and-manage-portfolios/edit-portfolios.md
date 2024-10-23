---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Redigera Portfolio
description: Du kan redigera information om portföljer som du har skapat eller som andra användare har skapat om de har delat dem med dig. I den här artikeln beskrivs hur du kan söka efter, söka efter och redigera en portfölj, om du har behörighet att göra det.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 0a2e18c3-1722-4fc6-8442-19e80eca9d47
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Redigera portföljer

Du kan redigera information om portföljer som du har skapat eller som andra användare har skapat om de har delat dem med dig.

Du kan redigera en [!UICONTROL portfolio] på portföljsidan eller redigera portföljer i en lista.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licenser*</td> 
   <td> <p>Nytt: Standard</p>
   <p>Aktuell: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] behörighet till Portfolio</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en portfölj</p>
   <p> Hantera behörigheter för projekten i portföljen för att lägga till eller ta bort dem från portföljen</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera portföljer

{{step1-to-portfolios}}

1. Klicka på namnet på en portfölj för att öppna den.
1. (Valfritt) Om du vill redigera begränsad information om portföljen klickar du på **[!UICONTROL Portfolio Details]** i den vänstra panelen.

   ![](assets/portfolio-details-tab-nwe-350x163.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the note below will also be true for Edit Portfolio box)</p>
   -->

   >[!NOTE]
   >
   >Beroende på hur administratören eller gruppadministratören för [!DNL Workfront] ändrade din layoutmall kan fälten i området [!UICONTROL Portfolio Details] ordnas om eller inte visas. Mer information finns i [Anpassa vyn [!UICONTROL Details] med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Så här redigerar du information i avsnittet [!UICONTROL Details]:

   1. (Valfritt) Klicka på ikonen **[!UICONTROL Collapse All]** i det övre högra hörnet om du vill komprimera alla områden.
   1. (Valfritt och villkorligt) När ett område är komprimerat klickar du på den **högerriktade pilen** ![](assets/right-pointing-arrow.png) bredvid varje område för att expandera det område som du vill redigera.
   1. Om du vill ha information om de fält som visas i avsnittet [!UICONTROL Portfolio Details] kan du fortsätta redigera portföljen i rutan [!UICONTROL Edit Portfolio] enligt beskrivningen nedan.
   1. (Valfritt) Om det inte finns några anpassade formulär kopplade till portföljen börjar du skriva namnet på ett formulär i fältet **[!UICONTROL Add custom form]**, markerar det när det visas i listan och klickar sedan på **[!UICONTROL Save Changes]**.
   1. (Valfritt) Klicka på ikonen **[!UICONTROL Export]** ![](assets/export.png) om du vill exportera [!UICONTROL Overview] och anpassad formulärinformation till en PDF-fil. Klicka sedan på **[!UICONTROL Export]**. Välj bland följande:

      * Markera alla (visas bara när det finns minst ett anpassat formulär bifogat)
      * Ökning
      * Namnet på ett eller flera anpassade formulär

      PDF-filen hämtas till datorn.

      ![](assets/export-portfolio-details-box-with-export-button-350x368.png)

      Mer information finns i [Exportera anpassade formulär och objektinformation](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).


1. Om du vill redigera all information om en eller flera portföljer gör du något av följande:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might have to be split in two sections if the single edit and the bulk edit won't come at the same time for portfolios)</p>
   -->

   * Klicka på menyn **[!UICONTROL More]** bredvid portföljnamnet och sedan **[!UICONTROL Edit].**

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will change in NWE with a new Edit Portfolio UI)</p>   
     -->

   * Gå till en lista med portföljer och välj en eller flera portföljer som du vill redigera. Klicka sedan på ikonen **[!UICONTROL Edit]** ![](assets/edit-icon.png) högst upp i listan.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to split into another section when they release the new [!UICONTROL Edit Portfolio] UI)</p>   
     -->
   Dialogrutan **[!UICONTROL Edit Portfolio]** visas.

   ![](assets/edit-portfolio-box-classic-350x224.png)

   Alla portföljfält är tillgängliga i rutan [!UICONTROL Edit Portfolio] och grupperas efter de områden som visas i den vänstra panelen.

1. Det kan vara bra att ange information i följande avsnitt:

   * [[!UICONTROL Overview]](#overview)
   * [Anpassad Forms](#Custom%C2%A0F)
   * [Kommentar](#comment)

### [!UICONTROL Overview] {#overview}

1. Börja redigera en portfölj enligt beskrivningen ovan.
1. Klicka på **[!UICONTROL Overview]** och ange följande fält:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: note below is drafted: drafted till they release new Edit Portfolio boxes)</p>
   -->

   <!--
   <note type="note">
   Depending on how your Workfront administrator or Group administrator sets up our Layout Template, the fields in the Edit Portfolio box might be rearranged or not display. For information, see
   <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>.
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Uppdatera namnet på portföljen. </p> <p>Tips! Detta är inte tillgängligt när du har valt mer än en portfölj. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Skriv en beskrivning av Portfolio för att ange vad som är unikt med det. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Börja skriva namnet på en användare som du vill ange som portföljförvaltare och markera den sedan när den visas i listan. Detta är samma som [!UICONTROL Portfolio Owner]. Detta är den person som kan övervaka arbetet som definieras i portföljens projekt och godkänna affärsärendet.</p> <p>Viktigt: När du anger någon som Portfolio Manager får de automatiskt [!UICONTROL Manage] behörigheter till portföljen, programmen och projekten i portföljen. </p> <p>Tips! Du kan snabbt uppdatera portföljförvaltaren i portföljrubriken. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Group]</td> 
      <td> <p>Lägg till namnet på en enskild grupp om gruppen är associerad med portföljen eller har ansvar för att slutföra den. </p> <p>Tips:  <p>Gör följande när du öppnar fältet [!UICONTROL Group] från sidan [!UICONTROL Portfolio Details]: </p> <p>Du kan se till att du väljer rätt grupp genom att hålla markören över den och klicka på ikonen [!UICONTROL information] <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> <p>Det här alternativet är inte tillgängligt i rutan [!UICONTROL Edit Portfolio]. </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Alignment Scorecard]</p> </td> 
      <td> <p>Välj det justeringskort som du vill använda i listrutan. Ett styrkort används för att mäta hur väl ett projekt överensstämmer med de fastställda kriterierna för ett Portfolio som ofta återspeglar en organisations uppdrag, värderingar och strategiska mål. Mer information finns i <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Använda ett styrkort i ett projekt och generera ett justeringsresultat</a> och <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Skapa ett styrkort</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Is Active]</td> 
      <td> <p> Markera den här kryssrutan om du vill att portföljen ska vara aktiv. Andra användare kan hitta aktiva portföljer och bifoga dem till projekt när de skapar eller redigerar projekt. Inaktiva portföljer kan inte kopplas till projekt. Detta är aktiverat som standard.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Save Changes]** eller fortsätt redigera följande avsnitt.

### Anpassad Forms

1. Börja redigera portföljen enligt beskrivningen ovan.
1. Klicka på listrutan **[!UICONTROL Add Forms]** för att välja ett anpassat formulär och lägga till det i portföljen.

   Du måste skapa anpassade portföljformulär innan de kan läggas till.

   >[!NOTE]
   >
   >Beroende på hur din [!DNL Workfront]-administratör anger behörigheter för avsnitten i ditt anpassade formulär kan inte alla visa eller redigera samma fält i ett visst anpassat formulär. Behörigheterna att redigera fält i ett avsnitt i ett anpassat formulär beror på vilka behörigheter du har på själva portföljen. Mer information om att ange behörigheter för avsnitt i ett anpassat formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Uppdatera fält i anpassade formulär och klicka sedan på **[!UICONTROL Save Changes]** eller fortsätt med följande avsnitt.

### Kommentar {#comment}

1. Börja redigera en portfölj enligt beskrivningen ovan.
1. Klicka på **[!UICONTROL Comment]**.

   ![](assets/comment-box-edit-portfolio-classic-350x227.png)

1. Lägg till en kommentar i fältet **[!UICONTROL Post an update to the portfolio]**.
1. (Valfritt) Klicka på ikonen **[!UICONTROL People]** för att lägga till en användare eller ett team i kommentaren.
1. (Valfritt) Klicka på ikonen **[!UICONTROL Lock]** om du vill låsa kommentaren och göra den privat för endast användare i ditt företag.
1. Klicka på **[!UICONTROL Save Changes]**.

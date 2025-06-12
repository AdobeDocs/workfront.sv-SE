---
product-area: projects;templates
navigation-topic: manage-projects
title: Spara ett projekt som en mall
description: Spara ett projekt som en mallSpara som mall på projektnivå, så att användarna ser det i användargränssnittet. Det finns en annan artikel där den här länken är mer detaljerad (steg för steg). Den här funktionaliteten måste finnas kvar i både projekt OCH mallområden.)"
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 0%

---

# Spara ett projekt som en mall

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Samma funktioner kommer också att vara tillgängliga i produktionsmiljön för alla kunder efter en vecka från förhandsversionen.

Mer information finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Om du bestämmer dig för att ett projekt ska inträffa igen någon gång i framtiden kan du skapa en mall från det befintliga projektet. Sedan kan du använda mallen igen för att skapa framtida projekt som kan innehålla liknande information eller som kan dela samma tidslinje eller tilldelningar med det befintliga projektet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard </p>
   eller 
   <p>Aktuell: Planera </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt </p> <p>Du får behörigheten Hantera för mallen när du har sparat projektet som en mall</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Spara ett projekt som en mall

Att spara ett projekt som en mall skiljer sig åt i produktions- och förhandsvisningsmiljöerna.

### Spara ett projekt som en mall i produktionsmiljön

1. Gå till det projekt som du vill spara som en mall.
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/qs-more-icon-on-an-object.png) och sedan på **Spara som mall**.
1. Ange följande information för mallen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td>Ange ett namn för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ja</strong>: Andra användare kan hitta mallen och bifoga den till projekt.</p> </li> 
        <li><strong>Nej</strong>: Andra användare kan inte hitta mallen och kan inte bifoga den till projekt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td>Använd listrutan för att välja anpassade formulär som ska bifogas mallen. Om några anpassade formulär redan har associerats med projektet visas alla datafält från dessa anpassade formulär.<br>Du kan inkludera upp till 10 anpassade formulär i en enda mall.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Hantera Forms** om du vill ta bort eller ordna om formulären. Mer information om hur du tar bort och ändrar ordning på anpassade formulär i mallen finns i [Anpassade formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Klicka på **Nästa steg.**
1. I avsnittet **Alternativ** markerar du kryssrutan bredvid all information som du vill ta bort från mallen.

   ![](assets/save-as-template-options-step-350x109.png)

1. Klicka på **Nästa steg.**
1. I avsnittet **Uteslut** väljer du de uppgifter du vill utesluta från projektet.

   ![](assets/save-as-template-exclude-350x205.png)

1. Klicka på **Slutför och spara mall.**

   Mallen visas nu i listan med tillgängliga mallar och kan antingen bifogas till ett befintligt projekt eller användas för att skapa ett nytt.


<div class="preview">

### Spara ett projekt som en mall i förhandsgranskningsmiljön

1. Gå till det projekt som du vill spara som en mall.
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/qs-more-icon-on-an-object.png) och sedan på **Spara som mall**.
1. I avsnittet **Spara som mall** anger du följande information för mallen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mallnamn</td> 
      <td>Ange ett namn för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ja</strong>: Andra användare kan hitta mallen och bifoga den till projekt.</p> </li> 
        <li><strong>Nej</strong>: Andra användare kan inte hitta mallen och kan inte bifoga den till projekt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td>Använd listrutan för att välja anpassade formulär som ska bifogas mallen. Om några anpassade formulär redan har associerats med projektet visas alla datafält från dessa anpassade formulär.<br>Du kan inkludera upp till 10 anpassade formulär i en enda mall.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Egen Forms** i den vänstra panelen för att ta bort eller ändra ordningen på formulären.

   Om du vill ändra ordningen på formulären drar och släpper du dem i rätt ordning.
Om du vill ta bort ett formulär markerar du det och klickar sedan på **Ta bort**. Klicka på **Avbryt** om du vill ta bort de markerade formulären.

   ![Anpassade formulärområden i rutan Spara som mall](assets/custom-forms-ara-in-save-as-template-box.png)

1. Uppdatera information i de bifogade anpassade formulären, om det behövs. Informationen överförs till mallen.

1. Klicka på **Alternativ** i det vänstra panelavsnittet och markera sedan kryssrutan bredvid eventuell information som du vill överföra till mallen. Avmarkerade objekt överförs inte till mallen. Alla alternativ är som standard avmarkerade.

   ![Alternativ i rutan Spara som mall](assets/options-area-in-save-as-template-box.png)

1. Klicka på **Uteslut** i den vänstra panelen och välj sedan de uppgifter som du vill utesluta från projektet. Alla åtgärder avmarkeras som standard.

   ![Uteslut område i rutan Spara som mall](assets/exclude-area-save-as-template-box.png)

1. Klicka på **Slutför och spara mall.**

   Mallen visas nu i listan med tillgängliga mallar och kan antingen bifogas till ett befintligt projekt eller användas för att skapa ett nytt.

</span>
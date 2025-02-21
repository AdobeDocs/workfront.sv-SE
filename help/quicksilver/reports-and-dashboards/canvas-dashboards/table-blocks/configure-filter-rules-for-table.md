---
title: Filtrera en tabell i rapportarbetsytan
description: Filtrera en tabell i rapportarbetsytan
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# Filtrera en tabell i rapportarbetsytan

När du har lagt till ett tabellblock i en rapport kan du ställa in filter för att begränsa den information som visas i tabellen.

Det finns tre komponenter i en filterregel:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fält</td> 
   <td> <p>Det fält som innehåller den information som du vill filtrera tabellen med.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operator</td> 
   <td> <p>Det sätt på vilket filtret avgör vilka fältvärden som tas med i eller utesluts från tabellen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Värde</td> 
   <td> <p>Värdena i det markerade fältet som utvärderas enligt operatorn.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exempel:** Om du vill begränsa resultaten i din rapport så att endast projekt som ägs av Jane Doe visas, kan du skapa en filterregel med fältet&quot;Projektägare&quot;, operatorn&quot;Lika med&quot; och värdet&quot;Jane Doe&quot;.

Du kan också visa endast projekt som har en tilldelad projektägare, som har fältet&quot;Projektägare&quot; och operatorn&quot;Inte tom&quot;.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurera filterregler för en tabell

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny ](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Rapportering**.

1. Klicka på **Ny rapport**.

   eller

   Gå till en befintlig rapport, klicka på ikonen **Mer meny** ![Mer ](assets/more-icon.png) i rapportrubriken och välj sedan **Redigera**.

1. Om du vill gruppera rader i en ny tabell drar eller dubbelklickar du på ett tabellblock på arbetsytan.

   eller

   Om du vill gruppera rader i en befintlig tabell klickar du på ikonen **Redigera** ![Redigera ](assets/edit-icon.png) i tabellhuvudet.

1. I den högra panelen letar du reda på det fält som du vill filtrera tabellen efter och drar det sedan till filteravsnittet.

   En filterregeluppsättning visas med namnet på det fält som du har markerat.

1. Välj den operator som du vill använda i listrutan:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Lika med</strong> </td> 
      <td> <p>Detta returnerar bara en exakt matchning av det sökda värdet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Inte lika med</strong> </td> 
      <td> <p>Detta returnerar bara resultat som inte är exakta träffar för det sökda värdet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>är tom</strong> </td> 
      <td> <p>Fältet finns för objektet men fältet har ännu inte fått något värde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>är inte tom</strong> </td> 
      <td> <p>Fältet som du filtrerar efter finns och har fått ett värde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>är mindre än</strong> </td> 
      <td> <p>Detta söker efter alla resultat med ett värde som är mindre än det som anges, utan att det angivna värdet tas med.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>är mindre än eller lika med</strong> </td> 
      <td> <p>Detta söker efter alla resultat med ett värde som är mindre än eller lika med det angivna värdet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>är större än</strong> </td> 
      <td> <p>Detta söker efter alla resultat med ett värde som är större än det angivna värdet, utan att det angivna värdet tas med.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>är större än eller lika med</strong> </td> 
      <td> <p>Detta söker efter alla resultat med värden som är större än eller lika med det angivna värdet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mellan</strong> </td> 
      <td> <p>Tillhandahåller två obligatoriska fältvärden och söker efter alla resultat inom intervallet för båda fälten inklusive de angivna värdena.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Innehåller</strong> </td> 
      <td> <p>Detta söker efter den angivna texten i en hel textsträng.</p> <p>Om du till exempel använder"Innehåller Inf" hämtas allt med"Inf" eller"inf" i det, till exempel ordet"Infinity".</p> <p>Obs! Adobe Workfront söker efter hela ordet eller frasen som du anger för varje filterregel. Om du t.ex. söker efter fält med frasen"nytt projekt" i namnet, visar inte Workfront projekt som bara innehåller"nytt" eller"projekt" i sina namn, eller fraser som innehåller extra ord mellan t.ex."nytt huvudprojekt". Filtret hittar bara projekt med den exakta frasen"nytt projekt" i namnet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Innehåller inte</strong> </td> 
      <td> <p>Detta filtrerar bort objekt som saknar angiven text.</p> <p>"innehåller inte inf" returnerar alla fält utan "Inf" eller "inf" i sina namn.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ange det sista värdet för att slutföra filterregeln, baserat på den operator du valde.

   >[!NOTE]
   >
   >De värden som anges här är **inte** skiftlägeskänsliga.

1. (Valfritt) Gör så här om du vill lägga till en till filterregel i regeluppsättningen:

   1. Dra ett annat fält till **Släpp om du vill lägga till ytterligare en regel** i filteravsnittet nedanför den andra regeln.
   1. Upprepa steg 4-6.
   1. I den nedrullningsbara listrutan till vänster om den nya regeln väljer du **AND** eller **OR**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>OCH</p> </td> 
         <td> <p>När du kopplar filterregler eller regeluppsättningar till operatorn AND anger du att du vill att alla regler på samma nivå ska uppfyllas.</p> <p>Programsatserna i ett filter förenas som standard med operatorn AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>ELLER</p> </td> 
         <td> <p>När du kopplar filterregler eller regeluppsättningar med OR-operatorn anger du att du vill att <strong>minst</strong> en regel - eller regeluppsättning - på den nivån ska uppfyllas.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >AND- och OR-operatorer på samma nivå - som kopplar ihop flera regler i en regeluppsättning eller hela regeluppsättningar - matchar alltid. Om du till exempel ändrar operatorn mellan två regler i en regeluppsättning, ändras alla andra operatorer i den regeluppsättningen automatiskt så att de matchar den.

1. (Villkorligt) Gör så här om du vill lägga till ytterligare en filterregeluppsättning:

   1. Dra fältet som du vill lägga till till i området **Lägg till en regeluppsättning** nedanför dina andra filterregeluppsättningar.
   1. Upprepa steg 4-7.
   1. Välj **AND** eller **OR** i den nedrullningsbara listan till vänster om den nya regeluppsättningen. Dessa operatorer fungerar på samma sätt som de som listas i steg 7, men gäller för hela regeluppsättningar i stället för enskilda regler i en uppsättning.***

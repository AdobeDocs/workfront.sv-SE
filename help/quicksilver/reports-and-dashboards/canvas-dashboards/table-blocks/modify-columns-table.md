---
title: Konfigurera en tabellkolumn i rapportarbetsytan
description: Konfigurera en tabellkolumn i rapportarbetsytan
hidefromtoc: true
hide: true
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Konfigurera en tabellkolumn i rapportarbetsytan

Kolumnerna i en tabell kan konfigureras för visning. Du kan ändra följande aspekter av en kolumn:

* Namn
* Sortering
* Redigera behörighet
* Hovringstext
* Aggregering
* Villkorsstyrd formatering

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Ändra kolumner i en tabell

1. Gå till en befintlig rapport, klicka på ikonen **Mer meny** ![Mer &#x200B;](assets/more-icon.png) i rapportrubriken och välj sedan **Redigera**.
1. Klicka på ikonen **Redigera** ![Redigera &#x200B;](assets/edit-icon.png) på tabellrubriken i rapporten.

   ![Ikonen Redigera i tabellrubriken](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Om du just har skapat tabellen och ännu inte har lagt till några fält klickar du i stället på knappen Redigera mitt i tabellen.

1. (Valfritt) Lägg till, flytta eller ta bort kolumner i tabellen. Mer information om hur du redigerar fälten i en tabell finns i [Lägga till eller redigera ett tabellblock i Rapporteringsarbetsyta](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Lägg till en ny kolumn | Om du vill lägga till en kolumn i en tabell kan du antingen klicka och dra ett fält från panelen **Fält** till höger på sidan till tabellen där du vill placera det, eller dubbelklicka på ett fält för att lägga till det som kolumnen längst till höger. |
   |---|---|
   | Flytta en kolumn | Om du vill ändra ordningen på kolumnerna i en tabell klickar du på ett kolumnnamn och drar det till en ny plats. |
   | Ta bort en kolumn | Om du vill ta bort en kolumn från en tabell klickar du på kolumnen som du vill ta bort och sedan på x till höger om kolumnnamnet. |

   {style="table-layout:auto"}

1. Om du vill konfigurera en kolumn klickar du på namnet på den kolumn som du vill ändra i tabellens rubrikrad och sedan på någon av följande flikar i den högra panelen:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Fliken Data</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Sammanställning baserad på</td>
      <td><p> Om du vill samla (sammanfatta i rubriken) informationen i en kolumn väljer du den typ av aggregering som du vill ha i listrutan <strong>Sammanställd baserat på</strong>. Vilka alternativ som är tillgängliga beror på vilken typ av data som finns i kolumnen.</p><p>Om du använder grupper i tabellen visas det aggregerade värdet i gruppraden ovanför kolumnnamnet i stället för bredvid kolumnnamnet.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Fältformat</td>
      <td><p>(Endast tillgängligt när kolumnen innehåller data om datum, procent, valuta eller tid, inte text.) Välj det format du vill använda för data i listrutan <b>Fältformat</b>. Du kan till exempel visa procenttecken efter talen i en kolumn eller ändra hur datum visas.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Fältet är redigerbart</td>
      <td><span>Aktivera fältet <strong>går att redigera</strong> om du vill tillåta användare som visar tabellen att redigera namnet på kolumnen.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sortera</strong></td>
      <td><p>Som standard sorteras tabellen efter data i den vänstra kolumnen i stigande ordning. Om du vill sortera efter den markerade kolumnen i stället klickar du på nedpilen bredvid <strong>Sortera</strong> och sedan på kryssrutan <b>Sortera efter den här kolumnen</b>. Du kan sedan välja en <strong>sorteringsriktning</strong> (stigande eller fallande värden) och en <strong>sorteringsordning</strong> (den relativa sorteringsprioriteten för den här kolumnen jämfört med andra sorteringskolumner i tabellen).</p><p>Du kan upprepa den här processen om du vill sortera tabellen i upp till fem olika kolumner. Kontrollera att varje kolumn har rätt <strong>sorteringsordning</strong> i förhållande till eventuella nya kolumner som du väljer för sortering.</p><p>Obs! Om du tar bort en kolumn som är markerad för att sortera en tabell och en annan kolumn också är markerad för sortering, används den kolumnen för att sortera tabellen i stället för i fallande ordning. Om inga andra kolumner är markerade för sortering återgår tabellen till standardvärdet: sortera efter den första kolumnen.</p><p>När du anger en kolumn som ska sorteras i tabellen visas en liten ruta bredvid kolumnnamnet med ett tal som anger den relativa prioriteten för den kolumnen när tabellen sorteras (tabellen sorteras först med 1, sedan 2 och så vidare) och en pil som anger om sorteringsriktningen är stigande eller fallande. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Fliken Format</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Egen kolumnetikett</strong> </td> 
      <td>Ange ett nytt visningsnamn för kolumnen (högst 100 tecken).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa hovringstext</td> 
      <td> <p>Ange om du vill att förklarande text ska visas när någon hovrar över ett kolumnnamn.</p> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hovringstext</td> 
      <td>(Endast tillgängligt när <strong>Visa hovringstext</strong> är aktiverat.) Anpassa den förklarande texten som visas när någon hovrar över ett kolumnnamn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Villkorsstyrd formatering</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Lägg till <img src="assets/add-rule.png">, redigera <img src="assets/edit-icon.png"> eller ta bort <img src="assets/delete.png"> en regel som formaterar celler i kolumnen när deras värden uppfyller de villkor du anger.</p> <p>Du kan till exempel skapa en regel som ändrar teckensnittet i fältet"Projektstatus" till lila i fet stil när fältets värde är lika med"Byggnad".</p> <p>Du kan också använda <b>Visa en ikon</b> för att lägga till en grön flaggikon för varje objekt i kolumnen som har statusen"Aktuell".</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Obs! Om du använder <strong>Visa en ikon</strong> är de andra formateringsalternativen inte tillgängliga.</p> <p>Du kan välja <strong>Använd på hela raden</strong> om du vill att formateringen ska påverka hela raden i en cell som uppfyller regelns villkor. Du kan t.ex. markera projekt som förfaller efter ett visst datum genom att använda en gul bakgrundsfärg inte bara på datumcellerna i kolumnen Förfaller den, utan på hela raden där dessa datum inträffar.</p> <p>Tips! När du lägger till formateringsalternativ i en regel visas det resulterande cellformatet under <strong>Förhandsgranska</strong> längst ned på panelen.</p> </li> 
        <li value="2">När du är klar med att lägga till en regel klickar du på <strong>Spara</strong>.</li> 
        <li value="3"> <p>(Valfritt) Klicka på <b>+ Lägg till regel </b> om du vill lägga till ytterligare regler i samma kolumn.</p> <p>Flera villkorsstyrda formateringsregler i en tabell används i följande ordning:</p> 
         <ul> 
          <li> <p>Regler som tillämpas på hela rader utvärderas först, från vänster till höger för varje kolumn och sedan uppifrån och ned i en kolumn.</p> <p>Obs! Radformatering åsidosätter annan villkorsstyrd formatering för celler i den raden, även om de annars skulle uppfylla villkoret i en annan kolumns regel.</p> </li> 
          <li> <p>Andra regler utvärderas härnäst, uppifrån och ned när de visas i den högra panelen för en kolumn. Du kan dra <img src="assets/drag-object-icon.png"> sparade regler på den panelen för att ändra deras ordning.</p> <p>Obs! Celler formateras baserat på det första villkoret som de uppfyller och kommer inte att formateras ytterligare även om de uppfyller andra villkor.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på pilen **Gå tillbaka** i det övre vänstra hörnet av skärmen för att återgå till rapporten.

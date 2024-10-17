---
product-area: reporting
navigation-topic: reporting-elements
title: Använd villkorsstyrd formatering i vyer
description: När du delar dina rapporter med andra användare i Adobe Workfront bör du överväga att anpassa rapportvyn så att viss information blir lättare att läsa eller bara sticka ut.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '1218'
ht-degree: 0%

---

# Använd villkorsstyrd formatering i vyer

<!--Audited: 01/2024-->

När du delar dina rapporter med andra användare i Adobe Workfront bör du överväga att anpassa rapportvyn så att viss information blir lättare att läsa eller bara sticka ut.

Du kan anpassa fliken Detaljer för dina rapporter genom att lägga till speciell eller villkorsstyrd formatering till rapportvyn.

Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Genom att villkorligt formatera kolumner i rapportvyn kan du ange regler som påverkar rapportens utseende. När dessa villkor eller regler är uppfyllda används den särskilda formateringen.

Om procentandelen färdigt för en uppgift till exempel är mindre än 20 procent kan du markera fältet genom att visa procenttalet i fet stil, röd text och en gul bakgrundsfärg.

Med en villkorsstyrd vy kan du:

* Ändra en kolumns rubrik.
* Ändra värdet för en kolumn till anpassad text eller en bild.
* Formatera visningen av ett fält genom att ändra teckensnittstyp, färg, justering eller bakgrundsfärgen.

De ändringar du gör i rapportvyn börjar bara gälla på rapportens flik Information. De här ändringarna påverkar inte rapportens flikar Sammanfattning, Matris eller Diagram.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Nytt:</p> 
   <ul><li>Standard för rapportvyer</li>
  <li> Medarbetare eller högre för listvyer</li></ul>

<p>Aktuell:</p>
   <ul>
    <li> Planera för rapportvyer </li>
    <li> Begär eller högre för listvyer </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera en vy i en rapport</p> <p><b>ANMÄRKNING</b></p> <p>Om du inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter till en rapport för att skapa eller redigera en vy i en rapport</p> <p>Hantera behörigheter till en vy</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

Du måste skapa en rapport innan du kan lägga till villkorsstyrd formatering i vyn.

Mer information om hur du skapar en rapport finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Skapa en villkorsstyrd vy

{{step1-to-reports}}

1. Klicka på namnet på en rapport där du vill skapa en villkorsstyrd vy

   eller

   Klicka på **Ny rapport** och välj sedan en objekttyp för att skapa en ny rapport.

1. (Villkorligt) Om du redigerar en befintlig rapport klickar du på **Rapportåtgärder** och sedan på **Redigera**.

1. Klicka för att markera en befintlig kolumn på fliken **Kolumner (Visa)** eller klicka på **Lägg till kolumn** för att skapa en kolumn.
1. I fältet **Visa i den här kolumnen** i det övre vänstra hörnet av rapportverktyget markerar du fältet som du vill visa i den nya kolumnen.
1. Klicka på **Avancerade alternativ**.

1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etikett för anpassad kolumn</strong></td> 
      <td> <p>Ange ett namn för kolumnen.</p> <p>Om du redigerar en befintlig kolumn ändras det befintliga kolumnnamnet om du anger ett namn här.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fältformat</strong></td> 
      <td>Välj i vilket format värdet i kolumnen ska visas. Beroende på vad kolumnfältet är kan du med det här alternativet ange hur datum, siffror och valutor ska visas. Det här alternativet visas inte för alla kolumner.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Visa den här kolumnen när du arbetar på en instrumentpanel</strong></td> 
      <td>Markera det här fältet om du vill att kolumnen ska visas när rapporten placeras på en kontrollpanel. Kolumnen visas alltid när du tittar på rapporten utanför en kontrollpanel.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Lägg till en regel för kolumnen**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. Ange en villkorssats för kolumnen i avsnittet **När:**.

   Till exempel:&quot;när aktivitetsprocenten är lika med (skiftlägeskänslig) 50.&quot;
1. I avsnittet **Visa fältet så här:** anger du hur det här fältet ska se ut när villkoret som definieras ovan uppfylls.

   Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Textfärg</strong></td> 
      <td> <p>Välj den färg som texten ska visas i med färgväljaren.</p> <p><b>ANMÄRKNING</b></p> <p> Om fältet innehåller en hyperlänk används inte textfärgmarkeringarna i det här fältet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Textformat</strong></td> 
      <td>Välj om texten ska visas i fet eller kursiv stil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Textjustering</strong></td> 
      <td>Välj om texten ska justeras åt höger, i mitten eller åt vänster i kolumnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bakgrund</strong></td> 
      <td>Välj bakgrundsfärg för texten med färgväljaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Visa ikon</strong></td> 
      <td>Välj en av 16 ikoner om du vill visa en ikon i stället för det faktiska värdet för den här kolumnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Visa text</strong></td> 
      <td> <p>Välj det här alternativet om du vill visa en anpassad etikett för den här kolumnen i stället för dess verkliga värde. Ange den text som ska visas i stället för värdet i det angivna fältet.</p> <p><b>VIKTIGT</b></p> <p>Om du väljer <strong>Visa text</strong> inaktiveras möjligheten att redigera texten i den här kolumnen.<br>Du kan inte heller ändra värdet för en föregående kolumn eftersom den innehåller inbyggd logik.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Använd på hela raden</strong></td> 
      <td>Välj det här alternativet om du vill använda inställningar för hela raden i stället för att bara använda inställningar för den markerade kolumnen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Lägg till regel**.\
   Du kan lägga till ytterligare regler i samma kolumn eller lägga till regler i andra kolumner.

   Reglerna tillämpas i den ordning de skapades. De kombineras men de skriver inte över varandra, men en kolumnregel har företräde framför en radregel i samma cell.

   **EXEMPEL 1**

   Du kan först skapa en regel som anger att textfärgen är lila och fet när ett projekt har statusen Byggnad. Sedan skapar du en andra regel som anger att när en uppgifts namn inte är tomt blir textfärgen röd och kursiv och bakgrundsfärgen grön. I det här exemplet händer följande:

   * Aktiviteter vars projektstatus är Byggnad visas i lila och fet text. Om aktivitetsnamnet inte är tomt har aktiviteterna också en grön bakgrund.
   * Uppgifter vars projektstatus är något annat än Byggnad (och aktivitetsnamnet inte är tomt) visas i röd och kursiv text med grön bakgrund.

   **EXEMPEL 2**

   Skapa en regel i kolumnen Datum för planerat slutförande i projektet som påverkar hela raden och gör bakgrunden grå om projektet avbryts (till exempel när Projektstatus är Inaktiv). Skapa sedan en kolumnregel som ändrar bakgrunden till röd när projektets planerade slutförandedatum är mindre än idag (vilket innebär att projektet är sent). I det här exemplet, om ett projekt som avbryts har ett sent avslutsdatum, visas cellen som röd även om de andra cellerna i raden är grå. Så här korrigerar du den här formateringen:

   * Redigera formateringen för det planerade slutförandedatumet och ta bort kolumnregeln för den röda bakgrunden i sena projekt.
   * Lägg till en kolumnregel med samma formatering som radregeln (grå bakgrund när Projektstatus = Dölj).
   * Lägg till kolumnregeln igen för den röda bakgrunden i sena projekt.
   * När du sparar reglerna och vyn används inte den röda bakgrunden i ett projekt som har avbrutits.

1. Klicka på **Spara**.
1. Klicka på **Spara + Stäng**.\
   I rapporten ser användare ändringar i formatet om de angivna villkoren har uppfyllts.

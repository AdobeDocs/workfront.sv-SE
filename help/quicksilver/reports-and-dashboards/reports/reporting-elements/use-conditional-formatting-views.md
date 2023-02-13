---
product-area: reporting
navigation-topic: reporting-elements
title: Använd villkorsstyrd formatering i vyer
description: När du delar dina rapporter med andra användare i Adobe Workfront bör du överväga att anpassa rapportvyn så att viss information blir lättare att läsa eller bara sticka ut.
author: Lisa
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 0%

---

# Använd villkorsstyrd formatering i vyer

När du delar dina rapporter med andra användare i Adobe Workfront bör du överväga att anpassa rapportvyn så att viss information blir lättare att läsa eller bara sticka ut.

Du kan anpassa fliken Detaljer för dina rapporter genom att lägga till speciell eller villkorsstyrd formatering till rapportvyn.

Du måste ha behörigheten Hantera för rapporten för att kunna redigera den och lägga till specialformatering i vyn.

Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Genom att villkorligt formatera kolumner i rapportvyn kan du ange regler som påverkar hur rapporten visas. När dessa villkor eller regler är uppfyllda används den särskilda formateringen.

Om procentandelen färdigt för en uppgift till exempel är mindre än 20 procent kan du markera fältet genom att visa procenttalet i fet stil, röd text och en gul bakgrundsfärg.

Med en villkorsstyrd vy kan du:

* Ändra en kolumns rubrik.
* Ändra värdet för en kolumn till anpassad text eller en bild.
* Formatera visningen av ett fält genom att ändra teckensnittstyp, färg, justering eller bakgrundsfärgen.

De ändringar du gör i rapportvyn börjar bara gälla på rapportens flik Information. De här ändringarna påverkar inte rapportens flikar Sammanfattning, Matris eller Diagram.

## Åtkomstkrav

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera en vy i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter till en rapport för att skapa eller redigera en vy i en rapport</p> <p>Hantera behörigheter till en vy</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste skapa en rapport innan du kan lägga till villkorsstyrd formatering i den.

Mer information om hur du skapar en rapport finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Skapa en villkorsstyrd vy

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.

1. Klicka på namnet på en rapport där du vill skapa en villkorsstyrd vy.

   eller

   Klicka **Rapportåtgärder** och sedan klicka **Redigera**.

1. (Villkorligt) Om du redigerade en rapport markerar du en befintlig kolumn eller skapar en ny kolumn.
1. Klicka **Avancerade alternativ**.

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
      <td>Välj i vilket format värdet i kolumnen ska visas. Beroende på vad kolumnfältet är kan du med det här alternativet ange hur datum, siffror och valutor ska visas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Visa den här kolumnen när du arbetar på en instrumentpanel</strong></td> 
      <td>Markera det här fältet om du vill att kolumnen ska visas när rapporten placeras på en kontrollpanel. Kolumnen visas alltid när du tittar på rapporten utanför en kontrollpanel.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Lägg till en regel för den här kolumnen**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. I **När:** anger du en villkorssats för kolumnen. Till exempel: när aktivitetsprocenten är lika med (skiftlägeskänslig) 50.
1. I **Visa fältet så här:** anger hur det här fältet ser ut när villkoret som definieras ovan är uppfyllt.

   Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Textfärg</strong></td> 
      <td> <p>Välj den färg som texten ska visas i. Det finns 8 tillgängliga färger.</p> <p>Obs! Om fältet innehåller en hyperlänk används inte textfärgmarkeringarna i det här fältet.</p> </td> 
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
      <td>Välj bakgrundsfärg för texten. Det finns 8 tillgängliga färger.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Visa ikon</strong></td> 
      <td>Välj en av 16 ikoner om du vill visa en ikon i stället för det faktiska värdet för den här kolumnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Visa text</strong></td> 
      <td> <p>Välj det här alternativet om du vill visa en anpassad etikett för den här kolumnen i stället för dess verkliga värde. Ange den text som ska visas i stället för värdet i det angivna fältet.</p> <p>Viktigt: Markera <strong>Visa text</strong> inaktiverar möjligheten att redigera texten i den här kolumnen.<br>Du kan inte heller ändra värdet för en Predecessor-kolumn eftersom den innehåller inbyggd logik.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Använd på hela raden</strong></td> 
      <td>Välj det här alternativet om du vill använda inställningar för hela raden i stället för att bara använda inställningar för den markerade kolumnen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Lägg till regel**.\
   Du kan lägga till ytterligare regler i samma kolumn eller lägga till regler i andra kolumner.

   Reglerna tillämpas i den ordning de skapades. De kombineras men skriver inte över varandra, men en kolumnregel har företräde framför en radregel i samma cell.

   Exempel 1: Du kan först skapa en regel som anger att textfärgen är lila och fet när projektstatus är Byggnad. Sedan skapar du en andra regel som anger när aktivitetsnamnet inte är tomt, att textfärgen är röd och kursiv och att bakgrundsfärgen är grön. I det här exemplet händer följande:

   * Aktiviteter vars projektstatus är Byggnad visas i lila och fet text. Om aktivitetsnamnet inte är tomt har aktiviteterna också en grön bakgrund.
   * Uppgifter vars projektstatus är något annat än Byggnad (och aktivitetsnamnet inte är tomt) visas i röd och kursiv text med grön bakgrund.

   Exempel 2: Skapa en regel på projektets planerade slutförandedatum som påverkar hela raden och gör om bakgrundsgrått om projektet avbryts (Status = &quot;Död&quot;). Skapa sedan en kolumnregel som ändrar bakgrunden till röd när projektets planerade slutförandedatum är mindre än idag (vilket innebär att projektet är sent). I det här exemplet, om ett projekt som avbryts har ett sent avslutsdatum, visas cellen som röd även om övriga celler i raden är grå. Så här korrigerar du formateringen:

   * Redigera formateringen för det planerade slutförandedatumet och ta bort kolumnregeln för den röda bakgrunden i sena projekt.
   * Lägg till en kolumnregel med samma formatering som radregeln (grå bakgrund när Projektstatus = &quot;Död&quot;)
   * Lägg till kolumnregeln igen för den röda bakgrunden i sena projekt.
   * När du sparar reglerna och vyn används inte den röda bakgrunden i ett projekt som har avbrutits.


1. Klicka **Klar**.
1. Klicka **Spara + Stäng**.\
   I rapporten ser användare ändringar i formatet om de angivna villkoren har uppfyllts.

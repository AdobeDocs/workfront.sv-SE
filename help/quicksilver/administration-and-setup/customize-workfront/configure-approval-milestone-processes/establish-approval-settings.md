---
title: Konfigurera globala inställningar för godkännande
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Som Adobe Workfront-administratör kan du ange globala inställningar för godkännandeprocesser i Workfront. De här inställningarna påverkar alla godkännandeprocesser för arbetsobjekt i systemet.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Konfigurera globala inställningar för godkännande

Som Adobe Workfront-administratör kan du ange globala inställningar för godkännandeprocesser i Workfront. De här inställningarna påverkar alla godkännandeprocesser för arbetsobjekt i systemet.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara systemadministratör eller ha en avtalslicens med administrativ åtkomst till godkännandeprocesser</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera globala inställningar för godkännande

1. Logga in på Workfront som Workfront-administratör.
1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Processer** > **Godkännanden** .

1. Klicka på ikonen **Inställningar** ![](assets/gear-icon-settings.png) bredvid namnet på området **Godkännanden** .

1. Ange följande information i rutan **Godkännandeinställningar** som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lägg till &lt;number&gt; dagar till planerat slutförandedatum för godkännandeprocesser</td> 
      <td> <p>Ange antalet minuter, timmar, dagar, veckor eller månader för att lägga till tid till det planerade slutförandedatumet för aktiviteten som behöver godkännas. Välj Förflutna minuter, timmar, dagar eller veckor för att lägga till tid som omfattar alla helger, helger och ej arbetstid som har angetts i systemets kalender för arbetsschema.</p> 
      <p>Om en uppgift till exempel tilldelas på fredag och har en varaktighet på 3 förflutna dagar, är aktivitetens slutförandedatum inställt på måndag (förutsatt att lördag och söndag är en helg). Om aktiviteten har en varaktighet på 3 dagar (inte förfluten), är datumet för aktivitetens slutförande inställt på onsdag.</p>
      <p><b>Obs!</b> Om du aktiverar den extra tiden för godkännande av aktiviteter påverkas tidslinjen för aktiviteten och tidslinjen för projektet.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännaren behöver inte vara med i projektteamet (för godkännandeprocesser som inkluderar en roll)</td> 
      <td> <p>Välj det här alternativet om en godkännare inte behöver vara med i projektteamet när en godkännandeprocess innehåller en roll. När du tilldelar ett godkännandebeslut till en jobbroll visas godkännandet endast för de användare som har en roll som är kopplad till dem i projektet. Om du aktiverar den här inställningen får alla användare med den jobbrollen godkännandebegäran oavsett om de är i projektteamet eller inte. Mer information om hur du redigerar en användares projektroll finns i <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Hantera projektteamet</a>. </p> 
      <p><b>TIPS</b>: När du tilldelar ett godkännande till en roll och alternativet <b>Godkännare måste inte finnas i projektteamet (för godkännandeprocesser som innehåller en roll)</b> inaktiveras, men det finns inga roller i projektteamet som matchar rollen vid godkännandet, tilldelas godkännandet om till projektägaren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inaktivera delegering av godkännande</td> 
      <td> <p>Välj det här alternativet om du vill inaktivera funktionen för användare i systemet att delegera godkännanden till en annan användare. När det här alternativet är markerat tas alternativet att delegera godkännanden bort från Workfront och alla befintliga godkännandedelegeringar stoppas.</p> <p>Mer information om delegering av godkännanden i Workfront finns i <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegera godkännandebegäran</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt redigering av det anpassade formuläret när projektet, aktiviteten eller problemet väntar på godkännande</td> 
      <td> <p>Välj det här alternativet om du vill tillåta användare att redigera den anpassade formen av projekt, uppgifter och utgåvor i statusen Väntande godkännande. Det här är standardinställningen.</p> 
      <p>När det här alternativet är markerat:</p> 
       <ul> 
       <li>Alla godkännare (och andra användare som har behörighet att redigera det anpassade formuläret) kan ändra det anpassade formuläret när objektet väntar på godkännande, oavsett aktuell godkännandeväg eller godkännandesteg.</li> 
       <li>Ändringar som görs i det anpassade formuläret under en godkännandeprocess påverkar inte några godkännandebeslut som har fattats före ändringen.</li> 
       <li> <p>Alla ändringar som görs i projektet, aktiviteten eller utgåvan spåras på samma sätt, oavsett den här inställningen. </p> <p>Om du till exempel har lagt till anpassade formulärfält som ska spåras i uppdateringsflödet spåras alla ändringar i formuläret i objektets uppdateringsström.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt användare att återkalla nyskapade begäranden som väntar på godkännande</td> 
      <td> <p>Välj det här alternativet om du vill konfigurera om användare kan återkalla ett problem eller en begäran som väntar på godkännande för sin första status. Du kan associera den första statusen för en utgåva eller en begäran med en godkännandeprocess genom att konfigurera köer för begäranden. </p> 
      <p>Mer information om begärandeköer finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>.</p> 
      <p>Gör något av följande:</p> 
       <ul> 
       <li>Välj det här alternativet om du vill tillåta användare att återkalla ett godkännande för den första statusen för en utgåva eller en förfrågan. I det här fallet kan de se knappen Återkalla&lt; för en ny utgåva eller förfrågan som väntar på att godkännas. När de återkallar ett problem får de en varning om att problemet också kommer att tas bort. Problemet tas bort när de har bekräftat att de återkallar det. </li> 
       <li> <p>Avmarkera det här alternativet om du inte vill att användare ska kunna återkalla ett problem eller en begäran vars första status väntar på godkännande. De kan inte se knappen Återkalla&lt; om den nya utgåvan eller begäran och godkännandet måste beviljas. Det här är standardalternativet.</p> 
       <p>Mer information om granskning av objekt som väntar på godkännande finns i <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Visa godkännanden </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara ändringar.**

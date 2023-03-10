---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Händelsemeddelanden är tillgängliga i Adobe Workfront
description: Händelsemeddelanden är e-postmeddelanden som utlöses av olika typer av händelser för objekt som projekt, uppgifter och problem, vilket förklaras i händelsemeddelanden.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '5070'
ht-degree: 0%

---

# Händelsemeddelanden är tillgängliga i Adobe Workfront

Händelsemeddelanden är e-postmeddelanden som utlöses av olika typer av händelser för objekt som projekt, uppgifter och problem, vilket förklaras i [Händelsemeddelanden](../../../workfront-basics/using-notifications/event-notifications.md).

Dessa meddelanden kan konfigureras på system- och gruppnivå:

* Information om hur du konfigurerar händelsemeddelanden på systemnivå finns i [Konfigurera händelsemeddelanden för alla i systemet](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Mer information om hur du konfigurerar händelsemeddelanden på gruppnivå finns i [Visa och konfigurera händelsemeddelanden för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Enskilda användare kan också aktivera och inaktivera sina meddelanden om enskilda händelser i sin individuella profil. Mer information finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

I följande tabeller visas alla Adobe Workfront händelsemeddelanden, en kort beskrivning av händelsen och om händelsen är aktiv eller inaktiv som standard.

## Åtgärd krävs

Se även [Meddelanden: Åtgärd krävs](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th>Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Användare</p> </td> 
   <td> <p>Åtkomstbegäran till användaren</p> </td> 
   <td> <p>Någon begär åtkomst från mig.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> <p> </p> </td> 
   <td> <p>Lägg till dokumentbegäran i begäran</p> </td> 
   <td> <p>Begär att jag ska överföra dokument.</p> <p>Begäranden får ett e-postmeddelande när de får en begäran om att överföra ett dokument.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokumentet väntar på godkännande till godkännare</p> </td> 
   <td> <p>Jag måste godkänna ett dokument.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utfärda tilldelning som ska utfärdas</p> </td> 
   <td> <p>Jag är tilldelad en utgåva.</p> <p>Den som tilldelat utgåvan får ett e-postmeddelande endast om projektets status är Aktuell och status för utgåvan inte är Stängd eller något som motsvarar Stängt.</p> <p>Användare med en licens för granskning eller begäran får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utfärda väntande godkännande till godkännare</p> </td> 
   <td> <p>Jag måste godkänna ett problem.</p> <p>Vilka användare som får ett e-postmeddelande för den här händelsen beror på om inställningen"Godkännaren behöver inte vara i projektteamet (för godkännandeprocesser som inkluderar en roll)" är aktiverad (enligt beskrivningen i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala inställningar för godkännande</a>). </p> <p>Om det här alternativet är aktiverat</strong>, skickas ett e-postmeddelande till alla användare i systemet med rollen "Godkännare".</p> <p>Om det här alternativet är inaktiverat</strong>, får endast projektgruppsmedlemmar med rollen "Godkännare" ett e-postmeddelande.</p> <p>Ett meddelande skickas om projektet har statusen Planering eller Aktuell. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utfärda väntande godkännande till delegerad godkännare</p> </td> 
   <td> <p>Jag måste granska ett godkännande som jag har delegerats.</p> <p>När någon delegerar ett ärende till en annan användare meddelas användaren. </p> <p>Ett meddelande skickas bara när projektet har statusen Aktuell.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projekt som väntar på godkännande till godkännare</p> </td> 
   <td> <p>Jag måste godkänna ett projekt.</p> <p>Vilka användare som får ett e-postmeddelande för den här händelsen beror på om inställningen"Godkännaren behöver inte vara i projektteamet (för godkännandeprocesser som inkluderar en jobbroll)" är aktiverad (enligt beskrivningen i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala inställningar för godkännande</a>).</p> <p>Om det här alternativet är aktiverat</strong>, skickas ett e-postmeddelande till alla användare i systemet med rollen "Godkännare".</p> <p>Om det här alternativet är inaktiverat</strong>, får endast projektgruppsmedlemmar med rollen "Godkännare" ett e-postmeddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Projekt som väntar på godkännande till delegerad godkännare</td> 
   <td> <p>Jag måste granska ett projektgodkännande som jag har delegerats.</p> </td> 
   <td> Aktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Uppgiftstilldelning till uppgift tilldelad till</p> </td> 
   <td> <p>Jag är den primära tilldelaren för en uppgift.</p> <p>Uppgiftstilldelningsmottagaren får ett e-postmeddelande om de är den primära tilldelningsmannen för uppgiften, såvida inte den tilldelande är den användare som tilldelat uppgiften.</p> <p>Ett meddelande skickas om projektstatusen är Aktuell och aktiviteten inte är markerad som Slutförd.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitet väntar på godkännande till godkännare</p> </td> 
   <td> <p>Jag måste godkänna en uppgift.</p> <p>Vilka användare som får ett e-postmeddelande för den här händelsen beror på om inställningen"Godkännaren behöver inte vara i projektteamet (för godkännandeprocesser som inkluderar en roll)" är aktiverad (enligt beskrivningen i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala inställningar för godkännande</a>). </p> <p>Om det här alternativet är aktiverat</strong>, skickas ett e-postmeddelande till alla användare i systemet med rollen "Godkännare".</p> <p>Om det här alternativet är inaktiverat</strong>, får endast projektgruppsmedlemmar med rollen "Godkännare" ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell vid tidpunkten för begäran.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitet väntar på godkännande till delegerad godkännare</p> </td> 
   <td> <p>Jag måste granska ett uppgiftsgodkännande som jag har delegerats.</p> <p>När någon delegerar ett ärende till en annan användare meddelas användaren. </p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell vid tidpunkten för begäran.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tidrapport</p> </td> 
   <td> <p>Tidrapporten öppnades igen för användaren</p> </td> 
   <td> <p>Min tidrapport öppnas igen.</p> <p>Ägaren av tidrapporten får ett e-postmeddelande när tidrapporten öppnas igen, såvida inte användaren som öppnat tidrapporten också är ägare till tidrapporten.</p> <p>Ett e-postmeddelande skickas endast om tidrapportens status är Öppen.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tidrapport</p> </td> 
   <td> <p>Tidrapportsavslag till användaren</p> </td> 
   <td> <p>Min tidrapport har avvisats.</p> <p>Ägaren av tidrapporten får ett e-postmeddelande när tidrapporten avvisas, såvida inte användaren som avvisade tidrapporten också är ägare.</p> <p>Ett e-postmeddelande skickas endast om tidrapportens status har avvisats.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tidrapport</p> </td> 
   <td> <p>Inlämning av tidrapport till godkännare</p> </td> 
   <td> <p>Jag måste godkänna en tidrapport.</p> <p>Godkännaren av tidrapporten får ett e-postmeddelande när en tidrapport som de måste godkänna skickas, såvida inte användaren som skickade tidrapporten också är godkännare av tidrapporten.</p> <p>Ett meddelande skickas endast om tidrapportens status har skickats.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tilldelning</p> </td> 
   <td> <p>Begäran om arbetsuppgift till team</p> </td> 
   <td> <p>Mitt team får en ny arbetsförfrågan.</p> <p>Teammedlemmar får ett e-postmeddelande när teamet får en ny arbetsförfrågan. (Användaren som skickade begäran får inget meddelande om han/hon är medlem i gruppen.)</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell vid den tidpunkt då arbetsbegäran görs och arbetsbegärans status är Ny.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tilldelning</p> </td> 
   <td> <p>Arbetsuppgiftsförfrågan till tilldelad arbetsuppgift</p> </td> 
   <td> <p>Jag får en ny arbetsförfrågan.</p> <p>Den som har tilldelats arbetsuppgiften får ett e-postmeddelande, såvida inte den som har gjort begäran också är tilldelad. </p> <p>Inget meddelande skickas om aktivitetsstatusen är Slutförd eller om utgivningsstatusen är Stängd.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell vid tidpunkten för begäran.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Begäranden som jag har gjort

Se även [Meddelanden: Begäranden som jag har gjort](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Ändra dokumentgodkännandestatus till begärande</p> </td> 
   <td> <p>En begäran om dokumentgodkännande har slutförts.</p> <p>Dokumentbegäraren får ett e-postmeddelande när dokumentets godkännandebegäran har slutförts.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokumentbegäran slutförd till begärande</p> </td> 
   <td> <p>En begäran om dokumentöverföring har uppfyllts.</p> <p>Dokumentbegäraren får ett e-postmeddelande när en begäran om att överföra ett dokument har slutförts.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utgåva till utleverans, primär kontakt</p> </td> 
   <td> <p>Jag lägger till ett problem i ett projekt.</p> <p>Den primära kontakten i ett problem får ett meddelande när de lägger till ett problem i ett projekt.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>Utfärda tilldelning för att utfärda primär kontakt</td> 
   <td> <p>Någon har tilldelats ett problem som jag är primär kontakt för.</p> <p>Den primära kontakten i ett problem får ett meddelande när utgåvan tilldelas en användare. </p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> Inaktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utleverans slutförd till Primär kontakt</p> </td> 
   <td> <p>Ett problem som jag är primär kontakt för har åtgärdats.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektstatusändring till Anges av</p> </td> 
   <td> <p>Statusen ändras för ett projekt som jag har skapat.</p> <p>Användaren som skapade projektet får ett e-postmeddelande när projektstatusen ändras.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Lägg till i ärende, primär kontakt</p> </td> 
   <td> <p>Jag skickar en begäran (bekräftelse).</p> <p>Den primära kontakten i ärendet får ett e-postmeddelande när de skickar ett problem.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet använder vyn "Är supportavdelningen".</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Begär tilldelning att utfärda primär kontakt</p> </td> 
   <td> <p>Någon har tilldelats min begäran.</p> <p>Den primära kontakten för utgåvan får ett e-postmeddelande när en användare tilldelas utgåvan, såvida inte den primära kontakten och den tilldelade användaren är samma användare.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet använder vyn "Är supportavdelningen".</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Begäran stängd för att utfärda primär kontakt</p> </td> 
   <td> <p>Min förfrågan är stängd (bekräftelse).</p> <p>Den primära kontakten får ett e-postmeddelande när begäran stängs.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet använder vyn "Är supportavdelningen".</p> <p>Om meddelanden om att"ärendet har slutförts" är aktiverat kommer de alltid att utlösas i stället för"begäran stängd för att skicka den primära kontakten". Om du vill att det här meddelandet ska utlösas måste du inaktivera meddelandena om att meddelandet har slutförts.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Begär att dokument ska läggas till i den primära kontakten</p> </td> 
   <td> <p>Ett dokument ändras eller överförs vid ett problem som jag är primär kontakt för.</p> <p>Den primära kontakten får ett e-postmeddelande när ett dokument överförs eller ändras i frågan, såvida inte den användare som överförde eller ändrade dokumentet också är den primära kontakten.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet har "Publicera som hjälpbegärandekö" aktiverat på fliken Köinställningar. <!-- DRAT I FLARE: Mer information om hur du publicerar ett projekt som en kö för hjälpbegäranden finns i 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Översikt över fliken Köinformation i ett projekt</a>.

    --></p> </td>
<td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Begär statusändring för utfärdande av primär kontakt</p> </td> 
   <td> <p>Statusen ändras på min begäran.</p> <p>Den primära kontakten för problemet får ett e-postmeddelande när utgivningsstatusen ändras, såvida inte den användare som ändrade statusen också är den primära kontakten.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och projektet använder vyn "Är supportavdelningen".</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Kommunikation

Se även [Meddelanden: Kommunikation](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Kommentera dokumentet till dokumentägaren</p> </td> 
   <td> <p>En kommentar läggs till i mitt dokument.</p> <p>Ägaren till ett dokument i Workfront får ett e-postmeddelande när en kommentar publiceras i dokumentet, såvida inte den användare som publicerade kommentaren också är dokumentägaren.</p> <p>Alla användare som är direkt inkluderade i kommentaren får också ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell. </p> <p>Ämnet för e-postmeddelandet är: <em>Kommentera &lt;request name=""&gt; på &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> Det dagliga sammandraget innehåller följande uppgifter:<em> Kommunikationssammanfattning &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Aktiv </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anteckning</p> </td> 
   <td> <p>Anteckning för förfrågan Lägg till i ärende, primär kontakt</p> </td> 
   <td> <p>När en kommentar har publicerats på en förfrågan skickar du den primära kontakten via e-post.</p> <p>Den primära kontakten för en utgåva får ett e-postmeddelande när en kommentar publiceras på en förfrågan, såvida inte den användare som publicerade kommentaren också är den primära kontakten för utgåvan.</p> <p>Alla användare som är direkt inkluderade i kommentaren får också ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Användare</p> </td> 
   <td>Riktad uppdatering till användare</td> 
   <td> <p>Någon inkluderar mig på en riktad uppdatering.</p> <p>En riktad uppdatering är när en användare specifikt inkluderar en annan användare i en uppdatering, vilket beskrivs i <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a>.</p> <p>I det här fallet får den användare som ingår i den riktade uppdateringen ett e-postmeddelande om uppdateringen.</p> <p>E-postmeddelandet skickas endast om användaren har åtkomstbehörighet till objektet&lt;!&gt;— DRAT I FLARE: och är inte samma användare som anger uppdateringen

    -->. &lt;/p> &lt;p>Händelsemeddelandet aktiveras som standard och kan inte inaktiveras.&lt;/p> &lt;/td>
<td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Direktuppdatering till team</p> </td> 
   <td> <p>Någon inkluderar mitt team i en riktad uppdatering.</p> <p>En riktad uppdatering är när en användare specifikt inkluderar en annan användare i en uppdatering, vilket beskrivs i <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a>.</p> <p>I det här fallet får alla medlemmar i teamet som ingår i den riktade uppdateringen ett e-postmeddelande om uppdateringen.</p> <p>E-postmeddelandet skickas endast till användare som har åtkomstbehörighet till uppdateringens objekt.</p> <p>Om användaren som skickar den dirigerade uppdateringen är medlem i det team som inkluderas får användaren som skickar uppdateringen inget e-postmeddelande.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anteckning</p> </td> 
   <td> <p>Arbetsobjektskommentar till kopplade deltagare</p> </td> 
   <td> <p>Någon kommenterar en tråd jag är med i.</p> <p>Deltagare i tråden och användare som är inkluderade i ett direktmeddelande får ett e-postmeddelande när en användare gör en kommentar i tråden.</p> <p>Användarna måste ha åtkomst till Visa för att få ett meddelande.</p> <p>Följande användare får inget meddelande:</p> 
    <ul> 
     <li> <p>Team som ingår i ett direktmeddelande</p> </li> 
     <li> <p>Anteckningens ägare</p> </li> 
     <li> <p>Den primära kontakten</p> </li> 
    </ul> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anteckning</p> </td> 
   <td> <p>Arbetsuppgiftskommentar till tilldelad arbetsuppgift</p> </td> 
   <td> <p>Någon kommenterar något av mina arbetsuppgifter.</p> <p>Den som har tilldelats arbetsuppgiften får ett e-postmeddelande när som helst när en användare lägger till en uppdatering av en arbetsuppgift, såvida inte den användare som lägger till uppdateringen också är den som har tilldelats uppgiften.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anteckning</p> </td> 
   <td> <p>Svar på arbetsförfrågan till arbetsbeställare</p> </td> 
   <td> <p>Någon besvarar min begäran.</p> <p>När en användare har skickat en begäran och en annan användare har svarat på den, får användaren som skickade begäran ett e-postmeddelande.</p> <p>Ett e-postmeddelande skickas inte om:</p> 
    <ul> 
     <li> <p>Användaren som svarar är samma användare som gjorde begäran</p> </li> 
     <li> <p>Användaren har inte åtkomst för att se anteckningen</p> </li> 
    </ul> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Godkännandeinformation

Se även [Meddelanden: Godkännandeinformation](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Användare</p> </td> 
   <td> <p>Delegering av godkännande till en annan användare</p> </td> 
   <td> <p>Jag är delegerad som godkännare.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Delegerad ändring av godkännandestatus</p> </td> 
   <td> <p>En begäran om delegerat godkännande av utfärdande har slutförts. </p> <p>När du delegerar ett utfärdandegodkännande till någon annan får du ett e-postmeddelande när de har slutfört det godkännandet (oavsett om de godkänner eller avvisar det). </p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Ändring av status för delegerat projektgodkännande</p> </td> 
   <td> <p>En delegerad begäran om projektgodkännande har slutförts.</p> <p>När du delegerar ett projektgodkännande till någon annan får du ett e-postmeddelande när de har slutfört det godkännandet (oavsett om de godkänner eller avvisar projektgodkännandet).</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Ändring av status för delegerat aktivitetsgodkännande</p> </td> 
   <td> <p>En status för godkännande av delegerad uppgift har slutförts.</p> <p>När du delegerar ett uppgiftsgodkännande till någon annan får du ett e-postmeddelande när de har slutfört det godkännandet (oavsett om de godkänner eller avvisar uppgiftsgodkännandet).</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Avbryt dokumentgodkännande till godkännare</p> </td> 
   <td> <p>En begäran om dokumentgodkännande har avbrutits.</p> <p>Dokumentgodkännaren får ett e-postmeddelande när dokumentets godkännandebegäran avbryts.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tidrapport</p> </td> 
   <td> <p>Godkännande av tidrapport till användare</p> </td> 
   <td> <p>Min tidrapport är godkänd.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information om arbete som tilldelats mig

Se även [Meddelanden: Information om arbete som tilldelats mig](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Uppgift</td> 
   <td>Alla föregående aktiviteter slutförda till aktivitetsberoende i tilldelat team</td> 
   <td> <p>Alla föregångare till teamets uppgifter är slutförda.</p> <p>Uppgiften som tilldelas (alla medlemmar i teamet) får ett e-postmeddelande.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td>Inaktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Alla föregående aktivitetsslutförande till aktivitetsberoende</p> </td> 
   <td> <p>Alla föregångare till mina uppgifter är slutförda.</p> <p>Uppgiftstilldelaren får ett e-postmeddelande.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Godkännandebeslut som ska utfärdas</p> </td> 
   <td> <p>Ett problem som jag löser har godkänts eller avvisats.</p> <p>Den som är tilldelad en utgåva får ett e-postmeddelande när ett godkännandebeslut fattas (godkänt eller avvisat).</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Godkännandebeslut för uppgift tilldelad till</p> </td> 
   <td> <p>En uppgift som jag har slutfört godkänns eller avvisas.</p> <p>Uppgiftstilldelande får ett e-postmeddelande när uppgiften har godkänts eller avvisats.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utfärda slutförande av ärende tilldelat</p> </td> 
   <td> <p>Ett problem som jag har tilldelats är slutfört.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Datum för planerat slutförande av ärende ändrat</p> </td> 
   <td> <p>Förfallodatumet ändras för en utgåva som jag har tilldelats.</p> <p>Den som tilldelats utgåvan får ett e-postmeddelande när det planerade slutförandedatumet ändras, såvida inte den användare som ändrade det planerade slutförandedatumet också är den som tilldelats utgåvan.</p> <p>Ett meddelande skickas bara om projektstatusen är något annat än Planering.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utgåva statusändring till Problem tilldelat</p> </td> 
   <td> <p>Statusen ändras för en av mina arbetsuppgifter.</p> <p>Den som är tilldelad utgåvan får ett e-postmeddelande när statusen ändras, såvida inte den användare som ändrade statusen också är tilldelad.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Begär att dokument ska läggas till i ärende som tilldelats</p> </td> 
   <td> <p>Dokument överförs eller ändras vid förfrågningar som jag har tilldelats.</p> <p>Den som tilldelats utgåvan får ett e-postmeddelande när dokument överförs eller ändras i ett ärende som de lagt till.</p> <p>Ett e-postmeddelande skickas inte om den användare som angav problemet är den som tilldelades problemet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och om projektet har "Publicera som hjälpbegärandekö" aktiverat på fliken Köinställningar.<!-- DRAT I FLARE: Mer information om hur du publicerar ett projekt som en kö för hjälpbegäranden finns i 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Översikt över fliken Köinformation i ett projekt</a>.

    --></p> </td>
<td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Uppgiften slutförd till uppgift tilldelad till</p> </td> 
   <td> <p>En uppgift som jag har tilldelats är slutförd.</p> <p>Uppgiftstilldelaren får ett e-postmeddelande när uppgiften har slutförts. Meddelanden skickas inte när en personlig uppgift har slutförts.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Användare med en Granska eller Begärande licens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförd uppgift till aktivitetsberoende</p> </td> 
   <td> <p>En föregångare till en av mina uppgifter är slutförd.</p> <p>Uppgiftstilldelande får ett e-postmeddelande när en av uppgiftens föregångare har slutförts.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitetsplanerat slutförandedatum har ändrats</p> </td> 
   <td> <p>Förfallodatumet ändras för en uppgift som jag har tilldelats.</p> <p>Uppgiftstilldelaren får ett e-postmeddelande när det planerade slutförandedatumet för uppgiften ändras, såvida inte användaren som ändrade det planerade slutförandedatumet också är Uppgiftstilldelningsmannen.</p> <p>Ett meddelande skickas bara om projektstatusen är något annat än Planering.</p> <p>Inget meddelande skickas om personliga uppgifter.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitetsstatus Ändra till Aktivitet tilldelad till</p> </td> 
   <td> <p>Statusen ändras för en uppgift som jag har tilldelats.</p> <p>Uppgiftstilldelaren får ett e-postmeddelande när uppgiftsstatus ändras, såvida inte den användare som ändrade statusen också är tilldelad.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> <p>Användare med en granskningslicens får inget meddelande. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information om projekt som jag är på

Se även [Meddelanden: Information om projekt som jag är på](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Aktuell projektstatus har ändrats till projektgruppen</p> </td> 
   <td> <p>Ett projekt jag håller på att bli aktivt.</p> <p>Användarna i projektet får ett e-postmeddelande när projektet blir aktivt.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Lägg till dokument i projektgruppen</p> </td> 
   <td> <p>Ett dokument läggs till i ett projekt som jag är på.</p> <p>Användare i projektteamet får ett e-postmeddelande när ett dokument läggs till i projektet, med undantag för den användare som lade till dokumentet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och dokumentet inte är Privat. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem Lägg till i projektgruppen</p> </td> 
   <td> <p>Ett problem har lagts till i ett projekt som jag är på.</p> <p>Användare i ett projekt får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Slutförande av problem till projektgruppen</p> </td> 
   <td> <p>Ett problem har åtgärdats i ett projekt som jag är med i.</p> <p>Alla användare i projektet får ett meddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförande av milstolpe-uppgift till projektgrupp</p> </td> 
   <td> <p>En milstolpe har slutförts i ett projekt som jag är på.</p> <p>Alla användare i projektteamet får ett meddelande när en milstolpeuppgift har slutförts. </p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektslutförande till projektgruppen</p> </td> 
   <td> <p>Ett projekt jag håller på med är färdigt.</p> <p>Användare i ett projektteam får ett e-postmeddelande när projektstatusen är Slutförd.</p> <p>Tips: Om projekten slutförs regelbundet kan du aktivera det här alternativet för att skapa många e-postmeddelanden för användare som har ett begränsat antal uppgifter i många projekt. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektstatusändring till projektgrupp</p> </td> 
   <td> <p>Status ändras för ett projekt som jag är på.</p> <p>Användare i projektgruppen får ett e-postmeddelande när projektstatus ändras. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektanvändare</p> </td> 
   <td> <p>Projektanvändare Lägg till i projektanvändare</p> </td> 
   <td> <p>Jag har lagts till i ett projekt.</p> <p>Användaren som lades till i projektet får ett e-postmeddelande när de läggs till, såvida inte användaren själv har lagts till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförd uppgift till projektgrupp</p> </td> 
   <td> <p>En uppgift är slutförd i ett projekt som jag är på.</p> <p>Projektteamets medlemmar får ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Ej tilldelat ärende tillagt i projektgruppen</p> </td> 
   <td> <p>Ett otilldelat problem läggs till i ett projekt som jag är på.</p> <p>Användare i ett projekt får ett e-postmeddelande när ett otilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information om projekt som jag äger

Se även [Meddelanden: Information om projekt som jag äger](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Lägg till dokument i projektägare</p> </td> 
   <td> <p>Ett dokument läggs till i ett projekt som jag äger.</p> <p>Projektägaren får ett e-postmeddelande när ett dokument läggs till i projektet, såvida inte den användare som lade till dokumentet också är projektägare.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och dokumentet inte är Privat.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utgåva till projektägare</p> </td> 
   <td> <p>Ett problem har lagts till i ett projekt som jag äger.</p> <p>Projektägaren får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Bekräftelsedatum för ärende, ändring till projektägare</p> </td> 
   <td> <p>Bekräftelsedatumet ändras för ett problem i ett av mina projekt.</p> <p>Projektägaren får ett e-postmeddelande när implementeringsdatumet ändras för en utgåva i projektet, såvida inte användaren som ändrar implementeringsdatumet är samma användare som projektägaren.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Slutförande av problem till projektägare</p> </td> 
   <td> <p>Ett problem har åtgärdats i ett projekt som jag äger.</p> <p>Projektägaren får ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförande av milstolpeaktivitet till projektägare</p> </td> 
   <td> <p>En milstolpe har slutförts i ett projekt som jag äger.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektägartilldelning till projektägare</p> </td> 
   <td> <p>Jag är nu ägare till ett nytt projekt.</p> <p>När en användare tilldelas som projektägare får användaren ett e-postmeddelande.</p> <p>Om projektägaren är samma användare som tilldelades skickas inget e-postmeddelande</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektförloppsändring till projektägare</p> </td> 
   <td> <p>Ett projekt som jag äger ligger efter.</p> <p>Projektägaren får ett e-postmeddelande när projektet är försenat.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitet, implementeringsdatum, ändring till projektägare</p> </td> 
   <td> <p>Bekräftelsedatumet ändras för en aktivitet i ett av mina projekt.</p> <p>Projektägaren får ett e-postmeddelande när implementeringsdatumet ändras för en aktivitet i projektet, såvida inte användaren som ändrade implementeringsdatumet också är projektägaren.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförd uppgift till projektägare</p> </td> 
   <td> <p>En uppgift slutförs i ett projekt som jag äger.</p> <p>Projektägaren får ett meddelande. </p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Förloppsändring för uppgift till projektägare</p> </td> 
   <td> <p>En uppgift i ett projekt som jag äger kommer efter.</p> <p>Projektägaren får ett e-postmeddelande när en aktivitet i projektet ligger efter schemat.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Ej tilldelat problem Lägg till i projektägare</p> </td> 
   <td> <p>Ett otilldelat problem läggs till i ett projekt som jag äger.</p> <p>Projektägaren får ett e-postmeddelande när ett ej tilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Information om projekt som jag sponsrar

Se även [Meddelanden: Information om projekt som jag sponsrar](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Lägg till dokument i projektsponsorer</p> </td> 
   <td> <p>Ett dokument läggs till i ett projekt som jag sponsrar.</p> <p>Projektsponsorn får ett e-postmeddelande när ett dokument läggs till i projektet, såvida inte dokumentet läggs till av projektsponsorn.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell och dokumentet inte är Privat.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utgåva till projektsponsorer</p> </td> 
   <td> <p>Ett problem läggs till i ett projekt som jag sponsrar.</p> <p>Projektsponsorn får ett e-postmeddelande när ett problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Slutförande av problem till projektsponsor</p> </td> 
   <td> <p>Ett problem har åtgärdats i ett projekt som jag sponsrar.</p> <p>Projektsponsorn får ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförande av milstolpeaktivitet till projektsponsor</p> </td> 
   <td> <p>En milstolpe i ett projekt som jag sponsrar slutförs.</p> <p>Projektsponsorn får ett e-postmeddelande när en milstolpe-uppgift har slutförts i ett projekt som de sponsrar.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektförloppsändring till projektsponsorer</p> </td> 
   <td> <p>Ett projekt som jag sponsrar släpar efter.</p> <p>Projektsponsorn får ett e-postmeddelande när projektet försenas.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektsponsor Tilldelning till projektsponsor</p> </td> 
   <td> <p>Jag utses till projektsponsor.</p> <p>Projektsponsorn får ett e-postmeddelande när de utses till projektsponsor.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Slutförd uppgift till projektsponsor</p> </td> 
   <td> <p>En uppgift slutförs i ett projekt som jag sponsrar.</p> <p>Projektsponsorn får ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitetsförloppet ändras till Projektsponsor</p> </td> 
   <td> <p>En uppgift i ett projekt som jag sponsrar släpar efter.</p> <p>Projektsponsorn får ett e-postmeddelande när en aktivitet i projektet försenas.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Ej tilldelat problem Lägg till i projektsponsor</p> </td> 
   <td> <p>Ett otilldelat problem läggs till i ett projekt som jag sponsrar.</p> <p>Projektsponsorn får ett e-postmeddelande när ett ej tilldelat problem läggs till i projektet.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Diverse information

Se även [Meddelanden: Diverse information](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Händelse</th> 
   <th>Beskrivning</th> 
   <th> Standardläge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Meddelande</td> 
   <td> <p>Meddelandet lades till</p> </td> 
   <td> <p>Ett meddelande skickas till meddelandecentret.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Avbryt dokumentbegäran till begäran</p> </td> 
   <td> <p>Avbryt en begäran om dokumentöverföring från mig.</p> <p>Dokumentbegäran får ett e-postmeddelande när en dokumentbegäran avbryts.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Felmeddelande</p> </td> 
   <td> <p>Ett fel som kräver din uppmärksamhet hittades.</p> <p>Ett e-postmeddelande genereras när Workfront försöker ansluta till ett POP-konto. Efter 25 försök inaktiverar Workfront anslutningen till POP-kontot för att bevara resurser och skickar ett meddelande. </p> <p>E-postmeddelandet skickas till projektägaren, om POP-e-postmeddelandet är kopplat till en begärandekö, eller till Workfront-administratörerna, om POP-kontot är kopplat till funktionen Inkommande e-post i e-postinställningarna.
     <!--
      DRAFTED IN FLARE:
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      --></p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Utfärda tilldelning till resursägare</p> </td> 
   <td> <p>En ändring av en problemtilldelning påverkar ett av mina medarbetare.</p> <p>Utgåva tilldelningshanteraren får ett e-postmeddelande när en ändring påverkar en användare som han/hon hanterar.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell eller Planering.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Användare</p> </td> 
   <td> <p>Ny användare till användare</p> </td> 
   <td> <p>När en ny användare skapas i Workfront skickar du ett e-postmeddelande till användaren.</p> <p>När den nya användaren har skapats får användaren en e-postinbjudan som meddelar användaren om att ett Workfront-konto har skapats och ber denne ange sitt lösenord.</p> <p>När du skapar en ny användare kan användare välja alternativet"Skicka en inbjudan via e-post till den här personen" (enligt beskrivningen i <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Lägg till användare</a><span style="font-weight: 400;">). När alternativet "Ny användare till användare" har aktiverats globalt får alla nya användare e-postinbjudan oavsett om alternativet "Skicka en inbjudan via e-post till den här personen" har valts.</span></p> </td> 
   <td> Inaktiv </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Objektdelning till team</p> </td> 
   <td> <p>Någon delar ett objekt med mitt team.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Användare</p> </td> 
   <td> <p>Objektdelning till användare</p> </td> 
   <td> <p>Någon delar objekt med mig.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektanvändare</p> </td> 
   <td> <p>Projektanvändare Lägg till i resursägare</p> </td> 
   <td> <p>En av mina medarbetare läggs till i ett projekt.</p> <p>En projektledare får ett e-postmeddelande när en av hans eller hennes direktrapporter läggs till i ett projekt.</p> <p>Användare med en granskningslicens får inget meddelande.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projekt som lagts till i en portfölj eller ett program</p> </td> 
   <td> <p>Någon lägger till ett projekt i en portfölj eller ett program som jag äger.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppgift</p> </td> 
   <td> <p>Aktivitetstilldelning till resursägare</p> </td> 
   <td> <p>En ändring av en uppgiftstilldelning påverkar ett av mina medarbetare.</p> <p>Uppgiftstilldelningshanteraren får ett e-postmeddelande.</p> <p>Ett meddelande skickas bara om projektstatusen är Aktuell.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> Projekt <br>Uppgift <br>Problem</td> 
   <td>Ny uppdatering till prenumerant </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Ett e-postmeddelande skickas när en uppdatering görs av en uppgift, en utgåva eller ett projekt som jag prenumererar på.</span> </p> </td> 
   <td>Aktiv</td> 
  </tr> 
 </tbody> 
</table>

## Delegering

Se även [Meddelanden: Delegering](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Objekttyp | Händelse | Beskrivning | Standardläge |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Uppgifter och problem | Uppgift och utfärda delegering till tilldelad | Jag delegerar mina uppgifter och ärenden (bekräftelse) | Aktiv |
| Uppgifter och problem | Stoppa aktiviteten och utfärda delegering till den som tilldelats | Jag avbryter delegeringen av mina uppgifter och frågor (bekräftelse) | Aktiv |
| Uppgifter och problem | Uppgift och utge delegering till delegat | Någon delegerar sina uppgifter och ärenden till mig | Aktiv |
| Uppgifter och problem | Stoppa aktiviteter och skicka delegering till delegering | Någon stoppar delegeringen av deras uppgifter och ärenden till mig | Aktiv |

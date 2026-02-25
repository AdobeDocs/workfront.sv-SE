---
title: Ställ in påminnelsemeddelanden
description: Påminnelsemeddelanden genererar e-postmeddelanden som skickas till användare baserat på angivna villkor. Påminnelsemeddelanden påminner användarna om en åtgärd som de behöver utföra för en uppgift, utgåva, projekt eller tidrapport.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: bb9ccfa61fa1a8ef41b0e873d5aa6313803c636d
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 0%

---

# Ställ in påminnelsemeddelanden

<!-- Audited: 1/2024 -->

Som Workfront-administratör kan du skapa påminnelsemeddelanden för användare och associera dem med objekt som du vill att dina användare ska vara särskilt uppmärksamma på.

Påminnelsemeddelanden genererar e-postmeddelanden som skickas till användare baserat på angivna villkor. Påminnelsemeddelanden påminner användarna om en åtgärd som de behöver utföra för en uppgift, utgåva, projekt eller tidrapport.

När du har skapat påminnelsemeddelandena kan användarna manuellt koppla dem till arbetsobjekt, till exempel projekt, uppgifter, utgåvor och tidrapporter. Mer information finns i [Bifoga ett påminnelsemeddelande till ett objekt](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard </p>
<p>Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Planering eller senare, med administrativ åtkomst till påminnelsemeddelanden</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassa påminnelsemeddelandet

Du kan anpassa ämnet, brödtexten och HTML i påminnelsemeddelandet.

Du kan också använda det standardmeddelande som ingår i påminnelsemeddelandet. I standardmeddelandet används påminnelsemeddelandets namn som e-postmeddelandets ämne och objektnamnet i e-postmeddelandets brödtext, inklusive händelsen som utlöste meddelandet.

Om du vill anpassa påminnelsemeddelandet måste du skapa en e-postmall och bifoga den till påminnelsemeddelandet.

Mer information om hur du skapar en e-postmall finns i [Konfigurera e-postmallar](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Skapa ett påminnelsemeddelande

{{step-1-to-setup}}

1. Klicka på **E-post** > **Meddelanden** > **Påminnelsemeddelanden**.

   ![Fliken Påminnelsemeddelanden](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Klicka på **Nytt påminnelsemeddelande**.

1. Klicka på den objekttyp som du vill associera med påminnelsemeddelandet i listrutan.

   Om du till exempel vill bifoga en påminnelse till en tidrapport klickar du på **Tidrapport**.

1. Ange följande information i rutan **Nytt påminnelsemeddelande** som visas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn på påminnelsemeddelande</td> 
      <td>Ange ett namn för påminnelsemeddelandet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kvalificeringsperiod</td> 
      <td> <p>Ange antalet timmar, arbetsdagar, dagar (kalenderdagar), veckor eller månader före eller efter datumet i fältet <strong>Timing</strong>.</p> <p><b>OBS</b>:  
        <ul> 
         <li> <p>Påminnelsemeddelanden börjar 24 timmar efter det angivna datumet och när alla villkor är uppfyllda.</p> </li> 
         <li> <p>Påminnelsemeddelanden för projekt, uppgifter och utgåvor som utlöses varje kväll vid midnatt i USA Mountain Time. Alla objekt som är berättigade till ett påminnelsemeddelande från den dagen utlöser ett meddelande till de avsedda användarna kort efter den tidpunkten.</p> </li> 
         <li> <p>Påminnelser om tidrapporter baseras på organisationens tidszon och tidrapportets slutdatum, startdatum eller senaste uppdateringsdatum. Tidszoner för enskilda användare påverkar inte tidpunkten för påminnelsemeddelanden.</p> 
      </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Välj den händelse som utlöser påminnelsemeddelandet som ska schemaläggas.</p> <p>Om påminnelsemeddelandet är avsett för projekt, aktiviteter eller utgåvor är de tillgängliga alternativen relaterade till Slutförandedatum eller Startdatum. Påminnelsemeddelandet tar hänsyn till tidsstämpeln för slutförande och startdatum för projekt, uppgifter och problem.</p>

   <p>Om påminnelsemeddelandet är avsett för tidrapporter är de tillgängliga alternativen relaterade till Slutdatum, Startdatum eller Senaste uppdateringsdatum. Påminnelsemeddelandet för tidrapporter tar hänsyn till tidsstämpeln för tidrapporgens slut-, start- och senaste uppdateringsdatum. Tidrapporten börjar vid midnatt på dagen för startdatumet (12:00) och slutar precis före midnatt på slutdatumet (11:59 PM).</p>

   <p><b>ANMÄRKNING</b></p>
      <p>Påminnelsemeddelanden för tidrapporter distribueras endast en gång var 24:e timme.</p> <p>När du konfigurerar flera påminnelsemeddelanden inom en 24-timmarsperiod skickar Workfront ut ett e-postmeddelande med alla påminnelser som ingår i det meddelandet.</p>
      <p>Om du till exempel konfigurerar tre påminnelsemeddelanden så att de utlöser 10 timmar före, 2 timmar före och 1 timme före ett förfallodatum, kombineras alla tre påminnelserna i samma meddelande om de inträffar under samma dag.</p> <p>Men om du ställer in ett påminnelsemeddelande för 26 timmar före och ytterligare en för 1 timme före ett förfallodatum får användarna två separata meddelanden. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kriterier</td> 
      <td> <p>Välj villkoren för att kvalificera påminnelsemeddelandet som ska schemaläggas. Påminnelsemeddelanden är inte schemalagda såvida inte valet av villkor uppfylls.</p> <p>Följande villkorsalternativ är tillgängliga, beroende på vilken objekttyp du valde i steg 4:</p> 
       <ul> 
        <li><strong>Ofullständigt i aktuella projekt:</strong> <i>(Tillgängligt för påminnelser om aktiviteter och ärenden)</i> Påminnelsemeddelandet schemaläggs att endast skickas när objektstatusen som påminnelsemeddelandet är associerat med inte är Fullständigt och projektstatusen är Aktuell.</li> 
        <li><strong>Alla i aktuella projekt:</strong> <i>(Tillgängligt för påminnelser om aktiviteter och utleveranser)</i> Påminnelsemeddelandet schemaläggs att skickas oavsett objektstatus och endast när det projektstatus som påminnelsemeddelandet är associerat med är Aktuell.</li> 
        <li><strong>Ofullständiga projekt:</strong> <i>(Tillgängligt för projektpåminnelser)</i> Påminnelsemeddelandet är schemalagt att skickas när projektstatusen är något annat än Fullständigt.</li> 
        <li><strong>Alla projekt:</strong> <i>(Tillgängligt för projektpåminnelser)</i> Påminnelsemeddelandet är schemalagt att skickas oavsett projektstatus.</li> 
        <li><strong>Öppna tidrapporter:</strong> <i>(Tillgängligt för tidrapportpåminnelser)</i> Påminnelsemeddelandet schemaläggs att skickas när tidrapportstatus är Öppen.</li> 
        <li><strong>Skickade tidrapporter:</strong> <i>(Tillgängligt för tidrapportpåminnelser)</i> Påminnelsemeddelandet schemaläggs att skickas när tidrapportstatusen har skickats.</li> 
        <li><strong>Öppna tidrapport eller mindre än 40 timmar per vecka:</strong> <i>(Tillgängligt för tidrapportpåminnelser)</i> Påminnelsemeddelandet schemaläggs att skickas när tidrapportstatusen är öppen eller när tidrapporten har loggats mindre än 40 timmar.</li> 
        <li><strong>E-postmall:</strong> I listrutan väljer du en e-postmall som ska bifogas påminnelsen.<br>Mer information om hur du skapar en e-postmall finns i <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Konfigurera e-postmallar</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mottagare</td> 
      <td><p>Beroende på vilket objekt påminnelsemeddelandet gäller väljer du bland följande typer av användare som du vill få meddelandet:</p>
      <ul>
      <li>Tilldelad till</li>
      <li>Anges av</li>
      <li>Projektgruppen (alla användare i projektteamet får påminnelsen)</li>
      <li>Beroende aktivitetstilldelningar (användare som tilldelats beroende uppgifter får påminnelsen)</li>
      <li>Projektägare</li>
      <li>Tilldelad (användare som tilldelats en uppgift eller en utgåva får påminnelsen)</li>
      <li>Ägare av tidrapport</li>
      <li>Godkännare av tidrapport</li>
      <li>Ansvarig för tidrapportsägare</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.
1. Bifoga påminnelsemeddelandet till ett arbetsobjekt, så som beskrivs i [Bifoga ett påminnelsemeddelande till ett objekt](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Få en påminnelseavisering

När villkoret är uppfyllt för det objekt som har påminnelsemeddelandet bifogat, utlöses ett e-postmeddelande till användaren som definierats i påminnelsemeddelandet.

Mer information om att ta emot påminnelsemeddelanden finns i avsnittet [Påminnelsemeddelanden](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) i [Adobe Workfront-meddelanden](../../../workfront-basics/using-notifications/wf-notifications.md).

## Leverans av testpåminnelsemeddelanden

Påminnelsemeddelanden utlöses varje kväll vid midnatt, Mountain Time. Alla objekt som är kvalificerade för ett påminnelsemeddelande utlöser ett meddelande till de avsedda användarna kort därefter.

Om du vill att påminnelsemeddelanden ska utlösas manuellt måste villkoret för påminnelsen vara uppfyllt.\
Om en påminnelse till exempel är inställd på att utlösa en timme efter det planerade slutförandedatumet för ett projekt, måste den tiden ha passerat mellan den tidpunkt då påminnelsen ställdes in och nu. Projekt som hade planerade slutförandedatum passerade innan påminnelsen aktiverades kommer inte att utlösa något meddelande.

Så här aktiverar du ett påminnelsemeddelande manuellt:

{{step-1-to-setup}}

1. Klicka på **System** > **Diagnostik** i det nedre vänstra hörnet av Workfront.

1. Klicka på **Skicka påminnelsemeddelanden** och vänta på bekräftelsen högst upp på skärmen att de har skickats.

   De användare som anges i påminnelsemeddelandet får ett e-postmeddelande.

![Påminnelseaviseringstest](assets/reminder-test.png)

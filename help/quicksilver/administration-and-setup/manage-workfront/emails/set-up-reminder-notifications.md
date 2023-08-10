---
title: Ställ in påminnelsemeddelanden
description: Ställ in påminnelsemeddelanden
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 1129f8ab93d349325bed56bc2b3ba94c2600c03f
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 0%

---

# Ställ in påminnelsemeddelanden

Påminnelsemeddelanden skickar e-postmeddelanden till mottagare baserat på angivna villkor. Som Adobe Workfront-administratör eller en användare med behörigheten Planering och administrativ åtkomst till påminnelsemeddelanden kan du manuellt associera påminnelsemeddelanden med dina arbetsobjekt, till exempel projekt, uppgifter, utgåvor och tidrapporter.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

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
   <td> <p>Planering eller senare, med administrativ åtkomst till påminnelsemeddelanden</p> <p>Mer information om hur du ger en Plan-användare administratörsåtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Anpassa påminnelsemeddelandet

Du kan anpassa påminnelsemeddelandet med ett anpassat e-postmeddelande som innehåller ett eget ämne och brödtext. E-postbrödtexten kan innehålla HTML.

Du kan också använda det standardmeddelande som ingår i påminnelsemeddelandet. I standardmeddelandet används påminnelsemeddelandets namn som e-postmeddelandets ämne och objektnamnet i e-postmeddelandets brödtext, inklusive händelsen som utlöste meddelandet.

Om du vill anpassa påminnelsemeddelandet måste du skapa en e-postmall och bifoga den till påminnelsemeddelandet.

Mer information om hur du skapar en e-postmall finns i [Konfigurera e-postmallar](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Skapa ett påminnelsemeddelande

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **E-post** > **Meddelanden** > **Påminnelsemeddelanden**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Klicka **Nytt påminnelsemeddelande**.

1. Klicka på den objekttyp som du vill associera med påminnelsemeddelandet i listrutan.

   Om du till exempel vill bifoga en påminnelse till en tidrapport klickar du på **Tidrapport**.

1. I **Nytt påminnelsemeddelande** anger du följande information.

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
      <td> <p>Ange antalet timmar, arbetsdagar, dagar (kalenderdagar), veckor eller månader före eller efter datumet i <strong>Timing</strong> fält.</p> <p><b>ANMÄRKNING</b>:  
        <ul> 
         <li> <p>Påminnelsemeddelanden börjar 24 timmar efter det angivna datumet och när alla villkor är uppfyllda.</p> </li> 
         <li> <p>Påminnelsemeddelanden för projekt, uppgifter och utgåvor som utlöses varje kväll vid midnatt i USA Mountain Time. Alla objekt som är berättigade till ett påminnelsemeddelande från den dagen utlöser ett meddelande till de avsedda användarna kort efter den tidpunkten.</p> </li> 
         <li> <p>Påminnelsemeddelanden för tidrapporter skickas vid den angivna tidpunkten baserat på din tidszon och tidrapportens slutdatum, startdatum eller senaste uppdateringsdatum.</p> </li> 
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
        <li><strong>Ofullständigt i aktuella projekt:</strong> (Tillgängligt för påminnelser om aktiviteter och ärenden) Påminnelsemeddelandet schemaläggs att skickas endast när objektstatusen som påminnelsemeddelandet är associerat med inte är Fullständig och projektstatusen är Aktuell.</li> 
        <li><strong>Alla i aktuella projekt:</strong>(Tillgängligt för påminnelser om aktiviteter och utleveranser) Påminnelsemeddelandet schemaläggs att skickas oavsett objektstatus och endast när den projektstatus som påminnelsemeddelandet är associerat med är Aktuell.</li> 
        <li><strong>Ofullständiga projekt:</strong> (Tillgängligt för projektpåminnelser) Påminnelsemeddelandet schemaläggs att skickas när projektstatusen är något annat än Fullständigt.</li> 
        <li><strong>Fullständiga projekt:</strong> (Tillgängligt för projektpåminnelser) Påminnelsemeddelandet schemaläggs att skickas när projektstatusen är Slutförd.</li> 
        <li><strong>Öppna tidrapporter:</strong> (Tillgängligt för tidrapportpåminnelser) Påminnelsemeddelandet schemaläggs att skickas när tidrapportens status är Öppen.</li> 
        <li><strong>Skickade tidrapporter:</strong> (Tillgängligt för tidrapportpåminnelser) Påminnelsemeddelandet schemaläggs att skickas när tidrapportens status har skickats.</li> 
        <li><strong>Öppna tidrapport eller mindre än 40 timmar per vecka:</strong> (Tillgängligt för tidrapportpåminnelser) Påminnelsemeddelandet schemaläggs att skickas när tidrapportens status är Öppen eller när tidrapporten har loggats under 40 timmar.</li> 
        <li><strong>E-postmall:</strong> I listrutan väljer du en e-postmall som ska bifogas påminnelsen.<br>Mer information om hur du skapar en e-postmall finns i <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Konfigurera e-postmallar</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mottagare</td> 
      <td>Välj de typer av användare som du vill ska få meddelandet. Välj bland olika objektintressenter, till exempel ägare, godkännare eller tilldelad.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara**.
1. Bifoga påminnelsemeddelandet till en arbetsuppgift enligt beskrivningen i [Bifoga ett påminnelsemeddelande till ett objekt](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Få en påminnelseavisering

När villkoret är uppfyllt för det objekt som har påminnelsemeddelandet bifogat, utlöses ett e-postmeddelande till användaren som definierats i påminnelsemeddelandet.

Mer information om hur du tar emot påminnelsemeddelanden finns i [Påminnelsemeddelanden](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) avsnitt i [Adobe Workfront-meddelanden](../../../workfront-basics/using-notifications/wf-notifications.md).

## Leverans av testpåminnelsemeddelanden

Påminnelsemeddelanden utlöses varje kväll vid midnatt, Mountain Time. Alla objekt som är kvalificerade för ett påminnelsemeddelande utlöser ett meddelande till de avsedda användarna kort därefter.

Om du vill att påminnelsemeddelanden ska utlösas manuellt måste villkoret för påminnelsen vara uppfyllt.\
Om en påminnelse till exempel är inställd på att utlösa en timme efter det planerade slutförandedatumet för ett projekt, måste den tiden ha passerat mellan den tidpunkt då påminnelsen ställdes in och nu. Projekt som hade planerade slutförandedatum passerade innan påminnelsen aktiverades kommer inte att utlösa något meddelande.

Så här aktiverar du ett påminnelsemeddelande manuellt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System** > **Diagnostik** i det nedre vänstra hörnet av Workfront.

1. Klicka **Skicka påminnelsemeddelanden** och vänta på att de skickas.

   De användare som anges i påminnelsemeddelandet får ett e-postmeddelande.

---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Redigera en godkännandeprocess
description: Om du är Adobe Workfront-administratör, eller har administrativ åtkomst till godkännandeprocesser, kan du se och redigera alla godkännandeprocesser i systemet.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1950'
ht-degree: 0%

---

# Redigera en godkännandeprocess

Om du är Adobe Workfront-administratör, eller har administrativ åtkomst till godkännandeprocesser, kan du se och redigera alla godkännandeprocesser i systemet.

Om du är gruppadministratör kan du se och redigera godkännandeprocesserna som är kopplade till gruppen eller grupperna som du hanterar.

Mer information om hur du skapar godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* När du redigerar en global godkännandeprocess som redan används, påverkar dina ändringar alla objekt i systemet som redan är kopplade till den.
>* Om du lägger till en ny godkännare på det aktuella steget i en godkännandeprocess som redan har startats för ett objekt, återställs processen för det objektet och godkännarna måste börja om.
>
>  Om du gör följande ändringar i en godkännandeprocess som redan har startats för ett objekt fortsätter den processen utan avbrott:
>
>* Lägg till en scen efter den aktuella scenen
>* Lägg till ytterligare en godkännare före den aktuella fasen

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

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
   <td> <p>Administrativ åtkomst till godkännandeprocesser om du inte är systemadministratör</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Redigera en befintlig godkännandeprocess

{{step-1-to-setup}}

1. (Villkorligt) Om du redigerar en godkännandeprocess på systemnivå klickar du på **Processer** > **Godkännanden** i den vänstra panelen.

   eller

   Om du redigerar en godkännandeprocess på gruppnivå gör du följande:

   1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.
   1. Klicka på namnet på gruppen som du vill visa eller hantera gruppgodkännandeprocesser för.
   1. Klicka på **Godkännanden** i den vänstra panelen. Du kan behöva klicka på **Visa fler** först.

1. Klicka på fliken **Projektgodkännanden**, **Uppgiftsgodkännanden** eller **Utfärdandegodkännanden**, beroende på vilken typ av godkännandeprocess du vill redigera.

1. Välj den godkännandeprocess som du vill redigera och klicka sedan på **Redigera** överst i listan. Rutan Redigera godkännandeprocess visas.

   ![](assets/edit-approval-process-global-area-new.png)

1. Ange följande information i rutan som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn på godkännandeprocess</td> 
      <td>Skriv ett beskrivande namn för godkännandeprocessen. Användarna ser det här namnet när de tillämpar godkännandeprocessen på ett objekt, vilket beskrivs i <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associera en ny eller befintlig godkännandeprocess med arbete</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Skriv en beskrivning av godkännandeprocessen. Detta visas i avsnittet <b>Godkännanden</b> i området <b>Inställningar</b> bredvid namnet på godkännandeprocessen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>Låt det här alternativet vara aktiverat om du vill att andra användare ska kunna koppla godkännandeprocessen till projekt, uppgifter och utgåvor som de skapar. </p> <p>Det här alternativet är aktiverat som standard.</p> <p>Tips! Det kan vara bra att markera en godkännandeprocess som inaktiv när organisationen inte längre behöver använda den, men du vill bevara historik om hur den används.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Den här godkännandeprocessen kan användas av </td> 
      <td> <p>Om du vill att godkännandeprocessen ska vara tillgänglig för projekt, uppgifter, utgåvor och mallar som bara tillhör en viss grupp börjar du skriva namnet på gruppen och väljer sedan namnet när den visas:</p> 
       <ul> 
        <li>Om du är systemadministratör eller har administrativ åtkomst till godkännandeprocesser kan du se vilken grupp som helst i systemet när du skriver dess namn. <b>Alla grupper</b> är markerade som standard. </li> 
        <li>Om du är gruppadministratör utan administrativ åtkomst till godkännandeprocesser kan du tilldela godkännandeprocessen till alla grupper som du hanterar när du skriver dess namn. Alternativet <b>Alla grupper</b> är inte tillgängligt.</li> 
       </ul> <p>Det här alternativet är inte tillgängligt för enstaka godkännandeprocesser.</p> <p><b>VARNING</b>: När du gör ändringar i den gruppspecifika godkännandeprocessen kan de befintliga godkännandeprocesserna som redan har associerats med arbetsobjekten ändras. Mer information om de här ändringarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser</a>.</p> <p>Mer information om hur du listar och hanterar gruppens godkännandeprocesser från gruppens sida finns i <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Godkännandeprocesser på gruppnivå</a>. </p> <p>Mer information om administrativ åtkomst till godkännandeprocesser finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurera en sökväg för godkännandeprocessen med följande alternativ.

   En sökväg är den plats där du anger vad som ska hända i godkännandeprocessen. Du skapar faser i en bana för att ange vem som ska utföra godkännandearbetet och i vilken ordning.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Starta godkännandeprocessen när statusen är inställd på</p> </td> 
      <td> <p>Välj den status som ska utlösa godkännandeprocessen för arbetsobjekt. När någon uppdaterar en arbetsuppgift till den här statusen påbörjas godkännandeprocessen. </p> <p>Samma status kan inte väljas för flera godkännandeprocesssökvägar.</p> <p>De tillgängliga statusvärdena baseras på vad som har valts under alternativet <b>Det här godkännandet kan användas av </b> (förklaras i tabellen ovan):</p> 
      <ul> 
      <li> Om <b>Alla grupper</b> har valts är endast låsta statusar som omfattar hela systemet tillgängliga. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Om en viss grupp är markerad är bara de statusar som är tillgängliga för den gruppen tillgängliga</p> </li> 
      </ul> <p>Mer information om hur godkännandeprocesser fungerar med status finns i avsnittet <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Hur godkännandeprocesser bygger på status</a> i artikeln <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Översikt över godkännandeprocessen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scennamn</td> 
      <td>(Valfritt) Skriv ett namn som beskriver banans första steg. Om du inte anger något scennamn är standardnamnet <b>Stage 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännare</td> 
      <td> <p>Börja skriva namnet på den användare, det team eller den jobbroll som du vill utse till godkännare för den här scenen och klicka sedan på namnet när det visas i listrutan. Du kan bara lägga till aktiva användare, jobbroller och team. </p>

   <p><b>TIPS</b>:</p>

   <p>När du lägger till en användare som godkännare ska du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.</p>
      <p>Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Bevilja åtkomst för användare</a></p>.

   <p><b>OBS</b>:

   När du lägger till en användare, ett team eller en roll som godkännare får de inte automatiskt behörighet till objektet som är kopplat till det godkännandet. De får behörigheter till objektet när godkännandesteget aktiveras. Annars måste objekten delas med dem innan de kan fatta ett beslut om godkännande. </p>
   <p>Du kan också utse en person till godkännare genom att ange den enskildes roll. Du kan till exempel tilldela en projektägare, en projektsponsor, en Portfolio-ägare, en programägare eller en projektledare som godkännare. Dessa alternativ visas automatiskt när du börjar skriva.</p> 
      <p><b>VIKTIGT</b>:  
      <ul> 
      <li> När du tilldelar ett godkännande till projektsponsorn och ingen utses till projektledare tilldelas godkännandet till projektägaren. Om ingen har utsetts till projektägare tilldelas Workfront-administratören godkännandet. </li> 
      <li> När du tilldelar ett godkännande till en roll och alternativet <b>Godkännare krävs inte för projektteamet</b> är inaktiverat, men inga roller i projektteamet matchar rollen vid godkännandet, tilldelas godkännandet om till projektägaren. Mer information om godkännandeinställningar finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala godkännandeinställningar</a>.
      </li> 
      <li>När du tilldelar projektägaren ett godkännande och ingen utses till projektägare tilldelas godkännandet till Workfront huvudadministratör enligt anvisningarna i avsnittet Kundinformation i inställningsområdet. Mer information finns i <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Konfigurera grundläggande information för systemet</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>När du tilldelar jobbroller som godkännare kan alla användare som är kopplade till den jobbrollen som också finns i projektteamet fatta ett beslut om godkännandet. </p> 
      <p>När du tilldelar ett team som godkännare kan alla användare i det teamet fatta ett beslut om godkännandet. </p> 
      <p>Mer information om projektteamet finns i <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Översikt över projektteamet</a>. Mer information om hur du godkänner arbete finns i <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Godkänna arbete </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Endast ett beslut krävs</td> 
      <td>(Visas endast om du lägger till flera godkännare på scenen) Välj det här alternativet om någon av godkännarna på scenen kan godkänna eller avvisa arbetsobjektet under den här fasen. Den här åtgärden gör att arbetsobjektet kan lämna scenen.  
      <p>När det här alternativet inte är markerat måste alla identifierade godkännare godkänna eller avvisa scenen (i valfri ordning) innan artikeln lämnar scenen. Om någon av godkännarna avvisar scenen avbryts processen och börjar om så att nödvändiga ändringar kan göras. Sedan kan godkännarna godkänna eller avvisa scenen en gång till.</p> 
      <p>När ett team utses till godkännare kan alla medlemmar i teamet bevilja eller avvisa en fas.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Lägg till fas</p> </td> 
      <td>(Valfritt) Lägg till ytterligare en scen i banan med alternativen som förklaras i de tre raderna ovan. Du kan lägga till så många steg som du behöver i banan.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Välj vad som ska hända när godkännandet avvisas</td> 
      <td> <p>Välj den åtgärd som du vill utföra om arbetsuppgiften avvisas i något skede av sökvägen:</p> 
      <ul> <li><strong>Skapa ett problem</strong>: (Endast tillgängligt för projekt- och uppgiftsgodkännandeprocesser) Ett problem skapas i projektet eller aktiviteten där godkännandeprocessen körs. Den tilldelade standardresursen för aktiviteten eller projektägaren är tilldelad till utgåvan. Som standard är namnet på det skapade problemet <strong>Godkännande nekat (projekt- eller aktivitetsnamn)</strong>. Det här är ett avvisningsproblem som anges under uppgiften eller projektet, beroende på vilken godkännandeprocess som avvisades.</li> 
      <li> <p><strong>Ange status till </strong>: Välj något av följande:</p> 
      <ul> <li><strong>Tidigare status</strong>: Det avvisade projektet, aktiviteten eller problemet återgår till den status som gällde före den status som aktiverar godkännandeprocessen.</li> 
      <li> <p><strong>Annan status i listan</strong>: Det avvisade objektet flyttas till den status du väljer, till exempel Väntande. Du kan välja en av standardstatusarna eller en anpassad status som du har lagt till i ditt Workfront-system.</p> <p>Om du väljer en status som är associerad med en godkännandeprocess som avvisningsstatus för en godkännandesökväg, flyttas det avvisade objektet till den valda statusen och markeras som"Väntar på godkännande".</p>
      <p>Om du t.ex. väljer Väntande som avvisningsstatus och statusen Väntande är associerad med en godkännandeprocess, placeras det avvisade objektet i statusen "Väntar på godkännande", vilket kräver godkännande.</p>    <p>För en systemomfattande godkännandeprocess är endast systemomfattande status tillgängliga.</p> <p>För en gruppspecifik godkännandeprocess är alla gruppstatusar tillgängliga. Detta omfattar alla anpassade statusvärden som gruppadministratören har skapat specifikt för gruppen, samt alla systemomfattande statusvärden. </p> <p>Mer information om hur godkännandeprocesser fungerar med status finns i avsnittet <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Hur godkännandeprocesser bygger på status</a> i artikeln <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Översikt över godkännandeprocessen</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Klicka på **Lägg till sökväg** om du vill lägga till en ny sökväg i godkännandeprocessen, som hänvisar till listan med alternativ i föregående steg.

   Den nya sökvägen måste associeras med en annan status. Sökvägen utlöses när objektet uppdateras för att visa den här statusen. Du kan inte ha två sökvägar för samma status.

1. Klicka på **Spara**.
1. (Valfritt) Gör något av följande:

   * Associera godkännandeprocessen med specifika projekt, uppgifter eller problem i hela systemet, enligt beskrivningen i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Meddela användare utanför Workfront att godkännandeprocessen är tillgänglig så att de kan associera med projekt, uppgifter eller utgåvor, enligt beskrivningen i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Skapa en annan godkännandeprocess som utlöses om den här godkännandeprocessen avvisas och artikeln får en annan status. På så sätt kan ni länka samman godkännandeprocesser.

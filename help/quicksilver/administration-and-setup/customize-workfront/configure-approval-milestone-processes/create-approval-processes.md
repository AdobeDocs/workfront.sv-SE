---
title: Skapa en godkännandeprocess för arbetsobjekt
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Du kan skapa en godkännandeprocess som användare kan koppla till en arbetsuppgift (projekt, uppgift, utleverans, mall eller malluppgift), ett dokument eller ett korrektur. En godkännandeprocess säkerställer att angivna tilldelningar på objektet granskar vissa ändringar innan objektet fortskrider i systemet.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2193'
ht-degree: 0%

---

# Skapa en godkännandeprocess för arbetsobjekt

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

Du kan skapa en godkännandeprocess som användare kan koppla till en arbetsuppgift (projekt, uppgift, utleverans, mall eller malluppgift), ett dokument eller ett korrektur. En godkännandeprocess säkerställer att angivna tilldelningar på objektet granskar vissa ändringar innan objektet fortskrider i systemet.

I den här artikeln beskrivs hur du skapar globala godkännandeprocesser på systemnivå eller gruppnivå för arbetsobjekt (projekt, uppgift, utgåva, mall eller malluppgift).

Mer information om godkännanden som är kopplade till dokument eller korrektur finns i följande artiklar:

* [Begär dokumentgodkännanden](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Användarna kan också skapa en godkännandeprocess för ett projekt, en uppgift, ett ärende, en mall eller en mall där de har behörigheten Hantera.
>
>I den här artikeln används termen&quot;global godkännandeprocess&quot; för att skilja sig från godkännandeprocess för enstaka användning. En global godkännandeprocess kan användas upprepade gånger.
>
>På gruppnivån är en global godkännandeprocess begränsad till arbetsobjekt och statusvärden som tillhör gruppen.
>
>Mer information om godkännandeprocesser för enstaka användning finns i [Översikt över godkännandeprocessen](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) och [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Godkännandeprocess på systemnivå eller för engångsbruk: Alla</p>
   <p>Godkännandeprocess på gruppnivå: Prime eller Ultimate</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard </p>
 <p>eller</p> 
<p>Aktuell: Planera </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Om du är systemadministratör eller har administrativ åtkomst till godkännandeprocesser kan du skapa en godkännandeprocess på systemnivå eller en godkännandeprocess på gruppnivå för en viss grupp.</p> 
   <p>Om du är gruppadministratör kan du skapa godkännandeprocesser på gruppnivå för grupper som du hanterar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en global godkännandeprocess på systemnivå eller gruppnivå för arbetsobjekt

{{step-1-to-setup}}

1. (Villkorligt) Om du skapar en godkännandeprocess på systemnivå klickar du på **Processer** > **Godkännanden** i den vänstra panelen.

   eller

   Om du skapar en godkännandeprocess på gruppnivå klickar du på ikonen **Grupper** ![Grupper](assets/groups-icon.png), klickar på gruppens namn och sedan på **Godkännanden**.

   <!--hidden for the new tab redesign - August 2023: 
   ![Approvals area in setup](assets/approvals-area-in-setup-processes.png)
   -->

1. Välj antingen fliken **Projektgodkännanden**, **Uppgiftsgodkännanden** eller **Utfärdandegodkännanden**.

1. Klicka på **Ny godkännandeprocess**.
1. Ange följande information i rutan som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn på godkännandeprocess</td> 
      <td><p>Skriv ett beskrivande namn för godkännandeprocessen. Användarna ser det här namnet när de tillämpar godkännandeprocessen på ett objekt, vilket beskrivs i <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associera en ny eller befintlig godkännandeprocess med arbete</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td><p>Skriv en beskrivning av godkännandeprocessen. Detta visas i avsnittet <b>Godkännanden</b> i området <b>Inställningar</b> bredvid namnet på godkännandeprocessen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>Låt det här alternativet vara aktiverat om du vill att andra användare ska kunna koppla godkännandeprocessen till projekt, uppgifter och utgåvor som de skapar. </p> <p>Det här alternativet är aktiverat som standard.</p> <p> Tips! Det kan vara bra att markera en godkännandeprocess som inaktiv när organisationen inte längre behöver använda den, men du vill bevara historik om hur den används.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Den här godkännandeprocessen kan användas av </td> 
      <td> <p>Om du vill att godkännandeprocessen ska vara tillgänglig för projekt, uppgifter, utgåvor och mallar som bara tillhör en viss grupp börjar du skriva namnet på gruppen och väljer sedan namnet när den visas:</p> 
       <ul> 
       <li>Om du är systemadministratör eller har administrativ åtkomst till godkännandeprocesser kan du se vilken grupp som helst i systemet när du skriver dess namn. <b>Alla grupper</b> är markerade som standard. </li> 
       <li>Om du är gruppadministratör utan administrativ åtkomst till godkännandeprocesser kan du tilldela godkännandeprocessen till alla grupper som du hanterar när du skriver dess namn. Alternativet <b>Alla grupper</b> är inte tillgängligt.</li> 
       </ul> 
       <p>Det här alternativet är inte tillgängligt för enstaka godkännandeprocesser.</p> 
       <p><b>VARNING</b>: När du gör ändringar i den gruppspecifika godkännandeprocessen kan de befintliga godkännandeprocesserna som redan har associerats med arbetsobjekten ändras. Mer information om de här ändringarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser</a>.</p> 
       <p>Mer information om hur du listar och hanterar gruppens godkännandeprocesser från gruppens sida finns i <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Godkännandeprocesser på gruppnivå</a>. </p> 
       <p>Mer information om administrativ åtkomst till godkännandeprocesser finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> </td> 
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
       <li> Om <b>alla grupper</b> är markerade är endast systemomfattande statusar tillgängliga
       <li> <p>Om en viss grupp är markerad är bara de statusar som är tillgängliga för den gruppen tillgängliga</p> </li> 
       </ul> <p>Mer information om hur godkännandeprocesser fungerar med status finns i avsnittet <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Hur godkännandeprocesser bygger på status</a> i artikeln <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Översikt över godkännandeprocessen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scennamn</td> 
      <td>(Valfritt) Skriv ett namn som beskriver banans första steg. Om du inte anger något scennamn är standardnamnet <b>Stage 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännare</td> 
      <td> <p>Börja skriva namnet på den användare, det team eller den jobbroll som du vill utse till godkännare för den här scenen och klicka sedan på namnet när det visas i listrutan. Du kan bara lägga till aktiva användare, <span>jobbroller</span> och team. </p>

   <p><b>TIPS</b>:</p>

   <p>När du lägger till en användare som godkännare ska du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.</p>
      <p>Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Bevilja åtkomst för användare</a>. </p>

   <p><b>OBS</b>:

   När du lägger till en användare, ett team eller en roll som godkännare får de inte automatiskt behörighet till objektet som är kopplat till det godkännandet. De får behörigheter till objektet när godkännandesteget aktiveras. Annars måste objekten delas med dem innan de kan fatta ett beslut om godkännande. </p> <p>Du kan också utse en person till godkännare genom att ange den enskildes roll. Du kan till exempel tilldela en projektägare, en projektsponsor, en Portfolio-ägare, en programägare eller en projektledare som godkännare. Dessa alternativ visas automatiskt när du börjar skriva.</p>

   <p><b>VIKTIGT</b>:  
       <ul> 
       <li> <p>När du tilldelar ett godkännande till projektsponsorn och ingen utses till projektledare tilldelas godkännandet till projektägaren. Om ingen har utsetts till projektägare tilldelas Workfront-administratören godkännandet. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>När du tilldelar ett godkännande till en roll och <b>Godkännaren behöver inte vara i projektteamet (för godkännandeprocesser som innehåller en roll)</b> är inaktiverad, men det finns inga roller i projektteamet som matchar rollen i godkännandet, tilldelas godkännandet om till projektägaren. Mer information om godkännandeinställningar finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurera globala godkännandeinställningar</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>När du tilldelar projektägaren ett godkännande och ingen utses till projektägare tilldelas godkännandet till Workfront huvudadministratör enligt anvisningarna i avsnittet Kundinformation i inställningsområdet. Mer information finns i <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Konfigurera grundläggande information för systemet</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>Du kan upprepa den här processen om du vill lägga till flera godkännare på scenen. I ett och samma steg kan en kombination av användare, team och jobbroller ingå som godkännare. Det finns ingen gräns för hur många godkännare du kan lägga till på en scen.</p> <p><b>VIKTIGT</b>:  <p>När du tilldelar jobbroller som godkännare kan alla användare som är kopplade till den jobbrollen som också finns i projektteamet fatta ett beslut om godkännandet. </p> <p>När du tilldelar ett team som godkännare kan alla användare i det teamet fatta ett beslut om godkännandet. </p> <p>Mer information om projektteamet finns i <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Översikt över projektteamet</a>. Mer information om hur du godkänner arbete finns i <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Godkänna arbete </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endast ett beslut krävs <br> <br> (visas bara om du lägger till flera godkännare på scenen) </td> 
      <td> <p>Välj det här alternativet om någon av godkännarna på scenen kan godkänna eller avvisa arbetsuppgiften under den här fasen. Den här åtgärden gör att arbetsobjektet kan lämna scenen. </p> <p>När det här alternativet inte är markerat måste alla identifierade godkännare godkänna eller avvisa scenen (i valfri ordning) innan artikeln lämnar scenen. Om någon av godkännarna avvisar scenen avbryts processen och börjar om så att nödvändiga ändringar kan göras. Sedan kan godkännarna godkänna eller avvisa scenen en gång till.</p> <p>När ett team utses till godkännare kan alla medlemmar i teamet bevilja eller avvisa en fas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Lägg till fas</p> </td> 
      <td><p>(Valfritt) Lägg till ytterligare en scen i banan med alternativen som förklaras i de tre raderna ovan. Du kan lägga till så många steg som du behöver i banan.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Välj vad som ska hända när godkännandet avvisas</p> </td> 
      <td> <p>Välj den åtgärd som du vill utföra om arbetsuppgiften avvisas i något skede av sökvägen:</p> 
       <ul> 
       <li><b>Skapa ett problem</b>: (Endast tillgängligt för projekt- och uppgiftsgodkännandeprocesser) Ett problem skapas i projektet eller aktiviteten där godkännandeprocessen körs. Den tilldelade standardresursen för aktiviteten eller projektägaren är tilldelad till utgåvan. Som standard är namnet på det skapade problemet <b>Godkännande nekat (&lt;projekt- eller aktivitetsnamn&gt;)</b>. Det här är ett avvisningsproblem som anges under uppgiften eller projektet, beroende på vilken godkännandeprocess som avvisades.</li> 
       <li> <p><b>Ange status till </b>: Välj något av följande:</p> 
       <ul> 
       <li><b>Tidigare status</b>: Det avvisade projektet, aktiviteten eller problemet återgår till den status som gällde före den status som aktiverar godkännandeprocessen.</li> 
       <li><p><b>Annan status i listan</b>: Det avvisade objektet flyttas till den status du väljer, till exempel Väntande. Du kan välja en av standardstatusarna eller en anpassad status som du har lagt till i ditt Workfront-system.</p>
       <p>Om du väljer en status som är associerad med en godkännandeprocess som avvisningsstatus, flyttas det avvisade objektet till den valda statusen och markeras som"Väntande godkännande".</p> 
       <p> Om du t.ex. väljer Väntande som avvisandestatus och statusen Väntande är associerad med en godkännandeprocess, placeras det avvisade objektet i statusen "Väntande - godkännande", vilket kräver godkännande.</p>

   </tr> 
    </tbody> 
   </table>

1. (Valfritt) Klicka på **Lägg till sökväg** om du vill lägga till en ny sökväg i godkännandeprocessen, som hänvisar till listan med alternativ i föregående steg.

   Den nya sökvägen måste associeras med en annan status. Sökvägen utlöses när objektet uppdateras för att visa den här statusen. Du kan inte ha två sökvägar för samma status.

1. Klicka på **Spara**.
1. Nu när godkännandeprocessen har skapats kan du fortsätta med något av följande:

   * Associera godkännandeprocessen med specifika projekt, uppgifter eller problem i hela systemet, enligt beskrivningen i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Meddela användare utanför Workfront att godkännandeprocessen är tillgänglig så att de kan associera med projekt, uppgifter eller utgåvor, enligt beskrivningen i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Skapa en annan godkännandeprocess som utlöses om den här godkännandeprocessen avvisas och artikeln får en annan status. På så sätt kan ni länka samman godkännandeprocesser.

Mer information om hur du redigerar en godkännandeprocess finns i [Redigera en godkännandeprocess](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Associera en godkännandeprocess med en arbetsuppgift

När du vill skapa en godkännandeprocess för en arbetsuppgift (projekt, uppgift eller utgåva)

1. Skapa godkännandeprocessen först
1. Skapa arbetsuppgiften
1. Associera godkännandeprocessen med arbetsuppgiften

Instruktioner om hur du associerar en godkännandeprocess med en arbetsuppgift finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Alla Workfront-användare som hanterar behörigheter för ett projekt, en uppgift eller ett problem kan skapa godkännandeprocesser som bara kan användas på det objekt de skapats i. Mer information finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Möjliggöra för användare att ändra globala godkännandeprocesser för en enskild arbetsuppgift

Som standard kan användare som har behörighet att hantera projekt, uppgifter och problem skapa godkännandeprocesser för dem. Mer information om hur du lägger till godkännandeprocesser för enstaka användning i projekt, uppgifter och utgåvor finns i avsnittet [Associera en godkännandeprocess för enstaka användning med ett projekt, en uppgift, ett ärende, en mall eller en malluppgift](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) i artikeln [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Användare kan också ändra inställningar för en global godkännandeprocess som är kopplad till en arbetsuppgift. De här ändringarna påverkar bara det projekt, den uppgift eller det problem som är kopplat till godkännandeprocessen på systemnivå. Mer information finns i avsnittet [Ändra en global godkännandeprocess för ett specifikt objekt](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) i artikeln [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)).

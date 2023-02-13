---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Skapa ett avancerat korrektur med ett automatiserat arbetsflöde
description: Ett automatiserat arbetsflöde gör det enklare att hantera granskningsprocessen om processen är komplex, eller om du skickar innehåll för granskning till samma personer regelbundet. Beviset flyttas från scen till scen och Adobe Workfront meddelar varje användare när det är deras tur att granska det. Mer information om automatiserade arbetsflöden finns i Översikt över automatiserat arbetsflöde.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# Skapa ett avancerat korrektur med ett automatiserat arbetsflöde

Ett automatiserat arbetsflöde gör det enklare att hantera granskningsprocessen om processen är komplex, eller om du skickar innehåll för granskning till samma personer regelbundet. Beviset flyttas från scen till scen och Adobe Workfront meddelar varje användare när det är deras tur att granska det. Mer information om automatiserade arbetsflöden finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Markera eller högre</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Valfritt (Du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för korrektur </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan, roll eller behörighetsprofil du har kontaktar du Workfront- eller Workfront-administratören.

## Skapa ett avancerat korrektur med ett automatiserat arbetsflöde

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på **Dokument** -fliken.
1. Klicka **Lägg till ny** > Korrektur, ladda upp innehållet och gå igenom avsnitten nedan.

   eller

   Håll pekaren över ett befintligt dokument och klicka sedan på **Skapa korrektur** > **Avancerat korrektur** och arbeta igenom avsnitten nedan.

## Konfigurera korrekturfaser

1. Välj **Automatiserad**.
1. (Valfritt) Om du vill använda en mall för automatiserat arbetsflöde som din Workfront-administratör har skapat och delat med dig klickar du på **Lägg till mall** markerar du mallen i rutan som visas och klickar sedan på **Lägg till mall**.

   >[!NOTE]
   >
   >Tänk på följande när du använder en mall för automatiserat arbetsflöde:
   >   
   >* Inställningarna i en mall för automatiserat arbetsflöde avgör vad du kan göra med det automatiserade arbetsflödet för ett korrektur. Om till exempel knappen Lägg till en scen är inaktiverad i mallen visas den inte när du arbetar med inställningarna för det automatiska arbetsflödet för korrekturet.
   * När en person läggs till i en bild i en mall för automatiserat arbetsflöde, men redan finns som granskare i korrekturet, tas granskaren bort från scenen när mallen används. Om du inte lägger till någon annan granskare på scenen visas ett meddelande som ber dig att lägga till en.
   * Din möjlighet att ändra en mall för automatiserat arbetsflöde beror på mallinställningarna som konfigurerats av Workfront-administratören, vilket beskrivs i . Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.


1. Konfigurera det första steget i det automatiserade arbetsflödet:

   1. (Valfritt) Om du vill skapa ett namn för den första scenen klickar du på **Steg 1** och skriv sedan namnet.
   1. I **Mottagare** för scenen lägger du till granskare på scenen.

      >[!NOTE]
      Tänk på följande när du lägger till granskare på en scen:
      * Du kan lägga till externa användare på en scen med en e-postadress.
      * När du har lagt till en användare på en scen kan du konfigurera inställningarna för den användaren på korrekturet.
      * Du kan dra användare direkt till en annan scen eller dra användare till en scen på **Steg** diagram. Om du vill markera flera användare trycker du på Skift+Ctrl (Windows) eller Skift+Kommando (Mac).
      * Du kan bara lägga till en granskare i ett korrektur en gång, vilket betyder att du inte kan lägga till samma person i mer än en fas i korrekturet.
      * Granskare som inte har lagts till på en privat scen kan inte se den scenen på det korrektur eller de kommentarer som har gjorts på den scenen.
      * Om du lägger till en användare på en scen får användaren som standard åtkomst till korrekturet från det att korrekturet skapas.\
         Din Workfront-administratör kan hindra användare från att komma åt korrekturet tills arbetsflödet går in på den scen där användaren lades till.


   1. Klicka **Sceninställningar**.
   1. Klicka på en **Aktivera fas** för att ange hur du vill att scenen ska aktiveras.

      För den första scenen kan du bara välja **Vid korrekturskapande**, **På ett visst datum och en viss tid**, eller **Manuellt**.

   1. (Villkorligt) Om du har valt **På ett visst datum och en viss tid** i föregående steg väljer du det datum och den tidpunkt då du vill aktivera scenen i **Aktivera den** som visas.

   1. Använd något av alternativen nedan om du vill konfigurera scenen ytterligare.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Ange slutdatum för fas</td>
         <td><p>Klicka på ett alternativ i dialogrutan <strong>Deadline-alternativ</strong> nedrullningsbar lista. Sedan, under <strong>Deadline</strong>gör du något av följande:</p>
          <ul>
           <li>Om du valde <strong>Ange specifikt datum</strong>: Välj önskat datum och klockslag för deadline.</li>
           <li>Om du valde <strong>Beräkna från aktiveringsdatum för fas</strong>: Välj det antal arbetsdagar du vill lägga till i scenens aktiveringsdatum för att bestämma tidsgränsen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Lås scen</td>
         <td>Ange när scenen kan låsas. </td>
        </tr>
        <tr>
         <td role="rowheader">Överför primära beslutsrättigheter till</td>
         <td><p>Välj den primära beslutsfattaren på scenen (endast tillgänglig efter att du har lagt till minst en person på scenen som har rollen Korrektur som godkännare eller högre). Om du väljer en primär beslutsfattare <strong>Endast ett beslut krävs</strong> är inaktiverat på den här scenen.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Kräv endast ett beslut för det här steget</td>
         <td>Slutför hela granskningsprocessen när en av beslutsfattarna fattar ett beslut.<p>Det här alternativet är inte tillgängligt om du har angett en användare i <strong>Primär beslutsfattare</strong>nedrullningsbar meny.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Gör det här steget privat</td>
         <td>Tillåter endast följande personer att visa kommentarer och beslut som fattats under den här fasen: Administratörer, Workfront-administratörer och Workfront korrekturadministratörer</td>
        </tr>
       </tbody>
      </table>

1. Så här lägger du till och konfigurerar en annan scen:

   1. Klicka **Ny fas**.
   1. (Valfritt) Om du vill skapa ett namn för den första scenen klickar du på **Steg 2** (eller **Steg 3**, **Steg 4** och så vidare) skriver du namnet.

   1. Klicka på **Aktivera fas** väljer du sedan ett alternativ för att ange om scenen ska aktiveras automatiskt eller manuellt.

      Förutom alternativen **Vid korrekturskapande**, **På ett visst datum och en viss tid**, eller **Manuellt** kan du välja ett alternativ som är beroende av vad som inträffade i föregående steg:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Om du har valt ett alternativ för att aktivera fas som är beroende av vad som inträffade i föregående steg, använder du de alternativ som visas för att konfigurera aktiveringsinställningen.

      Om du till exempel har valt **När status för föregående fas ändras** väljer du **Föregående fas** väljer du sedan status i **Status ändrad till** box.

1. Upprepa föregående steg om det behövs för att lägga till fler steg.

   När du lägger till faser i det automatiserade arbetsflödet visas ett diagramformulär på skärmen som representerar dem:

   ![](assets/stages-diagram-350x213.png)

1. Fortsätt med [Konfigurera e-postinställningar för korrekturet](#configure-email-settings-for-the-proof) nedan.

## Konfigurera e-postinställningar för korrekturet {#configure-email-settings-for-the-proof}

1. I **E-postmeddelande** väljer du om du vill skicka e-postmeddelanden och ett anpassat meddelande till de användare som du markerade i [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](#workflow) tidigare i den här artikeln:

   <table>
      <tbody>
      <tr>
      <td>Meddela mottagarna om det här beviset</td>
      <td>Välj det här alternativet om du vill skicka ett e-postmeddelande till användarna. När <strong>Grundläggande delning</strong> är markerat i <strong>Arbetsflöde</strong> skickas ett e-postmeddelande när korrekturet skapas. När <strong>Automatiserat arbetsflöde</strong> är markerat i <strong>Arbetsflöde</strong> skickas ett e-postmeddelande när korrekturet kommer in i det automatiserade arbetsflöde som användaren är kopplad till.</td>
      </tr>
      <tr>
      <td>Lägg till anpassat meddelande</td>
      <td>Välj det här alternativet om du vill inkludera ett anpassat meddelande i meddelandet. Du kan ange ämne och meddelandetext. Meddelandetexten kan innehålla formaterad text, t.ex. fet stil, punkter och hyperlänkar.</td>
      </tr>
      </tbody>
      </table>


1. Fortsätt med [Konfigurera korrekturinställningar](#configure-proof-settings) nedan.

## Konfigurera korrekturinställningar {#configure-proof-settings}

1. I **Korrekturinställningar** väljer du något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kräv inloggning - korrektur kan bara delas med andra användare</td> 
      <td>När det här alternativet är inaktiverat (standard) kan alla med URL-adressen visa korrekturet. <br>När det här alternativet är markerat:
       <ul>
        <li>Det är bara Workfront korrekturläsare som kan visa korrekturet.</li>
        <li>Användarna kan inte logga in på korrekturet om de inte har lagts till i korrekturet.</li>
        <li>Det går inte att aktivera prenumerationer.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endast ett beslut krävs för det här beviset</td> 
      <td>När det här alternativet har valts slutförs granskningen efter det att en av beslutsfattarna har fattat sitt beslut.<br>Det här alternativet är inaktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv att beslut signeras elektroniskt</td> 
      <td>Användarna måste ange sitt användarnamn och lösenord när de fattar beslut om ett korrektur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås korrektur när alla nödvändiga beslut har fattats</td> 
      <td>När den här inställningen är aktiverad låses korrekturläget när alla beslut har fattats. Läget ändras automatiskt från olåst till låst när den slutliga godkännaren fattar sitt beslut.<br>Det här alternativet är inaktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hämta originalfil</td> 
      <td>När det här alternativet är markerat kan granskarna hämta originalfilen som korrekturet skapades från.<br>När det här alternativet är avmarkerat visas inte längre ikonen Hämta.<br>Det här alternativet är aktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prenumerera på korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan personer som inte har lagts till explicit i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:
       <ul>
        <li><strong>Abonnentroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet. </li>
        <li><strong>Inställningar för e-postavisering för prenumeranter:</strong> Standardvarningsmeddelandet som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomstbevis via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till beviset. Du kan välja <strong>Ingen e-post</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>Endast e-postmeddelanden med korrektur</strong> (prenumeranten får en länk till beviset via e-post utan verifiering) eller <strong>E-postmeddelanden om validering och korrektur</strong> (prenumeranten får en länk till beviset via e-post och måste klicka på länken för att få tillgång till ett bevis. Syftet med det här alternativet är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till).</li>
        </ul><p><strong>Obs!</strong> Om korrekturet har ett automatiserat arbetsflöde bifogat, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Skapa korrektur**.

   Workfront börjar generera ett korrektur av de valda dokumenten eller webbplatserna. Beroende på filstorlek och typ kan fördröjningen för en dokumentöverföring variera. Ha tålamod när större filer tar längre tid att generera. Du kan navigera bort från sidan och Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.

1. När korrekturet har skapats klickar du på **Öppna korrektur** för att starta korrekturläsaren.

   ![](assets/open-proof-350x132.png)

   Användare som inte har språkkontroll aktiverat på sitt konto kan fortfarande visa dokumentet och kommentera korrekturet [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)

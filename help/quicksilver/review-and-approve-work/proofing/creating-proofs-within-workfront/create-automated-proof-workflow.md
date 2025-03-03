---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Skapa ett avancerat korrektur med ett automatiserat arbetsflöde
description: Ett automatiserat arbetsflöde gör det enklare att hantera granskningsprocessen om processen är komplex, eller om du skickar innehåll för granskning till samma personer regelbundet. Beviset flyttas från scen till scen och Adobe Workfront meddelar varje användare när det är deras tur att granska det. Mer information om automatiserade arbetsflöden finns i Översikt över automatiserat arbetsflöde.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# Skapa ett avancerat korrektur med ett automatiserat arbetsflöde

<!-- Audited: 2/2024 -->

Ett automatiserat arbetsflöde gör det enklare att hantera granskningsprocessen om processen är komplex, eller om du skickar innehåll för granskning till samma personer regelbundet. Beviset flyttas från scen till scen och Adobe Workfront meddelar varje användare när det är deras tur att granska det. Mer information om automatiserade arbetsflöden finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Nytt: Alla</p><p>Aktuell plan: Pro eller högre</p><p>Äldre plan: Välj eller högre</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard</p><p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett avancerat korrektur med ett automatiserat arbetsflöde

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på fliken **Dokument** .
1. Klicka på **Lägg till nytt** > Korrektur, ladda upp innehållet och arbeta sedan igenom avsnitten nedan.

   eller

   Håll muspekaren över ett befintligt dokument, klicka på **Skapa korrektur** > **Avancerat korrektur** och gå igenom avsnitten nedan.

## Konfigurera korrekturfaser

1. Välj **Automatiserad** i avsnittet Arbetsflödestyp.
1. (Valfritt) Om du vill använda en mall för automatiserat arbetsflöde som din Workfront-administratör har skapat och delat med dig klickar du på **Lägg till mall**, markerar mallen i rutan som visas och klickar sedan på **Lägg till mall**.

   >[!NOTE]
   >
   >Tänk på följande när du använder en mall för automatiserat arbetsflöde:
   >   
   >* Inställningarna i en mall för automatiserat arbetsflöde avgör vad du kan göra med det automatiserade arbetsflödet för ett korrektur. Om till exempel knappen Lägg till en scen är inaktiverad i mallen visas den inte när du arbetar med inställningarna för det automatiska arbetsflödet för korrekturet.
   >* När en person läggs till i en bild i en mall för automatiserat arbetsflöde, men redan finns som granskare i korrekturet, tas granskaren bort från scenen om mallen används. Om du inte lägger till någon annan granskare på scenen visas ett meddelande som ber dig att lägga till en.
   >* Din möjlighet att ändra en mall för automatiserat arbetsflöde beror på mallinställningarna som konfigurerats av Workfront-administratören, vilket beskrivs i . Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.

1. Konfigurera det första steget i det automatiserade arbetsflödet:

   1. (Valfritt) Om du vill skapa ett namn för den första scenen klickar du på **Scen 1** och skriver sedan namnet.
   1. Lägg till granskare på scenen i avsnittet **Mottagare** för scenen.

      >[!NOTE]
      >
      >Tänk på följande när du lägger till granskare på en scen:
      >   
      >* Du kan lägga till externa användare på en scen med en e-postadress.
      >* När du har lagt till en användare på en scen kan du konfigurera inställningarna för den användaren på korrekturet.
      >* Du kan dra användare direkt till en annan scen eller dra användare till en scen i diagrammet **Steg**. Om du vill markera flera användare trycker du på Skift+Ctrl (Windows) eller Skift+Kommando (Mac).
      >* Du kan bara lägga till en granskare i ett korrektur en gång, vilket betyder att du inte kan lägga till samma person i mer än en fas i korrekturet.
      >* Granskare som inte har lagts till på en privat scen kan inte se den scenen på det korrektur eller de kommentarer som har gjorts på den scenen.
      >* Om du lägger till en användare på en scen får användaren som standard åtkomst till korrekturet från det att korrekturet skapas. Din Workfront-administratör kan hindra användare från att komma åt korrekturet tills arbetsflödet går in på den scen där användaren lades till.

   1. Klicka på **Sceninställningar**.
   1. Klicka på ett **Aktivera stadium**-alternativ för att ange hur du vill att scenen ska aktiveras.

      I det första steget kan du bara välja **Vid korrekturskapande**, **Vid ett visst datum och en viss tid** eller **Manuellt**.

   1. (Villkorligt) Om du valde **På ett visst datum och en viss tid** i det föregående steget, markerar du det datum och den tidpunkt då du vill aktivera scenen i rutan **Aktivera den** som visas.

   1. Använd något av alternativen nedan om du vill konfigurera scenen ytterligare.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Ange slutdatum för fas</td>
         <td><p>Om du vill ange en deadline för scenen klickar du på ett alternativ i listrutan <strong>Deadline-alternativ</strong> . Gör sedan något av följande under <strong>Deadline</strong>:</p>
          <ul>
           <li>Om du väljer <strong>Ange specifikt datum</strong>: Välj önskat datum och önskad tid för deadline.</li>
           <li>Om du väljer <strong>Beräkna från fasens aktiveringsdatum</strong>: Välj det antal arbetsdagar som du vill lägga till i scenens aktiveringsdatum för att fastställa tidsgränsen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Lås scen</td>
         <td>Ange när scenen kan låsas. </td>
        </tr>
        <tr>
         <td role="rowheader">Överför primära beslutsrättigheter till</td>
         <td><p>Välj den primära beslutsfattaren på scenen (endast tillgänglig efter att du har lagt till minst en person på scenen som har rollen Korrektur som godkännare eller högre). Om du väljer en primär beslutsfattare är alternativet <strong>Endast ett beslut krävs</strong> inaktiverat på den här fasen.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Kräv endast ett beslut för det här steget</td>
         <td>Slutför hela granskningsprocessen när en av beslutsfattarna fattar ett beslut.<p>Det här alternativet är inte tillgängligt om du har angett en användare i listrutan <strong>Primär beslutsfattare</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Gör det här steget privat</td>
         <td>Endast följande personer kan se kommentarer och beslut som fattas under den här fasen: Supervisors, Workfront administrators och Workfront Proof administrators</td>
        </tr>
       </tbody>
      </table>

1. Så här lägger du till och konfigurerar en annan scen:

   1. Klicka på **Nytt stadium**.
   1. (Valfritt) Om du vill skapa ett namn för den första scenen klickar du på **scen 2** (eller **scen 3**, **scen 4** och så vidare) och skriver sedan namnet.

   1. Klicka på **Aktivera steg** och välj sedan ett alternativ som anger om scenen aktiveras automatiskt eller manuellt.

      Förutom alternativen **Vid korrekturskapande**, **På ett visst datum och en viss tid** eller **Manuellt** kan du välja ett alternativ som är beroende av vad som inträffade i föregående steg:

      ![Aktivera scenalternativ](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Om du har valt ett alternativ för att aktivera fas som är beroende av vad som inträffade i föregående steg, använder du de alternativ som visas för att konfigurera aktiveringsinställningen.

      Om du till exempel valde **När status för föregående fas ändras** markerar du **föregående stadium** och väljer sedan statusen i rutan **Status ändrad till**.

1. Upprepa föregående steg om det behövs för att lägga till fler steg.

   När du lägger till faser i det automatiserade arbetsflödet visas ett diagramformulär på skärmen som representerar dem:

   ![Deldiagram](assets/stages-diagram-350x213.png)

1. Fortsätt med [Konfigurera e-postinställningar för korrekturet](#configure-email-settings-for-the-proof) nedan.

## Konfigurera e-postinställningar för korrekturet {#configure-email-settings-for-the-proof}

1. I avsnittet **E-postmeddelande** väljer du om du vill skicka e-postmeddelanden och ett anpassat meddelande till de användare du valde i [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](#workflow) tidigare i den här artikeln:

   <table>
      <tbody>
      <tr>
      <td>Meddela mottagarna om det här beviset</td>
      <td>Välj det här alternativet om du vill skicka ett e-postmeddelande till användarna. När <strong>Grundläggande delning</strong> har valts i avsnittet <strong>Arbetsflöde</strong> skickas ett e-postmeddelande när korrekturet skapas. När <strong>Automatiskt arbetsflöde</strong> har valts i avsnittet <strong>Arbetsflöde</strong> skickas ett e-postmeddelande när korrekturet kommer in i det automatiserade arbetsflöde som användaren är kopplad till.</td>
      </tr>
      <tr>
      <td>Lägg till anpassat meddelande</td>
      <td>Välj det här alternativet om du vill inkludera ett anpassat meddelande i meddelandet. Du kan ange ämne och meddelandetext. Meddelandetexten kan innehålla formaterad text, t.ex. fet stil, punkter och hyperlänkar.</td>
      </tr>
      </tbody>
      </table>


1. Fortsätt med [Konfigurera korrekturinställningar](#configure-proof-settings) nedan.

## Konfigurera korrekturinställningar {#configure-proof-settings}

1. Välj något av följande alternativ i avsnittet **Korrekturinställningar**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kräv inloggning - korrektur kan bara delas med andra användare</td> 
      <td>När det här alternativet är inaktiverat (standard) kan alla med URL-adressen visa korrekturet. <br>När det här alternativet är markerat:
       <ul>
        <li>Endast Workfront Proof-användare kan visa korrekturet.</li>
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
      <td>När det här alternativet är markerat kan granskarna hämta originalfilen som korrekturet skapades från.<br>När det här alternativet är avmarkerat visas inte längre hämtningsikonen.<br>Det här alternativet är aktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prenumerera på korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan personer som inte har lagts till explicit i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:
       <ul>
        <li><strong>Prenumerantroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet.</li>
        <li><strong>E-postaviseringsinställningar för prenumeranter:</strong> Standardaviseringen för e-post som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomst via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till korrekturet. Du kan välja <strong>Inget e-postmeddelande</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>E-postmeddelande för korrektur endast</strong> (prenumeranten får en länk till korrekturet via e-post utan någon verifiering) eller <strong>E-postmeddelanden för validering och korrekturet </strong> (prenumeranten får en länk till korrekturet och måste klicka på ett bevis. Syftet med det här alternativet är att se till personen har angett korrekt e-postadress som de har tillgång till).</li>
        </ul><p><strong>Obs!</strong> Om korrektur har bifogat ett automatiskt arbetsflöde, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skapa bevis**.

   Workfront börjar generera ett korrektur av de valda dokumenten eller webbplatserna. Beroende på filstorlek och typ kan fördröjningen för en dokumentöverföring variera. Ha tålamod när större filer tar längre tid att generera. Du kan navigera bort från sidan och Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.

1. När korrekturet har skapats klickar du på **Öppna korrektur** för att starta korrekturläsaren.

   ![Öppna korrektur](assets/open-proof-350x132.png)

   Användare som inte har språkkontroll aktiverat på sitt konto kan fortfarande visa dokumentet och kommentera korrekturet [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)

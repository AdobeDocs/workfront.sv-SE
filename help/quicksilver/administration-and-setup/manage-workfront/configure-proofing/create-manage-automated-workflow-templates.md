---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Skapa och hantera automatiska arbetsflödesmallar
description: Som Adobe Workfront-administratör kan du skapa automatiska arbetsflödesmallar som innehåller de granskare som har korrekturroller och meddelandeinställningar som du anger, om ditt företags innehållsgranskningsprocess ofta upprepas eller innehåll ofta granskas av samma personer. En mall för automatiserat arbetsflöde kan vara enkel med bara en eller två granskare eller komplex med många faser och beroenden.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# Skapa och hantera automatiska arbetsflödesmallar

Som Adobe Workfront-administratör kan du skapa automatiska arbetsflödesmallar som innehåller de granskare som har korrekturroller och meddelandeinställningar som du anger, om ditt företags innehållsgranskningsprocess ofta upprepas eller innehåll ofta granskas av samma personer. En mall för automatiserat arbetsflöde kan vara enkel med bara en eller två granskare eller komplex med många faser och beroenden.

Automatiserade arbetsflödesmallar gör det enkelt att skapa ett korrektur med ett automatiserat arbetsflöde. När en användare skapar ett korrektur väljer han eller hon bara den mall han eller hon behöver.

Du kan enkelt ändra alla automatiska arbetsflödesmallar, lägga till eller ta bort granskare och faser när som helst. Och korrekturläsare som använder mallen kan lägga till eller ta bort granskare för korrekturet.

Tänk på följande när du använder en mall för automatiserat arbetsflöde:

1. Inställningarna i en mall för automatiserat arbetsflöde avgör vad du kan göra med det automatiserade arbetsflödet för ett korrektur. Om till exempel knappen Lägg till en scen är inaktiverad i mallen visas den inte när du arbetar med inställningarna för det automatiska arbetsflödet för korrekturet.
1. När en person läggs till i en bild i en mall för automatiserat arbetsflöde, men redan finns som granskare i korrekturet, tas granskaren bort från scenen när mallen används. Om du inte lägger till någon annan granskare på scenen visas ett meddelande som ber dig att lägga till en.
1. Din möjlighet att ändra en mall för automatiserat arbetsflöde beror på mallinställningarna som konfigurerats av Workfront-administratören, vilket beskrivs i . Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.

Mer information om automatiserade arbetsflöden finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Premium eller Select</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Valfritt (Du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administratör måste vara markerat i din behörighetsprofil för korrektur. Mer information finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurera en användares språkkontroll</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en mall för automatiserat arbetsflöde

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.
1. Klicka **Arbetsflöden** i den vänstra panelen.
1. På **Arbetsflöde** flik, klicka **Nytt** > **Ny mall**.

1. I **Detaljer** anger du följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mallnamn</td> 
      <td>(Obligatoriskt) Skriv ett namn på mallen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mallägare</td> 
      <td>Du kan välja den Workfront-administratör eller Workfront Proof-administratör som ska hantera mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mallgrupp</td> 
      <td> <p> Om organisationens automatiserade arbetsflöden är ordnade i grupper kan du välja namnet på gruppen. Se <a href="#create-automated-workflow-template-groups" class="MCXref xref">Skapa mallgrupper för automatiserat arbetsflöde</a> senare i den här artikeln om du vill ha mer information.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Tidszon för mall </td> 
      <td> <p>Standardtidszonen för mallen är den som du arbetar i. Om tidszonen för de som skapar korrektur och granskare som ska använda mallen är olika, kan du ändra den här för att säkerställa att deadlines för scenen ställs in vid rätt tidpunkt för dessa användare. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt</td> 
      <td> <p>Du kan välja de scenaktiviteter som du vill ska vara tillgängliga för personen som skapar korrektur med hjälp av mallen.</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. I **Steg** konfigurerar du varje steg i mallen för automatiserat arbetsflöde.

   Du kan lägga till flera faser och skapa mellan dem.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>Scennamnet visas i det automatiserade arbetsflödesdiagrammet längst upp i avsnittet Arbetsflöde, på sidan Korrekturinformation och i e-postmeddelanden som skickas till granskarna.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera fas</td> 
      <td> <p>Ange om scenen aktiveras automatiskt eller manuellt. För den första fasen kan du välja <strong>Vid korrekturskapande</strong>, <strong>På ett visst datum och en viss tid</strong>, eller <strong>Manuellt</strong>.</p> <p>De andra alternativen blir tillgängliga när du lägger till en andra scen eftersom de kräver att du väljer en överordnad scen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deadline beräknad utifrån</td> 
      <td> <p>Ange hur du vill att tidsgränsen ska beräknas:</p> 
       <ul> 
        <li> <p><strong>Korrektur</strong>: I listrutan under <strong>Deadline (+ arbetsdagar)</strong>väljer du antalet arbetsdagar du vill lägga till i datumet då korrekturet skapades för att automatiskt ange en deadline för korrekturet.</p> </li> 
        <li><strong>När scenen startar</strong>: I listrutan under <strong>Deadline (+ arbetsdagar)</strong>väljer du antalet arbetsdagar som du vill lägga till till i scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås scen</td> 
      <td>Ange om du vill tillåta att scenen låses för kommentarer. Alternativen är att låsa en scen manuellt eller automatiskt, antingen när nästa fas startar eller när alla beslut fattas på den överordnade scenen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primär beslutsfattare</td> 
      <td> <p>De tillgängliga beslutsfattarna visas i listan först när du har lagt till granskarna på scenen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endast ett beslut krävs</td> 
      <td>Granskningsprocessen för etappen kommer att slutföras så snart en av beslutsfattarna har lagt fram sitt beslut. Mer information finns i <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurera korrekturinställningar i Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privat fas</td> 
      <td>Döljer kommentarer och beslut från personer som inte har lagts till på scenen eller som inte är Workfront-administratörer&lt;!&gt;— DRAT I FLARE: Tillsynsmyndigheter och högre

       -->. Mer information finns i &lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>Översikt över automatiserat arbetsflöde&lt;/a>.&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">Tillåt inte att den här fasen tas bort</td> 
      <td> <p>Gör scenen obligatorisk.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Om korrektur som ska använda den här mallen alltid skickas till samma personer på scenen, lägger du till dem här så att användarna inte behöver lägga till dem varje gång de skapar ett korrektur.

   Välj varje persons **Roll** på korrektur som ska använda den här mallen och **E-postaviseringar** du vill att användaren ska få när han/hon arbetar med korrektur som använder den här mallen.

   Mer information om roller i ett korrektur finns i [Konfigurera standardspråkroller](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Mer information om korrekturmeddelanden via e-post finns i avsnittet [Konfigurera korrekturinställningar för en användare](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) i artikeln  [Konfigurera e-postmeddelandeinställningar i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Varje användare kan bara läggas till på en scen. Du kan lägga till så många användare som du vill på en scen.

   >[!TIP]
   >
   >Du kan dra och släppa namn på granskare mellan faserna i stegdiagrammet. Tillgängliga stadier markeras med blått.

1. Upprepa de två föregående stegen för alla andra steg som du vill lägga till i mallen.

   Överst på **Arbetsflöde** visas ett diagram över det automatiserade arbetsflöde som du konfigurerar. När du fortsätter att lägga till faser visas de i diagrammet med rader som visar beroenden mellan dem. Du kan klicka på en scen i diagrammet för att visa inställningarna för den scenen.

   Om du inte behöver se diagrammet kan du klicka på **Dölj diagram**.

1. I **Dela mall med** klickar du på ett alternativ (om mallen inte redan delas med hela organisationen) för att ange vem som ska kunna använda den.

   Som standard delas nya mallar för automatiserat arbetsflöde med alla i organisationen.

1. Klicka **Skapa**.

## Ändra en mall för automatiserat arbetsflöde

Som Workfront Korrekturadministratör kan du ändra en mall för automatiserat arbetsflöde. Dina ändringar sparas automatiskt när du gör dem.

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.
1. Klicka **Arbetsflöden** i den vänstra panelen.
1. I **Arbetsflödesmallar** som visas klickar du på mallen som du vill ändra.
1. I **Detaljer** anger du följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mallnamn</td> 
      <td>(Obligatoriskt) Skriv ett namn på mallen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mallägare</td> 
      <td>Du kan välja den Workfront-administratör eller Workfront Proof-administratör som ska hantera mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mallgrupp</td> 
      <td> <p> Om organisationens automatiserade arbetsflöden är ordnade i grupper kan du välja namnet på gruppen. Se <a href="#create-automated-workflow-template-groups" class="MCXref xref">Skapa mallgrupper för automatiserat arbetsflöde</a> senare i den här artikeln om du vill ha mer information.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tidszon för mall </td> 
      <td> <p>Standardtidszonen för mallen är den som du arbetar i. Om tidszonen för de som skapar korrektur och granskare som ska använda mallen är olika, kan du ändra den här för att säkerställa att deadlines för scenen ställs in vid rätt tidpunkt för dessa användare. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt</td> 
      <td> <p>Välj de scenaktiviteter som du vill ska vara tillgängliga för dem som skapar korrektur med hjälp av mallen. </p> <p><b>VARNING</b>: Om du inte markerar alternativen Lägg till en scen och Lägg till personer i faser, kan varken mallägaren eller ägaren av något korrektur som använder den här mallen lägga till en scen eller dela korrekturet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. I **Arbetsflöde** ändrar du namnet på alla scener och expanderar dess inställningar ![](assets/arrow-button.png) för att göra nödvändiga ändringar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Deadline beräknad utifrån</td> 
      <td> <p>Ange hur du vill att tidsgränsen ska beräknas:</p> 
       <ul> 
        <li> <p><strong>Deadline beräknad från korrekturskapande</strong>: I <strong>Ange deadline för fasen</strong> i den nedrullningsbara listan väljer du det antal arbetsdagar som du vill lägga till i datumet då korrekturet skapades för att automatiskt ange en deadline för korrekturet.</p> </li> 
        <li><strong>Tidsfrist beräknad utifrån fasaktivering</strong>: I <strong>Ange deadline för fasen</strong> i den nedrullningsbara listan väljer du det antal arbetsdagar som du vill lägga till i scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera fas</td> 
      <td> <p>Ange om scenen aktiveras automatiskt eller manuellt. För den första fasen kan du välja <strong>Vid korrekturskapande</strong>, <strong>På ett visst datum och en viss tid</strong>, eller <strong>Manuellt</strong>.</p> <p>De andra alternativen blir tillgängliga när du lägger till en andra scen eftersom de kräver att du väljer en överordnad scen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås scen</td> 
      <td>Ange om du vill tillåta att scenen låses för kommentarer. Alternativen är att låsa en scen manuellt eller automatiskt, antingen när nästa fas startar eller när alla beslut fattas på den överordnade scenen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beslut</td> 
      <td>Slutar fasen första gången en av beslutsfattarna fattar sitt beslut. Mer information finns i <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurera korrekturinställningar i Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Integritet</td> 
      <td>Döljer kommentarer och beslut från personer som inte har lagts till på scenen eller som inte är tillsynspersoner eller högre i kontot. Mer information finns i <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Översikt över automatiserat arbetsflöde</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Borttagning av scenen</td> 
      <td>Gör scenen obligatorisk.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mer <img src="assets/more-icon.png"></td> 
      <td>Lägg till granskare på scenen eller ta bort scenen.<p>Om alla korrektur skickas till samma personer i en viss fas kan du ange deras namn här, så att du inte behöver lägga till dem varje gång du skapar ett korrektur. Skriv och markera namnet på en användare som du vill lägga till på scenen och lägg sedan till namnet <strong>Roll</strong> på bevisen och <strong>E-postaviseringar</strong> inställningar som du vill använda för användaren. Mer information om språkroller finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Konfigurera standardspråkroller</a>. Mer information om korrekturmeddelanden via e-post finns i avsnittet <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Konfigurera korrekturinställningar för en användare</a> i artikeln <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Konfigurera e-postmeddelandeinställningar i Workfront Proof</a>.</p><p>Du kan lägga till så många användare som du vill på en scen</p><p>Tips: Du kan dra och släppa namn på granskare mellan faserna i stegdiagrammet. Tillgängliga stadier markeras med blått.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Upprepa steget för alla andra steg som du vill lägga till i mallen.

   Överst på **Arbetsflöde** visas ett diagram över det automatiserade arbetsflöde som du konfigurerar. När du fortsätter att lägga till faser visas de i diagrammet med rader som visar beroenden mellan dem. Du kan klicka på en scen i diagrammet för att visa inställningarna för den scenen.

   Om du inte behöver se diagrammet kan du klicka på **Dölj diagram**.

1. I **Delas med** om du vill ta bort en användare klickar du på knappen Mer ![](assets/more-icon.png) till höger och klicka sedan **Ta bort**.

## Skapa mallgrupper för automatiserat arbetsflöde {#create-automated-workflow-template-groups}

Som Workfront-administratör kan du visa och hantera alla mallar för automatiserat arbetsflöde i organisationens konto. Det kan vara praktiskt att ordna mallar i grupper.

Så här skapar du en mallgrupp för automatiserat arbetsflöde:

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.
1. Klicka **Arbetsflöden** i den vänstra panelen.
1. På **Arbetsflöde** flik, klicka **Nytt** > **Ny mallgrupp**.
1. Skriv ett beskrivande namn för den nya mallgruppen och tryck sedan på **Retur**.

Du kan flytta mallarna mellan grupper genom att dra och släppa.

## Hantera automatiserade arbetsflödesmallar

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.

1. Klicka på i den vänstra panelen i Workfront Proof **Arbetsflöden**.
1. På **Arbetsflöden** som visas gör du något av följande:

   * Lägg till en ny mall
   * Lägg till en ny mallgrupp
   * Ta bort en eller flera mallgrupper
   * Åtkomst till information om en mall
   * Dra en mall till en annan mallgrupp

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
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '2079'
ht-degree: 0%

---

# Skapa och hantera automatiserade arbetsflödesmallar

<!-- Audited: 2/2024 -->

Som Adobe Workfront-administratör kan du skapa automatiska arbetsflödesmallar som innehåller de granskare som har korrekturroller och meddelandeinställningar som du anger, om ditt företags innehållsgranskningsprocess ofta upprepas eller innehåll ofta granskas av samma personer. En mall för automatiserat arbetsflöde kan vara enkel med bara en eller två granskare eller komplex med många faser och beroenden.

Automatiserade arbetsflödesmallar gör det enkelt att skapa ett korrektur med ett automatiserat arbetsflöde. När en användare skapar ett korrektur väljer han eller hon bara den mall han eller hon behöver.

Du kan enkelt ändra alla automatiska arbetsflödesmallar, lägga till eller ta bort granskare och faser när som helst. Och korrekturläsare som använder mallen kan lägga till eller ta bort granskare för korrekturet.

Tänk på följande när du använder en mall för automatiserat arbetsflöde:

1. Inställningarna i en mall för automatiserat arbetsflöde avgör vad du kan göra med det automatiserade arbetsflödet för ett korrektur. Om till exempel knappen Lägg till en scen är inaktiverad i mallen visas den inte när du arbetar med inställningarna för det automatiska arbetsflödet för korrekturet.
1. När en person läggs till på en scen i en mall för automatiserat arbetsflöde, men redan finns som granskare i korrekturet, tas granskaren bort från scenen när mallen används. Om du inte lägger till någon annan granskare på scenen visas ett meddelande som ber dig att lägga till en.
1. Din möjlighet att ändra en mall för automatiserat arbetsflöde beror på mallinställningarna som konfigurerats av Workfront-administratören, vilket beskrivs i . Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.

Mer information om automatiserade arbetsflöden finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Nytt: Alla</p><p>Aktuell: Pro eller högre</p><p>Äldre: Premium eller Select</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard</p><p>Aktuell: Arbete eller plan</p> <p>Äldre: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administratör måste väljas i din behörighetsprofil för korrektur. </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en mall för automatiserat arbetsflöde

{{step1-to-proofing}}

1. Klicka på **Arbetsflöden** i den vänstra panelen.
1. Klicka på **Nytt** > **Ny mall** på fliken **Arbetsflöde**.

1. Ange följande information i avsnittet **Detaljer**:

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
      <td> <p> Om organisationens automatiserade arbetsflöden är ordnade i grupper kan du välja namnet på gruppen. Mer information finns i <a href="#create-automated-workflow-template-groups" class="MCXref xref">Skapa automatiska arbetsflödesmallgrupper</a> senare i den här artikeln.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Tidszon för mall </td> 
      <td> <p>Standardtidszonen för mallen är den som du arbetar i. Om tidszonen för de som skapar korrektur och granskare som ska använda mallen är olika, kan du ändra den här för att säkerställa att deadlines för scenen ställs in vid rätt tidpunkt för dessa användare. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt</td> 
      <td> <p>Du kan välja de scenaktiviteter som du vill ska vara tillgängliga för personen som skapar korrektur med hjälp av mallen.</p> 
      <p><b>VARNING</b>: Om du inte markerar alternativen Lägg till en scen och Lägg till personer i faser kommer varken mallägaren eller ägaren till något korrektur som använder den här mallen att kunna lägga till en scen eller dela korrekturet. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurera varje steg i mallen för automatiserat arbetsflöde i avsnittet **Steg**.

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
      <td> <p>Ange om scenen aktiveras automatiskt eller manuellt. I det första steget kan du välja <strong>Vid korrekturskapande</strong>, <strong>Vid ett visst datum och en viss tid</strong> eller <strong>Manuellt</strong>.</p> <p>De andra alternativen blir tillgängliga när du lägger till en andra scen eftersom de kräver att du väljer en överordnad scen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deadline beräknad utifrån</td> 
      <td> <p>Ange hur du vill att tidsgränsen ska beräknas:</p> 
       <ul> 
        <li> <p><strong>Skapande av korrektur</strong>: I listrutan under <strong>Deadline (+ arbetsdagar)</strong> väljer du antalet arbetsdagar som du vill lägga till till datumet för skapande av korrektur för att automatiskt ange en deadline för korrekturet.</p> </li> 
        <li><strong>När scenen startar</strong>: I listrutan under <strong>Deadline (+ arbetsdagar)</strong> väljer du det antal arbetsdagar du vill lägga till i scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.</li> 
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
      <td>Döljer kommentarer och beslut från personer som inte har lagts till på scenen eller som inte är Workfront-administratörer. Mer information finns i <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Översikt över automatiserat arbetsflöde</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt inte att den här fasen tas bort</td> 
      <td> <p>Gör scenen obligatorisk.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Om korrektur som ska använda den här mallen alltid skickas till samma personer på scenen, lägger du till dem här så att användarna inte behöver lägga till dem varje gång de skapar ett korrektur.

   Välj varje persons **roll** på de korrektur som ska använda den här mallen och de **e-postaviseringar** som du vill att användaren ska ta emot när han eller hon arbetar med korrektur som använder den här mallen.

   Mer information om roller i ett korrektur finns i [Konfigurera standardspråkroller](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Mer information om korrekturmeddelanden via e-post finns i avsnittet [Konfigurera korrekturinställningar för en användare](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) i artikeln [Konfigurera e-postaviseringsinställningar i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Varje användare kan bara läggas till på en scen. Du kan lägga till så många användare som du vill på en scen.

   >[!TIP]
   >
   >Du kan dra och släppa namn på granskare mellan faserna i stegdiagrammet. Tillgängliga stadier markeras med blått.

1. Upprepa de två föregående stegen för alla andra steg som du vill lägga till i mallen.

   Överst i avsnittet **Arbetsflöde** visas ett diagram över det automatiska arbetsflöde som du konfigurerar. När du fortsätter att lägga till faser visas de i diagrammet med rader som visar beroenden mellan dem. Du kan klicka på en scen i diagrammet för att visa inställningarna för den scenen.

   Om du inte behöver visa diagrammet kan du klicka på **Dölj diagram**.

1. I avsnittet **Dela mall med** klickar du på ett alternativ (om mallen inte redan delas med hela organisationen) för att ange vem som ska kunna använda den.

   Som standard delas nya mallar för automatiserat arbetsflöde med alla i organisationen.

1. Klicka på **Skapa**.

## Ändra en mall för automatiserat arbetsflöde

Som Workfront Proof-administratör kan du ändra en mall för automatiserat arbetsflöde. Dina ändringar sparas automatiskt när du gör dem.

{{step1-to-proofing}}

1. Klicka på **Arbetsflöden** i den vänstra panelen.
1. Klicka på mallen som du vill ändra i listan **Arbetsflödesmallar** som visas.
1. Ange följande information i avsnittet **Detaljer**:

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
      <td> <p> Om organisationens automatiserade arbetsflöden är ordnade i grupper kan du välja namnet på gruppen. Mer information finns i <a href="#create-automated-workflow-template-groups" class="MCXref xref">Skapa automatiska arbetsflödesmallgrupper</a> senare i den här artikeln.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tidszon för mall </td> 
      <td> <p>Standardtidszonen för mallen är den som du arbetar i. Om tidszonen för de som skapar korrektur och granskare som ska använda mallen är olika, kan du ändra den här för att säkerställa att deadlines för scenen ställs in vid rätt tidpunkt för dessa användare. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt</td> 
      <td> <p>Välj de scenaktiviteter som du vill ska vara tillgängliga för dem som skapar korrektur med hjälp av mallen. </p> <p><b>VARNING</b>: Om du inte markerar alternativen Lägg till en scen och Lägg till personer i faser kommer varken mallägaren eller ägaren till något korrektur som använder den här mallen att kunna lägga till en scen eller dela korrekturet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. I avsnittet **Arbetsflöde** ändrar du namnet på en scen och expanderar dess inställningar ![Utöka-knappen](assets/arrow-button.png) för att göra nödvändiga ändringar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Deadline beräknad utifrån</td> 
      <td> <p>Ange hur du vill att tidsgränsen ska beräknas:</p> 
       <ul> 
        <li> <p><strong>Deadline beräknad från korrekturskapande</strong>: I listrutan <strong>Ange deadline för scenen</strong> väljer du det antal arbetsdagar du vill lägga till till datumet för korrekturskapande för att automatiskt ange en deadline för korrekturet.</p> </li> 
        <li><strong>Deadline beräknad från scenaktivering</strong>: I listrutan <strong>Ange deadline för scenen</strong> väljer du det antal arbetsdagar som du vill lägga till till scenens aktiveringsdatum för att automatiskt ställa in en deadline för korrekturet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera fas</td> 
      <td> <p>Ange om scenen aktiveras automatiskt eller manuellt. I det första steget kan du välja <strong>Vid korrekturskapande</strong>, <strong>Vid ett visst datum och en viss tid</strong> eller <strong>Manuellt</strong>.</p> <p>De andra alternativen blir tillgängliga när du lägger till en andra scen eftersom de kräver att du väljer en överordnad scen. </p> </td> 
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
      <td>Lägg till granskare på scenen eller ta bort scenen.<p>Om alla korrektur skickas till samma personer i en viss fas kan du ange deras namn här, så att du inte behöver lägga till dem varje gång du skapar ett korrektur. Skriv och markera namnet på en användare som du vill lägga till på scenen och lägg sedan till användarens <strong>roll</strong> i korrekturet och <strong>e-postaviseringar</strong> som du vill använda för användaren. Mer information om språkroller finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Konfigurera standardspråkroller</a>. Mer information om korrekturmeddelanden via e-post finns i avsnittet <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Konfigurera korrekturinställningar för en användare</a> i artikeln <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Konfigurera e-postaviseringsinställningar i Workfront Proof</a>.</p><p>Du kan lägga till så många användare som du vill på en scen</p><p>Tips! Du kan dra och släppa namn på granskare mellan faserna i stegdiagrammet. Tillgängliga stadier markeras med blått.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Upprepa steget för alla andra steg som du vill lägga till i mallen.

   Överst i avsnittet **Arbetsflöde** visas ett diagram över det automatiska arbetsflöde som du konfigurerar. När du fortsätter att lägga till faser visas de i diagrammet med rader som visar beroenden mellan dem. Du kan klicka på en scen i diagrammet för att visa inställningarna för den scenen.

   Om du inte behöver visa diagrammet kan du klicka på **Dölj diagram**.

1. Om du vill ta bort en användare klickar du på ikonen Mer ![Mer](assets/more-icon.png) till höger i avsnittet **Delad med** och sedan på **Ta bort**.

## Skapa mallgrupper för automatiserat arbetsflöde {#create-automated-workflow-template-groups}

Som Workfront-administratör kan du visa och hantera alla mallar för automatiserat arbetsflöde i organisationens konto. Det kan vara praktiskt att ordna mallar i grupper.

Så här skapar du en mallgrupp för automatiserat arbetsflöde:

{{step1-to-proofing}}

1. Klicka på **Arbetsflöden** i den vänstra panelen.
1. Klicka på **Nytt** > **Ny mallgrupp** på fliken **Arbetsflöde**.
1. Skriv ett beskrivande namn för den nya mallgruppen och tryck sedan på **Retur**.

Du kan flytta mallarna mellan grupper genom att dra och släppa.

## Hantera automatiserade arbetsflödesmallar

{{step1-to-proofing}}

1. Klicka på **Arbetsflöden** i den vänstra panelen i Workfront Proof.
1. Gör något av följande på sidan **Arbetsflöden** som visas:

   * Lägg till en ny mall
   * Lägg till en ny mallgrupp
   * Ta bort en eller flera mallgrupper
   * Åtkomst till information om en mall
   * Dra en mall till en annan mallgrupp

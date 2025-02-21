---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Skapa eller redigera ett automatiserat arbetsflöde för ett befintligt korrektur
description: Automatiska arbetsflöden gör det enklare att hantera granskningsprocessen om processen är komplex eller om du regelbundet skickar innehåll för granskning till samma grupper av personer. När du skapar ett korrektur med ett automatiserat arbetsflöde flyttas korrekturet från scen till scen tills det är slutgiltigt godkänt. Deltagarna meddelas när det är deras tur att granska dokumentet.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Skapa eller redigera ett automatiserat arbetsflöde för ett befintligt korrektur

Automatiska arbetsflöden gör det enklare att hantera granskningsprocessen om processen är komplex eller om du regelbundet skickar innehåll för granskning till samma grupper av personer. När du skapar ett korrektur med ett automatiserat arbetsflöde flyttas korrekturet från scen till scen tills det är slutgiltigt godkänt. Deltagarna meddelas när det är deras tur att granska dokumentet.

Mer information om hur du skapar ett automatiserat arbetsflöde för ett nytt korrektur finns i [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Gammal plan: Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Skapa eller redigera ett automatiserat arbetsflöde för ett befintligt korrektur:

1. Håll muspekaren över dokumentet i området Dokument och klicka sedan på Arbetsflöde för korrektur.

   eller

   Om du granskar korrekturet i korrekturläsaren klickar du på ikonen **Arbetsflöde** ![Arbetsflöde](assets/workflow-icon-proofing-viewer.png) i den vänstra panelen och sedan på ikonen Redigera ![Redigera](assets/edit-icon-proofing-viewer.png) för att öppna inställningarna för det automatiserade arbetsflödet för korrekturet.

1. (Villkorligt) Om korrekturet för närvarande använder ett grundläggande arbetsflöde (utan stadier) klickar du på **Konvertera till automatiserat arbetsflöde** på skärmen som visas.

   >[!NOTE]
   >
   >Du kan inte redigera det första steget när du konverterar från ett grundläggande arbetsflöde till ett automatiserat arbetsflöde, men du kan lägga till och konfigurera nya steg.

1. Villkorligt) Om du vill använda en mall för automatiserat arbetsflöde som din Adobe Workfront-administratör har skapat och delat med dig klickar du på **Lägg till mall**, markerar mallen i rutan som visas och klickar sedan på **Lägg till mall**.

   Mer information finns i [Använda automatiska arbetsflödesmallar](#about-using-automated-workflow-templates) i den här artikeln.

1. Lägg till en scen i det automatiserade arbetsflödet:

   1. Klicka på **Ny scen** i det övre högra hörnet.
   1. I rutan som visas skriver du **Namn** för scenen.
   1. (Valfritt) Ange en deadline för scenen.
   1. I avsnittet **Aktivera scen** väljer du hur du vill att scenen ska aktiveras:


      <table>
      <tbody>
      <tr>
      <td><strong>Vid korrekturskapande</strong></td>
      <td>Scenen aktiveras automatiskt eftersom korrekturet redan har skapats.</td>
      </tr>
      <tr>
      <td><strong>När deadline för föregående fas passeras</strong></td>
      <td>Klicka på föregående scen i listrutan <strong>Överordnad scen</strong> .</td>
      </tr>
      <tr>
      <td><strong>På ett visst datum och en viss tid</strong></td>
      <td>Markera datumet genom att klicka i rutan <strong>På</strong> och sedan klicka i rutan till höger för att välja tid.</td>
      </tr>
      <tr>
      <td><strong>Alla beslut godkänns eller godkänns med ändringar på den överordnade fasen</strong></td>
      <td>Klicka på den överordnade scenen i listrutan <strong>Överordnad scen</strong>.</td>
      </tr>
      <tr>
      <td><strong>Alla beslut godkänns på överordnad fas</strong></td>
      <td>Klicka på den överordnade scenen i listrutan <strong>Överordnad scen</strong>.</td>
      </tr>
      <tr>
      <td><strong>Alla beslut fattas</strong></td>
      <td>Klicka på den överordnade scenen i listrutan <strong>Överordnad scen</strong>.</td>
      </tr>
      </tbody>
      </table>


   1. Ange ett kontaktnamn eller en e-postadress och konfigurera inställningar för granskarna för scenen.

      Mer information om hur du lägger till granskare finns i [Om att lägga till granskare på en scen](#about-adding-reviewers-to-a-stage) i den här artikeln.

   1. Använd något av följande alternativ för att ytterligare konfigurera scenen:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Deadline-alternativ</strong> </td>
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
         <td role="rowheader">Primär beslutsfattare</td>
         <td><p>Välj den primära beslutsfattaren på scenen (endast tillgänglig efter att du har lagt till minst en person på scenen som har rollen Korrektur som godkännare eller högre). Om du väljer en primär beslutsfattare är alternativet <strong>Endast ett beslut krävs</strong> inaktiverat på den här fasen.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Endast ett beslut krävs</td>
         <td>Slutför hela granskningsprocessen när en av beslutsfattarna fattar ett beslut.<p>Det här alternativet är inte tillgängligt om du har angett en användare i listrutan <strong>Primär beslutsfattare</strong> .</p></td>
        </tr>
        <tr>
         <td role="rowheader">Privat fas</td>
         <td>Endast följande personer kan se kommentarer och beslut som fattas under den här fasen: Supervisors, Adobe Workfront administrators och Workfront Proof administrators</td>
        </tr>
        <tr>
         <td role="rowheader">Meddela personer via e-post</td>
         <td>Aviserar granskarna med ett e-postmeddelande när det är deras tur att arbeta med korrekturet.</td>
        </tr>
       </tbody>
      </table>

   1. Klicka på **Lägg till scen**.

1. Upprepa föregående steg om det behövs för att lägga till fler steg.

   När du lägger till faser i det automatiserade arbetsflödet visas ett diagramformulär på skärmen som representerar dem:

   ![Arbetsflödesdiagram](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. När du är klar med att lägga till faser klickar du på **Klar**.

## Använda automatiska arbetsflödesmallar {#about-using-automated-workflow-templates}

Tänk på följande när du använder en mall för automatiserat arbetsflöde:

1. Inställningarna i en mall för automatiserat arbetsflöde avgör vad du kan göra med det automatiserade arbetsflödet för ett korrektur. Om till exempel knappen Lägg till en scen är inaktiverad i mallen visas den inte när du arbetar med inställningarna för det automatiska arbetsflödet för korrekturet.
1. När en person läggs till i en bild i en mall för automatiserat arbetsflöde, men redan finns som granskare i korrekturet, tas granskaren bort från scenen om mallen används. Om du inte lägger till någon annan granskare på scenen visas ett meddelande som ber dig att lägga till en.
1. Din möjlighet att ändra en mall för automatiserat arbetsflöde beror på mallinställningarna som konfigurerats av Workfront-administratören, vilket beskrivs i . Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.

## Lägga till granskare på en scen {#about-adding-reviewers-to-a-stage}

Tänk på följande när du lägger till granskare på en scen:

* När du har lagt till en användare på en scen kan du konfigurera inställningar för den användaren på korrekturet, t.ex. korrekturrollen och eventuella ytterligare behörigheter som de ska ha och vilken typ av e-postaviseringar de ska få när de får kommentarer och beslut om korrekturet.
* Du kan dra en eller flera användare från en scen till en annan. Du kan dra användare direkt till en annan scen eller dra användare till en scen i diagrammet **Steg**. Om du vill markera flera användare trycker du på Skift+Ctrl (Windows) eller Skift+Kommando (Mac).
* Du kan bara lägga till en granskare i ett korrektur en gång, vilket betyder att du inte kan lägga till samma person i mer än en fas i korrekturet.
* Granskare som inte har lagts till på en privat scen kan inte se den scenen på det korrektur eller de kommentarer som har gjorts på den scenen.
* Om du lägger till en användare på en scen får användaren som standard åtkomst till korrekturet från det att korrekturet skapas.

  Din Workfront-administratör kan hindra användare från att komma åt korrekturet tills arbetsflödet går in på den scen där användaren lades till. Mer information finns i  in .

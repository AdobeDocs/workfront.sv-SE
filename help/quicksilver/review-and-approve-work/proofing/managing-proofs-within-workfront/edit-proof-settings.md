---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Redigera korrekturinställningar
description: Du kan redigera korrekturinställningar när som helst efter att du har skapat ett korrektur.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: a036a99c13d80a2ba2305ebcdc799ad6e5b62b39
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Redigera korrekturinställningar

Du kan redigera korrekturinställningar när som helst efter att du har skapat ett korrektur.

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
   <td role="rowheader">Korrekturroll</td> 
   <td>Författare eller moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Redigera korrekturinställningar

Vissa inställningar kan vara låsta om Workfront-administratören har inaktiverat dem på kontonivån.

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på fliken **Dokument** .
1. För musen över korrekturet och klicka sedan på **Dokumentinformation**.
1. Klicka på **Inställningar för språkkontroll** i den vänstra panelen.
1. Justera följande inställningar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kräv inloggning. Det här korrekturet kan inte delas med gästanvändare</td> 
      <td> <p>Om du behöver högre säkerhetsnivå för din granskning och godkännandeprocess kan du använda Kräv inloggning till korrekturet. Detta innebär att det endast går att lägga till Workfront-användare till korrekturet. De måste ange sina e-postadresser och lösenord innan de kan komma åt dem.</p> <p>Obs! <em style="font-style: normal;">Om inloggning krävs är aktiverad går det inte att aktivera prenumerationer.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv att beslut signeras elektroniskt</td> 
      <td> <p>Du kan begära en elektronisk signatur från alla granskare som fattar beslut om korrekturet. När en granskare fattar ett beslut visas en uppmaning om att ange e-postadress och lösenord och bekräfta sitt beslut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås korrektur när alla nödvändiga beslut har fattats</td> 
      <td> <p>Du kan ställa in ett korrekturläge så att det låses när den slutliga godkännaren fattar sitt beslut. Detta är användbart om du vill vara säker på att granskarna inte kan gå tillbaka till korrekturet och lägga till ytterligare kommentarer eller ändra sina beslut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt hämtning av originalfilen</td> 
      <td> <p>Du kan tillåta granskare som har ett korrektur att hämta originalfilen från vilken ett korrektur skapades. Detta är aktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt delning av korrektur via offentlig URL eller inbäddningskod</td> 
      <td>Du kan tillåta användare att dela korrekturet med en offentlig URL eller inbäddningskod. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt prenumerationer på korrektur via offentlig URL eller inbäddningskod</td> 
      <td> <p>Om du aktiverar prenumeration på korrekturet kan personer som inte har lagts till explicit i beviset prenumerera på själva beviset (d.v.s. lägga till sig själva till beviset). De tilldelas sedan den roll och e-postavisering som du väljer för dem i prenumerationsinställningarna.</p> <p>Om Prenumeration har aktiverats för ett korrektur aktiveras fälten nedan:</p> 
       <ul> 
        <li><strong>Prenumerantvalidering krävs</strong> - Prenumeranten måste klicka på en länk i ett e-postmeddelande för att få åtkomst till ett korrektur<br>Om du väljer det här alternativet får den som prenumererar inte omedelbar åtkomst till korrekturet, utan en länk till korrekturet i ett e-postmeddelande. Syftet med prenumerantvalidering är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till.</li> 
        <li><strong>Standardroll för nya prenumeranter -</strong> Det här är standardkorrekturrollen som tilldelas alla granskare som prenumererar på själva korrekturet.</li> 
        <li><strong>Standardmeddelande för e-post för nya prenumeranter</strong> - Det här är standardmeddelandet som tilldelas alla granskare som abonnerar på korrekturet.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

 

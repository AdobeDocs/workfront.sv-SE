---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Konfigurera åtkomst- och prenumerationsinställningar för ett bevis
description: Du kan konfigurera vissa åtkomst- och prenumerationsinställningar för enskilda korrektur, t.ex. om användare ska behöva logga in och om användare ska kunna prenumerera på korrekturet. Du kan ställa in åtkomst- och prenumerationsinställningar för ett korrektur medan du skapar det, eller så kan du ställa in dem för ett korrektur som redan finns i Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Konfigurera åtkomst- och prenumerationsinställningar för ett bevis

Du kan konfigurera vissa åtkomst- och prenumerationsinställningar för enskilda korrektur, t.ex. om användare ska behöva logga in och om användare ska kunna prenumerera på korrekturet. Du kan ställa in åtkomst- och prenumerationsinställningar för ett korrektur medan du skapar det, eller så kan du ställa in dem för ett korrektur som redan finns i Workfront.

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

## Konfigurera åtkomst- och prenumerationsinställningar när du skapar ett bevis

Så här ställer du in åtkomst- och prenumerationsinställningar för ett korrektur när du skapar det:

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på avsnittet **Dokument**.
1. Klicka på **Lägg till ny** i det övre högra området.
1. Bläddra till avsnittet **Korrekturinställningar** i det nedre högra hörnet på sidan **Nytt korrektur**.

1. Konfigurera följande inställningar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Tillåt delning av korrektur via offentlig URL eller inbäddningskod</strong> </td> 
      <td>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tillåt prenumerationer på korrektur via offentlig URL eller inbäddningskod</strong> </td> 
      <td>När det här alternativet är markerat kan personer som inte har lagts till explicit i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:
       <ul>
        <li><p><strong>Prenumerantroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet. </p><p>Viktigt: Om <strong>Tillåt delning med</strong> är inställt på något annat än <strong>Alla</strong> i Workfront Proof-inställningarna fungerar prenumerationen bara för personer i organisationen. Mer information finns i <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurera korrekturinställningar i Workfront Proof</a>.</p></li>
        <li><strong>E-postaviseringsinställningar för prenumeranter:</strong> Standardaviseringen för e-post som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomst via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till korrekturet. Du kan välja <strong>Inget e-postmeddelande</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>E-postmeddelande för korrektur endast</strong> (prenumeranten får en länk till korrekturet via e-post utan någon verifiering) eller <strong>E-postmeddelanden för validering och korrekturet </strong> (prenumeranten får en länk till korrekturet och måste klicka på ett bevis. Syftet med det här alternativet är att se till personen har angett korrekt e-postadress som de har tillgång till).</li>
        </ul><p>Obs!  Om korrekturet har ett automatiserat arbetsflöde bifogat, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt skapa korrektur.

## Konfigurera åtkomst- och prenumerationsinställningar för ett befintligt bevis

Så här ställer du in åtkomst- och prenumerationsinställningar för ett bevis som redan finns i Workfront:

1. I området Dokument markerar du det dokument som innehåller det korrektur som du vill konfigurera inställningar för och klickar sedan på **Dokumentinformation**.
1. Klicka på **Inställningar för språkkontroll** i den vänstra panelen.
1. Konfigurera följande inställningar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Tillåt delning av korrektur via offentlig URL eller inbäddningskod</strong><strong>e</strong> </td> 
      <td>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tillåt prenumerationer på korrektur via offentlig URL eller inbäddningskod</strong> </td> 
      <td>När det här alternativet är markerat kan personer som inte har lagts till explicit i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:
       <ul>
        <li><p><strong>Prenumerantroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet. </p><p>Viktigt: Om <strong>Tillåt delning med</strong> är inställt på något annat än <strong>Alla</strong> i Workfront Proof-inställningarna fungerar prenumerationen bara för personer i organisationen. Mer information finns i <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurera korrekturinställningar i Workfront Proof</a>.</p></li>
        <li><strong>E-postaviseringsinställningar för prenumeranter:</strong> Standardaviseringen för e-post som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomst via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till korrekturet. Du kan välja <strong>Inget e-postmeddelande</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>E-postmeddelande för korrektur endast</strong> (prenumeranten får en länk till korrekturet via e-post utan någon verifiering) eller <strong>E-postmeddelanden för validering och korrekturet </strong> (prenumeranten får en länk till korrekturet och måste klicka på ett bevis. Syftet med det här alternativet är att se till personen har angett korrekt e-postadress som de har tillgång till).</li>
        </ul><p>Obs!  Om korrekturet har ett automatiserat arbetsflöde bifogat, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Konfigurera åtkomst- och prenumerationsinställningar för ett bevis
description: Du kan konfigurera vissa åtkomst- och prenumerationsinställningar för enskilda korrektur, t.ex. om användare ska behöva logga in och om användare ska kunna prenumerera på korrekturet. Du kan ställa in åtkomst- och prenumerationsinställningar för ett korrektur medan du skapar det, eller så kan du ställa in dem för ett korrektur som redan finns i Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Konfigurera åtkomst- och prenumerationsinställningar för ett bevis

Du kan konfigurera vissa åtkomst- och prenumerationsinställningar för enskilda korrektur, t.ex. om användare ska behöva logga in och om användare ska kunna prenumerera på korrekturet. Du kan ställa in åtkomst- och prenumerationsinställningar för ett korrektur medan du skapar det, eller så kan du ställa in dem för ett korrektur som redan finns i Workfront.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Premium</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
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

## Konfigurera åtkomst- och prenumerationsinställningar när du skapar ett bevis

Så här ställer du in åtkomst- och prenumerationsinställningar för ett korrektur när du skapar det:

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på **Dokument** -avsnitt.
1. Klicka **Lägg till ny** i det övre högra området.
1. Bläddra till **Korrekturinställningar** i det nedre högra hörnet av **Nytt korrektur** sida.

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
        <li><p><strong>Abonnentroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet. </p><p>Viktigt: If <strong>Tillåt delning med</strong> är inställt på något annat än <strong>Alla</strong> i inställningarna för Workfront-korrektur fungerar prenumerationen bara för personer inom organisationen. Mer information finns i <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurera korrekturinställningar i Workfront Proof</a>.</p></li>
        <li><strong>Inställningar för e-postavisering för prenumeranter:</strong> Standardvarningsmeddelandet som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomstbevis via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till beviset. Du kan välja <strong>Ingen e-post</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>Endast e-postmeddelanden med korrektur</strong> (prenumeranten får en länk till beviset via e-post utan verifiering) eller <strong>E-postmeddelanden om validering och korrektur</strong> (prenumeranten får en länk till beviset via e-post och måste klicka på länken för att få tillgång till ett bevis. Syftet med det här alternativet är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till).</li>
        </ul><p>Obs!  Om korrekturet har ett automatiserat arbetsflöde bifogat, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt skapa korrektur.

## Konfigurera åtkomst- och prenumerationsinställningar för ett befintligt bevis

Så här ställer du in åtkomst- och prenumerationsinställningar för ett bevis som redan finns i Workfront:

1. I området Dokument markerar du det dokument som innehåller det korrektur som du vill konfigurera inställningar för och klickar sedan på **Dokumentinformation**.
1. Klicka på i den vänstra panelen **Inställningar för korrekturläsare**.
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
        <li><p><strong>Abonnentroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet. </p><p>Viktigt: If <strong>Tillåt delning med</strong> är inställt på något annat än <strong>Alla</strong> i inställningarna för Workfront-korrektur fungerar prenumerationen bara för personer inom organisationen. Mer information finns i <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurera korrekturinställningar i Workfront Proof</a>.</p></li>
        <li><strong>Inställningar för e-postavisering för prenumeranter:</strong> Standardvarningsmeddelandet som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomstbevis via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till beviset. Du kan välja <strong>Ingen e-post</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>Endast e-postmeddelanden med korrektur</strong> (prenumeranten får en länk till beviset via e-post utan verifiering) eller <strong>E-postmeddelanden om validering och korrektur</strong> (prenumeranten får en länk till beviset via e-post och måste klicka på länken för att få tillgång till ett bevis. Syftet med det här alternativet är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till).</li>
        </ul><p>Obs!  Om korrekturet har ett automatiserat arbetsflöde bifogat, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara**.

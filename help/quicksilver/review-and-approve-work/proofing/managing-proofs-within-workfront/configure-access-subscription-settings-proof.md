---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Konfigurera åtkomst- och prenumerationsinställningar för ett bevis
description: Du kan konfigurera vissa åtkomst- och prenumerationsinställningar för enskilda korrektur, t.ex. om användare ska behöva logga in och om användare ska kunna prenumerera på korrekturet. Du kan ställa in åtkomst- och prenumerationsinställningar för ett korrektur medan du skapar det, eller så kan du ställa in dem för ett korrektur som redan finns i Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Konfigurera åtkomst- och prenumerationsinställningar för ett bevis

Du kan konfigurera vissa åtkomst- och prenumerationsinställningar för enskilda korrektur, t.ex. om användare ska behöva logga in och om användare ska kunna prenumerera på korrekturet. Du kan ställa in åtkomst- och prenumerationsinställningar för ett korrektur medan du skapar det, eller så kan du ställa in dem för ett korrektur som redan finns i Workfront.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Standard</p>
   <p>Arbete eller plan</p> 
    </td> 
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

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

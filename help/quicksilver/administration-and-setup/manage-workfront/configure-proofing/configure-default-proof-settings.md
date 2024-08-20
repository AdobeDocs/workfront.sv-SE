---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurera standardkorrekturinställningar
description: Med de här inställningarna kan du ange standardvärden som gäller för alla nya korrektur som skapas av användarna. Användarna kan dock åsidosätta de flesta av dessa inställningar när de skapar ett korrektur.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: 5676910e53f1c4f49cab196e42bfbce8704887ca
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Konfigurera standardinställningar för korrektur

Med de här inställningarna kan du ange standardvärden som gäller för alla nya korrektur som skapas av användarna. Användarna kan dock åsidosätta de flesta av dessa inställningar när de skapar ett korrektur.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara Workfront-administratör. Mer information om Workfront-administratörer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Konfigurera nya standardinställningar för korrektur

{{step-1-to-setup}}

1. Klicka på **Korrekturinställningar** > **Korrekturinställningar** i den vänstra panelen.
1. Konfigurera följande inställningar i avsnittet **Nya korrekturinställningar**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Mottagare</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv inloggning</td> 
      <td> <p>Granskarna måste logga in med sina e-postadresser och lösenord innan de kan visa korrektur som har skapats i organisationens konto. När det här alternativet är aktiverat kan användare inte dela korrekturet med gästgranskare.</p> <p><b>VIKTIGT</b>: När det här alternativet är aktiverat krävs inloggning för alla nya korrektur.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiera ägare från originalkorrektur för nya versioner</td> 
      <td> <p>Ägaren till den första versionen av ett korrektur är också ägare av alla efterföljande versioner av beviset, oavsett vem som skapar dessa versioner. Den här inställningen är aktiverad som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt användare att ta bort sina korrekturkommentarer</td> 
      <td>Användarna kan ta bort sina egna kommentarer. Den här inställningen är aktiverad som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv att beslut signeras elektroniskt </td> 
      <td> <p>Beslutsfattarna uppmanas att ange sina inloggningsuppgifter för Workfront när de fattar beslut om ett bevis.</p> <p><b>VIKTIGT</b>: När det här alternativet är aktiverat kan användare inte dela korrekturet med gästgranskare som inte har inloggningsuppgifter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Deadline</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ange standarddeadline</td> 
      <td> <p>Systemet tillämpar den här tidsgränsen på alla nya korrektur på ditt konto som inte har något automatiserat arbetsflöde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meddela mottagarna innan beviset är i farozonen</td> 
      <td>Mottagarna meddelas via e-post innan beviset anses vara i riskzonen beroende på den deadline som anges ovan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>E-postaviseringar</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meddela mottagarna när de läggs till i ett korrektur</td> 
      <td>Mottagarna meddelas via e-post när de läggs till i ett korrektur.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

## Konfigurera korrekturbeslut

Användare kan använda korrekturbeslut för att ange korrekturstatus efter granskning.

>[!NOTE]
>
>Logiken bakom korrekturbeslut används för att beräkna den övergripande statusen för ett korrekturarbetsflöde om det finns flera beslut på olika nivåer. Besluten Godkänd och Godkänd med ändringar utlöser nästa steg i ett automatiskt arbetsflöde.

Så här konfigurerar du korrekturbeslut:

{{step-1-to-setup}}

1. Klicka på **Korrekturinställningar** > **Korrekturinställningar** i den vänstra panelen.
1. I avsnittet **Beslut** kan du

   1. **Byt namn på beslutet**: Klicka på texten i beslutsrutan och börja skriva den nya beslutsetiketten.

      >[!TIP]
      >
      >Behåll logiken för ett beslut när du byter namn på det. Det gick till exempel att ändra standardbeslutet Avvisat till *Ny version krävs*, men det bör inte ändras till *Skicka till skrivare*.

      ![](assets/rename-decision-350x109.png)

   1. **Ordna om beslutsordningen**: Dra beslutsrutorna i den ordning som du vill att de ska visas i korrekturläsaren.

      ![](assets/move-decision-350x110.png)

   1. **Dölj ett beslut**: Håll markören över beslutsrutan och klicka på Dölj-ikonen i det övre högra hörnet.

      ![](assets/hide-decision-350x109.png)

1. (Valfritt) Om du vill gå tillbaka till standardinställningarna för Workfront klickar du på **Återställ standardvärden**.
1. Klicka på **Spara**.

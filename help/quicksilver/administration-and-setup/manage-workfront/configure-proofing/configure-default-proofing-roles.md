---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurera roller för standardkorrektur
description: Som Adobe Workfront-administratör kan du konfigurera standardspråkroller för användare och gästanvändare som har åtkomst till korrektur som skapats i Workfront. Alla som lägger till användare i ett korrektur kan justera de här rollerna åt dem.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Konfigurera standardspråkroller

Som Adobe Workfront-administratör kan du konfigurera standardspråkroller för användare och gästanvändare som har åtkomst till korrektur som skapats i Workfront. Alla som lägger till användare i ett korrektur kan justera de här rollerna åt dem.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara Workfront-administratör. Mer information om Workfront-administratörer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Konfigurera standardspråkroller

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Klicka på **Granska och godkänn** längst ned i listan till vänster.
1. I avsnittet **Roller för angivna mottagare av dokumentkorrektur** väljer du standardrollen för användare och gästanvändare som läggs till i ett korrekturarbetsflöde.

   I [Rättigheter som är kopplade till språkroller](#rights-associated-with-proofing-roles) nedan finns en lista över alla språkroller och de rättigheter som är kopplade till dem.

   >[!NOTE]
   >
   >* Den här inställningen gäller endast användare som har skapats i Workfront-systemet efter att rollen har angetts, inte befintliga användare.
   >* Den person som lägger till användare i korrekturet kan justera den här rollen enligt beskrivningen i [Lägg till användare i ett korrektur](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) i [Dela ett korrektur i Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. I avsnittet **Roller för icke-mottagare som öppnar dokumentkorrektur** väljer du standardrollen för användare och gästanvändare som kan få åtkomst till ett korrektur, men som inte har lagts till i korrekturets arbetsflöde.

   Detta inträffar när användare och gäster har åtkomst till ett dokument som har bevisats. Även om de inte har lagts till i korrekturets arbetsflöde kan de öppna korrekturet.

   **Exempel:** Här är exempel på hur du kan använda den här inställningen:

   * Du väljer **Skrivskyddad** om du vill begränsa alla korrekturaktiviteter, till exempel att lägga till kommentarer och fatta beslut till dem som har ombetts att göra det.
   * Du väljer **Granskare** eftersom du vill att alla i teamet ska kunna lägga till markeringar och kommentarer i ett korrektur.

1. Klicka på **Spara**.

## Rättigheter som är kopplade till språkroller {#rights-associated-with-proofing-roles}

I följande tabell visas varje roll och de rättigheter som är kopplade till den:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Visa ett bevis</strong> </p> </th> 
   <th> <p><strong>Lägg till markeringar</strong> </p> </th> 
   <th> <p><strong>Lägg till kommentarer</strong> </p> </th> 
   <th> <p><strong>Redigera egna kommentarer om det inte finns några svar</strong> </p> </th> 
   <th> <p><strong>Fatta ett beslut</strong> </p> </th> 
   <th> <p><strong>Ta bort kommentarer från andra</strong> </p> </th> 
   <th>Lös kommentarer</th> 
   <th>Tillämpa åtgärder på kommentarer</th> 
   <th> <p><strong>Redigera korrekturet</strong> </p> </th> 
   <th>Dela korrekturet med andra</th> 
   <th>Skapa ny version</th> 
   <th> <p><strong>Visa godkännandebegäranden i hemområdet</strong> </p> </th> 
   <th>Lägg till nya granskare</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Skrivskyddad</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Granskare</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Godkännare</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Granskare och godkännare</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Författare</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderator</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Användare med nya Workfront-planer kan tilldela författare eller moderatorroller till alla användare i systemet. Användare med äldre planer kan tilldela författare eller moderatorroller till alla användare som har en korrekturlicens i systemet.

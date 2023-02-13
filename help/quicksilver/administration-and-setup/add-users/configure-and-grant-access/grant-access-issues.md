---
title: Bevilja åtkomst till utleveranser
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till problem i Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Bevilja åtkomst till utleveranser

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till problem, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Mer information om hur du använder anpassade åtkomstnivåer för att hantera användarnas åtkomst till andra objekttyper i Workfront finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bevilja användaråtkomst vid problem med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på **Visa** eller **Redigera** till höger om Utgåvor och välj sedan de funktioner du vill bevilja under **Finjustera inställningarna**.

1. (Valfritt) Om du vill begränsa ärvda behörigheter för utgåvor från objekt med högre rankning klickar du på **Ange ytterligare begränsningar** väljer **Ärv aldrig dokumentåtkomst från projekt, uppgifter, ärenden osv.**.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med någon av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Tillgång till utleveranser per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med problem finns i avsnittet [Problem](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Tillgång till delade problem

Som ägare eller skapare av ett problem kan du dela med andra användare genom att ge dem behörighet till det, vilket förklaras i [Dela ett ärende](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

När du delar ett objekt med en annan användare bestäms mottagarens rättigheter till det av en kombination av två saker:

* De behörigheter som du ger mottagaren för objektet
* Mottagarens åtkomstnivåinställningar för objektets typ

Om åtkomstnivån tillåter det kan användarna även få åtkomst till ett problem via objekthierarkin: om en användare redan har behörighet för ett ärende överordnade projekt eller en uppgift, har de även behörighet för problemet (se steg 3 ovan). När du delar ett problem kan du se en lista över de användare som har ärvt behörighet till det.

![](assets/inherited-permissions.png)

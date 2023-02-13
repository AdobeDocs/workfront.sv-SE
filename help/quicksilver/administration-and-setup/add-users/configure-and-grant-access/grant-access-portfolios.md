---
title: Bevilja åtkomst till portföljer
user-type: administrator
product-area: system-administration;portfolios
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till portföljer i Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f4a9c4f3-8ed4-4629-aced-9cc09b8acd3f
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Bevilja åtkomst till portföljer

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till portföljer, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Konfigurera användaråtkomst till portföljer med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på **Visa** eller **Redigera** till höger om Portfolio och sedan välja de funktioner du vill bevilja under **Finjustera inställningarna**.

   ![](assets/fine-tune-portfolios.png)

   >[!NOTE]
   >
   >När du konfigurerar en åtkomstnivåinställning för en viss typ av objekt påverkar den konfigurationen inte användarens åtkomst till objekt med lägre rankning. Du kan t.ex. hindra användare från att ta bort portföljer på åtkomstnivån, men detta förhindrar dem inte från att ta bort projekt, som har lägre rankning än portföljer.Mer information om objekthierarkin finns i avsnittet [Objektens inbördes beroende och hierarki](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med någon av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Tillgång till portföljer per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med portföljer finns i avsnittet [Portfolio](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#portfoli) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Tillgång till delade portföljer

Som ägare eller skapare av en portfölj kan du dela med andra användare genom att ge dem behörighet till den, vilket förklaras i [Dela en portfölj](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

När du delar ett objekt med en annan användare bestäms mottagarens rättigheter till det av en kombination av två saker:

* De behörigheter som du ger mottagaren för objektet
* Mottagarens åtkomstnivåinställningar för objektets typ

Mer information om behörigheter som användare kan ge i en portfölj när de delar den finns i [Dela en portfölj](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

---
title: Bevilja åtkomst till aktiviteter
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till uppgifter i Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aafa8886-82e2-41c4-8fcb-cbb9df2d55dd
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Bevilja åtkomst till uppgifter

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till uppgifter, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Mer information om hur du använder anpassade åtkomstnivåer för att hantera användarnas åtkomst till andra objekttyper i Workfront finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Konfigurera användaråtkomst för uppgifter med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen **Visa** eller **Redigera** till höger om Aktiviteter och välj sedan de funktioner som du vill ge under **Finjustera dina inställningar**.

   ![finjustera aktivitetsinställningarna](assets/fine-tune-tasks.png)

   >[!NOTE]
   >
   >När du konfigurerar en åtkomstnivåinställning för en viss typ av objekt påverkar den konfigurationen inte användarens åtkomst till objekt med lägre rankning. Du kan till exempel begränsa användarnas möjlighet att ta bort uppgifter på åtkomstnivå, men detta förhindrar inte att de tar bort problem som är mindre rankade än uppgifter. Mer information om objekthierarkin finns i avsnittet [Objektens inbördes beroende och hierarki](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Valfritt) Om du vill begränsa ärvda behörigheter för aktiviteter från högre rankningsobjekt klickar du på **Ange ytterligare begränsningar** och väljer sedan **Ärv aldrig dokumentåtkomst från projekt, aktiviteter, utgåvor osv.**.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Åtkomst till uppgifter per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med uppgifter finns i avsnittet [Åtgärder](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#tasks) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Åtkomst till delade uppgifter

Som ägare eller skapare av ett problem kan du dela med andra användare genom att ge dem behörighet till det, vilket förklaras i [Dela en uppgift](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

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

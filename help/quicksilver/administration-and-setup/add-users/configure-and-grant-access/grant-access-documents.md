---
title: Bevilja åtkomst till dokument
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till dokument i Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Bevilja åtkomst till dokument

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till dokument, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Den här åtkomsten gäller även dokumentmappar.

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
   <td> <p>Du måste vara Workfront-administratör.&gt;.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera användaråtkomst till dokument med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på **Visa** eller **Redigera** till höger om Dokument och välj sedan de funktioner som du vill bevilja under **Finjustera inställningarna**.

   ![document_access.png](assets/document-access.png)

   Du kan tillåta användare att göra följande i projekt, uppgifter och ärenden som de har tillgång till:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Skapa</td> 
      <td>Överför dokument.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort</td> 
      <td> <p>Ta bort överförda dokument.</p> <p>The <b>Skapa</b> aktiveras automatiskt när det här alternativet är aktiverat.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela</td> 
      <td>Dela dokument med specifika användare, roller, team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela dokument offentligt</td> 
      <td>Dela dokument med externa användare (saknar Workfront-licens).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela hela systemet</td> 
      <td> <p>Gör dokumenten tillgängliga för alla i Workfront.</p> <p>Alla i systemet kan se ett dokument som delas på det här sättet om:</p> 
       <ul> 
        <li> <p>Du skickar en länk till sidan Dokument där den har överförts.</p> </li> 
        <li> <p>De söker i Workfront</p> </li> 
       </ul> <p>The <b>Dela</b> aktiveras automatiskt när det här alternativet är aktiverat.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >När du konfigurerar en åtkomstnivåinställning för en viss typ av objekt påverkar den konfigurationen inte användarens åtkomst till objekt med lägre rankning. Du kan t.ex. hindra användare från att ta bort projekt på åtkomstnivån, men detta förhindrar dem inte från att ta bort dokument som har lägre rankning än projekt.Mer information om objekthierarkin finns i avsnittet [Objektens inbördes beroende och hierarki](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Valfritt) Om du vill begränsa ärvda behörigheter för dokument från högre rankningsobjekt klickar du på **Ange ytterligare begränsningar** väljer **Ärv aldrig dokumentåtkomst från projekt, uppgifter, ärenden osv.**.
1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med någon av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Åtkomst till dokument per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med dokument finns i avsnittet [Dokument](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Åtkomst till delade dokument

När du har överfört ett dokument till Workfront kan du dela det med andra användare genom att ge dem behörighet till det, vilket förklaras i [Dela ett dokument](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

När du delar ett objekt med en annan användare bestäms mottagarens rättigheter till det av en kombination av två saker:

* De behörigheter som du ger mottagaren för objektet
* Mottagarens åtkomstnivåinställningar för objektets typ

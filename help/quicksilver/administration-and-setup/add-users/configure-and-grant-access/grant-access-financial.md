---
title: Bevilja åtkomst till finansiella data
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du definiera en användares åtkomst till ekonomiska data i Workfront via åtkomstnivån.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 97f5adc8811a3be7be23137a82d10d45b76ec605
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Bevilja åtkomst till finansiella uppgifter

{{highlighted-preview}}

Som Adobe Workfront-administratör kan du definiera en användares åtkomst till följande via användarens åtkomstnivå, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Ekonomisk information om projekt i Workfront
* Resursbudgetinformation i Resursplaneringsverktygen

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
    <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överväganden att bevilja tillgång till finansiella uppgifter

Tänk på följande när du ger användare tillgång till ekonomiska data i Workfront:

* En användare vars åtkomstnivå inte tillåter åtkomst till ekonomiska data kan inte ge åtkomst som skulle göra det möjligt för andra att visa ekonomiska data. Detta innefattar att ge åtkomst till projekt som skulle visa ekonomiska data, eller ändra en åtkomstnivå för att tillåta visning av ekonomiska data.
* En användare vars åtkomstnivå inte tillåter åtkomst till ekonomiska data kan inte skapa en risk för ett projekt. Mer information finns i [Skapa och redigera risker i projekt](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* Du kan också använda en åtkomstnivå för att avgöra vilka resurshanteringsaktiviteter en användare kan använda för att budgetera eller visa resursallokering. Mer information finns i [Bevilja åtkomst till resurshantering](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Konfigurera användaråtkomst till ekonomiska data med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen **Visa** eller **Redigera** till höger om Finansiella data och välj sedan de funktioner som du vill ge under **Finjustera dina inställningar**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Valfritt) Välj följande alternativ i området **Tillåt administrativ åtkomst för**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Växelkurser</td> 
      <td> <p>Lägg till ny valuta i Workfront.</p> <p>Utan den här åtkomsten kan användaren bara lägga till en befintlig valuta i ett projekt som han/hon skapar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td> <p>Visa alla utgifter för objekt i Workfront.</p> <p>Detta gör att användaren inte kan skapa nya utgiftstyper.</p> <p>Utan den här åtkomsten kan användaren bara visa följande:</p> 
       <ul> 
        <li>Utgifter för projekt, uppgifter eller ärenden som de hanterar</li> 
        <li>Deras egna utgifter</li> 
        <li>Utgifter för underordnade</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Tillgång till delad finansiell information

Du kan dela ekonomisk information om ett projekt, en uppgift eller ett problem med andra användare genom att ge dem behörighet till det, vilket förklaras i [Dela ekonomiska behörigheter för ett objekt](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

När du delar ett objekt med en annan användare bestäms mottagarens rättigheter till det av en kombination av två saker:

* De behörigheter som du ger mottagaren för objektet
* Mottagarens åtkomstnivåinställningar för objektets typ

## Tillgång till ekonomisk information per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med ekonomisk information finns i avsnittet [Ekonomisk information](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Tillgång till ekonomisk information genom att ställa in

Följande information kan hjälpa dig att förstå hur du använder åtkomstnivåinställningarna för att styra användarnas åtkomst till ekonomiska data.

### Ingen åtkomst

En användare utan åtkomst till ekonomiska data har inte åtkomst till följande:

* Avsnittet Ekonomi under Projekt och uppgifter
* Affärsärende
* Faktureringspriser och faktureringsposter
* <span class="preview">Betygsätt kort</span>
* Kostnad per timme och fakturering per timme i användarinställningarna

  Du kan konfigurera detta med kugghjulsikonen ![](assets/gear-icon-settings.png) på Visa-knappen i steg 4 ovan.

* Kostnad per timme och fakturering per timme för jobbroller

  Du kan konfigurera detta med kugghjulsikonen ![](assets/gear-icon-settings.png) på Visa-knappen i steg 4 ovan.

### Visa åtkomst

En användare med behörigheten Visa för ekonomiska data kan visa (inte redigera) följande:

* Avsnittet Ekonomi under Projekt och uppgifter
* Affärsärende
* Faktureringspriser och faktureringsposter
* Kostnad per timme och fakturering per timme i användarinställningarna

  Du kan konfigurera detta med kugghjulsikonen ![](assets/gear-icon-settings.png) på Visa-knappen i steg 4 ovan.

* Kostnad per timme och fakturering per timme för jobbroller

  Du kan konfigurera detta med kugghjulsikonen ![](assets/gear-icon-settings.png) på Visa-knappen i steg 4 ovan.

### Redigera åtkomst

En användare med Redigera-åtkomst till ekonomiska data kan visa och redigera följande:

* Avsnittet Ekonomi under Projekt och uppgifter
* Affärsärende
* Faktureringspriser och faktureringsposter
* <span class="preview">Betygsätt kort</span>
* Kostnad per timme och fakturering per timme i användarinställningarna

  Du kan konfigurera detta med kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen Redigera i steg 4 ovan.

* Kostnad per timme och fakturering per timme för jobbroller

  Du kan konfigurera detta med kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen Redigera i steg 4 ovan.

---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Dela en kontrollpanel
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera kontrollpaneler när de tilldelar åtkomstnivåer. Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera specifika instrumentpaneler som du har åtkomst till att dela.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Dela en kontrollpanel

Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera kontrollpaneler när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till problem finns i [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera specifika instrumentpaneler som du har åtkomst till att dela. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

## Åtkomstkrav

Du måste ha följande för att kunna dela objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Visa åtkomst eller högre till rapporter, instrumentpaneler, kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa behörigheter eller högre på kontrollpanelen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Kontrollpanelen måste skapas innan du kan dela den.

Mer information om hur du skapar instrumentpaneler finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Att tänka på när det gäller att dela kontrollpaneler

Förutom övervägandena nedan finns även [Dela rapporter, instrumentpaneler och kalendrar](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Den som har skapat en kontrollpanel har som standard behörigheten Hantera.

* Du kan dela kontrollpaneler som du skapar med andra personer, team, grupper, jobbroller eller företag. Du kan också dela kontrollpaneler som andra har skapat och som delats med dig.
* Du kan också dela dem med hela organisationen genom att göra dem synliga i hela systemet.
* Du kan dela en enskild kontrollpanel eller dela flera kontrollpaneler från en lista.
* När du delar en kontrollpanel ärver användarna som standard behörigheten Visa till alla rapportobjekt på kontrollpanelen.

  Mer information om objekthierarkin i Workfront finns i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Mer information om hur du visar ärvda behörigheter finns i [Visa ärvda behörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Dela en kontrollpanel

Att dela en eller flera kontrollpaneler från en lista är identiskt.

1. Gå till en lista med instrumentpaneler och markera en eller flera instrumentpaneler. Klicka sedan på **Dela** ![](assets/share-icon.png).

   eller

   Klicka på namnet på en instrumentpanel och klicka sedan på **Instrumentpanelsåtgärder >****Delning**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. I fältet **Lägg till personer, team, roller, grupper eller företag ...** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela instrumentpanelen med och klickar sedan på namnet i listrutan.
1. (Valfritt) Om du vill att instrumentpanelen ska vara tillgänglig för alla användare i systemet klickar du på ikonen **Inställningar** i det övre högra hörnet av delningsdialogrutan och väljer sedan **Gör den synlig i hela systemet**.

1. Klicka på **Spara**.

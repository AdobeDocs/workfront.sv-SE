---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Dela ett mål i Workfront-mål
description: När du delar ett mål ger du ett mål behörigheten Hantera till någon som inte skapat det.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# Dela ett mål i Adobe Workfront-mål

När du delar ett mål ger du ett mål behörigheten Hantera till någon som inte skapat det.

## Åtkomstkrav

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för Adobe Workfront Goals för att få tillgång till de funktioner som beskrivs i den här artikeln. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mål eller högre</p> <p><b>ANMÄRKNING</b><p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Bevilja åtkomst till Adobe Workfront-mål</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <div> 
     <p>Hantera behörigheter för målet</p> 
     <p>Mer information om delningsmål finns i <a href="#" class="MCXref xref selected">Dela ett mål i Workfront-mål</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du ha följande:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Överväganden om att dela mål

* Användarna kan ha följande behörigheter för ett mål:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Målbehörigheter</b></p></td> 
      <td>
      <p><b>Beskrivning</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Visa</p></td> 
      <td>
      <p>Användarna har behörighet att visa målet, men de kan inte redigera information för målet, de kan inte lägga till eller redigera information för resultat, aktiviteter, uppdateringsstatus eller ta bort målet.</p>      
      <p>Som standard kan alla användare med åtkomst till mål visa alla mål i systemet. Användarna kan kopiera målet om de har Redigera-åtkomst till mål på åtkomstnivå.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Hantera</p></td> 
      <td> <p>Användarna kan redigera all information för målet, även för resultaten, eller aktiviteter, inklusive ta bort dem.</p> 
      <p>Det är bara målskapare eller målanvändare som specifikt får behörigheten Hantera för ett mål som kan hantera ett mål.</p> 
      Endast användare med behörigheten Hantera för ett mål kan dela målet med andra för att ge dem behörigheten Hantera för målet. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Du kan dela följande typer av mål med andra:

   * Ett mål du skapat
   * Ett mål som har skapats av någon annan som du har fått behörighet att hantera.

* Om du har behörigheten Hantera för ett mål kan du ändra behörigheterna för målskaparen. Som standard har de behörigheten Hantera när de skapar målet, men du kan ändra deras behörigheter till Visa.

## Dela ett mål

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Mållistan visas.

1. Klicka på namnet på ett mål i listan. Målsidan öppnas.

1. Klicka på **Mer-ikon** bredvid målnamnet och klicka sedan på **Dela**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Rutan Målåtkomst visas.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Gör något av följande:

   * Välj **Hantera hela systemet** inställning för att ge hanteringsbehörighet till alla i systemet som har Redigera-åtkomst till mål på åtkomstnivå. Detta är som standard avmarkerat för alla nya mål.
   * Börja skriva namnet på en användare som du vill ge behörigheten Hantera i **Ge Hantera åtkomst till** box. Markera namnet när det visas i listan.

      >[!TIP]
      >
      >Du kan bara dela ett mål med andra användare. Du kan inte dela mål med grupper, team eller ditt företag.

1. Klicka **Dela**.

   Målet delas med de användare som du har angett. En etikett för hela systemet eller namnet på de användare som har behörigheten Hantera för målet visas i fältet Åtkomst till hantering på panelen Målinformation.

## Alternativ för målbehörighet

I följande tabell visas de behörigheter som du kan ge när du delar ett mål. Mer information om vilka användare som får åtkomst baserat på deras licens finns i [Bevilja åtkomst till Adobe Workfront-mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Åtgärder</strong> </p> </th> 
   <th> <p><strong>Hantera</strong> </p> </th> 
   <th> <p><strong>Visa</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Visa mål</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visa resultat eller aktiviteter</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Kopiera mål* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konvertera resultat eller aktiviteter till andra mål*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Visa projekt som lagts till som aktiviteter** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Redigera mål</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera resultat eller aktiviteter</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Lägg till resultat eller aktiviteter för målet</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Associera ett projekt som en aktivitet med målet**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ta bort mål</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Radera resultat eller aktiviteter</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Koppla bort projekt från målet</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Du måste ha behörighet att redigera för mål på din åtkomstnivå för att kunna konvertera resultat och aktiviteter till mål.

**Du måste ha åtkomst till Visa projekt och behörigheten Visa för de projekt som läggs till eller som du vill lägga till i målet för att kunna visa dem.

Mer information om åtkomstnivå för projekt finns i [Bevilja åtkomst till projekt](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Mer information om projektbehörigheter finns i [Dela ett projekt i Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 

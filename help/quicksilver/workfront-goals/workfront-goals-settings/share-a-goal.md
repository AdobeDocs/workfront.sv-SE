---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Dela ett mål i Workfront-mål
description: När du delar ett mål ger du ett mål behörigheten Hantera till någon som inte skapat det.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# Dela ett mål i Adobe Workfront-mål

När du delar ett mål ger du ett mål behörigheten Hantera till någon som inte skapat det.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> 
   <p>För den nya planen och licensstrukturen:
  <ul><li>En Ultimate-plan </li></ul>
   </p>
<p>För aktuell plan och licensstruktur: 
<ul><li> En Pro eller högre </li>
  <li>En Adobe Workfront Goals-licens förutom en Workfront-licens.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens*</td>
 <td>
 <p>Ny licens: Medarbetare eller högre</p>
 eller
 <p>Aktuell licens: Begär eller högre</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Nytt produktkrav, något av följande: </p>
<ul>
<li>A Select- eller Prime Adobe Workfront-plan och ytterligare licens för Adobe Workfront Goals.</li>
<li>En Ultimate Workfront-plan som innehåller Workfront-mål som standard. </li></ul>
 <p>eller</p>
 <p>Aktuellt produktkrav: En Workfront-plan och ytterligare licens för Adobe Workfront-mål. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Mållistan visas.

1. Klicka på namnet på ett mål i listan. Målsidan öppnas.

1. Klicka på ikonen **Mer** bredvid målnamnet och klicka sedan på **Dela**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Rutan Målåtkomst visas.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Gör något av följande:

   * Välj inställningen **Hantera i hela systemet** om du vill ge alla i systemet som har Redigera-åtkomst till mål på åtkomstnivån Hantera-behörighet. Detta är som standard avmarkerat för alla nya mål.
   * Börja skriva namnet på en användare som du vill ge behörigheten Hantera i rutan **Ge behörigheten Hantera till**. Markera namnet när det visas i listan.

     >[!TIP]
     >
     >Du kan bara dela ett mål med andra användare. Du kan inte dela mål med grupper, team eller ditt företag.

1. Klicka på **Dela**.

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

 

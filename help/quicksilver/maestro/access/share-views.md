---
title: Visa
description: Du kan dela en vy med andra för att säkerställa samarbete när du använder Adobe Workfront-planering.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Visa

{{maestro-important-intro}}

Du kan dela en vy med andra för att säkerställa samarbete när du arbetar med poster i Adobe Workfront-planering.

Om du ger behörighet till en arbetsyta ger det inte andra användare behörighet till vyerna på posttypssidorna. Du måste tilldela behörigheter till enskilda vyer på en posttypsida för att kunna dela dem med andra användare.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Workfront planerar stängda. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> Det finns inga åtkomstkontroller för Adobe Workfront-planering </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td> <p>Hantera behörigheter till en vy</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/maestro/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Dela behörigheter till en vy

Du kan dela vyer som du har skapat eller vyer som du har behörighet att hantera.

>[!NOTE]
>
>Systemadministratörer kan inte visa eller dela vyer som de inte själva skapat. De kan bara komma åt eller dela vyer som delas med dem.
>
>Systemadministratörer kan bara ha behörigheten Hantera för en vy.

{{step1-to-maestro}}

1. Öppna arbetsytan vars vy du vill dela och klicka sedan på ett posttypskort.

   Då öppnas posttypssidan.

1. Håll markören över den vy du vill dela på fliken Visa och klicka på **Mer** meny ![](assets/more-menu.png) till höger om vynamnet och klicka sedan på **Dela**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. I **Ge vy åtkomst till** börjar du skriva namnet på en användare eller grupp och klickar sedan på den när den visas i listan.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Välj någon av följande behörighetsnivåer i listrutan:
   * Visa
   * Hantera

     Mer information om behörighetsnivåer och vilka åtgärder användare kan utföra för varje nivå finns i [Översikt över delningsbehörigheter i Adobe Workfront-planeringen](../access/sharing-permissions-overview.md).

     <!--System administrators always receive Manage permissions to views shared with them.-->

1. Klicka **Kopiera länk** om du vill kopiera en länk till vyn till Urklipp.
1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt posttypssidan och visa den i den valda vyn.
1. Klicka **Spara**.

## Ta bort behörigheter till en vy

{{step1-to-maestro}}

1. Öppna arbetsytan vars vy du vill dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.
1. Håll markören över den vy du vill dela i listrutan Visa och klicka på **Mer** meny ![](assets/more-menu.png) till höger om vynamnet och klicka sedan på **Dela**.
1. Hitta användaren eller gruppen du vill ta bort och klicka sedan på **Ta bort** i listrutan Behörigheter till höger om användarens eller gruppens namn.
1. Klicka **Spara**.
Användaren eller användarna som tillhör gruppen som tagits bort har inte längre åtkomst till vyn. Det finns inget meddelande för de användare som har tagits bort från vyn.

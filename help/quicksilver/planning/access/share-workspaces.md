---
title: Dela arbetsytor
description: Du kan dela en arbetsyta med andra för att säkerställa samarbete när du arbetar i Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Planning as a product ??-->

# Dela arbetsytor

{{planning-important-intro}}

Du kan dela en arbetsyta med andra för att säkerställa samarbete när du arbetar i Adobe Workfront Planning.

>[!NOTE]
>
>Om du ger behörighet till en arbetsyta ger det inte andra användare behörighet till vyerna på posttypssidorna. Du måste tilldela behörigheter till enskilda vyer på en posttypsida för att kunna dela dem med andra användare. Mer information finns i [Dela en vy](/help/quicksilver/planning/access/share-views.md).


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela behörigheter till en arbetsyta

Följande användare kan dela en arbetsyta med andra användare:

* Systemadministratörer kan dela alla arbetsytor, inklusive de som de inte skapade.
* Alla andra användare kan bara dela arbetsytor som de har behörighet att hantera.

Så här delar du en arbetsyta med andra:

{{step1-to-planning}}

1. Öppna arbetsytan som du vill dela och klicka sedan på **Dela** i skärmens övre högra hörn.

   ![](assets/share-button-on-workspace-top-right.png)

1. I fältet **Bevilja arbetsyteåtkomst till** börjar du skriva namnet på en användare eller grupp och klickar sedan på den när den visas i listan.

   ![](assets/sharing-ui-with-groups.png)

1. Välj någon av följande behörighetsnivåer i listrutan:
   * Visa
   * Contribute
   * Hantera

     Mer information om behörighetsnivåer och vilka åtgärder användare kan utföra för varje nivå finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Klicka på **Kopiera länk** om du vill kopiera en länk till arbetsytan till Urklipp.
1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan.
1. Klicka på **Spara**.


## Ta bort behörigheter till en arbetsyta


{{step1-to-planning}}

1. Öppna arbetsytan som du vill ta bort behörigheter till och klicka sedan på **Dela** i skärmens övre högra hörn.
1. Klicka på listrutan till höger om ett användar- eller gruppnamn och klicka sedan på **Ta bort**.
1. Klicka på **Spara**.

   Användaren eller användarna som tillhör gruppen som tagits bort har inte längre åtkomst till arbetsytan eller dess objekt.
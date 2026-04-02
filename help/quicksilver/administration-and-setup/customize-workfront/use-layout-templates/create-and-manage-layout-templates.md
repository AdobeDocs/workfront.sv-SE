---
title: Skapa och hantera layoutmallar
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Som Workfront-administratör eller gruppadministratör kan du skapa och ändra layoutmallar för att anpassa layoutelement i Workfront för dina användare.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Skapa och hantera layoutmallar

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

{{highlighted-preview}}

Som Adobe Workfront-administratör eller gruppadministratör kan du skapa och ändra layoutmallar för att anpassa följande layoutelement i Workfront:

* Huvudmeny
* Navigeringspanelen till vänster
* Hemsida
* Panelen Sammanfattning
* Vyer, filter och grupperingar som andra använder med listor och rapporter.
* Terminologi på skärmen
* <span class="preview">Objektrubriker</span>
* <span class="preview">Mer meny (trepunktsmeny) för ett objekt</span>

När du har skapat eller ändrat en layoutmall kan du tilldela den till enskilda användare, team, grupper eller jobbroller.

Alla användares standardlayout för Workfront beror på åtkomstnivå och licenstyp. Vissa användare kanske inte ser vissa områden på huvudmenyn. Mer information finns i [Om Adobe Workfront standardlayout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.</p>
        <p>Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du skapar och hanterar layoutmallar

* Användarna kan anpassa några områden i sin egen layout. När du ändrar en layoutmall sammanfogas ändringarna med eventuella anpassningar som de har gjort, utan att de skrivs över eller återställs. Detta gäller även om du tilldelar användare till en ny layoutmall.
* Gruppadministratörer och användare med en planlicens som kan redigera andra användare kan lägga till layoutmallar på system- och gruppnivå till de användare som de kan hantera när de redigerar sin profil.
* Gruppadministratörer kan inte tilldela layoutmallar till jobbroller eller team.

Mer information om layoutmallar finns i [Layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Skapa eller ändra en layoutmall

{{step-1-to-setup}}

1. Klicka på **Gränssnitt** > **Layoutmallar** i den vänstra panelen.

1. Klicka på **Ny layoutmall**.

   eller

   Klicka på namnet på layoutmallen som du vill ändra.

1. Om du skapar en ny layoutmall skriver du ett **layoutmallnamn** och (valfritt) en **beskrivning** för den.

1. Anpassa delar av användargränssnittet enligt följande artiklar:

   * [Anpassa huvudmenyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Anpassa den vänstra panelen med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Anpassa menyn Mer med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-more-menu.md)
   * [Anpassa fästa sidor med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Anpassa panelen Sammanfattning med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Anpassa startsidan med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [Anpassa landningssidan med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Anpassa användargränssnittsterminologi med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Fortsätt att testa layoutmallen och göra den tillgänglig för användare, så som beskrivs i artiklarna nedan:

   * [Testa en ny layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Bevilja administrativ åtkomst för en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Tilldela användare till en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Du kan också skapa en layoutmall genom att kopiera den och ändra den kopierade versionen. Mer information finns i [Kopiera en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).


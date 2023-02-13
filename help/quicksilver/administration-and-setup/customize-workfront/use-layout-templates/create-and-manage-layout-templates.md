---
title: Skapa och hantera layoutmallar
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Som Workfront-administratör eller gruppadministratör kan du skapa och ändra layoutmallar för att anpassa layoutelement i Workfront för dina användare.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Skapa och hantera layoutmallar

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Som Workfront-administratör eller gruppadministratör kan du skapa och ändra layoutmallar för att anpassa följande layoutelement i Workfront för dina användare:

* Huvudmeny
* Navigeringspanelen till vänster
* Hemsida
* Vyer, filter och grupperingar som andra använder med listor och rapporter.
* Terminologi på skärmen

När du har skapat eller ändrat en layoutmall kan du tilldela den till enskilda användare, team, grupper eller jobbroller.

Alla användares standardlayout för Workfront beror på åtkomstnivå och licenstyp. Vissa användare kanske inte ser vissa områden på huvudmenyn. Mer information finns i [Om Adobe Workfront standardlayout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.
Om du vill utföra dem för en grupp måste du vara gruppchef.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Att tänka på när du skapar och hanterar layoutmallar

* Användarna kan anpassa några områden i sin egen layout. När du ändrar en layoutmall sammanfogas ändringarna med eventuella anpassningar som de har gjort, utan att de skrivs över eller återställs. Detta gäller även om du tilldelar användare till en ny layoutmall.
* Dina äldre layoutmallar som skapats i Adobe Workfront Classic har automatiskt varit tillgängliga i den nya Adobe Workfront-upplevelsen sedan de migrerades i början av hösten 2019. Layoutmallar som skapats i Adobe Workfront Classic efter den tidpunkten migrerades i april 2020. Vi rekommenderar att du uppdaterar dessa layoutmallar i den nya Adobe Workfront-upplevelsen för att utnyttja de nya funktionerna och göra dem ännu mer användbara i den miljön.
* Gruppadministratörer och användare med en planlicens som kan redigera andra användare kan lägga till layoutmallar på system- och gruppnivå till de användare som de kan hantera när de redigerar sin profil.
* Gruppadministratörer kan inte tilldela layoutmallar till jobbroller eller team.

Mer information om layoutmallar finns i [Layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Skapa eller ändra en layoutmall

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Gränssnitt** > **Layoutmallar**.

1. Klicka **Ny layoutmall**.

   eller

   Klicka på namnet på layoutmallen som du vill ändra.

1. Om du skapar en ny layoutmall skriver du en **Namn på layoutmall** och (valfritt) a **Beskrivning** för den.

1. Anpassa delar av användargränssnittet enligt följande artiklar:

   * [Anpassa huvudmenyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Anpassa den vänstra panelen med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Anpassa fästa sidor med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Anpassa hem och sammanfattning med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Anpassa landningssidan med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Anpassa användargränssnittsterminologi med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Fortsätt med att testa layoutmallen och göra den tillgänglig för användare, så som beskrivs i artiklarna nedan:

   * [Testa en ny layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Bevilja administrativ åtkomst för en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Tilldela användare till en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

Du kan också skapa en ny layoutmall genom att kopiera den och ändra kopian. Mer information finns i [Kopiera en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

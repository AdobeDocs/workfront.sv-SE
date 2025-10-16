---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Lås upp eller lås konfigurationen av händelsemeddelanden för alla grupper
description: Om du är Adobe Workfront-administratör kan du låsa upp eller låsa upp möjligheten för gruppadministratörer att konfigurera ett händelsemeddelande för de grupper på den översta nivån som de hanterar. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Lås upp eller lås konfigurationen av händelsemeddelanden för alla grupper

Om du är Adobe Workfront-administratör kan du låsa upp eller låsa upp möjligheten för gruppadministratörer att konfigurera ett händelsemeddelande för de grupper på den översta nivån som de hanterar. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

När en administratör konfigurerar ett händelsemeddelande för en grupp påverkar konfigurationen användare för vilka gruppen, eller en av dess undergrupper, är deras hemgrupp. I sina användarprofiler ser dessa användare händelsemeddelanden som aktiveras för hemgruppen i stället för händelsemeddelanden som aktiveras i hela systemet. Mer information finns i [Visa och konfigurera händelsemeddelanden för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* En Workfront-administratör kan låsa upp och låsa upp konfigurationen på nytt för ett händelsemeddelande i både Adobe Workfront Classic och den nya Adobe Workfront-upplevelsen. Men en gruppadministratör kan bara konfigurera händelsemeddelandet för en grupp i den nya Adobe Workfront-upplevelsen. Gruppadministratörer som använder Adobe Workfront Classic kan växla till den nya Adobe Workfront-funktionen för att konfigurera olåsta händelsemeddelanden för en grupp och sedan växla tillbaka till Adobe Workfront Classic för att se ändringarna.
>* Undergrupper ärver händelsemeddelandekonfigurationer på gruppnivå från de översta grupperna ovanför dem.
>

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
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Systemadministratör</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lås upp eller låsa upp möjligheten att konfigurera ett händelsemeddelande igen

>[!IMPORTANT]
>
>När du låser ett meddelande igen ärver alla grupper i systemet meddelandet exakt som du ställt in det. Detta åsidosätter ändringar som gruppadministratörer kan ha gjort för sina grupper, så det är en bra idé att först rådfråga dem.

{{step-1-to-setup}}

1. Klicka på **E-post** > **Meddelanden**.

1. Kontrollera att fliken **Händelsemeddelanden** är öppen.
1. Klicka på ikonen till höger om meddelandet för att växla till den låsta ![låsikonen](assets/lock-toggle-button.png) eller upplåst ![upplåsikonen](assets/unlock-toggle-button.png) .

   eller

   Om du vill låsa upp eller låsa upp flera meddelanden samtidigt markerar du dem och klickar sedan på knappen Lås upp ![ikon](assets/unlock-icon-toolbar.png) eller Lås ![ikon](assets/lock-icon-locked-qs.png) som visas i verktygsfältet ovanför listan.

1. Klicka på **Spara**.
1. (Valfritt) Om du vill konfigurera händelsemeddelandet för en grupp på den översta nivån i stället för att lämna den här uppgiften till gruppens administratör kan du göra något av följande:

   * Ta bort **systemhändelsemeddelanden** i sökrutan ovanför listan med meddelanden, sök efter och markera namnet på den översta gruppen för att visa dess meddelanden och aktivera eller inaktivera sedan de olåsta meddelandena i listan som visas.
   * Klicka på **Grupper** i den vänstra menyn och klicka sedan på namnet på den översta gruppen. Klicka på **Händelsemeddelanden** i den vänstra panelen och konfigurera sedan det olåsta händelsemeddelandet enligt beskrivningen i [Visa och konfigurera händelsemeddelanden för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

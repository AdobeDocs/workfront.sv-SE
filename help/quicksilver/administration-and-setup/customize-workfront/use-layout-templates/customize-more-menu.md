---
title: Anpassa menyn Mer med hjälp av en layoutmall
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 'Du kan använda en layoutmall för att avgöra vilka alternativ som visas när en användare klickar på Mer-menyn (menyn med tre punkter) när du visar följande objekt i Adobe Workfront: projekt, uppgifter, utgåvor, portföljer och program.'
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 2faeea4f8128b7858232048d687c270a1e3709f5
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Anpassa menyn Mer med en layoutmall

{{highlighted-preview-article-level}}

Du kan använda en layoutmall för att avgöra vilka alternativ som visas när en användare klickar på Mer-menyn (menyn med tre punkter) när du visar följande objekt i Adobe Workfront: projekt, uppgifter, utgåvor, portföljer och program.

![Menyn Mer exempel för ett projekt](assets/more-menu-display-for-project.png)

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla</td> 
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

## Anpassa menyn Mer för ett område i Workfront

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på namnet på en objekttyp eller ett Workfront-område vars Mer-meny du vill anpassa på den nedrullningsbara menyn **Anpassa vad användare ser**.
1. Klicka på **Välj menyalternativ**.
1. Gör något av följande i rutan **Välj menyalternativ** för att avgöra vad användare ska se på Mer-menyn för det Workfront-område eller den objekttyp som du har valt:

   * Klicka på ikonerna **Visa** ![Visa ](assets/add-secondary-nav-item.png) eller **Dölj** ![Dölj ikon](assets/delete-secondary-nav-item.png) om du vill visa eller dölja avsnitt i den vänstra panelen. Du kan inte dölja objekt som inte har en **Visa**- eller **Dölj**-ikon.

   * Dra objekt ![Flytta ikon](assets/move-icon---dots.png) om du vill ändra deras ordning på den vänstra panelen.

1. Klicka på **Klar**.

---
title: Konfigurera en anpassad hjälp-URL
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Om du skapar en anpassad intern hjälpwebbplats som innehåller information om hur din organisation använder Workfront kan du konfigurera hjälpikonen för huvudmenyn för att gå till den webbplatsen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Konfigurera en anpassad hjälp-URL

Om du skapar en anpassad intern hjälpwebbplats som innehåller information om hur din organisation använder Workfront kan du konfigurera hjälpikonen för huvudmenyn för att gå till den webbplatsen.

![](assets/custom-help-button.png)

Detta påverkar inte de sammanhangsberoende hjälplänkarna i Workfront, som tar användarna till Workfront hjälpwebbplats.

Mer information om hur användare kommer åt både en anpassad hjälp-URL som du konfigurerar i Workfront och den vanliga Workfront-hjälpwebbplatsen finns i [Få åtkomst till Adobe Workfront-hjälpen](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera en anpassad hjälp-URL

{{step-1-to-setup}}

1. Klicka på **System** > **Inställningar**.
1. I avsnittet **Allmänna inställningar** skriver du den URL där din anpassade hjälpwebbplats finns i fältet **Anpassad hjälp-URL**.

   Om din anpassade hjälpplats kräver inloggningsuppgifter krävs dessa för användare när de kommer åt webbplatsen från Workfront. Autentiseringsuppgifterna till din anpassade hjälpwebbplats kan behöva hanteras separat från Workfront-autentiseringsuppgifterna om du inte använder enkel inloggning (SSO).

1. Klicka på **Spara**.

   När du har sparat en anpassad hjälp-URL kan du gå tillbaka till Workfront standardhjälpwebbplats genom att ta bort den anpassade URL:en och klicka på **Spara**.

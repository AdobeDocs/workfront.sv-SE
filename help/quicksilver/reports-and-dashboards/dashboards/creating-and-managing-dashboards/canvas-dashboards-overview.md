---
product-area: dashboards
navigation-topic: creating-and-managing-dashboards
title: Översikt över kontrollpaneler på arbetsytan
description: Du kan skapa kontrollpaneler för arbetsytan som integrerar visualiseringar för arbetsytan i rapporten med traditionella rapporter och har nya layoutalternativ.
author: Nolan
feature: Reports and Dashboards
exl-id: b02ca181-e3c3-41e9-ab45-b1b606909127
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Översikt över kontrollpaneler på arbetsytan

<!-- Audited: 12/2023 -->

Canvas Dashboards, en funktion som för närvarande är under utveckling för Dashboards, erbjuder ett nytt alternativ för att skapa effektiva kontrollpaneler i Workfront. Arbetsytans kontrollpaneler gör det enkelt att ta med visualiseringar av arbetsytan i befintliga rapporter, vilket ger större flexibilitet och nya layoutalternativ.

Den här funktionen är under utveckling och stöder ännu inte:
* externa sidor
* kalenderintegrering
* rapporter
* distribution via layoutmallar

En fullständig lista över funktioner som har lagts till på arbetsytans kontrollpaneler finns på [Kontrollpaneler på arbetsytan: frisläppningsaktivitet](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md)

## Åtkomst till Canvas-instrumentpaneler

Ett nytt alternativ för Canvas Dashboards på den vänstra panelen på den befintliga kontrollpanelens startsida kan aktiveras för att få åtkomst till Canvas Dashboards. Det här menyalternativet är som standard inaktiverat och måste vara aktiverat för att du ska få åtkomst. Se instruktionerna nedan för mer information om hur du aktiverar menyalternativet och navigerar till det.

### Lägg till kontrollpaneler för arbetsytan på den vänstra panelen på kontrollpanelerna

>[!IMPORTANT]
>
>Du måste ha minst behörigheten Visa för rapporter och instrumentpaneler för att kunna växla till objektet Kontrollpaneler på arbetsytan i layoutmallen.

1. Börja arbeta med layoutmallen där du vill aktivera Canvas-kontrollpaneler enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicka på **Anpassa det användarna ser** listrutemeny och klicka sedan på **Kontrollpaneler**.

1. I **Vänster panel** listan som visas nedan klickar du på ![](assets/delete-secondary-nav-item.png) ikon bredvid **Kontrollpaneler på arbetsytan**. Ikonen ändras till ![](assets/add-secondary-nav-item.png) om du vill visa att den nu visas i den vänstra panelen för kontrollpaneler.

1. Klicka **Spara** längst ned på skärmen.

### Öppna Canvas-instrumentpaneler

1. Kontrollera att du har aktiverat alternativet Kontrollpaneler på arbetsytan i layoutmallen. Se **Lägga till kontrollpaneler för arbetsytan på kontrollpanelmenyn** ovan för instruktioner.

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon.png)och sedan klicka **Kontrollpaneler**.

1. Klicka på i den vänstra panelen **Kontrollpaneler på arbetsytan**.

## Använda Canvas-paneler

### Skapa en ny arbetsytans kontrollpanel

1. Öppna Canvas-instrumentpaneler enligt beskrivningen i **Öppna Canvas-instrumentpaneler** ovan.

1. Klicka **+ Ny instrumentpanel**

1. Klicka **Namnlös** i det övre vänstra hörnet om du vill ange ett namn för instrumentpanelen.

1. Klicka **Klar** i det övre högra hörnet för att spara din nya instrumentpanel eller börja lägga till widgetar enligt beskrivningen i **Lägga till en rapport på en arbetsytans kontrollpanel** nedan.

### Lägga till en rapport på en arbetsytans kontrollpanel

1. Öppna Canvas-instrumentpaneler enligt beskrivningen i **Öppna Canvas-instrumentpaneler** ovan.

1. Klicka på den kontrollpanel där du vill lägga till en rapport från listan med kontrollpaneler.

1. Klicka **Hantera widgetar** i det övre högra hörnet och klicka sedan på **Lägg till widget**.

1. Håll muspekaren över den typ av rapportwidget som du vill lägga till och klicka sedan på kryssrutan som visas.

1. När du har markerat alla widgetar du vill lägga till klickar du på **Lägg till** längst upp till höger.

1. De valda widgetarna visas på kontrollpanelen. Klicka **Konfiguration** i mitten av en widget för att välja vilken rapport som ska visas.

1. Börja skriva in namnet på rapporten som du vill visa i dialogrutan **Sök rapport** fält. När du ser rapporten i listan klickar du på **Listrapport** eller **Diagramrapport** -ikonen bredvid dess namn för att visa informationen från rapporten i det format du valt.

>[!WARNING]
> Det går för närvarande att lägga till flera widgetar som visar information från samma rapport, men vi rekommenderar att du bara visar varje rapport en gång eftersom det kan påverka kontrollpanelens prestanda.

### Redigera en widget på en arbetsytans kontrollpanel

1. Öppna Canvas-instrumentpaneler enligt beskrivningen i **Öppna Canvas-instrumentpaneler** ovan.

1. Klicka på den kontrollpanel som du vill redigera i listan med kontrollpaneler.

1. (Valfritt) Dra och släpp **Ändra storlek** -ikonen i det nedre vänstra hörnet av widgeten till önskad storlek.

1. (Valfritt) Om du vill flytta en widget drar du i den intilliggande tomma ytan för widgeten och drar den till önskad relativ position på kontrollpanelen.

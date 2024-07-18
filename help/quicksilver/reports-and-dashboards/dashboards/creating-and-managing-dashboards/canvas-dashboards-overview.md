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

En fullständig lista över funktioner som har lagts till på arbetsytans kontrollpaneler finns i [Arbetsytans kontrollpaneler: versionsaktivitet](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md)

## Åtkomst till Canvas-instrumentpaneler

Ett nytt alternativ för Canvas Dashboards på den vänstra panelen på den befintliga kontrollpanelens startsida kan aktiveras för att få åtkomst till Canvas Dashboards. Det här menyalternativet är som standard inaktiverat och måste vara aktiverat för att du ska få åtkomst. Se instruktionerna nedan för mer information om hur du aktiverar menyalternativet och navigerar till det.

### Lägg till kontrollpaneler för arbetsytan på den vänstra panelen på kontrollpanelerna

>[!IMPORTANT]
>
>Du måste ha minst behörigheten Visa för rapporter och instrumentpaneler för att kunna växla till objektet Kontrollpaneler på arbetsytan i layoutmallen.

1. Börja arbeta med layoutmallen där du vill aktivera Canvas-kontrollpaneler, enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicka på listrutan **Anpassa det som användarna ser** och klicka sedan på **Kontrollpaneler**.

1. Klicka på ikonen ![](assets/delete-secondary-nav-item.png) bredvid **Arbetsytans kontrollpaneler** i listan **Vänster panel** som visas nedan. Ikonen ändras till ![](assets/add-secondary-nav-item.png) för att visa att den nu visas i den vänstra panelen i instrumentpaneler.

1. Klicka på **Spara** längst ned på skärmen.

### Öppna Canvas-instrumentpaneler

1. Kontrollera att du har aktiverat alternativet Kontrollpaneler på arbetsytan i layoutmallen. Mer information finns i **Lägga till kontrollpaneler på kontrollpanelmenyn** ovan.

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon.png) och sedan på **Kontrollpaneler**.

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

## Använda Canvas-paneler

### Skapa en ny arbetsytans kontrollpanel

1. Öppna arbetsytans kontrollpaneler enligt beskrivningen i **Öppna arbetsytans kontrollpaneler** ovan.

1. Klicka på **+ Ny instrumentpanel**

1. Klicka på **Namnlös** i det övre vänstra hörnet för att ange ett namn för instrumentpanelen.

1. Klicka på **Klar** i det övre högra hörnet om du vill spara din nya instrumentpanel, eller börja lägga till widgetar enligt beskrivningen i **Lägg till en rapport på en arbetsytans kontrollpanel** nedan.

### Lägga till en rapport på en arbetsytans kontrollpanel

1. Öppna arbetsytans kontrollpaneler enligt beskrivningen i **Öppna arbetsytans kontrollpaneler** ovan.

1. Klicka på den kontrollpanel där du vill lägga till en rapport från listan med kontrollpaneler.

1. Klicka på **Hantera widgetar** i det övre högra hörnet och klicka sedan på **Lägg till widget**.

1. Håll muspekaren över den typ av rapportwidget som du vill lägga till och klicka sedan på kryssrutan som visas.

1. När du har markerat alla widgetar som du vill lägga till klickar du på **Lägg till** i det övre högra hörnet.

1. De valda widgetarna visas på kontrollpanelen. Klicka på **Konfiguration** i mitten av en widget för att välja vilken rapport som ska visas.

1. Börja skriva in namnet på rapporten som du vill visa i fältet **Sök efter rapport**. När du ser rapporten i listan klickar du på ikonen **Listrapport** eller **Diagramrapport** bredvid namnet för att visa informationen från rapporten i det format du valt.

>[!WARNING]
> Det går för närvarande att lägga till flera widgetar som visar information från samma rapport, men vi rekommenderar att du bara visar varje rapport en gång eftersom det kan påverka kontrollpanelens prestanda.

### Redigera en widget på en arbetsytans kontrollpanel

1. Öppna arbetsytans kontrollpaneler enligt beskrivningen i **Öppna arbetsytans kontrollpaneler** ovan.

1. Klicka på den kontrollpanel som du vill redigera i listan med kontrollpaneler.

1. (Valfritt) Om du vill ändra storlek på en widget drar och släpper du ikonen **Ändra storlek** längst ned till vänster i widgeten till önskad storlek.

1. (Valfritt) Om du vill flytta en widget drar du i den intilliggande tomma ytan för widgeten och drar den till önskad relativ position på kontrollpanelen.

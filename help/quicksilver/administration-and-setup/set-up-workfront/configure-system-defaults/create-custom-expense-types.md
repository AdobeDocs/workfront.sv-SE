---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa anpassade utgiftstyper
description: Som  [!DNL Adobe Workfront] administratör kan du skapa anpassade utgiftstyper för att definiera och spåra utgifter som är kopplade till dina aktiviteter och projekt. Utgifter är icke-arbetskostnader som kan kopplas till uppgifter eller projekt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 7f95df7acfb1afd0974c0138152a68326631d265
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Skapa anpassade utgiftstyper

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Som [!DNL Adobe Workfront]-administratör kan du skapa anpassade utgiftstyper för att definiera och spåra utgifter som är kopplade till dina aktiviteter och projekt. Utgifter är icke-arbetskostnader som kan kopplas till uppgifter eller projekt.

Du kan redigera eller ta bort alla utgiftstyper som du skapar. Du kan inte ta bort eller redigera de inbyggda [!DNL Workfront] utgiftstyperna.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standardutgiftstyper

Standardutgiftstyperna i [!DNL Workfront] som inte kan tas bort eller redigeras är följande:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Entertainment]
* [!UICONTROL General]
* [!UICONTROL Materials]
* [!UICONTROL Travel]

## Skapa anpassade utgiftstyper

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Expense Types]**.
1. Klicka på **[!UICONTROL New expense type]**.
1. Ange följande information i dialogrutan **[!UICONTROL New Expense Type]**:

   * **Namn** - Ett namn för utgiften.
   * **Beskrivning** - En beskrivning av utgiften.
   * **Beräknad enhet** - Välj måttenhet för utgiftstypen i listrutan. Följande måttenheter är tillgängliga:

      * Miljö
      * Kilometer
      * Kilogram
      * Dollar
      * Timme
      * Dag
      * Annat - Om du väljer det här alternativet uppmanas du att ange namnet på din måttenhet och att definiera måttenheten som något som är bekant för din organisation.

   * **Rate** - Priset per enhet. Det här är ett valutaformaterat fält och representerar kostnaden för varje enhet som har upprättats i fältet **Beräknad enhet**. Frekvensen kan innehålla ett numeriskt värde med upp till 4 siffror efter decimaltalet. Exempel: 1.0375.

1. Klicka på **[!UICONTROL Save]**.

   Utgiftstypen är nu tillgänglig så att användare kan associera den med sina utgifter för projekt och uppgifter.

## Ändra anpassade utgiftstyper

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Expense Types]**.
1. Välj den utgiftstyp som du vill ändra och klicka sedan på ikonen **[!UICONTROL Edit]** ![Redigera](assets/edit-icon.png) .

   Dialogrutan **[!UICONTROL Edit Expense Type]** visas.

1. Gör önskade ändringar och klicka sedan på **[!UICONTROL Save]**.

   Utgiftstypen är nu tillgänglig så att användare kan associera den med sina utgifter för projekt och uppgifter.

Mer information om hur du använder utgifter och hur de kan påverka kostnaden för ett projekt finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

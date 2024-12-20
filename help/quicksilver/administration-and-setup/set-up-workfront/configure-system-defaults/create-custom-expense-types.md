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
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '370'
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

Utgiftstyperna som finns i [!DNL Workfront] kan inte tas bort eller redigeras med följande:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Entertainment]
* [!UICONTROL General]
* [!UICONTROL Materials]
* [!UICONTROL Travel]

## Skapa anpassade utgiftstyper

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Expense Types]**.
1. Klicka på **[!UICONTROL New Expense Type]**.
1. Ange följande information i rutan **[!UICONTROL New Expense Type]** som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Ange ett namn för utgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ange en beskrivning för utgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>Välj måttenhet för utgiftstypen i listrutan.</p> <p>Följande måttenhet är tillgänglig:</p> 
       <ul> 
        <li>Miljö</li> 
        <li>Kilometer</li> 
        <li>Kilogram</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Dag</li> 
        <li>Annat - Om du väljer det här alternativet uppmanas du att ange namnet på din måttenhet och att definiera måttenheten som något som är bekant för din organisation.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hastighet</td> 
      <td> <p>Ange priset per enhet. Det här är ett valutaformaterat fält och representerar kostnaden för varje enhet som har upprättats i fältet <strong>[!UICONTROL Calculated Unit]</strong>. </p> <p>Frekvensen kan innehålla ett numeriskt värde med upp till 4 siffror efter decimaltalet. Exempel: 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create Expense Type]**.\
   Utgiftstypen är nu tillgänglig så att användare kan associera den med sina utgifter för projekt och uppgifter.

## Ändra anpassade utgiftstyper

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Expense Types]**.
1. Välj den utgiftstyp som du vill ändra och klicka sedan på **[!UICONTROL Edit]**.

   Dialogrutan **[!UICONTROL Edit Expense Type]** visas.

1. Gör önskade ändringar och klicka sedan på **[!UICONTROL Save Changes]**.\
   Utgiftstypen är nu tillgänglig så att användare kan associera den med sina utgifter för projekt och uppgifter.

Mer information om hur du använder utgifter och hur de kan påverka kostnaden för ett projekt finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa anpassade utgiftstyper
description: Som [!DNL Adobe Workfront] administratör kan du skapa anpassade utgiftstyper för att definiera och spåra de utgifter som är kopplade till dina uppgifter och projekt. Utgifter är icke-arbetskostnader som kan associeras med uppgifter eller projekt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 428e6a9365c793ce5944941ec5368a674c208c78
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 1%

---

# Skapa anpassade utgiftstyper

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Som [!DNL Adobe Workfront] administratör kan du skapa anpassade utgiftstyper för att definiera och spåra de utgifter som är kopplade till dina uppgifter och projekt. Utgifter är icke-arbetskostnader som kan associeras med uppgifter eller projekt.

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
   <td><p>Ny: [!UICONTROL Standard]</p>
   Eller
   <p>Ström: [!UICONTROL Plan]</p>
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
1. **[!UICONTROL New Expense Type]** I dialogrutan anger du följande information:

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
      <td>Ange en beskrivning av utgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>Välj måttenhet för din utgiftstyp i listrutan.</p> <p>Följande måttenhet är tillgänglig:</p> 
       <ul> 
        <li>Miljö</li> 
        <li>Kilometer</li> 
        <li>Kilogram</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Dag</li> 
        <li>Annat – Om du väljer det här alternativet uppmanas du att namnge din måttenhet och definiera måttenheten som något som är bekant för din organisation.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxera</td> 
      <td> <p>Ange priset per enhet. Det här är ett valutaformaterat fält och representerar kostnaden för varje enhet som anges i <strong>[!UICONTROL Calculated Unit]</strong> fältet. </p> <p>Hastigheten kan innehålla ett numeriskt värde med upp till 4 siffror efter decimaltecknet. Exempel: 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Save]**.

   Utgiftstypen är nu tillgänglig så att användare kan associera den med sina utgifter för projekt och uppgifter.

## Ändra anpassade utgiftstyper

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Expense Types]**.
1. Välj den utgiftstyp som du vill ändra och klicka sedan på **[!UICONTROL Edit]**.

   Dialogrutan **[!UICONTROL Edit Expense Type]** visas.

1. Gör önskade ändringar och klicka sedan på **[!UICONTROL Save]**.

   Utgiftstypen är nu tillgänglig för användare att koppla den till sina utgifter för projekt och uppgifter.

Mer information om hur du använder utgifter och hur de kan påverka kostnaden för ett projekt finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

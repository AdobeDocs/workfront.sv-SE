---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Anpassa standardproblemtyper
description: Du kan anpassa etiketterna för varje standardutgåva för att bättre matcha den terminologi som används i organisationen. Problemtyper är användbara när du vill anpassa utgivningsstatus och skapa begärandeköer.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Anpassa standardproblemtyper

Problemtyper är användbara i följande fall:

* När du anpassar utgivningsstatus, enligt beskrivningen i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* När du skapar en begärandekö, vilket beskrivs i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Du kan anpassa etiketterna för varje standardutgåva för att bättre matcha den terminologi som används i organisationen.

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

## Standardutgivningstyper

Om du har [!DNL Adobe Workfront] [!UICONTROL administrator]-åtkomst finns det fyra standardtyper av problem som du kan konfigurera och byta namn på:

* **[!UICONTROL Bug Report]** Används för att spåra rapporterade fel i systemet.
* **[!UICONTROL Change Order]** Används för att spåra problem som behöver uppdateras eller revideras.
* **[!UICONTROL Issue]** Ett objekt i [!DNL Workfront] som kommunicerar oplanerat arbete, ett problem som uppstår eller något som måste lösas för att en uppgift ska kunna fortsätta.
* **[!UICONTROL Request]** En problemtyp som gäller för en frågekö där användare gör förfrågningar i Workfront.

![](assets/default-issue-types.png)

## Anpassa en problemtyp

Tänk på följande när du anpassar problemtyper:

* Du kan ändra etiketten för en problemtyp, men du kan inte ändra dess funktion.
* Du kan inte skapa ytterligare problemtyper.
* Du kan inte ändra filtervärdena för namnet på en utgåva. Om du skapar ett filter i en problemrapport, återspeglar värdet på filtret (nyckeln) inte problemtypens egna namn.
* Tre standardstatusvärden är associerade med varje utgåva: [!UICONTROL New], [!UICONTROL In Progress] och [!UICONTROL Closed]. Du kan inte ta bort dessa statusar eller ta bort dem från en problemtyp, men du kan byta namn på dem.
* Du kan ändra ordningen på alternativen som visas på den nedrullningsbara menyn för varje problemtyp.

Så här anpassar du en problemtyp:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]**.

1. Klicka på fliken **[!UICONTROL Issues]**.
1. Gör något av följande:

   * Håll muspekaren över den problemtyp som du vill anpassa, klicka på [!UICONTROL Edit]-ikonen ![](assets/edit-icon.png) som visas längst till höger och skriv ett nytt namn för problemtypen.

     ![](assets/customize-issue-type.png)

   * Klicka på en [!UICONTROL issue type] om du vill visa de associerade statusarna, dra sedan handtagen som visas när du hovrar över dem och släpp dem i den ordning som du vill att de ska visas i den nedrullningsbara menyn **[!UICONTROL Status]** för dina användares problem.

---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definiera frågetyper för ett projekt
description: Du kan ordna den typ av problem eller förfrågningar som är loggade i Adobe Workfront med hjälp av frågetyper.
author: Becky
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Definiera frågetyper för ett projekt

<!-- Audited: 6/2025 -->

Du kan ordna den typ av problem eller förfrågningar som är loggade i Adobe Workfront med hjälp av frågetyper. Detta är användbart för att rapportera orsaker och hjälpa användarna att förstå vilken typ av oväntat arbete som kan inträffa under ett projekts livstid.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar måste du göra följande:

* Ha eller skapa ett projekt.

  Mer information om hur du skapar projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

## Överväganden om frågetyper

* Du kan ange vilken typ av ärenden eller förfrågningar som kan loggas i ett projekt när du konfigurerar området Köinformation för projektet.
* Du behöver inte aktivera projektet som en frågekö för att kunna definiera frågetyper för ett projekt. Alla problem som loggas för ett projekt kan märkas med en annan frågetyp.
* Om du lägger till köämnen i ditt projekt måste du definiera frågetyper för varje köämne för att kunna visa dem när du lägger till ett nytt problem eller en ny begäran. Mer information finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definiera utgåva eller förfrågningstyper för ett projekt

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på **Köinformation** i den vänstra panelen.
1. I avsnittet **Köegenskaper** väljer du de **typer av begäranden** som du vill använda för projektet:
   * Felrapport
   * Ändra ordning
   * Problem
   * Begäran

   >[!NOTE]
   >
   >* Du måste välja minst en begärandetyp. Du kan välja flera typer.
   >* Din Workfront-administratör kan ha bytt namn på några av dessa alternativ. Mer information finns i [Konfigurera typer av förfrågningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Klicka på **Spara**. De begärda typerna som du har angett kan väljas när du anger en ny utgåva för en uppgift eller ett projekt, eller när du skickar en ny begäran till projektet (om projektet är aktiverat som en frågekö).

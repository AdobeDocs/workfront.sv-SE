---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definiera frågetyper för ett projekt
description: Du kan ordna den typ av problem eller förfrågningar som är loggade i Adobe Workfront med hjälp av frågetyper.
author: Lisa
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Definiera frågetyper för ett projekt

Du kan ordna den typ av problem eller förfrågningar som är loggade i Adobe Workfront med hjälp av frågetyper.

Den här organisationen är användbar för att rapportera orsaker och för att hjälpa användare förstå vilken typ av oväntat arbete som kan inträffa under ett projekts livstid.

## Åtkomstkrav

+++

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
    <p>Nytt: Standard</p>
    <p>eller</p>
    <p>Aktuell: Planera</p></td>  
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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar måste du göra följande:

* Ha eller skapa ett projekt

  Mer information om hur du skapar projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

## Överväganden om frågetyper

* Du kan ange vilken typ av ärenden eller förfrågningar som kan loggas i ett projekt när du konfigurerar området **Köinformation** för projektet.
* Du behöver inte aktivera projektet som en frågekö för att kunna definiera frågetyper för ett projekt. Alla problem som loggas för ett projekt kan märkas med en annan frågetyp.
* Om du lägger till köämnen i ditt projekt måste du definiera frågetyper för varje köämne för att kunna visa dem när du lägger till ett nytt problem eller en ny begäran. Mer information finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definiera utgåva eller förfrågningstyper för ett projekt

{{step1-to-projects}}

1. Klicka på namnet på projektet för att öppna det.
1. Klicka på **Köinformation** i den vänstra panelen.
1. I avsnittet **Köegenskaper** väljer du de **typer av begäranden** som du vill använda för projektet.

   >[!NOTE]
   >
   >Du måste välja minst en begärandetyp. Du kan välja flera typer av förfrågningar.

   Välj bland följande typer:

   * Felrapport
   * Ändra ordning
   * Problem
   * Begäran

   >[!TIP]
   >
   >Din Workfront-administratör kan ha bytt namn på några av dessa alternativ. Mer information finns i [Konfigurera typer av förfrågningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Klicka på **Spara**.

   De begärandetyper du har angett kan väljas när du anger en ny utgåva för en uppgift eller ett projekt, eller när du skickar en ny begäran till projektet, om projektet är aktiverat som en begärandekö.

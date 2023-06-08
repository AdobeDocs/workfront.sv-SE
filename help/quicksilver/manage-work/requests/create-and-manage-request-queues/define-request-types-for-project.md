---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definiera frågetyper för ett projekt
description: Du kan ordna den typ av problem eller förfrågningar som är loggade i Adobe Workfront med hjälp av frågetyper.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Definiera frågetyper för ett projekt

Du kan ordna den typ av problem eller förfrågningar som är loggade i Adobe Workfront med hjälp av frågetyper.

Den här organisationen är användbar för att rapportera orsaker och för att hjälpa användare förstå vilken typ av oväntat arbete som kan inträffa under ett projekts livstid.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront</a>*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Översikt över licenser</a>*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du göra följande:

* Ha eller skapa ett projekt

  Mer information om hur du skapar projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

## Överväganden om frågetyper

* Du kan ange vilken typ av problem eller förfrågningar som kan loggas i ett projekt när du konfigurerar **Köinformation** området för projektet.
* Du behöver inte aktivera projektet som en frågekö för att kunna definiera frågetyper för ett projekt. Alla problem som loggas för ett projekt kan märkas med en annan frågetyp.
* Om du lägger till köämnen i ditt projekt måste du definiera frågetyper för varje köämne för att kunna visa dem när du lägger till ett nytt problem eller en ny begäran. Mer information finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definiera utgåva eller förfrågningstyper för ett projekt

1. Klicka **Projekt** på huvudmenyn. ![](assets/main-menu-icon.png)

1. Klicka på namnet på projektet för att öppna det.
1. Klicka på i den vänstra panelen **Köinformation**.
1. I **Köegenskaper** väljer du **Typ av begäran** du vill ha för projektet.

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
   >Din Workfront-administratör kan ha bytt namn på några av dessa alternativ. Mer information finns i [Konfigurera begärandetyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Klicka **Spara**.

   De begärandetyper du har angett kan väljas när du anger en ny utgåva för en uppgift eller ett projekt, eller när du skickar en ny begäran till projektet, om projektet är aktiverat som en begärandekö.

---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Skicka ett dokument med den utökade kopplingen
description: Du kan skicka dokument från Workfront till Experience Manager Assets. Dokument som överförs och skickas från Workfront till Experience Manager Assets räknas fortfarande av mot den totala dokumentlagringen. Assets som är länkat från Experience Manager Assets räknas inte in i den totala lagringen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Skicka ett dokument med den utökade kopplingen

Du kan skicka dokument från Workfront till Experience Manager Assets. Dokument som överförs och skickas från Workfront till Experience Manager Assets räknas fortfarande av mot den totala dokumentlagringen. Assets som är länkat från Experience Manager Assets räknas inte in i den totala lagringen.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller senare för dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du

* Installera den utökade Workfront för Experience Manager-anslutningen.

## Skicka ett dokument till Experience Manager Assets

När en användare skickar ett dokument från Workfront till Experience Manager Assets överförs mappade metadata längs dokumentet. Om den är konfigurerad synkroniseras metadata kontinuerligt varje gång en ändring görs.

Skicka ett dokument:

1. Gå till området **Dokument** i Workfront och markera det dokument som du vill skicka.
1. Klicka på **Skicka till** och välj sedan den Experience Manager Assets-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Valfritt namn kan väljas för denna integration, så det får inte uttryckligen nämnas Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Välj vart du vill att resursen ska gå och klicka sedan på **Välj mapp**.
1. Klicka på **Spara** när du har hittat önskat mål.

## Skicka en ny version till Experience Manager Assets

Du kan lägga till en ny version i ett dokument som du tidigare har överfört till Workfront. Mer information finns i [Överföra en ny version av ett dokument](../../../documents/managing-documents/upload-new-document-version.md). När den senaste versionen har överförts kan du skicka den till Experience Manager Assets. Om ett mappat fält i Workfront har ändrats uppdateras metadata i Experience Manager Assets när den skickas.

Så här skickar du den senaste versionen:

1. Gå till området **Dokument** i Workfront och leta upp dokumentet.
1. Klicka på **Skicka till** och välj sedan den Experience Manager Assets-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Valfritt namn kan väljas för denna integration, så det får inte uttryckligen nämnas Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicka på **Spara**. Den nya versionen sparas på samma plats som den tidigare versionen.

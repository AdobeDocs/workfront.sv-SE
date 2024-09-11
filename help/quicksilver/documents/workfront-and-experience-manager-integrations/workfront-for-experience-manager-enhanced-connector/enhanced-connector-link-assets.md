---
title: Länka resurser och mappar med den förbättrade kopplingen
description: Du kan länka en resurs eller mapp från Experience Manager Assets till ett Workfront-objekt som stöder dokument.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: dd8718b00a310bee6caa13db7644b86174b476f4
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---


# Länka resurser och mappar med den förbättrade kopplingen

Du kan länka en resurs eller mapp från Experience Manager Assets till ett Workfront-objekt som stöder dokument. Assets som skickas från Experience Manager Assets räknar inte med att bli din totala dokumentlagring i Workfront. Dokument som överförs och skickas från Workfront till Experience Manager Assets räknas med i det övergripande lagringsutrymmet.


>[!NOTE]
>
>Excel-filer som är länkade via den utökade kopplingen kan inte förhandsgranskas i Workfront. Du måste hämta filen för att kunna komma åt den.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell: Begäran eller senare</p> 
   eller
   <p>Nytt: Medarbetare eller högre</p> </td> 
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
   <td> <p>Visa åtkomst eller senare i ett dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.
+++

## Förutsättningar

Innan du börjar måste du

* Installera den utökade Workfront för Experience Manager-anslutningen

## Länka en resurs från Experience Manager Assets

Du kan länka en resurs från Experience Manager Assets till Workfront. När resursen är länkad kan du

* [Korrektur för länkad resurs för Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Överföra en ny version av ett dokument](../../../documents/managing-documents/upload-new-document-version.md)

Så här länkar du en resurs till Experience Manager Assets:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Klicka på **Lägg till ny** och välj sedan den Experience Manager Assets-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Valfritt namn kan väljas för denna integration, så det får inte uttryckligen nämnas Experience Manager Assets.

1. Välj de resurser du vill ha.

   ![](assets/select-an-asset.png)

1. Klicka på **Länk**.

## Länka en mapp från Experience Manager Assets

Behörigheter att visa enskilda resurser i en mapp kräver Experience Manager Assets-behörigheter.

Länka en mapp till Experience Manager Assets:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Klicka på **Lägg till ny** och välj sedan den Experience Manager Assets-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Valfritt namn kan väljas för denna integration, så det får inte uttryckligen nämnas Experience Manager Assets.

1. Markera de mappar du vill använda.

   ![](assets/select-a-folder.png)

1. Klicka på **Länk**.

## Länka en ny version från Experience Manager Assets

Du kan hämta en ny resurs från Experience Manager Assets och lägga till den i en befintlig resurs som en ny version i Workfront. Om dokumentet redan är länkat och en ny version har lagts till i Experience Manager Assets, visas den nya versionen automatiskt i Workfront.

>[!TIP]
>
>Du kan visa alla versioner av en resurs om du går till **Dokumentinformation** > **Versioner**.

Så här länkar du en ny version från Experience Manager Assets:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Markera den resurs som du vill ersätta med en ny version. Du kan inte skapa en ny version av en resurs i en länkad mapp.
1. Klicka på **Lägg till ny** och välj sedan den Experience Manager Assets-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Valfritt namn kan väljas för denna integration, så det får inte uttryckligen nämnas Experience Manager Assets.

1. Välj den resurs du vill använda.

   ![](assets/select-an-asset.png)

1. Klicka på **Länk**.

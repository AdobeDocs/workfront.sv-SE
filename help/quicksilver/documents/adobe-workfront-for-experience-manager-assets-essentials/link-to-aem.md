---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Länka resurser och mappar från Experience Manager Assets eller Assets Essentials
description: Du kan länka en resurs eller mapp från Experience Manager Assets eller Assets Essentials till ett Adobe Workfront-objekt som stöder dokument. Assets som skickas från Assets Essentials räknas inte in i ditt totala dokumentlagringsutrymme i Workfront. Dokument som överförs och skickas från Workfront till Assets Essentials räknas in i det totala lagringsutrymmet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Länka resurser och mappar från Experience Manager Assets eller Assets Essentials

Du kan länka en resurs eller mapp från Experience Manager Assets eller Assets Essentials till ett Adobe Workfront-objekt som stöder dokument. Assets som skickas från Assets Essentials räknas inte in i ditt totala dokumentlagringsutrymme i Workfront. Dokument som överförs och skickas från Workfront till Assets Essentials räknas in i det totala lagringsutrymmet.

Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Om Workfront-administratören har aktiverat synkronisering av objektmetadata, förblir fälten aktuella om de ändras i något av programmen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha Experience Manager as a Cloud Service eller Assets Essentials, och du måste läggas till i produkten som användare i Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-behörigheter</td> 
    <td>Du måste ha skrivåtkomst till mappen.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller högre</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en Experience Manager-integrering. Mer information finns i [Konfigurera integreringen med Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen med Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Länka en resurs från Experience Manager Assets eller Assets Essentials

Du kan länka en resurs från Experience Manager Assets eller Assets Essentials till Workfront. När resursen är länkad kan du

* [Korrektur för en länkad resurs för Experience Manager Assets eller Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md)

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Välj **Lägg till ny** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för den här integreringen, så den får inte särskilt nämna Assets eller Assets Essentials.

1. Välj de resurser du vill ha.

   ![Välj en resurs](assets/select-an-asset.png)

1. Klicka på **Markera**.

## Länka en mapp från Experience Manager Assets eller Assets Essentials

Behörigheter att visa enskilda resurser i en mapp kräver Experience Manager Assets- eller Assets Essentials-behörigheter.

1. Gå till området **Dokument** i Workfront där du vill ha mappen.
1. Välj **Lägg till ny** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Assets eller Assets Essentials.

1. Markera de mappar du vill använda.

   ![Välj en mapp](assets/select-a-folder.png)

1. Klicka på **Markera**.

## Länka en ny version från Experience Manager Assets eller Assets Essentials

Du kan hämta en ny resurs från Resurser Essentials och lägga till den i en befintlig resurs som en ny version. Om dokumentet redan är länkat och en ny version läggs till i Resurser Essentials, visas den nya versionen automatiskt i Workfront.

Så här länkar du en ny version från Assets Essentials:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Markera den resurs som du vill ersätta med en ny version. Du kan inte skapa en ny version av en resurs i en länkad mapp.
1. Välj **Lägg till ny** > **Version** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Assets eller Assets Essentials.

1. Välj den resurs du vill använda.

   ![Välj en resurs](assets/select-an-asset.png)

1. Klicka på **Markera**.

>[!TIP]
>
>Du kan visa alla versioner av en resurs om du går till **Dokumentinformation** > **Versioner**.

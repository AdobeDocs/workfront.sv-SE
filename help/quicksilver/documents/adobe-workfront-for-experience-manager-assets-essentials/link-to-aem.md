---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Länka resurser och mappar från Experience Manager Assets eller Assets Essentials
description: Du kan länka en resurs eller mapp från Experience Manager Assets eller Assets Essentials till ett Adobe Workfront-objekt som stöder dokument. Assets som skickas från Assets Essentials räknas inte in i ditt totala dokumentlagringsutrymme i Workfront. Dokument som överförs och skickas från Workfront till Assets Essentials räknas in i det totala lagringsutrymmet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Länka resurser och mappar från Experience Manager Assets eller Assets Essentials

Du kan länka en resurs eller mapp från Experience Manager Assets eller Assets Essentials till ett Adobe Workfront-objekt som stöder dokument. Assets som skickas från Assets Essentials räknas inte in i ditt totala dokumentlagringsutrymme i Workfront. Dokument som överförs och skickas från Workfront till Assets Essentials räknas in i det totala lagringsutrymmet.

Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Om Workfront-administratören har aktiverat synkronisering av objektmetadata, förblir fälten aktuella om de ändras i något av programmen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare produkter</td> 
   <td>Du måste ha Experience Manager as a Cloud Service eller Assets Essentials, och du måste läggas till i produkten som användare i Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-behörigheter</td> 
    <td>Du måste ha skrivåtkomst till mappen.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

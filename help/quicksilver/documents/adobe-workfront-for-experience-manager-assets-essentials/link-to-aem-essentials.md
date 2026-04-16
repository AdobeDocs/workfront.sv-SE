---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Länka resurser och mappar från Experience Manager Assets Essentials
description: Du kan länka en resurs eller mapp från Experience Manager Assets Essentials till ett Adobe Workfront-objekt som stöder dokument. Assets som skickas från Assets Essentials räknas inte in i ditt totala dokumentlagringsutrymme i Workfront. Dokument som överförs och skickas från Workfront till Assets Essentials räknas in i det totala lagringsutrymmet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a9dfc5c7838668bd3007c157a4e1a53ab4bd86f5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Länka resurser och mappar från Experience Manager Assets Essentials

Du kan länka en resurs eller mapp från Experience Manager Assets Essentials till ett Adobe Workfront-objekt som stöder dokument.

Mer information om hur du länkar resurser och mappar från Experience Manager Assets med hjälp av Content Advisor finns i [Länka resurser och mappar med Content Advisor från Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).


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

Innan du börjar:

* Din Workfront-administratör måste konfigurera en Experience Manager-integrering. Mer information finns i [Konfigurera integreringen av Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Länka en resurs från Experience Manager Assets Essentials

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Välj **Lägg till ny** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets Essentials.

1. Välj de resurser du vill ha.

   ![Välj en resurs](assets/select-an-asset.png)

1. Klicka på **Markera**.

## Länka en ny version från Experience Manager Assets Essentials

Du kan hämta en ny resurs från Experience Manager Assets Essentials och lägga till den i en befintlig resurs som en ny version. Om dokumentet redan är länkat och en ny version har lagts till i Experience Manager Assets Essentials, visas den nya versionen automatiskt i Workfront.

Länka en ny version:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Markera den resurs som du vill ersätta med en ny version. Du kan inte skapa en ny version av en resurs i en länkad mapp.
1. Välj **Lägg till ny** > **Version** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets Essentials.

1. Markera den resurs som du vill länka.

1. Klicka på **Markera**.

## Länka en mapp från Experience Manager Assets Essentials

Behörigheter att visa enskilda resurser i en mapp kräver behörigheter i Experience Manager Assets Essentials.

1. Gå till området **Dokument** i Workfront där du vill ha mappen.
1. Välj **Lägg till ny** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets Essentials.

1. Markera de mappar du vill använda.

   ![Välj en mapp](assets/select-a-folder.png)

1. Klicka på **Markera**.

## Överväganden

* Funktionen Content Advisor är inte tillgänglig för Assets Essentials. Mer information om hur du länkar resurser och mappar med hjälp av Content Advisor finns i [Länka resurser och mappar med Content Advisor från Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Assets som skickas från Assets Essentials räknas inte in i ditt totala dokumentlagringsutrymme i Workfront. Dokument som överförs och skickas från Workfront till Assets Essentials räknas in i det totala lagringsutrymmet.

* Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets Essentials. Om Workfront-administratören har aktiverat synkronisering av objektmetadata, förblir fälten aktuella om de ändras i något av programmen.

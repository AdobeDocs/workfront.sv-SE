---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Skapa en mapp som är länkad till Experience Manager Assets eller Assets Essentials
description: Du kan skapa en mapp som är länkad till Experience Manager Assets eller Assets Essentials i Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Skapa en mapp som är länkad till Experience Manager Assets eller Assets Essentials

Du kan skapa en mapp som är länkad till Experience Manager Assets eller Assets Essentials i Workfront. Eftersom mappen är länkad visas alla resurser som läggs till i mappen automatiskt i både Workfront och Experience Manager. Du behöver inte skicka resursen manuellt om den finns i en länkad mapp.

Om en resurs tas bort eller flyttas från en länkad mapp i Experience Manager Assets eller Resurser Essentials, sparar Workfront en kopia av resursen i området Projekt > Dokument.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table>
  <tr>
   <td><strong>Adobe Workfront-paket</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenser</strong>
   </td>
   <td>
   <p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td><strong>Ytterligare produkter</strong>
   </td>
   <td>Du måste ha Experience Manager Assets as a Cloud Service eller Assets Essentials, och du måste läggas till i produkten som användare.
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager-behörigheter</strong>
   </td>
   <td>Du måste ha skrivåtkomst till målmappen i Experience Manager-integreringen.
   </td>
  </tr>
  <tr>
   <td><strong>Åtkomstnivåkonfigurationer</strong>
   </td>
   <td>Du måste vara Workfront-administratör för att kunna konfigurera en Experience Manager-integrering. När den har konfigurerats kan användare med en planlicens ställa in länkade mappar i enskilda projekt.
   </td>
  </tr>
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en Experience Manager-integrering. Mer information finns i [Konfigurera integreringen med Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen med Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Skapa en länkad mapp

Den länkade mappen skapas på den plats som anges av Workfront-administratören när integreringen konfigureras. Varje integrering kan bara ha en mapplats för länkade mappar.

Namnet på den länkade mappen skapas automatiskt baserat på associerat Portfolio, Program, Project och kan inte ändras. Om projektet inte är associerat med en Portfolio eller ett program visas projektnamnet och skapandedatumet i den länkade mappen.

>[!NOTE]
>
>Du kan inte skapa ett nytt dokument eller en korrekturversion inuti en länkad mapp.


Så här skapar du en länkad mapp:

1. Gå till det projekt där du vill ha mappen.
1. Välj **Lägg till ny** och gå sedan till den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets eller Assets Essentials.

1. Välj **Skapa länkad mapp**. En mapp skapas automatiskt i Experience Manager baserat på den plats som angavs när integreringen konfigurerades.
   ![skapa en länkad mapp](assets/linked-folder.png)

---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Skapa en mapp länkad till Experience Manager Assets eller Assets Essentials
description: Du kan skapa en mapp som är länkad till Experience Manager Assets eller Assets Essentials i Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 1744e6f2b78c64ba2fa4856d9c6a0611404e4458
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Skapa en mapp länkad till Experience Manager Assets eller Assets Essentials

Du kan skapa en mapp som är länkad till Experience Manager Assets eller Assets Essentials i Workfront. Eftersom mappen är länkad visas alla resurser som läggs till i mappen automatiskt i både Workfront och Experience Manager. Du behöver inte skicka resursen manuellt om den finns i en länkad mapp.


## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>Adobe Workfront-plan*</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenser*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td>Du måste ha Experience Manager Assets as a Cloud Service eller Assets Essentials och du måste läggas till som användare i produkten.
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager behörigheter</strong>
   </td>
   <td>Du måste ha skrivåtkomst till målmappen i Experience Manager-integreringen.
   </td>
  </tr>
  <tr>
   <td><strong>Åtkomstnivåkonfigurationer</strong>
   </td>
   <td>Du måste vara Workfront-administratör för att kunna konfigurera en integrering med Experience Manager. När den har konfigurerats kan användare med en planlicens ställa in länkade mappar i enskilda projekt.
   </td>
  </tr>
</table>


*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.


## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en integrering med Experience Manager. Mer information finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera Experience Manager Assets Essentials-integrering](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Skapa en länkad mapp

Den länkade mappen skapas på den plats som anges av Workfront-administratören när integreringen konfigureras. Varje integrering kan bara ha en mapplats för länkade mappar.

Namnet på den länkade mappen skapas automatiskt baserat på Portfolio, Program, Projekt som är associerat med mappen och kan inte ändras. Om projektet inte är kopplat till ett Portfolio eller program visas projektnamnet och skapandedatumet i den länkade mappen.

Så här skapar du en länkad mapp:



1. Gå till det projekt där du vill ha mappen.
1. Välj **Lägg till ny** och gå sedan till den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets eller Assets Essentials.

1. Välj **Skapa länkad mapp**. En mapp skapas automatiskt i Experience Manager baserat på den plats som angavs när integreringen konfigurerades.
   ![skapa en länkad mapp](assets/linked-folder.png)

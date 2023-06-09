---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Skicka ett dokument till Experience Manager Assets eller Assets Essentials
description: Du kan skicka dokument från Workfront till Experience Manager Assets eller Assets Essentials. Dokument som överförs och skickas från Workfront till Assets Essentials räknas fortfarande av mot den totala dokumentlagringen. Resurser som är länkade från Assets Essentials räknas inte in i det totala lagringsutrymmet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 91da06fe23b464e0422d50b0db69f4eae3db642f
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Skicka ett dokument till Experience Manager Assets eller Assets Essentials


Du kan skicka dokument från Workfront till Experience Manager Assets eller Assets Essentials. Dokument som överförs och skickas från Workfront till Assets Essentials räknas fortfarande av mot den totala dokumentlagringen. Resurser som är länkade från Assets Essentials räknas inte in i det totala lagringsutrymmet.

Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Alla metadata som har konfigurerats för att mappa för överordnade objekt skickas också. Mer information om hur du konfigurerar metadatamappning finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen av Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exempel** När du först skickar en resurs som är kopplad till en uppgift mappas metadata för uppgiften till Experience Manager Assets eller Assets Essentials samt alla mappade metadata från överordnade objekt som ett projekt, en portfölj och ett program.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront</a>*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över äldre licenser</a>*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha Experience Manager as a Cloud Service eller Assets Essentials, och du måste läggas till som användare i Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller senare för dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en integrering med Experience Manager. Mer information finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen av Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Skicka ett dokument från Workfront

När en användare skickar ett dokument från Workfront till Experience Manager Assets eller Assets Essentials överförs mappade metadata längs dokumentet. När dokumentet har skickats återspeglas inte ändringar i dokumentets metadata i Workfront i Resurser eller Assets Essentials. Om ett mappat fält i Workfront ändras måste du skicka en ny version av dokumentet med de uppdaterade metadata till Assets eller Assets Essentials. Information om hur du ställer in eller redigerar metadata finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen av Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Så här skickar du ett dokument:

1. Gå till **Dokument** i Workfront och markera dokumentet som du vill skicka.
1. Klicka **Skicka till** väljer du sedan den integrering av Experience Manager som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för den här integreringen, så den får inte särskilt nämna Assets eller Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Välj vart du vill att resursen ska gå och klicka sedan på **Välj mapp**.
1. Klicka på **Spara**.

## Skicka en ny version

Du kan lägga till en ny version i ett dokument som du tidigare har överfört till Workfront. Mer information finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md). När den senaste versionen har överförts kan du skicka den till Assets Essentials. Om ett mappat fält i Workfront har ändrats uppdateras metadata i Assets Essentials när den skickas.

>[!IMPORTANT]
>
>Innan du överför en ny version till Workfront rekommenderar vi att du byter namn på filen. Om du överför en ny version med exakt samma filnamn som en tidigare version kan du bara hämta den senaste versionen från Workfront. Alla versioner kan laddas ned från Experience Manager Assets eller Assets Essentials oavsett filnamn.

Så här skickar du den senaste versionen:

1. Gå till **Dokument** i Workfront och leta upp dokumentet.
1. Välj **Skicka till** väljer du sedan den integrering av Experience Manager som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Assets eller Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicka **Spara**. Den nya versionen sparas på samma plats som den tidigare versionen.

## Flytta ett dokument till en länkad mapp i Experience Manager Assets

>[!NOTE]
>
>Den här funktionen är bara tillgänglig för Experience Manager Assets as a Cloud Service. Det finns inte för Experience Manager Assets Essentials.

Du kan flytta ett dokument till en länkad mapp i Experience Manager Assets om både dokumentet och den länkade mappen finns i samma dokumentlista (till exempel dokumentområdet i ett projekt).

1. Leta reda på dokumentet som du vill flytta.
1. Dra och släpp dokumentet till den länkade Experience Manager Assets-mappen som du vill flytta det till.

Dokumentalternativen är inte tillgängliga när dokumentet håller på att flyttas. När dokumentet har flyttats till Experience Manager Assets visas det inte längre i dokumentlistan i Workfront.

>[!NOTE]
>
> De åtgärder eller redigeringar du gör i dokumentet när det flyttas visas inte i dokumentet i Experience Manager Assets och kommer därför att gå förlorade.


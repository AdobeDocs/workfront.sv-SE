---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Skicka ett dokument till Experience Manager Assets eller Assets Essentials
description: Du kan skicka dokument från Workfront till Experience Manager Assets eller Assets Essentials. Dokument som överförts och skickats från Workfront till Assets Essentials räknas fortfarande av mot den totala dokumentlagringen. Assets som är länkat från Assets Essentials räknas inte in i det totala lagringsutrymmet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Skicka ett dokument till Experience Manager Assets eller Assets Essentials

Du kan skicka dokument från Workfront till Experience Manager Assets eller Assets Essentials. Dokument som överförts och skickats från Workfront till Assets Essentials räknas fortfarande av mot den totala dokumentlagringen. Assets som är länkat från Assets Essentials räknas inte in i det totala lagringsutrymmet.

Assets som skickas till Experience Manager via den här integreringen har en storleksgräns på **5 GB**.

I förhandsvisningsmiljön har Assets som skickas till Experience Manager via den här integreringen en storleksgräns på **30 GB**.

Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Alla metadata som har konfigurerats för att mappa för överordnade objekt skickas också. Mer information om hur du konfigurerar metadatamappning finns i [Konfigurera Experience Manager Assets as a Cloud Service-integreringen](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera Experience Manager Assets Essentials-integreringen](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exempel** När du först skickar en resurs som är kopplad till en aktivitet mappas metadata för aktiviteten till Experience Manager Assets eller Assets Essentials samt alla mappade metadata från överordnade objekt som ett projekt, en portfölj och ett program.

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


## Skicka ett dokument från Workfront

När en användare skickar ett dokument från Workfront till Experience Manager Assets eller Assets Essentials överförs mappade metadata längs dokumentet. När dokumentet har skickats återspeglas inte ändringar som görs i dokumentets metadata i Workfront i Assets eller Resurser Essentials. Om ett mappat fält i Workfront ändras måste du skicka en ny version av dokumentet med de uppdaterade metadata till Assets eller Assets Essentials. Information om hur du konfigurerar eller redigerar metadata finns i [Konfigurera Experience Manager Assets as a Cloud Service-integreringen](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera Experience Manager Assets Essentials-integreringen](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Skicka ett dokument:

1. Gå till området **Dokument** i Workfront och markera det dokument som du vill skicka.
1. Klicka på **Skicka till** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för den här integreringen, så den får inte särskilt nämna Assets eller Assets Essentials.

   ![Skicka till](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Välj vart du vill att resursen ska gå och klicka sedan på **Välj mapp**.
1. Klicka på **Spara** när du har hittat önskat mål.

## Skicka en ny version

Du kan lägga till en ny version i ett dokument som du tidigare har överfört till Workfront. Mer information finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md). När den senaste versionen har överförts kan du skicka den till Assets Essentials. Om ett mappat fält i Workfront har ändrats uppdateras metadata i Assets Essentials när den skickas.

>[!IMPORTANT]
>
>Innan du överför en ny version till Workfront rekommenderar vi att du byter namn på filen. Om du överför en ny version med exakt samma filnamn som en tidigare version kan du bara hämta den senaste versionen från Workfront. Alla versioner kan laddas ned från Experience Manager Assets eller Assets Essentials oavsett filnamn.

Så här skickar du den senaste versionen:

1. Gå till området **Dokument** i Workfront och leta upp dokumentet.
1. Välj **Skicka till** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Assets eller Assets Essentials.

   ![Skicka till](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicka på **Spara**. Den nya versionen sparas på samma plats som den tidigare versionen.

## Flytta ett dokument till en länkad mapp i Experience Manager Assets

>[!NOTE]
>
>Den här funktionen är endast tillgänglig för Experience Manager Assets as a Cloud Service. Det finns inte för Experience Manager Assets Essentials.

Du kan flytta ett dokument till en länkad mapp i Experience Manager Assets om både dokumentet och den länkade mappen finns i samma dokumentlista (till exempel dokumentområdet i ett projekt).

1. Leta reda på dokumentet som du vill flytta.
1. Dra och släpp dokumentet till den länkade Experience Manager Assets-mappen som du vill flytta det till.

Dokumentalternativen är inte tillgängliga när dokumentet håller på att flyttas. När dokumentet har flyttats till Experience Manager Assets visas det inte längre i dokumentlistan i Workfront.

>[!NOTE]
>
> De åtgärder eller redigeringar du gör i dokumentet när det flyttas visas inte i dokumentet i Experience Manager Assets och kommer därför att gå förlorade.


---
title: 23.3 Integration enhancements
description: 23.3 Integration enhancements
author: Lisa
feature: Product Announcements
source-git-commit: 3ebf408bb03a97de78600ab771834a7d7f29e2e0
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 23.3 Integration enhancements

Den här sidan beskriver alla integreringsförbättringar som gjorts i version 23.3 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön med version 23.3.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i 23.3-versionscykeln finns på [23.3 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Adobe Creative Cloud-integreringar har nu stöd för flera tilldelade användare

Integreringen med Adobe Creative Cloud ger nu möjlighet att välja mellan&quot;Klar med min del&quot; och&quot;Klar&quot; (eller&quot;Löst&quot;) när en uppgift eller ett problem har flera tilldelade användare.

Tidigare kunde användaren markera en uppgift som klar utan att ange &quot;Klar med min del&quot; eller &quot;Fullständig&quot;/&quot;Löst&quot;.

Om du vill använda den här funktionen hämtar och installerar du de senaste plugin-programmen för Workfront för Creative Cloud.

Mer information om funktionerna finns i [Markera arbetsobjekt som slutförda med Adobe Workfront-plugin](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Information om hur du installerar Workfront for Creative Cloud-plugin-program finns i [Installera Adobe Workfront-plugin-programmet för Creative Cloud-program](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Visa och hantera Workfront-meddelanden från Workfront för plugin-program för Creative Cloud

För att förenkla för dig att få de meddelanden du behöver har vi gjort det möjligt att visa och hantera Workfront-meddelanden utan att behöva lämna Adobe Creative Cloud. Nu kan du visa meddelanden och komma åt arbetsobjekt och kommentarer som hör till dessa meddelanden direkt från Workfront plugin-fönster i programmet Creative Cloud.

Tidigare var meddelanden bara tillgängliga i Workfront och via e-post.

Om du vill använda den här funktionen hämtar och installerar du de senaste plugin-programmen för Workfront för Creative Cloud.

Mer information finns i [Visa och hantera [!DNL Adobe Workfront] aviseringar från Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Information om hur du installerar Workfront for Creative Cloud-plugin-program finns i [Installera Adobe Workfront-plugin-programmet för Creative Cloud-program](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Förbättrad upplevelse när du flyttar ett dokument till en länkad mapp med dra och släpp

Vi har lagt till viss genomskinlighet i processen att dra och släppa ett dokument i en länkad mapp. Dokumentet som du har flyttat till en länkad mapp finns kvar i dokumentlistan tills det har flyttats helt. Dokumentalternativen är inaktiverade, men du kan fortfarande öppna dokumentet för visning medan det flyttas. När dokumentet har slutfört överföringen tas det bort från dokumentlistan eftersom det nu finns helt i den länkade mappen.

Tidigare skulle dokument omedelbart försvinna från dokumentlistan innan de hade flyttats till den länkade mappen.

Mer information finns i [Länka dokument från externa program](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Skapa automatiskt länkade mappar till Adobe Experience Manager Assets när du skapar ett projekt

Med det nya arbetsflödet Skapa länkad mapp för Adobe Experience Manager-integreringen kan du konfigurera integreringen med en sökväg till en Adobe Experience Manager Assets-mapp. När integreringen läggs till i en projektmall skapas automatiskt en länkad undermapp i Experience Manager Assets i den angivna mappen för projekt som skapas från mallen.

Tidigare krävdes åtgärder från användaren för att skapa länkade mappar.

Den här funktionaliteten är bara tillgänglig om Adobe Experience Manager as a Cloud Service är integrerat med Workfront. Detta är inte tillgängligt i Adobe Experience Manager förbättrade anslutning.

Mer information finns i [Använda arbetsflöden i Experience Manager Assets-integrering](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Koppla Workfront-fältvärden till taggar i Experience Manager Assets

Nu kan du kategorisera och snabbt hitta resurser baserat på data från Workfront. Du kan mappa dessa data som en del av din metadatakonfiguration i integreringen med Workfront för Experience Manager Assets.

Tidigare var det inte möjligt att mappa Workfront-data till Experience Manager Assets-taggar.

Mer information om den här funktionen i Experience Manager Assets as a Cloud Service finns i [Konfigurera [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Mer information om den här funktionen i Experience Manager Assets Essentials finns i [Konfigurera integreringen av Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Mappa Workfront-fält till anpassade Experience Manager Assets-metadatafält

Med den inbyggda integreringen kan du nu mappa både inbyggda och inbyggda Workfront-fält till anpassade metadatamatchschemafält i Experience Manager Assets as a Cloud Service.

Mer information om den här funktionen i Experience Manager Assets as a Cloud Service finns i [Konfigurera [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Mer information om den här funktionen i Experience Manager Assets Essentials finns i [Konfigurera integreringen av Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Justera mallinställningar för korrekturrödning med Adobe Workfront för Creative Cloud

Nu kan du justera befintliga automatiska inställningar för arbetsflödesmallar direkt i Creative Cloud. När du har valt en befintlig automatiserad arbetsflödesmall kan du:

* Inaktivera faser
* Lägg till ytterligare mottagare
* Ändra korrekturroller
* Justera deadline
* Uppdatera e-postmeddelanden
* Och mycket mer!

Mer information finns i [Ladda upp dokument och korrektur med [!DNL Adobe Workfront] plugin för [!DNL Creative Cloud] Program](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Dessa förbättringar är tillgängliga för följande Creative Cloud-program:

* Photoshop
* XD
* InDesign
* Illustrator

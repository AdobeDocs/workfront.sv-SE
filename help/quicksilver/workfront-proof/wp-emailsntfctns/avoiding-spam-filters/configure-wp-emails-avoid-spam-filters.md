---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Konfigurera [!DNL Workfront Proof] e-postmeddelanden för att undvika skräppostfilter
description: "Din e-postklients skräppostfilter har ett viktigt syfte: skydda dig mot irriterande och eventuellt skadliga skräppost. Men om du inte har rätt inställningar i skräppostfiltret kan det hindra dig från att se följande viktiga [!DNL Workfront Proof] e-post: korrekturmeddelanden, nyhetsbrev och specialmeddelanden."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Konfigurera [!DNL Workfront Proof] e-postmeddelanden för att undvika skräppostfilter

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

E-postklientens skräppostfilter har ett viktigt syfte: skydda dig mot irriterande och eventuellt skadliga skräppost. Men om du inte har rätt inställningar i skräppostfiltret kan det hindra dig från att se följande viktiga [!DNL Workfront Proof] e-post: korrekturmeddelanden, nyhetsbrev och specialmeddelanden.

För att vara säker på att [!DNL Workfront Proof] e-postmeddelanden dirigeras alltid till din inkorg i stället för till din skräppostmapp. Du bör lägga till följande i tillåtelselista:

* [!DNL Workfront Proof] e-postserver: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-postadresser (t.ex. notification@proofhq.com)

Mer information om URL:er att lägga till i tillåtelselista finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) i artikeln [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-postadresser

Beroende på vilken typ av e-postklient du har kan du behöva lägga till [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-postadresser till något av följande för att förhindra att skräppostfiltret dirigerar dina e-postmeddelanden till din skräppostmapp i framtiden:

* Din kontaktlista
* Dina [!UICONTROL Safe Senders] list
* Ett filter som du skapar för att leverera e-post från adresserna till din inkorg

Du kan också behöva ta bort befintliga [!DNL Workfront Proof] e-postmeddelanden från din skräppostmapp och kontrollera om någon av dem[!UICONTROL from]&quot; finns i listan över spärrade adresser. Den här hjälpsidan visar [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; adresser och visar hur du lägger till dem i skräppostfiltret i följande e-postklienter:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Om du har några frågor om en procedur som beskrivs här kan du få hjälp av din e-postklient.

Mer information finns i [Konfigurera skräppostinställningar för vanliga e-postklienter](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## The [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-postadresser att kopiera

För att vara säker på att [!DNL Workfront Proof] e-postmeddelanden når din inkorg, du måste lägga till två [!DNL Workfront Proof] e-postadresser separat till e-postklientens skräppostfilter:

* Den allmänna supportadressen, [!DNL support@proofhq.com]som [!DNL Workfront Proof] skickar ut många e-postmeddelanden
* En meddelandeadress som [!DNL Workfront Proof] skickar e-postmeddelanden med korrektur till den som skapat beviset och granskarna med länkar till beviset. Det kan vara en allmän adress, notification@support.proofhq.com, eller en specifik adress om du har en anpassad underdomän eller en vit etikettdomän.

Lägg till [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; adresser till e-postklientens filter:

1. Kopiera den allmänna [!DNL Workfront Proof] support &quot;[!UICONTROL from]&quot; e-postadress (support@proofhq.com) och klistra in den i fältet som anges för din e-postklient.
1. Kopiera ett av följande [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-postadresser och klistra in dem SEPARAT i fältet som anges för din e-postklient:

   * notification@support.proofhq.com om du INTE har en anpassad underdomän eller en vit etikettdomän
   * notification@yoursubdomain.proofhq.com om du har en anpassad underdomän; ange ditt underdomännamn i den här adressen
   * notification@yoursubdomain.yourdomain.com om du har en vit etikettdomän; byt ut ditt underdomännamn och domännamn mot den här adressen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->

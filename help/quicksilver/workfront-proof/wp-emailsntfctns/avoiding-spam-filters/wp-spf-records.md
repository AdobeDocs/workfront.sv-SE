---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF-poster
description: Workfront Proof skickar e-postmeddelanden till granskarna från en e-postadress från Workfront Proof som notification@proofing.yourdomain.com. För att se till att mottagarnas e-postservrar litar på alla e-postmeddelanden från Workfront Proof måste du konfigurera en  [!DNL Sender Policy] Framework-post (SPF) för din anpassade domän som är ansluten till  [!DNL Workfront Proof] kontot (till exempel proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Workfront Proof SPF-poster

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] skickar e-postmeddelanden till granskarna från en [!DNL Workfront Proof]-e-postadress, till exempel notification@proofing.yourdomain.com. För att se till att mottagarnas e-postservrar litar på alla [!DNL Workfront Proof] e-postmeddelanden måste du konfigurera en [!UICONTROL Sender Policy Framework] (SPF)-post för den anpassade domän som är ansluten till [!DNL Workfront Proof]-kontot (till exempel **proofing.dindomain.com**).

Om du vill konfigurera en SPF-post måste du inkludera den SPF-post som används för vår primära domän.

1. Lägg till en **[!UICONTROL DNS TXT]**-post för din domän med följande värde:

   `v=spf1 a:mx.proofhq.com -all`

   Din e-postadministratör eller IT-personal kan hjälpa dig att konfigurera detta.

   >[!TIP]
   >
   >Du kan använda det kostnadsfria verktyget på [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) för att granska SPF-poster i [!DNL Workfront].

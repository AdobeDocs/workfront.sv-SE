---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Korrektur för SPF-poster
description: Workfront Proof skickar e-postmeddelanden till granskarna från en e-postadress som t.ex. notification@proofing.yourdomain.com. Om du vill vara säker på att mottagarnas e-postservrar litar på alla e-postmeddelanden för Workfront Proof måste du konfigurera en [!DNL Sender Policy] Ramverkspost (SPF) för din anpassade domän som är ansluten till [!DNL Workfront Proof] account (till exempel proofing.dindomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Workfront Korrektur för SPF-poster

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] skickar e-postmeddelanden till granskarna från en [!DNL Workfront Proof] e-postadress, till exempel notification@proofing.yourdomain.com. För att se till att mottagarnas e-postservrar litar på alla [!DNL Workfront Proof] e-postmeddelanden, du måste konfigurera en [!UICONTROL Sender Policy Framework] (SPF)-post för din anpassade domän som är ansluten till [!DNL Workfront Proof] konto (till exempel **proofing.dindomain.com**).

Om du vill konfigurera en SPF-post måste du inkludera den SPF-post som används för vår primära domän.

1. Lägg till en **[!UICONTROL DNS TXT]** domänpost med följande värde:

   `v=spf1 a:mx.proofhq.com -all`

   Din e-postadministratör eller IT-personal kan hjälpa dig att konfigurera detta.

   >[!TIP]
   >
   >Du kan använda det kostnadsfria verktyget på [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) att granska [!DNL Workfront] SPF-poster.

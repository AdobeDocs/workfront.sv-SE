---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatering,release
navigation-topic: 2021-2-release-activity
title: 21.2 Förbättringar av korrektur
description: Den här sidan beskriver alla korrekturförbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i versionsöversikt 21.2.
author: Luke
feature: Product Announcements, Workfront Proof, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 1f82c397-5cb6-4adc-bb84-f5b1e1ed9d5e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 21.2 Förbättringar av korrektur

Den här sidan beskriver alla korrekturförbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i [21.2 versionsöversikt](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Handläggningsbevis visas nu i listan Dokument

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Det övergripande korrekturbeslutet visas nu i standarddokumentlistvyn.

Med den här förbättringen kan du enkelt se alla korrektur som har ett övergripande beslut direkt i standardlistvyn. Det gör det mycket enkelt att hitta korrekturförloppet utan att behöva navigera till olika sidor.

Tidigare var du tvungen att gå till arbetsflödet för dokumentinformation och korrektur för att kunna se det övergripande korrekturbeslutet, som krävde flera klick.

Mer information om korrekturbeslut finns i [Dokumentområdet](../../../documents/managing-documents/documents-area.md).

Den här funktionen ingår nu i [Hantera korrektur och versioner i den nya inlärningsvägen för Workfront Experience](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/home) på Workfront One.

## Nya fält i rapporten Korrektur för godkännande

Vi har lagt till följande fält i rapporten för korrektur av godkännande för att kunna visa användbar korrekturinformation:

* **Beslutsdatum:** Visar datumet som en godkännare fattar ett beslut om ett bevis. Det här datumet finns också på sidan Skriv ut sammanfattning av korrekturet.
* **Godkännarstadium:** Visar aktuell sceninformation.
* **Arbetsflödesmall:** Visar alla arbetsflödesmallar som är kopplade till korrekturet. Om ingen mall är kopplad är kolumnen tom.

Dessa fält ingår inte i standardrapporten. Du måste lägga till dem om du vill se dem.

Den här funktionen ingår nu i [Korrektursysteminställningarna, del 2: Arbetsflödeshantering](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/home) utbildningsväg på Workfront One.

## Överför det befintliga korrekturarbetsflödet när en ny version genereras

>[!NOTE]
>
>Den här funktionen togs bort från förhandsvisningsmiljön den 30 mars 2021 och från produktionsmiljön den 1 april 2021. Den ingår inte i version 21.1.

Det befintliga korrekturarbetsflödet överförs nu till alla nya versioner du skapar, oavsett vilken metod de skapas i.

Tidigare fanns det en liten skillnad i hur korrekturarbetsflödet överfördes beroende på var du skapade dem i Workfront.

Mer information finns i [Skapa en ny version av ett korrektur](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/create-new-proof-version.md).

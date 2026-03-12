---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: Området Dokument
description: Under Dokument kan du ordna, hantera och visa metadata för dokument som överförts till Adobe Workfront. Du kan också se bevisbeslutet.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
source-git-commit: abff7d82c89992e2e494aae13c9eb20868259b54
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Området Dokument

Under Dokument kan du ordna, hantera och visa metadata för dokument som överförts till Adobe Workfront. Du kan också se bevisbeslutet.

Workfront har för närvarande två versioner av dokumentområdet: det gamla dokumentområdet och det nya dokumentområdet. Vilken version din organisation använder beror på om din organisation använder äldre Workfront-lagring eller Enterprise-lagring. Mer information om de här lagringstyperna finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Äldre dokumentområde

Det finns två typer av dokumentområden. Funktionerna är desamma för båda:

* **Dokumentområde i ett program, en portfölj, ett projekt, en aktivitet eller ett ärende:** Visar alla dokument som du har tillgång till för ett visst projekt, en viss aktivitet eller ett visst problem. Om du vill komma åt det här området klickar du på ikonen **Dokument** ![Dokument](assets/document-icon-12x14.png) i den vänstra panelen när du visar ett projekt, en uppgift eller ett problem.

* **Området Globala dokument:** Visar alla dokument som du har tillgång till i Workfront. Om du vill komma åt det här området klickar du på ikonen **Dokument** ![Dokument](assets/document-icon.png) på huvudmenyn ![Huvudmeny-ikon](assets/main-menu-icon.png).

Mer information om hur du överför dokument till Workfront finns i [Lägga till dokument till Adobe Workfront från ditt filsystem](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).


Dokumentområdet registrerar ett antal av följande objekt:

* Workfront-mappar
* Filer som överförts från filsystemet
* Filer som lagts till i Workfront från integreringar
* Länkad Experience Manager Assets

### Panelen Sammanfattning

När du markerar ett dokument i dokumentområdet kan du använda Sammanfattning till höger för att visa dokumentinformation, hantera dokumentuppdateringar och godkännanden, visa dokumentversioner samt lägga till och redigera anpassad Forms för dokumentet.

Om korrektur är inställt för dokumentet innehåller avsnittet Detaljer information som förfallodatum för korrektur och aktuell korrekturstatus.

Du kan klicka på rubriken Detaljer för att gå till hela dokumentinformationsdelen när du behöver all information om ett dokument.

![Dokumentområde](assets/documents-area-v2-350x199.png)

Mer information om sammanfattningen finns i [Sammanfattning för dokumentöversikt](../../documents/managing-documents/summary-for-documents.md).

### Beslutsbevis

När du har fattat ett korrekturbeslut visas det i dokumentlistan.

![Bekräftelsebeslut i dokumentlistan](assets/proof-decision---doc-list-350x168.png)

### Mappar

I ett projekt, en uppgift eller ett problem där dokument överförs, kan du konfigurera mappar för att ordna dokumenten. Mer information finns i [Skapa dokumentmappar](../../documents/organizing-documents/create-documents-folder.md).

I det globala dokumentområdet kan du ställa in två typer av mappar för att ordna de dokument du har tillgång till:

* **Smarta mappar:** Visa endast de dokument som du vill visa. Mer information finns i [Skapa och hantera smarta mappar](../../documents/organizing-documents/create-manage-smart-folders.md).

* **Mina mappar:** Ordna dokument som du vill ha dem. Mer information finns i [Skapa dokumentmappar](../../documents/organizing-documents/create-documents-folder.md).

### Utökad dokumentinformation

På sidan Dokumentinformation finns en mer fullskalig version av Dokumentinformation i Sammanfattning till höger.

## Nytt dokumentområde

>[!NOTE]
>
>Det globala dokumentområdet är inte tillgängligt i det nya dokumentområdets upplevelse. Du kan bara komma åt dokument från program, portföljer, projekt, uppgifter eller utgåvor.

### Använda sammanfattningspanelen

När du markerar ett dokument i dokumentområdet kan du använda panelen Sammanfattning till höger för att visa information om dokumentet, lägga till och redigera kopplade anpassade formulär, skapa och hantera arbetsflöden för godkännande, visa dokumentversioner och mycket mer.

#### Granska och godkänn med Frame.io

Du kan granska och godkänna dokument i det nya dokumentområdet med visningsprogrammet Frame.io.

Mer information finns i [Kom igång med Frame.io-integreringen](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Hantera versioner

Du kan överföra nya versioner av ett dokument i området för nya dokument. När du överför en ny version behålls den tidigare versionen och du kommer åt den från panelen Sammanfattning. Versionerna får automatiskt namn med datum och tid för överföringen, men de kan få nya namn efter behov.

Du kan också starta ett nytt arbetsflöde för godkännande för en viss version av ett dokument.

#### Visa dokumenthistorik

Du kan visa ett dokuments historik i området för nya dokument. Historiken innehåller följande typer av information:

* När dokumentet överfördes
* När nya versioner överfördes
* När arbetsflöden för godkännande startades för dokumentet
* Och mer

### Mappar på systemnivå för dokumentbehörigheter

Workfront skapar automatiskt en mapp på systemnivå när det första dokumentet överförs till en uppgift eller ett problem. De här mapparna ärver behörigheter från uppgiften eller utgåvan och visas i dokumentområdet på projektnivå. Alla dokument som överförs till den uppgiften eller utgåvan lagras i den mappen och ärver behörigheter från den. Detta är det primära sättet att hantera behörigheter för dokument i området för nya dokument. Mer information finns i [Objektbehörigheter och översikt över åtkomstnivån för Adobe Enterprise-lagringsmodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).
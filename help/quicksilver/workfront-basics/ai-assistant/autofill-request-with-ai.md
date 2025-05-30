---
title: Fyll i en begäran automatiskt med hjälp av AI
content-type: reference
description: Du kan använda AI för att fylla i begärandefält automatiskt.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: 977817157e016b7cbe591d8627031208d7bf3bb3
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---

# Fyll i en begäran automatiskt med hjälp av AI

>[!NOTE]
>
>Den här funktionen är för närvarande en del av en sluten betaversion. Kontakta sargism@adobe.com om du vill aktivera den här funktionen.
>
>För att bli berättigad till en sluten betaversion måste din organisation uppfylla kraven för att få använda Workfront AI Assistant. Mer information finns i [Förutsättningar för AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

AI kan hjälpa dig att fylla i begärandefält automatiskt. Den kan föreslå fältvärden baserat på tidigare förfrågningar eller tolka dem från text som e-post är överförda dokument.

Du kan godkänna eller avvisa dessa förslag innan du skickar in begäran.

Autofyll skriver inte över fält som du redan har fyllt i.

## Få förslag när du fyller i formulär

Autofyll kan föreslå fältvärden medan du fyller i formuläret. När du anger värden i begärandefälten jämför Workfront dessa värden med tidigare begäranden. Om det angivna värdet har en nära koppling till andra fältvärden i liknande sammanhang i tidigare begäranden föreslår Workfront dessa värden.

Om t.ex. en klinik alltid använder samma faktureringskod föreslår Workfront att faktureringskoden anges i rätt fält när det kliniska namnet anges.

Så här använder du förslag som baseras på tidigare begäranden:

1. Börja skapa en begäran.

   Instruktioner finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Börja fylla i fält.

   När du fyller i fält kan andra fält visa förslag.

1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** under det fältet.

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

## Få förslag från en textfråga

Autofyll kan föreslå fältvärden baserade på text som e-post. Du klistrar in i ett textblock och Workfront bearbetar texten för att föreslå fältvärden som baseras på texten.

Om e-postmeddelandet t.ex. innehåller&quot;Detta förfaller den 1 juni&quot; och formuläret innehåller ett fält för förfallodatum, föreslår Workfront 1 juni för det fältvärdet.

Den här typen av förslag kontrollerar även tidigare begäranden om liknande sammanhang. Om uppmaningen t.ex. anger att begäran gäller en viss klient kan Workfront automatiskt hitta och ange faktureringsadressen för den klienten baserat på tidigare begäranden.

Du kan klistra in text som ska användas i hela formuläret eller i ett enskilt avsnitt i formuläret.

Så här använder du förslag som baseras på en inklistrad textfråga:

1. Börja skapa en begäran.

   Instruktioner finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Klicka på AI-ikonen ![AI-ikonen](assets/request-prompt-icon.png) under formulärnamnet om du vill använda textprompten i hela formuläret.

   eller

   Klicka på AI-ikonen ![AI-ikonen](assets/request-prompt-icon.png) bredvid avsnittsnamnet om du vill använda textprompten för ett enskilt avsnitt.

1. Klistra in texten i rutan.
1. Klicka på **Fyll i formuläret**.

   Workfront genererar förslag för formuläret.
1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** under det fältet.

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

## Få förslag baserade på ett dokument som du överför

Autofyll kan föreslå fältvärden baserat på ett dokument som du överför.

Den här typen av förslag kontrollerar även tidigare begäranden om liknande sammanhang. Om uppmaningen t.ex. anger att begäran gäller en viss klient kan Workfront automatiskt hitta och ange faktureringsadressen för den klienten baserat på tidigare begäranden.

### Dokumentöverföringsgarantier

#### Filtyper som stöds

Följande filtyper stöds:

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XSX

#### Filstorlek som stöds

Varje fil kan vara upp till 100 MB stor

#### Antal filer

Du kan överföra upp till 50 filer (sidor, bilder eller ark).

>[!IMPORTANT]
>
>Dokument konverteras till en serie bilder, som alla betraktas som separata filer.
>
>Du kan t.ex. överföra en PowerPoint med 50 bilder eller fem Word-dokument med 10 sidor.

#### Andra bästa metoder

Tänk på följande när du överför ett dokument för automatisk ifyllning av begäran:

* Autofyll är optimerat för det latinska alfabetet.
* Vi rekommenderar att du använder en textstorlek på 8 punkter eller större.
* Autofyll kan ha problem med bilder i dokumentet, t.ex. roterade eller förvrängda bilder, diagram och räkning eller med spatiala orsaker på objekt i bilder.
* Som alltid rekommenderar vi att du kontrollerar resultatet innan du skickar in begäran.

### Överföra ett dokument för att autofylla en begäran

Du kan överföra ett dokument som ska användas på hela formuläret eller till ett enskilt avsnitt i formuläret.

1. Börja skapa en begäran.

   Instruktioner finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Om du vill använda dokumentet på hela formuläret klickar du på AI-ikonen ![AI-ikonen](assets/request-prompt-icon.png) under formulärnamnet.

   eller

   Om du vill använda dokumentet för ett enskilt avsnitt klickar du på AI-ikonen ![AI-ikonen](assets/request-prompt-icon.png) bredvid avsnittsnamnet.

1. Klicka på **Överför filer** och välj sedan filen i din filhanterare.

   eller

   Dra dokumentet från din filhanterare till rutan **Överför filer till begärandeformuläret** för automatisk ifyllning.
1. Klicka på **Fyll i formuläret** av **Fyll i avsnittet**.

   Workfront genererar förslag för formuläret.
1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** under det fältet.

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

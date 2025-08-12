---
title: Autofyll en begäran med uppmaningar eller dokument
content-type: reference
description: Du kan använda AI för att autofylla begärandefält genom att ange en uppmaning eller genom att ange ett dokument.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: fd42ac97be05df9499ea3214642099738ccc69b1
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 0%

---

# Autofyll en begäran med uppmaningar eller dokument

>[!NOTE]
>
>* Den här funktionen kommer att vara tillgänglig som en öppen betaversion enligt följande schema:
>
>   * Månadsutgåva: 11 september 2025
>   * kvartalsvis version: 16 oktober 2025
>
>* Om du vill använda den här funktionen måste din organisation uppfylla kraven för att kunna använda Workfront AI Assistant. Mer information finns i [Förutsättningar för AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

AI kan hjälpa dig att fylla i begärandefält automatiskt baserat på en uppmaning du anger. Det kan även fylla i fält som är baserade på text som e-post är överförda dokument. Du kan godkänna eller avvisa dessa förslag innan du skickar in begäran.

Autofyll skriver inte över fält som du redan har fyllt i.

Användarna får inga förslag på data som de annars inte har tillgång till.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Medarbetare eller högre</p>
   eller
   <p>Aktuell: Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  </td> 
  </tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td><p>Åtkomst att lägga till begäranden i en begärandekö</p> <p>Visa eller högre behörigheter för den befintliga begäran</p> <p>Mer information om hur du konfigurerar en begärandekö finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Om du vill fylla i begäranden automatiskt med hjälp av en prompt eller ett dokument måste **alla** av följande gälla:

* Din organisation måste ha migrerat till Adobe IMS (Identity Management System)
* Adobe Unified Experience måste aktiveras
* Din organisation måste ha en Select-, Prime- eller Ultimate Workfront-plan
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands

  Mer information om hur du signerar avtalet finns i [Signera Adobe Gen AI-avtalet](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) i artikelns AI Assistant-översikt.
* AI Assistant måste aktiveras i organisationens systeminställningar. Detta hanteras av din Workfront-administratör.

  Mer information om hur du aktiverar AI Assistant i systeminställningarna finns i [Aktivera eller inaktivera AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

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
1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** för fältet.

   ![Godkänn eller avvisa förslag](assets/accept-reject-suggestion.png)

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

   >[!NOTE]
   >
   >Alla ogranskade förslag godkänns automatiskt när du skickar in begäran.

## Få förslag baserade på ett dokument som du överför

Autofyll kan föreslå fältvärden baserat på ett dokument som du överför.

Den här typen av förslag kontrollerar även tidigare begäranden om liknande sammanhang. Om uppmaningen t.ex. anger att begäran gäller en viss klient kan Workfront automatiskt hitta och ange faktureringsadressen för den klienten baserat på tidigare begäranden.

### Dokumentöverföringsgarantier

#### Filtyper som stöds

Följande filtyper stöds:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XSX</li>
</ul>
</td>
</tr>
</table>

#### Filstorlek som stöds

Varje fil kan vara upp till 100 MB stor

#### Antal filer

Du kan överföra upp till 50 filer (sidor, bilder eller ark).

>[!IMPORTANT]
>
>Dokument konverteras till en serie bilder, som alla betraktas som separata filer.
>
>Du kan t.ex. överföra en PowerPoint med 50 bilder eller fem Word-dokument med 10 sidor.

#### Fälttyper som stöds

Workfront-fälttyper påverkar om ett visst fält kan fyllas i automatiskt.

<table>
<tr>
<td><b>Automatisk fyllning som stöds </b><br> kan användas</td>
<td><b>Autofyll stöds inte</b> <br>Autofyll fylls inte</td>
</tr>
<tr>
<td>
<ul>
<li>Enkelradig text</li>
<li>Textområde eller stycke</li>
<li>Datumfält</li>
<li>Kryssruta</li>
<li>Alternativknappar</li>
<li>Enkel- och flervalslistrutor</li>
</ul>
</td>
<td><li>Typeahead</li>
<li>Extern sökning</li>
<li>Intern sökning</li>
<li>Referens</li>
<li>WF Planerar inbäddade fält</li>
</ul>
</td>
</tr>
</table>

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
1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** för fältet.

   ![Godkänn eller avvisa förslag](assets/accept-reject-suggestion.png)

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

   >[!NOTE]
   >
   >Alla ogranskade förslag godkänns automatiskt när du skickar in begäran.

## Felsökning

Om du inte får de förväntade förslagen kan det bero på något av följande:

* Du måste ha minst en månads begärandedata i systemet innan det kan föreslå fältvärden från tidigare begäranden.
* Du kanske inte har följt upp dokumentets överföringsskyddsutkast när du överför ett dokument för att hämta förslag. Mer information finns i [Dokumentöverföringsskyddsutkast](#document-upload-guardrails) i den här artikeln.

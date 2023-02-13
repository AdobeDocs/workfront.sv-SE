---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer - översikt
description: Adobe Workfront har två olika korrekturläsare - EDIT ME.
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer - översikt

Adobe Workfront har två olika korrekturläsare:

* **Web Proofing Viewer:** Utformad främst för korrektur av statiska filer och videofiler. Körs i Google Chrome, Firefox eller Safari.
* **Desktop Proofing Viewer:** Utformad för korrektur av interaktiva filer samt video och statiska filer. Kör som ett fristående program på din arbetsstation. Mer information finns i [Förstå Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* Om din organisation av säkerhetsskäl inte kan använda appen Desktop Proofing Viewer kan din Workfront-administratör konfigurera ditt system så att du kan granska interaktivt innehåll som paketerats i en ZIP-arkivfil i Web Proofing Viewer. Mer information finns i  [Konfigurera korrektur av interaktivt innehåll i Web Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

Följande lista hjälper dig att förstå vilket korrekturläsare du kan använda för att kontrollera vissa typer av innehåll:

* **Interaktivt webbinnehåll - URL**: Om du skapar ett korrektur för webbinnehåll med en URL-adress och vill korrekturgranska innehållet interaktivt, måste du använda Desktop Proofing Viewer.
* **Interaktivt webbinnehåll - ZIP-fil**: Om du skapar ett korrektur för webbinnehåll med en ZIP-fil kan du antingen använda Web Proofing Viewer (med vissa begränsningar) eller Desktop Proofing Viewer. Mer information om begränsningarna med att använda Web Proofing Viewer för interaktivt innehåll finns i [Konfigurera korrektur av interaktivt innehåll i Web Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **Statiskt och videomaterial**: Om du skapar ett korrektur som innehåller statiskt innehåll kan du antingen använda Web Proofing Viewer eller Desktop Proofing Viewer.

## Statiska korrektur

| **Funktion** | **Webbkorrekturläsare** | **Desktop Proofing Viewer** |
|---|---|---|
| Öppna statiskt korrektur | ✓ | ✓&#42; |
| Enkelt, magasin och kontinuerliga vyer | ✓ | ✓&#42; |
| Panorering | ✓ | ✓&#42; |
| Zooma | ✓ | ✓&#42; |
| Rotera | ✓ | ✓&#42; |
| Mätningsverktyg | ✓ (ange ett område med anpassad storlek) | ✓&#42; |
| Miniatyrbildsvisning | ✓ | ✓&#42; |
| Navigator för statiskt korrektur | ✓ | ✓&#42; |
| Dokumentsökning | ✓ | ✓&#42; |
| Posta kommentar på flera sidor | ✓ (tillgänglig i alla vyer) | ✓&#42; (tillgängligt på alla vyer) |
| Avancerade statiska kortkommandon | ✓ (mer information finns i [Kortkommandon i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;(mer information finns i [Kortkommandon i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style=&quot;table-layout:auto&quot;}

&#42; Den här funktionen fungerar bara om Workfront-administratören har konfigurerat Desktop Proofing Viewer som standardvisningsprogram för alla korrektur.

## Videokorrektur

| **Funktion**  | **Webbkorrekturläsare** | **Desktop Proofing Viewer** |
|---|---|---|
| Öppna videokorrektur | ✓ | ✓&#42; |
| Buffring | ✓ | ✓&#42; |
| Granska med tiden | ✓ | ✓&#42; |
| Granska med bildrutor eller tidskod | ✓ | ✓&#42; |
| Granska snabbare eller långsammare | ✓ | ✓&#42; |
| Volymreglering | ✓ | ✓&#42;  |
| helskärmsläge | ✓ | ✓&#42;  |
| Intervallkommentarer | ✓ | ✓&#42;  |
| Gör videokorrektur (videoklippen blir klara och startar automatiskt) | ✓ | ✓&#42;  |
| Avancerade kortkommandon för video | ✓ (mer information finns i [Kortkommandon i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;  |

{style=&quot;table-layout:auto&quot;}

&#42; Den här funktionen fungerar bara om Desktop Proofing Viewer har konfigurerats som standardvisningsprogram för alla korrektur.

## Interaktiva korrektur

| **Funktion**  | **Webbkorrekturläsare** | **Desktop Proofing Viewer** |
|---|---|---|
| Öppna interaktiva korrektur som skapats av innehåll som paketerats i en ZIP-fil | ✓ | ✓ (rekommenderas) |
| Öppna ett interaktivt korrektur som skapats från en URL | Stöds inte | ✓ |
| Visa interaktiva korrektur (som skapats från innehåll som paketerats i en ZIP-fil) i olika skärmstorlekar | ✓ | ✓ |
| Visa interaktiva korrektur (som skapats från innehåll som paketerats i en ZIP-fil) för olika enheter | Stöds inte | ✓ |
| Granska oskyddade HTTP-platser | Stöds inte | ✓ |
| Granska iFrame-skyddade webbplatser (webbplatser som skyddas från att visas i en iFrame) | Stöds inte | ✓ |

{style=&quot;table-layout:auto&quot;}

## Kommentarer

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Funktion</th> 
   <th>Webbkorrekturläsare </th> 
   <th>Desktop Proofing Viewer </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Lägga till, ta bort och redigera kommentarer</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Lägga till och ta bort svar</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Rektangel-, pil-, linje-, frihand- och markeringsverktyg</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Polyline, verktyg</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Verktyg för beskärningsmaskmarkering</p> </td> 
   <td>Stöds inte</td> 
   <td>Stöds inte</td> 
  </tr> 
  <tr> 
   <td> <p>Markeringsverktyg för textmarkering</p> </td> 
   <td>Endast ✓ statiska korrektur</td> 
   <td>Endast ✓ statiska korrektur</td> 
  </tr> 
  <tr> 
   <td> <p>Ändra markeringsfärg</p> </td> 
   <td>✓ (32 färger finns) </td> 
   <td>✓ (32 färger finns) </td> 
  </tr> 
  <tr> 
   <td> <p>Ändra markeringens opacitet</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Ändra markeringstjocklek</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Klippa ut, kopiera och klistra in markeringar</p> </td> 
   <td> Stöds inte</td> 
   <td> Stöds inte</td> 
  </tr> 
  <tr> 
   <td> <p>Ångra och göra om senaste åtgärd</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Duplicera markeringar</p> </td> 
   <td> Stöds inte</td> 
   <td> Stöds inte</td> 
  </tr> 
  <tr> 
   <td>Ange åtgärder för kommentarer</td> 
   <td>✓ (Åtgärder visas i kommentarer direkt efter att åtgärden har ställts in)</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ange markeringsfärg som standard</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Lös kommentarer</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Lås kommentarer</p> </td> 
   <td>Stöds inte</td> 
   <td> Stöds inte</td> 
  </tr> 
  <tr> 
   <td> <p>Tagga användare</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Återuppta kommentarer</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Visa kommentarlistan i en komprimerad vy</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Visa kommentarlistan i en standardvy, fullständig vy eller enkelvy</p> </td> 
   <td>Planerad för framtiden</td> 
   <td>Planerad för framtiden</td> 
  </tr> 
  <tr> 
   <td> <p>Sök kommentarer</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrera kommentarer efter användare</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrera kommentarer och svar efter användare</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sortera kommentarer</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Automatiska uppdateringar av kommentarer</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Beslut

| Funktion | Webbkorrekturläsare | Desktop Proofing Viewer |
|---|---|---|
| Fatta beslut | ✓ | ✓ |
| Anpassa beslut | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

## Jämför korrektur

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Funktion</th> 
   <th>Webbkorrekturläsare </th> 
   <th>Desktop Proofing Viewer </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Jämför olika versioner av korrektur</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>Jämför separata korrektur</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## Korrekturåtgärder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Funktion</th> 
   <th>Webbkorrekturläsare </th> 
   <th>Desktop Proofing Viewer </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ändra korrekturversionen </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>Skapa en ny version</td> 
   <td> <p>Finns endast i Workfront Proof (framtidsplanerat vid korrektur i Workfront)<br></p> </td> 
   <td>Finns endast i Workfront Proof (framtidsplanerat vid korrektur i Workfront)</td> 
  </tr> 
  <tr> 
   <td>Granska korrekturinformation </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Granska korrekturarbetsflöden</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Redigera arbetsflödesfaser</td> 
   <td>Stöds inte</td> 
   <td>Stöds inte</td> 
  </tr> 
  <tr> 
   <td>Dela korrektur</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hämta team-URL</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ändra e-postmeddelanden</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hämta originalfil</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Låsa och låsa upp korrektur och faser</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Skriv ut korrektursammanfattning</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ta bort korrektur</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hantera korrektur från samma mapp</td> 
   <td><strong>Finns endast i Workfront Proof</strong> </td> 
   <td><strong>Finns endast i Workfront Proof</strong> </td> 
  </tr> 
  <tr> 
   <td>Varumärke (anpassade logotyper)</td> 
   <td>✓</td> 
   <td> ✓<br>(Workfront logotyp på startsidan) </td> 
  </tr> 
  <tr> 
   <td>Anpassade länkar (endast Workfront Proof)</td> 
   <td>Stöds inte</td> 
   <td> Stöds inte </td> 
  </tr> 
  <tr> 
   <td>Integrering med basecamp (endast Workfront Proof) </td> 
   <td>Planerad för framtiden</td> 
   <td>Planerad för framtiden</td> 
  </tr> 
  <tr> 
   <td>Indikator för närvaro </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Korrektur för automatiska uppdateringar (behörighetsändringar och nya versioner)</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## Miniviewer

| **Funktion**  | **Webbkorrekturläsare**  | **Desktop Proofing Viewer** |
|---|---|---|
| Inbäddad kod | Planerad för framtiden för statiskt och inbyggt videokort | Stöds inte  |

{style=&quot;table-layout:auto&quot;}

## Översättningar

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funktion</strong> </th> 
   <th><strong>Webbkorrekturläsare</strong> </th> 
   <th><strong>Desktop Proofing Viewer</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Andra supportspråk än engelska</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>

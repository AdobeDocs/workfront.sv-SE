---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,modell,tratt,diagram,nivåer,behörigheter
navigation-topic: access-levels
title: Tillgängliga funktioner för varje objekttyp för olika åtkomstnivåer (äldre)
description: I följande tabeller visas de funktioner som är tillgängliga för varje objekttyp på olika åtkomstnivåer.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 57632f1949e849aca3f26874382f1101b9b0cf89
workflow-type: tm+mt
source-wordcount: '1585'
ht-degree: 1%

---

# Tillgängliga funktioner för varje objekttyp för olika åtkomstnivåer (äldre)

>[!NOTE]
>
>Informationen i den här artikeln avser de äldre åtkomstnivåerna. Mer information om de aktuella åtkomstnivåerna finns i [Översikt över nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

I följande tabeller visas de funktioner som är tillgängliga för varje objekttyp på olika åtkomstnivåer.

Det anger också vilka åtgärder Workfront-administratörer kan inaktivera eller aktivera med en åtkomstnivå.

>[!NOTE]
>
>I den här artikeln beskrivs de funktioner som är tillgängliga för åtkomstnivåer i den aktuella paketmodellen för Workfront. Information om vilka funktioner som är tillgängliga i den nya paketmodellen finns i [Tillgängliga funktioner för varje objekttyp för nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Projekt

Endast användare med en planlicens kan beviljas fullständig åtkomst till projekt.

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; |  |  |  |  |
| Kopiera | ✓&#42; |  |  |  |  |
| Ta bort | ✓&#42; |  |  |  |  |
| Dela | ✓&#42; | ✓&#42; |  |  |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Lägga till ett anpassat formulär | ✓ |  |  |  |  |
| Uppdatera anpassade fält | ✓ | ✓ |  |  |  |
| Lägga till en godkännandeprocess | ✓ |  |  |  |  |
| Godkänn ett projekt | ✓ | ✓ | ✓ |  |  |
| Lägg till dokument | ✓ | ✓ | ✓ |  |  |
| Lägg till utgåva | ✓ | ✓ |  |  |  |
| Lägga till uppgifter | ✓ | ✓ |  |  |  |
| Ge uppdateringar/kommentarer | ✓ | ✓ | ✓ |  |  |
| Ändra status | ✓ |  |  |  |  |
| Loggtimmar | ✓ | ✓ |  |  |  |
| Redigera uppdrag | ✓ | ✓ |  |  |  |
| Hantera en baslinje | ✓ |  |  |  |  |
| Hantera risker | ✓ |  |  |  |  |
| Hantera ekonomi | ✓ |  |  |  |  |
| Lägg till/redigera utgifter | ✓ | ✓ |  |  |  |
| Bifoga mallar | ✓ |  |  |  |  |
| Spara som mall | ✓ |  |  |  |  |
| Lägga till/redigera ett affärsärende | ✓ |  |  |  |  |
| Redigera projektinformation | ✓ |  |  |  |  |
| Redigera personal | ✓ |  |  |  |  |
| Exportera till MS-projekt | ✓ | ✓ | ✓ |  |  |
| Beräkna om ekonomi/tidslinje | ✓ |  |  |  |  |
| Ange köegenskaper | ✓ |  |  |  |  |



&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Uppgifter

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; | ✓&#42; |  |  |  |
| Ta bort | ✓&#42; | ✓&#42; |  |  |  |
| Dela | ✓&#42; | ✓&#42; |  |  |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Lägg till föregående aktiviteter | ✓ | ✓ |  |  |  |
| Lägg till problem | ✓ | ✓ |  |  |  |
| Redigera en uppgift (exklusive status) | ✓ | ✓ |  |  |  |
| Ändra aktivitetsstatus | ✓ | ✓ |  |  |  |
| Lägga till dokument | ✓ | ✓ | ✓ |  |  |
| Kopiera en uppgift | ✓ | ✓ |  |  |  |
| Flytta en uppgift | ✓ | ✓ |  |  |  |
| Loggtimmar | ✓ | ✓ |  |  |  |
| Acceptera ett uppdrag | ✓ | ✓ |  |  |  |
| Skapa ett uppdrag | ✓ | ✓ | Endast infogad redigering | Endast infogad redigering |  |
| Bifoga ett eget formulär | ✓ | ✓ |  |  |  |
| Redigera anpassade fält | ✓ | ✓ |  |  |  |
| Skapa en godkännandeprocess | ✓ | ✓ |  |  |  |
| Godkänn en uppgift | ✓ | ✓ | ✓ |  |  |
| Redigera finanser | ✓ |  |  |  |  |
| Lägg till/redigera utgifter | ✓ | ✓ |  |  |  |
| Visa finansiering | ✓ | ✓ | ✓ |  |  |
| Uppdateringar/kommentarer | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problem

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Redigera | ✓ | ✓ | ✓ | ✓ |  |
| Ta bort | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Dela | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Bifoga anpassade formulär | ✓ | ✓ | ✓ | ✓ |  |
| Redigera anpassade fält | ✓ | ✓ | ✓ | ✓ |  |
| Godkänn problem | ✓ | ✓ | ✓ | ✓ |  |
| Lägga till en godkännandeprocess | ✓ | ✓ | ✓ | ✓ |  |
| Lägga till dokument | ✓ | ✓ | ✓ | ✓ |  |
| Kopiera problem | ✓ | ✓ | ✓ | ✓ |  |
| Flytta problem | ✓ | ✓ | ✓ | ✓ |  |
| Loggtimmar | ✓ | ✓ |  |  |  |
| Konvertera ett ärende till ett projekt | ✓ | ✓ |  |  |  |
| Konvertera ett problem till en uppgift | ✓ |  |  |  |  |
| Acceptera tilldelningar | ✓ | ✓ |  |  |  |
| Skapa uppdrag | ✓ | ✓ |  |  |  |
| Lägga till uppdateringar och kommentarer | ✓ | ✓ | ✓ | ✓ |  |



&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portföljer

Endast användare med en planlicens kan ha fullständig åtkomst till portföljer.

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; |  |  |  |  |
| Ta bort | ✓&#42; |  |  |  |  |
| Dela | ✓&#42; |  |  |  |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Redigera information | ✓ |  |  |  |  |
| Bifoga anpassade formulär | ✓ |  |  |  |  |
| Redigera anpassade fält | ✓ |  |  |  |  |
| Lägga till och ta bort projekt | ✓ |  |  |  |  |
| Godkänn projekt | ✓ |  |  |  |  |
| Portfolio-optimering | ✓ |  |  |  |  |
| Lägga till dokument | ✓ | ✓ | ✓ |  |  |
| Lägga till uppdateringar och kommentarer | ✓ | ✓ | ✓ |  |  |



&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Program

Endast användare med en planlicens kan ha fullständig åtkomst till program.

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; |  |  |  |  |
| Ta bort | ✓&#42; |  |  |  |  |
| Dela | ✓&#42; |  |  |  |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Redigera information | ✓ |  |  |  |  |
| Bifoga anpassade formulär | ✓ |  |  |  |  |
| Redigera anpassade fält | ✓ |  |  |  |  |
| Lägga till och ta bort projekt | ✓ |  |  |  |  |
| Godkänn projekt | ✓ |  |  |  |  |
| Portfolio Optimization | ✓ |  |  |  |  |
| Lägga till dokument | ✓ | ✓ | ✓ |  |  |
| Lägg till uppdateringar och kommentarer | ✓ | ✓ | ✓ |  |  |



&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Rapporter, kontrollpaneler och kalendrar

Användare med en planlicens har fullständig åtkomst till rapporter. Alla andra åtkomstnivåer har Visa-åtkomst till rapporter.

| Åtgärd | Planering | Arbetare | Granskare | Begäran | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; |  |  |  |  |
| Ta bort | ✓&#42; |  |  |  |  |
| Visa inbyggda rapporter | ✓&#42; |  |  |  |  |
| Dela | ✓&#42; | ✓ | ✓ |  |  |
| Dela kalendrar och rapporter offentligt | ✓&#42; |  |  |  |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Redigera | ✓ |  |  |  |  |
| Kopiera | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>Beställare kan bara visa rapporter som har delats med dem

## Filter, vyer och grupperingar

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Åtgärd</p> </th> 
   <th> <p>Planering</p> </th> 
   <th> <p>Arbetare</p> </th> 
   <th> <p>Granskare</p> </th> 
   <th> <p>Begärande</p> </th> 
   <th>Extern användare<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Skapa</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dela</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dela hela systemet</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Dokument

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Ta bort (dokument och mappar) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Dela | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Dela offentligt (externt) | ✓&#42; |  |  |  |  |
| Dela hela systemet | ✓&#42; | ✓&#42; |  |  |  |
| Visa | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Redigera information | ✓ | ✓ | ✓ | ✓ |  |
| Ladda ned | ✓ | ✓ | ✓ | ✓ | ✓ |
| Utcheckning | ✓ | ✓ | ✓ | ✓ |  |
| Lägg till godkännare | ✓ | ✓ | ✓ | ✓ |  |
| Godkänn dokument | ✓ | ✓ | ✓ | ✓ | ✓ |
| Bifoga anpassade formulär | ✓ | ✓ | ✓ | ✓ |  |
| Redigera anpassade fält | ✓ | ✓ | ✓ | ✓ |  |
| Flytta till (objekt) | ✓ | ✓ | ✓ | ✓ |  |
| Skicka till (integration) | ✓ | ✓ | ✓ | ✓ |  |
| Lägga till uppdateringar och kommentarer | ✓ | ✓ | ✓ | ✓ |  |
| Ladda upp ny version | ✓ | ✓ | ✓ | ✓ |  |
| Ta bort en version | ✓ | ✓ | ✓ | ✓ |  |
| Förhandsgranskning | ✓ | ✓ | ✓ | ✓ | ✓ |
| Korrektur | ✓ | ✓ | ✓ | ✓ |  |
| Generera korrektur | ✓ | ✓ |  |  |  |
| Ta bort korrektur | ✓ | ✓ | ✓ | ✓ |  |
| Lägg till/ta bort&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| Byt namn på &#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| Länk (med integration) | ✓ | ✓ | ✓ | ✓ |  |
| Bryt länk (med integration) | ✓ | ✓ | ✓ | ✓ |  |

{style="table-layout:auto"}

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Endast tillgängligt för dokumentmappar, inte dokument

## Användare

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Åtgärd</p> </th> 
   <th> <p>Planering</p> </th> 
   <th>Arbetare</th> 
   <th> <p>Granskare</p> </th> 
   <th> <p>Begärande</p> </th> 
   <th> <p>Extern användare**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Skapa</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera, ta bort, inaktivera, logga in som eller återställa lösenordet för alla användare</td> 
   <td>✓*<p><b>Obs!</b> Du kan inte logga in som någon användare som är systemadministratör.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera, ta bort, inaktivera, logga in som eller återställa lösenordet för alla användare i en grupp som de administrerar</td> 
   <td>✓*<p><b>Obs!</b> Du kan inte logga in som någon användare som är systemadministratör.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa användare</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa kontaktinformation</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Externa användare kan bara söka efter andra användare

## Team

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Åtgärd</p> </th> 
   <th> <p>Planering</p> </th> 
   <th>Arbetare</th> 
   <th> <p>Granskare</p> </th> 
   <th> <p>Begärande</p> </th> 
   <th> <p>Extern användare*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Skapa</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera team som de är på</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera team i grupper som de hanterar</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa alla team</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa team som är associerade med deras grupper</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Mallar

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa | ✓&#42; |  |  |  |  |
| Ta bort | ✓&#42; |  |  |  |  |
| Dela | ✓&#42; |  |  |  |  |
| Dela hela systemet | ✓&#42; |  |  |  |  |
| Visa | ✓&#42; |  |  |  |  |
| Kopiera | ✓ |  |  |  |  |
| Redigera mallinformation | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Finansiella uppgifter

Endast användare med en planlicens har fullständig tillgång till ekonomiska data.

Licenstyperna Begär och Extern användare inkluderas inte här eftersom de inte har tillgång till dessa objekt och områden.

| Åtgärd | Planering | Arbetare | Granskare |
|---|---|---|---|
| Redigera rollfakturering och kostnadstariffer | ✓&#42; |  |  |
| Redigera fakturering och kostnadstariffer för användare | ✓&#42; |  |  |
| Visa rollfakturering och kostnadstariffer | ✓&#42; |  |  |
| Visa fakturering och kostnadstariffer för användare | ✓&#42; |  |  |
| Hantera faktureringsposter | ✓ |  |  |
| Hantera utgifter | ✓ | ✓ |  |
| Visa ekonomiska data | ✓&#42; | ✓&#42; | ✓&#42; |
| Visa information efter kostnad i Resursplaneringsverktygen | ✓ |  |  |
| Budgetresurser i resursplaneringsverktygen &#42;&#42; | ✓ |  |  |
| Visa resursallokering i resursplaneringsverktygen &#42; | ✓ | ✓ | ✓ |
| Skapa risker i projekt | ✓ |  |  |
| Visa risker i projekt | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Kräver ytterligare åtkomst till Resurshantering.

## Resurshantering

Endast användare med en planlicens kan ha fullständig åtkomst till [utvalda objekt eller område]. Andra licenstyper kan ha begränsad eller ingen åtkomst till Resource Management i Workfront.

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Redigera prioriteringar och budgettimmar i planeraren | ✓&#42; |  |  |  |  |
| Skapa, redigera och ta bort resurspooler&#42;&#42; | ✓&#42; |  |  |  |  |
| Uppdatera planerade timmar i arbetsbelastningsutjämnaren &#42;&#42;&#42; | ✓* |  |  |  |  |
| Visa projektprioriteringar i Resursplanering | ✓&#42; |  |  |  |  |
| Visa resursallokering i verktygen för resursplanering | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Visa resurspooler | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Budgetresurser i resursplaneringsverktygen &#42;&#42; | ✓ |  |  |  |  |
| Bifoga resurspooler till projekt, mallar och användare | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Med en åtkomstnivå kan Workfront-administratörer inaktivera eller aktivera den här funktionen. Mer information finns i [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Kräver ytterligare åtkomst till finansiella data och behörigheter för projektekonomi. Om du ger en planeringsanvändare åtkomst till Resurshantering som inte har tillgång till ekonomiska data, kan användaren fortfarande se timallokeringarna i resursplaneraren, men inte växla till kostnadsvyn eller visa affärsärendet. Mer information finns i [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) och [Dela ekonomiska behörigheter för ett objekt](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Kräver behörighet att Contribute ska vara tillgängligt för objektet, med Aktivera tilldelningar under Avancerade inställningar. Mer information finns i avsnittet [Förstå ärvda behörigheter och objekthierarkin](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) i artikeln [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Område för scenarioplanering

| Åtgärd | Planering | Arbetare | Granskare | Begärande | Extern användare |
|---|---|---|---|---|---|
| Skapa/redigera befintliga planer och initiativ | ✓ | ✓ | ✓ |  |  |
| Lägg till eller redigera jobbrollinformation för planer och initiativ &#42; | ✓ | ✓ | ✓ |  |  |
| Lägg till eller redigera kostnadsinformation om planer och initiativ &#42; | ✓ | ✓ | ✓ |  |  |
| Ta bort planer och initiativ | ✓ | ✓ | ✓ |  |  |
| Visa scenarier på huvudmenyn ![Ikon för scenarioplanering](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |  |
| Visa planer och initiativ som användaren har skapat&#42; | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

>[!NOTE]
>
>Användare kan visa en plan som en annan användare har skapat endast om en länk till planen delas med dem.

&#42; För att användare ska kunna visa ekonomiska data i en plan eller ett initiativ måste de ha tillgång till ekonomiska data. Mer information finns i [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront målområde

| Instruktioner | Visa | Redigera |
|---|---|---|
| Skapa |  | ✓ |
| Redigera/ta bort alla mål |  | ✓ |
| Visa mål på huvudmenyn | ✓ | ✓ |
| Visa målområdet från en delad länk | ✓ | ✓ |
| Visa alla mål i systemet | ✓ | ✓ |
| Aktivera/inaktivera/stäng alla mål |  | ✓ |
| Skapa/redigera/ta bort aktiviteter |  | ✓ |
| Skapa/redigera/ta bort resultat |  | ✓ |
| Lägg till ett justerat mål |  | ✓ |
| Uppdatera förloppet för ett resultat eller en aktivitet |  | ✓ |
| Äger ett mål, ett resultat eller en aktivitet | ✓ | ✓ |
| Kommentera ett mål | ✓ | ✓ |
| Kopiera mål |  | ✓ |
| Visa avsnittet Mållista i den vänstra panelen | ✓ | ✓ |
| Visa avsnittet Diagram i den vänstra panelen | ✓ | ✓ |
| Visa avsnittet Måljustering på den vänstra panelen | ✓ | ✓ |



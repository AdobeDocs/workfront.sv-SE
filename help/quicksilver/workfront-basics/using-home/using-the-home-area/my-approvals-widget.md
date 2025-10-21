---
product-area: home
navigation-topic: use-the-home-area
title: Hantera dina godkännanden med widgeten Mina godkännanden
description: Widgeten Mina godkännanden visar alla dina väntande, tilldelade, delegerade och skickade godkännanden på ett och samma ställe. Här kan du filtrera och organisera dina godkännanden, fatta beslut och delegera godkännanden efter behov.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Hantera dina godkännanden med widgeten Mina godkännanden

Widgeten Mina godkännanden visar alla dina väntande, tilldelade, delegerade och skickade godkännanden på ett och samma ställe. Här kan du filtrera och organisera dina godkännanden, fatta beslut och delegera godkännanden efter behov.

Widgeten Mina godkännanden stöder godkännanden från följande Workfront-objekt:

* Uppgifter
* Problem
* Projekt
* Dokument
* Korrektur
* Förfrågningar om planeringsposter
* Tidrapporter

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller högre</p>
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomsten till objekt som är kopplade till godkännanden</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för objekt som är associerade med godkännanden</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Godkänn arbete från widgeten Mina godkännanden

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Klicka på **Anpassa** för att lägga till widgeten **Mina godkännanden**.
1. (Villkorligt) Klicka på listrutan **Filter** och välj sedan **Alla** för att visa godkännanden som tilldelats och delegerats till dig.

   >[!NOTE]
   >
   >Godkännanden som tilldelats till jobbroller eller grupper visas inte i Hem. Godkännanden som tilldelats team visas i widgeten Mina godkännanden för varje teammedlem.


1. Markera objektet där du vill fatta ett beslut om godkännande.

   ![Widgeten Mina godkännanden](assets/my-approvals-widget.png)

1. Klicka på ett av de tillgängliga alternativen när du ska fatta ett beslut om godkännande på den högra panelen. Följande alternativ visas i det övre högra hörnet av sidan, beroende på vilken typ av objekt du godkänner:

   <table>
   <tr>
      <td>
      <p><strong>Åtkomst</strong></p>
      </td>
      <td>
      <p><strong>Arbetsobjekt</strong></p>
      </td>
      <td>
      <p><strong>Dokument</strong></p>
      </td>
      <td>
      <p><strong>Korrektur</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Bidrag</li>
      <li>Ignorera</li>
      </ul>
      Du kan justera åtkomstnivån i listrutan <b>Ändra åtkomst</b> om du vill.
      </td>
      <td>
         <ul>
         <li>Godkänn</li>
         <li>Avvisa</li>
         </ul>
      Du kan lämna en kommentar med ditt beslut genom att klicka på listrutan i beslutsknappen.
      </td>
      <td>
   Tilldelad som godkännare
         <ul>
         <li>Godkänn</li>
         <li>Godkänn med ändringar</li>
         <li>Behöver göras</li>
         </ul>
   Tilldelad som granskare
         <ul>
         <li>Slutför min granskning</li>
         </ul>
      Alternativen i den här kolumnen gäller endast för enhetliga godkännanden. Godkännanden av äldre dokument visas på samma sätt som godkännanden av arbetsobjekt. 
      </td>
      <td>
         <ul>
         <li>Gå till korrektur</li>
         </ul>
         Du fattar ditt beslut i korrekturläsaren. Mer information om hur du granskar korrektur finns i <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Granska korrektur i Adobe Workfront</a>.
      </td>
   </tr>
   </table>

När du har fattat ett beslut tas godkännandet bort från widgeten Mitt godkännande.
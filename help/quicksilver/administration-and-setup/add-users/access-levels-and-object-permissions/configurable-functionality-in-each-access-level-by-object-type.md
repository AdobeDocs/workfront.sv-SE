---
title: Konfigurerbar äldre åtkomst till funktioner för varje objekttyp
description: I den här artikeln förklaras vad du kan tillåta som Adobe Workfront-administratör för varje objekttyp, i varje äldre åtkomstnivå. Det förklarar också vilken standardkonfiguration som används för varje typ av äldre åtkomstnivå.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '3456'
ht-degree: 0%

---

# Konfigurerbar äldre åtkomst till funktioner för varje objekttyp

I den här artikeln förklaras vad du kan tillåta som Adobe Workfront-administratör för varje objekttyp, i varje äldre åtkomstnivå. Det förklarar också vilken standardkonfiguration som används för varje typ av äldre åtkomstnivå.

Information om alla funktioner som är tillgängliga för en objekttyp på varje åtkomstnivå finns i [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projekt

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för projekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering (planlicenstyp)</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela projekt. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till projekt.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Kopiera</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Visa</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela projekt. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Tillåter begränsad redigeringsåtkomst till projekt. Om du vill se hur redigeringsåtkomsten är begränsad för en arbetaråtkomstnivå jämfört med en planeraråtkomstnivå (som tillåter fullständig redigeringsåtkomst till projekt) läser du avsnittet <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projekt</a> i artikeln <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Tillgängliga funktioner för varje objekttyp</a>.</p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela projekt. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Redigera och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> (standardval) <p>Visningsåtkomst är begränsad eftersom du inte kan finjustera den för att aktivera eller inaktivera projektdelning.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till projekt är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Uppgifter

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för uppgifter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela uppgifter. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till uppgifter.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela uppgifter. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till uppgifter.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> (standardval)<p>Visningsåtkomst är begränsad eftersom du inte kan finjustera den för att aktivera eller inaktivera projektdelning.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till uppgifter är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för problem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b></p><p>Om du vill finjustera detta kan du konfigurera möjligheten att dela problem. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst vid problem.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Om du vill finjustera detta kan du konfigurera möjligheten att dela problem. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst vid problem.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Om du vill finjustera detta kan du konfigurera möjligheten att dela problem. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst vid problem.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Om du vill finjustera detta kan du konfigurera möjligheten att dela problem. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst vid problem.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Det går inte att få åtkomst till utgåvor. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfolio

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för portföljer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela portföljer. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till portföljer.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> <p>Det går inte att få åtkomst till portföljer.</p> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Det går inte att få åtkomst till portföljer. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Program

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för program:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela program. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till program.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> <p>Åtkomst till program är inte tillgänglig.</p> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till program är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Rapporter, kontrollpaneler och kalendrar

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för rapporter, instrumentpaneler och kalendrar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b></p><p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera någon av följande åtgärder. Båda är aktiverade som standard:</p> 
      <ul> 
       <li> <p>Visa inbyggda rapporter</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till rapporter, kontrollpaneler och kalendrar.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard utom <b>Visa inbyggda rapporter</b>, <b>Dela rapporter offentligt</b>och <b>Dela hela systemet</b>.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Visa inbyggda rapporter</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela rapporter offentligt (externt)</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> (standardval)<p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera någon av följande åtgärder. Båda är aktiverade som standard:</p> 
      <ul> 
       <li> <p>Visa inbyggda rapporter</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b> (standardval)<p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera någon av följande åtgärder. Endast alternativet Dela är aktiverat som standard.</p> 
      <ul> 
       <li> <p>Visa inbyggda rapporter</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b> (standardval): Tillåter skrivskyddad åtkomst till rapporter, instrumentpaneler och kalendrar som har delats med dem.</p> <p>Om du vill finjustera detta kan du konfigurera möjligheten att visa inbyggda rapporter. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera <b>Visa inbyggt</b>(inaktiverat som standard).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till rapporter, instrumentpaneler och kalendrar är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filter, vyer och grupperingar

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för filter, vyer och grupperingar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b></p><p>Du kan finjustera detta genom att konfigurera möjligheten att dela filter, vyer och grupperingar. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till filter, vyer och grupperingar.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b></p><p>Du kan finjustera detta genom att konfigurera möjligheten att dela filter, vyer och grupperingar. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till filter, vyer och grupperingar.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela filter, vyer och grupperingar. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till filter, vyer och grupperingar.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b>:</p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela filter, vyer och grupperingar. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till filter, vyer och grupperingar.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Det går inte att komma åt filter, vyer och grupperingar. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dokument

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för dokument:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela dokument. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till dokument.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard utom <b>Dela dokument offentligt</b> och <b>Dela hela systemet</b>.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela dokument offentligt (externt)</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b></p><p>Du kan finjustera detta genom att konfigurera möjligheten att dela dokument. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till dokument.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard utom <b>Dela dokument offentligt</b> och <b>Dela hela systemet</b>.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela dokument offentligt (externt)</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela dokument. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till dokument.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera någon av följande åtgärder. Alla är aktiverade som standard utom de två sista, <b>Dela dokument offentligt</b> och <b>Dela hela systemet</b>.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela dokument offentligt (externt)</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b></p><p>Du kan finjustera detta genom att konfigurera möjligheten att dela dokument. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till dokument.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till dokument kan inte konfigureras på den här åtkomstnivån. Men externa användare kan använda Workfront för att visa, granska och ladda ned dokument.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Användare

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för användare:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b></p><p>Du kan finjustera detta genom att konfigurera möjligheten att visa användarnas kontaktinformation. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera <b>Visa kontaktinformation</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger användare fullständig redigeringsåtkomst.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera någon av följande åtgärder. Bara de två första alternativen <b>Skapa</b> och <b>Ta bort</b>, är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li>Användaradministratör (alla användare)</li> 
       <li> <p>Användaradministratör (gruppanvändare)</p> </li> 
      </ul> <p>Mer information om de två alternativen för användaradministratörer finns i avsnittet <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Konfigurera användaråtkomst för att redigera användare med en anpassad åtkomstnivå</a> i artikeln <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li><p> <b>Visa</b> (endast alternativ tillgängligt)</p><p>Du kan finjustera detta genom att konfigurera möjligheten att visa användarnas kontaktinformation. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera <b>Visa kontaktinformation</b> (aktiverat som standard).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li><p> <b>Visa</b> (endast alternativ tillgängligt)</p> <p>Du kan finjustera detta genom att konfigurera möjligheten att visa användarnas kontaktinformation. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan aktivera eller inaktivera <b>Visa kontaktinformation</b> (inaktiverat som standard).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b> (endast alternativ tillgängligt)</p><p>Du kan finjustera detta genom att konfigurera möjligheten att visa användarnas kontaktinformation. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan aktivera eller inaktivera <b>Visa kontaktinformation</b> (inaktiverat som standard).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till användare är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Team

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för team:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li><b>Visa</b> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Båda är inaktiverade som standard.</p> 
      <ul> 
       <li>Visa alla team</li> 
       <li> <p>Visa team som är associerade med mina grupper</p> </li> 
      </ul> </li> 
     <li> <p><b>Redigera</b> (standardval): Tillåter fullständig redigeringsåtkomst till team.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Alla är aktiverade som standard, förutom <b>Redigera team som jag är på</b>.</p> 
      <ul> 
       <li>Skapa</li> 
       <li>Ta bort</li> 
       <li> <p>Redigera team som jag är på</p> </li> 
       <li> <p>Redigera team i grupper som jag hanterar (endast gruppadministratörer)</p> </li> 
       <li> <p>Visa alla team</p> </li> 
       <li> <p>Visa team som är associerade med mina grupper</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <b>Visa</b>
      <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Båda är aktiverade som standard.</p> 
      <ul> 
       <li>Visa alla team</li> 
       <li> <p>Visa team som är associerade med mina grupper</p> </li> 
      </ul> </li> 
     <li> <p><b>Redigera</b> (standardval): Tillåter fullständig redigeringsåtkomst till team.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Bara det första alternativet, <b>Redigera team som jag är på</b>, är inaktiverat som standard.</p> 
      <ul> 
       <li> <p>Redigera team som jag är på</p> </li> 
       <li> <p>Visa alla team</p> </li> 
       <li> <p>Visa team som är associerade med mina grupper</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b> (endast alternativ tillgängligt)</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Båda är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Visa alla team</p> </li> 
       <li>Visa team som är associerade med mina grupper</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <p><b>Visa</b> (endast alternativ tillgängligt)</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Båda är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Visa alla team</p> </li> 
       <li>Visa team som är associerade med mina grupper</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Det finns ingen åtkomst till team. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Mallar

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för mallar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li><p> <b>Visa</b></p> <p>Du kan finjustera detta genom att konfigurera möjligheten att dela mallar. Klicka på kugghjulsikonen <img src="assets/gear-icon-in-access-levels.png"> på knappen Visa och sedan inaktivera eller aktivera <b>Dela</b> (aktiverat som standard).</p> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till mallar.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Alla är aktiverade som standard.</p> 
      <ul> 
       <li> <p>Skapa</p> </li> 
       <li> <p>Ta bort</p> </li> 
       <li> <p>Dela</p> </li> 
       <li> <p>Dela hela systemet</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <p><b>Ingen åtkomst</b> (endast alternativ tillgängligt)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <p><b>Ingen åtkomst</b> (endast alternativ tillgängligt)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <p><b>Ingen åtkomst</b> (endast alternativ tillgängligt)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Det går inte att komma åt mallar. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Finansiella uppgifter

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för ekonomiska data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <p><b>Visa</b>:</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Båda är aktiverade som standard.</p> 
      <ul> 
       <li>Visa fakturering och kostnadstariffer för roller</li> 
       <li> <p>Visa fakturering och kostnadstariffer för användare</p> </li> 
      </ul> </li> 
     <li> <p><b>Redigera</b> (standardval): Ger fullständig redigeringsåtkomst till ekonomiska data.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Visa</b> och sedan inaktivera eller aktivera något av följande alternativ*. Bara de två sista alternativen, <b>Visa fakturering och kostnadstariffer för roller</b> och <b>Visa fakturering och kostnadstariffer för användare</b>, är aktiverade som standard.</p> 
      <ul> 
       <li>Redigera rollfakturering och kostnadstariffer</li> 
       <li> <p>Redigera fakturering och kostnadstariffer för användare</p> </li> 
       <li>Visa fakturering och kostnadstariffer för roller</li> 
       <li> <p>Visa fakturering och kostnadstariffer för användare</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li> <p><b>Ingen åtkomst</b> (standardval)</p> </li> 
     <li> <b>Visa</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <p><b>Ingen åtkomst</b> (standardval)</p> </li> 
     <li><b>Visa</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <p><b>Ingen åtkomst</b> (endast alternativ tillgängligt)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst till ekonomiska data är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Mer information om de här alternativen finns i [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Resurshantering

I varje äldre åtkomstnivå kan du konfigurera följande alternativ för Resurshantering:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtkomstnivå</th> 
   <th>Alternativ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planering </td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> </li> 
     <li> <p><b>Redigera</b> (standardval): Tillåter fullständig redigeringsåtkomst till resurshantering.</p> <p>Klicka på kugghjulsikonen för att finjustera detta <img src="assets/gear-icon-in-access-levels.png"> på <b>Redigera</b> och sedan inaktivera eller aktivera något av följande alternativ. Bara det första alternativet, <b>Redigera prioriteringar och budgettimmar i planeraren</b>, är aktiverat som standard.</p> 
      <ul> 
       <li> <p> Redigera prioriteringar och budgettimmar i planeraren</p> </li> 
       <li> <p>Hantera resurspooler</p> <p><b>ANMÄRKNING</b>: För att kunna hantera resurspooler behöver en användare ytterligare åtkomst till ekonomiska data och behörigheter för projektekonomi. Om du ger en planeringsanvändare åtkomst till resurshantering som inte har tillgång till ekonomiska data, kan användaren fortfarande se allokeringarna per timme i resursplaneraren, men inte växla till kostnadsvyn eller visa affärsärendet. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till finansiella uppgifter</a> och <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Dela ekonomiska behörigheter för ett objekt</a>.</p> </li> 
       <li> <p>Uppdatera planerade timmar i arbetsbelastningsutjämnaren</p> <p><b>ANMÄRKNING</b>: För att kunna uppdatera planerade timmar i Utjämning av arbetsbelastning måste användaren ha behörighet att bidra till objektet, med Aktivera tilldelningar under Avancerade inställningar. Mer information finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbetare </td> 
   <td> 
    <ul> 
     <li><b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Granskare</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> </li> 
     <li> <b>Visa</b> (standardval)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Begärande</td> 
   <td> 
    <ul> 
     <li> <b>Ingen åtkomst</b> (endast alternativ tillgängligt) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Extern användare</td> 
   <td> <p>Åtkomst är inte tillgänglig. Externa användare kan bara använda Workfront för att granska och ladda ned dokument och för att se kalendrar som delas med dem.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Område för scenarioplanering

Standardinställningen för alla äldre åtkomstnivåer är Ingen åtkomst. En Workfront-administratör kan ändra detta för att visa eller redigera åtkomst för alla åtkomstnivåer för planerare, arbetare och granskare.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Användare kan visa en plan som en annan användare har skapat endast om en länk till planen delas med dem.

## Workfront målområde

Alla sex av standardnivåerna för äldre åtkomst (och alla fyra av licenstyperna) kan redigera och visa Workfront-mål.

Redigera är standardalternativet.

---
navigation-topic: get-started-with-workfront
title: Filtrera och gruppera ditt arbete med prioritet
description: Du kan använda filter för att hitta det arbete du söker och sedan använda en gruppering för att ordna det.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 8eb9dcaf-bba3-466d-b06d-5383991bc4ea
source-git-commit: b886284eb44c2154987019655ff07cdeb0e1ae22
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Filtrera och gruppera ditt arbete med prioritet

Du kan använda filter för att hitta det du söker efter och sedan använda en gruppering för att ordna det.

Prioriteter visar arbetsuppgifter som tilldelats dig. Du kan inte se arbetsobjekt som tilldelats ditt team i listan Prioriteter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> 
   <p>Aktuell: Begäran eller senare</p>
   <p>Nytt: Medarbetare eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Visa eller redigera åtkomst för objektet som uppdateringen är aktiverad för</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till objektet</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrera arbetet med standardfilter

Du kan filtrera uppgifter och ärenden som tilldelats dig.

{{step1-to-priorities}}

1. Klicka på **Filter** i det övre vänstra hörnet i arbetslistan.
1. I avsnittet **Standardfilter** väljer du ett eller flera filter för att begränsa dina arbetsobjekt.
   ![Filter](assets/filter-new.png)

+++Expandera om du vill se detaljerad information om tillgängliga filter
<table>
  <tbody>
   <tr>
   <th>Filter</th>
   <th>Beskrivning</th>
   </tr>
    <tr>
      <td>Att arbeta med den</td>
      <td>Visar objekt som du arbetar med</td>
    </tr>
    <tr>
      <td>Klar att börja</td>
      <td>Visar objekt med 
      <ul>
      <li>Inga ofullständiga föregångare eller aktivitetsbegränsningar</li>
      <p>och</p>
      <li>Det planerade startdatumet har passerat eller är upp till två veckor i framtiden</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Inte klar</td>
      <td>Visar objekt som har
       <ul>
      <li>Ofullständiga föregående aktiviteter eller aktivitetsbegränsningar som förhindrar att objektet bearbetas</li></ul>
      <p>eller</p>
      <ul>
      <li>Det planerade startdatumet är mer än två veckor i framtiden</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Begärd</td>
      <td>Visar problem som du inte har börjat arbeta med</td>
    </tr>
      <td>Klar</td>
      <td>Visar det arbete som utförts de senaste två veckorna. Det här filteralternativet inkluderar inte godkännanden.</td>
    </tr>
    <tr>
    <td>Projekt</td>
    <td>Visar projekt som innehåller uppgifter eller ärenden som du har tilldelats</td>
    </tr>
    <tr>
    <td>Förfallodatum</td>
    <td>Visar arbete efter planerat slutförandedatum</td>
    </tr>
    <tr>
    <td>Mitt fokus</td>
    <td>Visar uppgifter eller problem som har tilldelats fokusnivåer. Fokusnivåer tilldelas och hanteras av den enskilda användaren.</td>
    </tr>
    <tr>
    <td>Status</td>
    <td>Visar uppgifter eller problem i nya, pågående och slutförda statusar.</td>
    </tr>
  </tbody>
</table>

+++

1. (Valfritt) Klicka på **Tillbaka till standard** om du vill återställa markeringen.

## Filtrera arbetet med smarta filter

Använd naturligt språk för att snabbt filtrera arbetet.

>[!NOTE]
>
>Den här funktionen är endast tillgänglig för kunder som har en enhetlig Adobe Experience med hjälp av AI Assistant. Mer information om AI Assistant finns i [Översikt över AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

{{step1-to-priorities}}

1. Klicka på **Filter** i det övre vänstra hörnet i arbetslistan.
1. Klicka på **Smarta filter**.
1. Skriv hur du vill filtrera materialet.

   Du kan skriva saker som:

   * *Visa mig sena uppgifter*
   * *Visa mina topprioriteringar*
   * *Visa arbete som förfaller idag*

## Gruppera ditt arbete

{{step1-to-priorities}}

1. Klicka på **Grupper** längst upp till vänster i arbetslistan.
1. Välj en grupp för att ordna din arbetslista.
   ![Grupper](assets/groups-new.png)

+++Expandera om du vill visa detaljerad information om tillgängliga grupper

| Grupp | Beskrivning |
|-----------|-------------|
| Projekt | Detta grupperar objekt efter projekt. |
| Förfallodatum | Detta grupperar objekt baserat på när de förfaller. Förfallodatum avgörs av planerat slutförandedatum. |
| Mitt fokus | Detta grupperar objekt baserat på den fokusnivå som du tilldelar. |
| Status | Detta grupperar objekt efter följande statusar: Nytt, Pågår, Fullständigt. <br><b>Obs!</b>: Du kan inte använda anpassade statusvärden i prioriteter just nu. |

+++

### Dra och släpp arbetsobjekt vid gruppering efter Min prioritet eller Status

Du kan dra och släppa enskilda arbetsobjekt mellan kategorier när du grupperar efter Min prioritet eller Status.

1. Gruppera ditt arbete efter **status** eller **Min prioritet**.
2. Håll markören över arbetsobjektet för att klicka på ikonen **Dra** och flytta det till önskad kategori.
   ![dra-ikon](assets/drag-and-drop.png)

## Sortera materialet

### Sortera i grupper

Om du vill sortera ditt arbete i en grupp öppnar du **Grupp** och väljer om du vill sortera i stigande eller fallande ordning.

![Sortera i grupper](assets/sort-in-groups.png)

### Sortera kolumner

Om du vill sortera enskilda kolumner går du till kolumnen och klickar på nedpilen.

![nedpil i kolumn](assets/sort-columns.png)

### Expandera eller komprimera alla gruppavsnitt

Om du vill expandera eller komprimera alla gruppavsnitt öppnar du **Grupp** och klickar på **Expandera alla** eller **Komprimera alla**.

![Expandera eller komprimera grupper](assets/expand-collapse-groups.png)

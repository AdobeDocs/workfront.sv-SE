---
navigation-topic: get-started-with-workfront
title: Filtrera och gruppera ditt arbete med prioritet
description: Du kan använda filter för att hitta det arbete du söker och sedan använda en gruppering för att ordna det.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 75396c3f066abc6070ae2a89c2ded0255dbc0751
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# Filtrera och gruppera ditt arbete med prioritet

Du kan använda filter för att hitta det du söker efter och sedan använda en gruppering för att ordna det.

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

## Filtrera ditt arbete

Du kan filtrera uppgifter och ärenden som tilldelats dig.

{{step1-to-priorities}}

1. Klicka på **Filter** längst upp till höger i arbetslistan.
1. Markera ett eller flera filter om du vill begränsa arbetsobjekten.
   ![](assets/filters.png)

+++Expandera för att se detaljerad information om tillgängliga filter
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
      <li>Ofullständiga föregående aktiviteter eller aktivitetsbegränsningar som förhindrar att objektet bearbetas</li>
      <p>eller</p>
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
    <td>Status</td>
    <td>Visar uppgifter eller problem i nya, pågående och slutförda statusar</td>
    </tr>
    <tr>
    <td>Mitt fokus</td>
    <td>Visar aktiviteter eller problem med tilldelade fokusnivåer. Fokusnivåer tilldelas och hanteras av den enskilda användaren.</td>
    </tr>
  </tbody>
</table>

+++

1. (Valfritt) Klicka på **Tillbaka till standard** om du vill återställa markeringen.

## Gruppera ditt arbete

{{step1-to-priorities}}

1. Klicka på **Grupper** överst till höger i arbetslistan.
1. Välj en grupp för att ordna din arbetslista
   ![](assets/groups.png)

+++Expandera för att se detaljerad information om tillgängliga grupper

| Grupp | Beskrivning |
|-----------|-------------|
| Ingen | Detta tar bort grupperingar från arbetslistan. |
| Mitt fokus | Detta grupperar objekt baserat på den fokusnivå som du tilldelar. |
| Vecka förfaller | Den här gruppen objekt baserat på vilken vecka de förfaller. Förfallodatum avgörs av planerat slutförandedatum. |
| Status | Detta grupperar objekt efter följande statusar: Nytt, Pågår, Fullständigt. <br>Obs! Du kan inte använda anpassade statusvärden i prioriteter just nu. |
| Projekt | Detta grupperar objekt efter projekt. |

+++

## Sortera materialet

Om du vill sortera ditt arbete öppnar du **Gruppera** och klickar på **Sortera stigande** eller **Sortera fallande**.

![](assets/expand-sort-groups.png)

>[!IMPORTANT]
>
>Sorteringsalternativet är inte tillgängligt för tillfället om du har använt en grupp.



## Expandera eller komprimera alla avsnitt

Om du vill expandera eller komprimera alla avsnitt öppnar du **Grupp** och klickar på **Expandera alla** eller **Komprimera alla**.

![](assets/expand-sort-groups.png)



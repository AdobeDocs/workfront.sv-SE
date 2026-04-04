---
navigation-topic: get-started-with-workfront
title: Hantera ditt arbete i Prioritetskalendern
description: Spåra arbetet med en tydlig, visuell kalender.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: d24ad7d1-3a88-479e-beaf-69f8264c9a6b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Hantera ditt arbete i Prioritetskalendern

Håll ordning på ditt material med en tydlig, visuell kalender. Med Prioritetskalendern kan du

* Använd filter för att hitta ditt material
* Använd anpassade fält som status och fokusnivå för att identifiera högprioriterat arbete
* Använd färger för snabb sortering

>[!IMPORTANT]
>
>Projekt måste ha statusen Aktuell eller en status som är lika med aktuell för att kunna visa projekt samt deras underordnade uppgifter och ärenden.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Reviewer or higher</p>
   <p>Light or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller redigera åtkomst för objektet som uppdateringen är aktiverad för</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till objektet</p></td> 
  </tr> 
 </tbody> 
</table>

[](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)

+++

## View your work in the calendar

Prioriteter visar arbetsuppgifter som tilldelats dig. Det går inte att se arbetsobjekt som tilldelats ditt team i prioriteringskalendern.

{{step1-to-priorities}}

1. Klicka på ikonen **Kalender** längst upp i arbetslistan.
   ![kalenderikon](assets/calendar-tab.png)
1. Markera ett eller flera filter om du vill begränsa arbetsobjekten.

   +++Expandera om du vill se detaljerad information om tillgängliga filter
   <table>
    <tbody>
    <tr>
    <th>Filter</th>
    <th>Beskrivning</th>
    </tr>
        <tr>
        <td>Att arbeta med den</td>
        <td>Visar objekt som du arbetar med.</td>
        </tr>
        <tr>
        <td>Klar att börja</td>
        <td>Displays items with 
        <ul>
        <li>No incomplete predecessors or task constraints</li>
        <p>and</p>
        <li>The Planned Start Date is in the past or up to two weeks in the future</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Not ready</td>
        <td>Displays items that have
        <ul>
        <li>Ofullständiga föregående aktiviteter eller aktivitetsbegränsningar som förhindrar att objektet bearbetas</li>
        <p>or</p>
        <li>The Planned Start Date more than two weeks in the future.</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Requested</td>
        <td>Displays issues that you have not started work on.</td>
        </tr>
        <td>Klar</td>
        <td>Visar det arbete som utförts de senaste två veckorna. Det här filteralternativet inkluderar inte godkännanden.</td>
        </tr>
        <tr>
        <td>Projekt</td>
        <td>Visar projekt som innehåller uppgifter eller ärenden som du har tilldelats.</td>
        </tr>
        <tr>
        <td>Förfallodatum</td>
        <td>Visar arbetet efter planerat slutförandedatum.</td>
        </tr>
        <tr>
        <td>Status</td>
        <td>Displays tasks or issues in new, in progress, and complete statuses.</td>
        </tr>
        <tr>
        <td>My Focus</td>
        <td>Displays tasks or issues in that have assigned focus levels. Focus levels are assigned and managed by the individual user.</td>
        </tr>
    </tbody>
    </table>

   +++

1. Klicka på arbetsobjektsfältet i kalendern för att öppna sidsammanfattningen. Med sidsammanfattningen kan du

   * Visa och redigera information om projekt och arbetsuppgift
   * Göra och visa kommentarer
   * Visa och överföra dokument
   * Create a proof
   * Navigera till projektsidan i Workfront
   * Navigera till sidan med information om arbetsobjekt i Prioriteringar
   * Loggtid
   * Lägga till snabblänkar

1. (Valfritt) Klicka på **Skapa ny** om du vill lägga till en ny arbetsuppgift i kalendern. Mer information finns i [Skapa en ny uppgift eller ett nytt problem i Prioriteter](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md).

## Konfigurera kalendern

{{step1-to-priorities}}

1. Klicka på ikonen **Kalender** längst upp i arbetslistan.
   ![kalenderikon](assets/calendar-tab.png)
1. Klicka på ikonen **Inställningar** i kalenderns högra hörn.

1. På fliken **Stapelstil** väljer du upp till 5 fält som ska visas i arbetsobjektsfältet i kalendern.
   ![exempelfält](assets/sample-task-for-field-config.png)

1. **** ****
   ![](assets/sample-calendar-projects.png)

---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Skapa personliga uppgifter
description: Personliga uppgifter är tillfälliga arbetsförfrågningar som du skickar till en användare, till dig själv eller att göra-uppgifter som du skapar själv i hemområdet. Workfront sparar tillfälliga arbetsförfrågningar och gör objekt som personliga uppgifter.
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: a1081b7ce0877b08f9546ab57cfac3f2a580ea76
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Skapa personliga uppgifter

<!--Audited: 10/2024-->

Personliga uppgifter är tillfälliga arbetsförfrågningar som du skickar till en användare eller skickar till eller lägger till själv.

Adobe Workfront sparar tillfälliga arbetsförfrågningar och gör saker som personliga uppgifter i ett användarprojekt som Wprfront automatiskt skapar för varje användare.

Följande är egenskaper för en användares personliga projekt:

* Alla användare i Workfront har ett personligt projekt som heter &quot;&lt; Användarens fullständiga namn>&#39;s Tasks&quot;. Exempel: &quot;Svensson Svensson&#39;s Tasks&quot;.
* Det personliga projektet för varje användare visas inte i sökningar och är dolt.
* Ett personligt projekt kan inte tas bort, även om användare har inaktiverats.
* Status för ett personligt projekt är alltid Aktuell. Personliga projekt kan inte slutföras eller avbrytas.
* Alla personliga uppgifter lagras i en användares personliga projekt.
* Du kan flytta personliga uppgifter till ett annat projekt om det behövs.

Du kan skapa personliga uppgifter på följande sätt:

* Skapa en att göra-uppgift i hemområdet

  Mer information finns i [Skapa arbetsobjekt och projekt från startdelen](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Skapa och skicka en personlig arbetsförfrågan till en annan användare från användarprofilsidan
* Skapa och skicka en personlig arbetsförfrågan till dig själv från din profilsida

I den här artikeln beskrivs hur du kan skapa en personlig arbetsförfrågan för en användare eller för dig själv från sidan med användarprofiler.

Oavsett hur du lägger till en personlig uppgift kan du hitta den i samma delar av Workfront. Mer information finns i avsnittet [Leta reda på personlig uppgift](#locate-personal-tasks) i den här artikeln.

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
   <p>Nytt: Standard för att skicka begäranden till andra användare. Alla användare kan skapa egna arbetsförfrågningar.</p> 
   <p>Aktuell: Planerar att skicka begäranden till andra användare. Alla användare kan skapa egna arbetsförfrågningar.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Redigera åtkomsten till Användare för att skapa en arbetsbegäran för dem. Visa åtkomst för att skapa en personlig arbetsförfrågan för dig själv. </p>
   </td> 
  </tr>

</tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Skapa en personlig arbetsförfrågan

1. Gå till din användares profilsida eller gå till en annan användares profilsida som du har tillgång till för att visa.

   >[!TIP]
   >
   >Din Workfront-administratör kan hindra dig från att se vissa användare när de konfigurerar din åtkomstnivå.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om användarens namn i sidhuvudet.
1. Klicka på **Skicka arbetsförfrågan**.
Rutan **Skicka en arbetsförfrågan** till användaren visas.

   ![](assets/personal-task-box.png)
1. Uppdatera följande information:

   * **Aktivitetsnamn**: Detta är namnet på ad hoc-arbetsbegäran eller den personliga aktiviteten.
   * **Beskrivning**: Lägg till en beskrivning för aktiviteten.
   * **Tilldela till**: Namnet på användaren som du valde visas som standard. Du kan lägga till fler användare eller team.
   * **Förfallodatum**: Detta är det datum då du vill att den här aktiviteten ska slutföras. Som standard är detta dagens datum. Du kan inte välja ett tidigare datum
   * **Tid**: Detta är den tidpunkt då du vill att den här aktiviteten ska slutföras. Som standard är detta den aktuella tiden.

1. Klicka på **Skicka begäran** för att spara arbetsbegäran.

   Arbetsbegäran sparas som en personlig uppgift i Workfront och läggs till i användarens Att göra-widget i hemområdet. Om du skickar en arbetsförfrågan till dig själv visas den i din Att göra-widget i Hem.


## Hitta personliga uppgifter

Du kan hitta personliga uppgifter i följande områden:

* The To-dos widget in the Home area of the user the personal request was sent to.

  Mer information finns i [Skapa arbetsobjekt och projekt från startdelen](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* En personlig uppgiftsrapport eller -lista. Du kan skapa och använda ett personligt uppgiftsfilter på en aktivitetsrapport eller -lista om du bara vill visa personliga uppgifter och exkludera projektuppgifter.

  Mer information finns i [Filtrera: personliga uppgifter](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).

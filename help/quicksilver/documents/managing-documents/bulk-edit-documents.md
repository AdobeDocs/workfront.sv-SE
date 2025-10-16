---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Redigera flera dokument samtidigt
description: Du kan redigera flera dokument samtidigt i området Dokument.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Redigera flera dokument samtidigt

Du kan redigera beskrivningen, lägga till anpassade formulär och redigera anpassade formulär i flera dokument samtidigt.

## Att tänka på när du redigerar anpassade formulär

Tänk på följande när du redigerar flera anpassade formulär samtidigt:

* Informationen som du ändrar i alla markerade dokument skriver över befintlig information om enskilda dokument.
* När du markerar dokument som har olika värden för samma fält visas indikatorn &quot;Flera värden&quot; i fältet. Fält som är kryssrutor, alternativknappar och växlar har en &quot;Multiple values&quot;-indikator bredvid sig.
* När du uppdaterar ett alternativ i ett fält med flera alternativ (t.ex. ett fält som visas som en uppsättning av växlar eller kryssrutor) måste alla andra alternativ matcha de markerade dokumenten.

>[!BEGINSHADEBOX]

**Exempel**
Det kan finnas ett anpassat formulär med ett kryssrutefält med tre kryssrutor (alternativ1, alternativ 2 och alternativ 3) och alternativ 1 är avmarkerat för alla markerade dokument, och alternativ 2 och 3 är markerade för vissa och avmarkerade för andra dokument som du har valt. Om du vill markera Alternativ 1 för alla dokument måste du också göra alternativ 2 och 3 matchande för alla markerade projekt innan du kan spara ändringarna. Därför måste du antingen markera dem eller avmarkera dem så att de matchar alla markerade projekt. Om du inte ändrar något av alternativen kan du spara fältet som det är och dokumenten behåller sin aktuella markering för alla alternativ.

>[!ENDSHADEBOX]

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td><p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till dokumentet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera flera dokument samtidigt

Så här redigerar du flera dokument:

1. Navigera till fliken Dokument i ett projekt eller till området Dokument på huvudmenyn.
1. Tryck på Ctrl eller Cmd på tangentbordet och markera de dokument som du vill redigera.
1. Klicka på ikonen Redigera ![redigera](assets/edit-icon.png).
   ![redigera ikonens plats på sidan](assets/edit-multiple-documents.png)
1. (Valfritt) Lägg till eller redigera **beskrivningen**. Om beskrivningen för varje dokument är annorlunda visas _Flera värden_ i beskrivningsrutan. Du kan lägga till samma beskrivning för alla dokument, men du kan inte redigera enskilda dokumentbeskrivningar när du redigerar flera.
1. Gör följande ändringar med anpassade formulär:

   <table>
    <tr>
    <td><strong>Lägg till formulär</strong></td>
    <td>I rutan <strong>Lägg till anpassat formulär</strong> kan du välja mellan bifogade formulär och formulär som ska läggas till. Bifogade formulär finns i vissa av de markerade dokumenten, men inte i alla. Ett formulär som bifogas till alla markerade dokument visas automatiskt i redigeringsfönstret.  </td>
    </tr>
    <tr>
    <td><strong>Redigera formulär</strong></td>
    <td>Redigera eventuella kopplade anpassade formulär. Den information du ändrar skriver över befintlig information om enskilda dokument. Fält med olika värden i olika dokument visas som"Flera värden". </td>
    </tr>
    <tr>
    <td><strong>Ordna om formulär</strong></td>
    <td>Klicka och dra det anpassade formuläret för att ordna om det.</td>
    </tr>
    </table>
1. Klicka på **Spara**.


## Redigera flera dokument samtidigt i en dokumentrapport

1. Navigera till en befintlig dokumentrapport.
eller
Skapa en dokumentrapport enligt beskrivningen i [Skapa en anpassad rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Markera de dokument som du vill redigera.
1. Klicka på ikonen Redigera ![redigera](assets/edit-icon.png).
   ![redigera ikonens plats på sidan](assets/edit-multiple-documents.png)
1. (Valfritt) Lägg till eller redigera **beskrivningen**. Om beskrivningen för varje dokument är annorlunda visas _Flera värden_ i beskrivningsrutan. Du kan lägga till samma beskrivning för alla dokument, men du kan inte redigera enskilda dokumentbeskrivningar när du redigerar flera.
1. Gör följande ändringar med anpassade formulär:

   <table>
    <tr>
    <td><strong>Lägg till formulär</strong></td>
    <td>I rutan <strong>Lägg till anpassat formulär</strong> kan du välja mellan bifogade formulär och formulär som ska läggas till. Bifogade formulär finns i vissa av de markerade dokumenten, men inte i alla. Ett formulär som bifogas till alla markerade dokument visas automatiskt i redigeringsfönstret.  </td>
    </tr>
    <tr>
    <td><strong>Redigera formulär</strong></td>
    <td>Redigera eventuella kopplade anpassade formulär. Den information du ändrar skriver över befintlig information om enskilda dokument. Fält med olika värden i olika dokument visas som"Flera värden". </td>
    </tr>
    <tr>
    <td><strong>Ordna om formulär</strong></td>
    <td>Klicka och dra det anpassade formuläret för att ordna om det.</td>
    </tr>
    </table>
1. Klicka på **Spara**.

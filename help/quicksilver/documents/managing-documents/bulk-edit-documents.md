---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Redigera flera dokument samtidigt
description: Du kan redigera flera dokument samtidigt i området Dokument.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c1f829eb29d8cd13524814d98ed353add15e881
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---


# Redigera flera dokument samtidigt

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

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

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td><p> Nytt: Medarbetare eller högre</p> 
   <p> Aktuell: Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till dokumentet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

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



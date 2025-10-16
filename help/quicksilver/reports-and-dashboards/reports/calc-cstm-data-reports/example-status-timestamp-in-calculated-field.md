---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Exempel på beräknat anpassat fält: visa en tidsstämpel för status i ett anpassat formulär'
description: I följande beräkningsfält visas det datum då objektets status markeras som Pågår (INP). Du kan använda samma information för beräknade anpassade fält för utgåvor, uppgifter eller projekt.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Exempel på beräknat anpassat fält: visa en statustidsstämpel i ett anpassat formulär

I följande beräkningsfält visas det datum då objektets status markeras som Pågår (INP). Du kan använda samma information för beräknade anpassade fält för utgåvor, uppgifter eller projekt.

>[!NOTE]
>
>Om objektets status ändras till INP, ändras den till en annan status och sedan tillbaka till INP, hämtar Adobe Workfront bara tidsstämpeln från den första ändringen till INP.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront package</p> </td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licens</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Konfigurationer på åtkomstnivå</p></td> 
   <td> <p>Redigera åtkomst till Skapa rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektbehörigheter</p> </td> 
   <td> <p>Hantera behörigheter för objektet som formuläret är kopplat till</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättning

Om du vill lägga till ett beräknat fält som visar ett fälts redigeringshistorik i ett anpassat formulär måste du först skapa det anpassade formuläret.

## Visa en tidsstämpel för status i ett anpassat formulär

1. Gå till ett anpassat formulär där du vill lägga till fältet.
1. Klicka på **Beräknat** för att lägga till ett beräknat anpassat fält i formuläret.
1. Ange en **etikett** för det anpassade fältet. Exempel: &quot;Status för tidsstämpelfält&quot;.
1. Klicka på **Spara+Stäng**.
1. Öppna det anpassade formuläret igen och välj sedan det nya **statustidsstämpelsfältet** i formuläret.
1. Kopiera och klistra in följande beräkning för det anpassade fältet i rutan **Beräkning**:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Den här beräkningen är identisk för alla objekt och för alla statusvärden. Du måste alltid använda tangenten med tre bokstäver och inte statusnamnet för objektstatusen i den här beräkningen.
   >
   >Mer information om nycklarna för status finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicka på **Spara+Stäng**.

   Du kan nu rapportera om det anpassade statustidsstämpelfältet eller använda det i andra beräkningar, i rapporter eller i anpassade fält.

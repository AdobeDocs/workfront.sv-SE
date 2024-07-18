---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Exempel på beräknat anpassat fält: visa en statustidsstämpel i ett anpassat formulär'
description: I följande beräkningsfält visas det datum då objektets status markeras som Pågår (INP). Du kan använda samma information för beräknade anpassade fält för utgåvor, uppgifter eller projekt.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Exempel på beräknat anpassat fält: visa en statustidsstämpel i ett anpassat formulär

I följande beräkningsfält visas det datum då objektets status markeras som Pågår (INP). Du kan använda samma information för beräknade anpassade fält för utgåvor, uppgifter eller projekt.

>[!NOTE]
>
>Om objektets status ändras till INP, ändras den till en annan status och sedan tillbaka till INP, hämtar Adobe Workfront bara tidsstämpeln från den första ändringen till INP.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licens*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Åtkomstnivåkonfigurationer*</strong> </td> 
   <td> <p>Redigera åtkomst till Skapa rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>Hantera behörigheter för objektet som formuläret är kopplat till</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.<br>Mer information om behörigheter för instrumentpaneler finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Dela rapporter, instrumentpaneler och kalendrar </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättning

Om du vill lägga till ett beräknat fält som visar ett fälts redigeringshistorik i ett anpassat formulär måste du först skapa det anpassade formuläret.

## Visa en tidsstämpel för status i ett anpassat formulär

1. Gå till ett anpassat formulär där du vill lägga till fältet.
1. Klicka på **Beräknat** för att lägga till ett beräknat anpassat fält i formuläret.
1. Ange en **etikett** för det anpassade fältet, till exempel *Anpassat fält för tidsstämpel för status*.
1. Klicka på **Klar** och sedan på **Spara+stäng**.
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

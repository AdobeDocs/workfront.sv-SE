---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: Ogiltig parameter: konverteringsvärde'
description: '"Du får följande felmeddelande när du försöker ändra formatet för ett anpassat fält i ett befintligt anpassat formulär: "Ogiltig parameter: konverteringsvärdet `&lt;..&gt;`"'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Felmeddelande: Ogiltig parameter: konverteringsvärde

## Problem

Du får följande felmeddelande när du försöker ändra formatet för ett anpassat fält i ett befintligt anpassat formulär: &quot;Ogiltig parameter: konverteringsvärdet &quot;&lt;..>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Orsak

Det här meddelandet visas i följande scenario:

Du har t.ex. ett anpassat fält som är formaterat som text.  Nu vill du ändra formatet för det anpassade fältet till Valuta. Någonstans i din Adobe Workfront-instans är det här fältet redan kopplat till ett objekt och innehåller redan angiven information. Den befintliga informationen i minst ett sådant fält är redan formaterad som text. Därför kan inte fältets format ändras till Valuta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront-plan</a>*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Licensöversikt</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Åtkomstnivå*</strong> </td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösning

Gör följande:

1. Skapa rapporter för alla objekt som kan ha det här fältet kopplat till sina anpassade Forms.\
   Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Inkludera det anpassade fält som du försöker redigera i rapportvyn, så att du kan se vilket objekt som har det här fältet ifyllt med ett textvärde.
1. Korrigera värdena för anpassade fält för de objekt som visas i ett textformat och ge dem ett värde som är formaterat som Valuta. Försök sedan att ändra fältet Format på det anpassade formuläret igen.\
   eller\
   Om du redan har för många fältvärden med textformaterad information kan du lägga till ett nytt anpassat fält i det anpassade formuläret och formatera det som valuta.

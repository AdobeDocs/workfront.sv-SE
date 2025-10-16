---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: Ogiltig parameter: Konverteringsvärde'
description: 'Du får följande felmeddelande när du försöker ändra formatet för ett anpassat fält i ett befintligt anpassat formulär: "Ogiltig parameter: konverteringsvärdet `&lt;..&gt;`"'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Felmeddelande: Ogiltig parameter: konverteringsvärde

## Problem

Du får följande felmeddelande när du försöker ändra formatet för ett anpassat fält i ett befintligt anpassat formulär: &quot;Ogiltig parameter: konverteringsvärdet &quot;&lt;..>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Orsak

Det här meddelandet visas i följande scenario:

Du har t.ex. ett anpassat fält som är formaterat som text.  Nu vill du ändra formatet för det anpassade fältet till Valuta. Någonstans i din Adobe Workfront-instans är det här fältet redan kopplat till ett objekt och innehåller redan angiven information. Den befintliga informationen i minst ett sådant fält är redan formaterad som text. Därför kan inte fältets format ändras till Valuta.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösning

Gör följande:

1. Skapa rapporter för alla objekt som kan ha det här fältet kopplat till sina anpassade Forms.\
   Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Inkludera det anpassade fält som du försöker redigera i rapportvyn, så att du kan se vilket objekt som har det här fältet ifyllt med ett textvärde.
1. Korrigera värdena för anpassade fält för de objekt som visas i ett textformat och ge dem ett värde som är formaterat som Valuta. Försök sedan att ändra fältet Format på det anpassade formuläret igen.\
   eller\
   Om du redan har för många fältvärden med textformaterad information kan du lägga till ett nytt anpassat fält i det anpassade formuläret och formatera det som valuta.

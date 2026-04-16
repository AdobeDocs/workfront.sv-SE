---
content-type: overview
product-area: projects
navigation-topic: financials
title: Åsidosätt användarens faktureringstariffer på projektnivå
description: I den här artikeln beskrivs hur du kan åsidosätta systemanvändarnas faktureringstaxor för ett projekt.
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Åsidosätt användarfakturering på projektnivå

Som projektledare kan du ange faktureringssatsen för en användare i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här användaren. Workfront använder användarens faktureringstaxa på projektnivå för att beräkna intäkten, i stället för att använda faktureringstaxan på systemnivå.

I den här artikeln beskrivs hur du kan åsidosätta systemanvändarnas faktureringstaxor för ett projekt.

Allmän information om hur du åsidosätter faktureringstariffer för projekt och beräknar projektintäkter finns i [Översikt över åsidosättande av faktureringstariffer och beräkning av intäkter för ett projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Mer information om hur du beräknar intäkter för projektet finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) och i avsnittet [Intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) i artikeln [Översikt över fakturering och intäkter](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>När det gäller Faktisk intäkt bör de faktureringstariffer som tillämpas på timmar som läggs till i en faktureringspost som är markerad som Fakturerad inte påverkas av åsidosättningar av faktureringstaxor som inträffar efter att faktureringsposten har fakturerats.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p>
       <p><p>Du måste också ha något av följande:</p> 
        <ul> 
          <li> <p>Åtkomstnivån Systemadministratör. </li> 
          <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för det projekt som innehåller Redigera ekonomiska data </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åsidosätt användarfaktureringstariffer på projektnivå

När du åsidosätter faktureringssatsen för en användare i ett projekt kan du tilldela giltighetsdatum och varje datumintervall har olika taxa. Om du inte tilldelar giltighetsdatum används den åsidosättning av faktureringssatsen som du anger för hela projektets varaktighet för att beräkna intäkten.

Så här åsidosätter du en användarfaktureringstaxa för ett projekt:

1. Gå till det projekt som du vill åsidosätta faktureringstariffer för.
1. Klicka på **Kurser** i den vänstra panelen. Du måste kanske först klicka på **Visa mer**.
1. Klicka på fliken **Fakturering** om den inte redan är markerad.
1. Klicka på **Lägg till faktureringsfrekvens** > **Ny faktureringsfrekvens för användare**.

   Rutan Ny faktureringsfrekvens för användare öppnas.

1. I fältet **Användare** väljer du den användare som du vill ändra faktureringsfrekvensen för.
1. Välj **Valuta** för åsidosättning av faktureringsfrekvens.
1. I fältet **Faktureringstakt** anger du den första åsidosättningen av faktureringstariff.
1. (Valfritt) Klicka på **Lägg till giltighetsfrekvens** om du vill lägga till fler åsidosättningar av faktureringsfrekvens.
1. (Villkorligt) Om du lägger till flera åsidosättningar av faktureringsfrekvens anger du följande information för varje rad:

   * **Faktureringsränta**: värdet på faktureringssatsen under den angivna tidsperioden.
   * **Startdatum**: det datum då åsidosättningen av faktureringstariff börjar.
   * **Slutdatum**: det datum då faktureringstariff-åsidosättningen upphör.

   ![Rutan Ny faktureringsfrekvens för användare med giltighetsdatum](assets/new-user-billing-rate-on-project2.png)

   Workfront tillämpar användarpriset för åsidosättning på de timmar som inträffar under dessa tidsramar vid beräkning av projektets intäkter.

   I Workfront kan du lämna luckor mellan åsidosättandetidsramar, men du får en varning som bekräftar att detta är avsiktligt.

   Du behöver inte ange ett startdatum för den första åsidosättningsfrekvensen eller ett slutdatum för den senaste åsidosättningsfrekvensen.

   Om du bara anger en åsidosättning av faktureringssatsen gäller den avgiften för hela projektperioden. Om du lägger till flera datumgiltiga åsidosättningar förutsätter Workfront att den första åsidosättningen gäller alla timmar före slutdatumet och att den sista åsidosättningen gäller alla timmar efter startdatumet.

   Workfront antar att den första åsidosättandefrekvensen används för alla timmar med ett datum som är äldre än slutdatumet för den första åsidosättningen och att den senaste åsidosättandefrekvensen används för alla timmar med ett datum som är senare än startdatumet för den senaste åsidosättningen.

   Om en timme loggas före projektets planerade startdatum används den första faktureringstakten.

   Om en timme loggas efter projektets planerade slutförandedatum används den sista faktureringstakten.

1. Klicka på **Spara**.

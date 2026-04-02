---
product-area: projects
navigation-topic: financials
title: Åsidosätt faktureringshastigheter för jobbroller på projektnivå
description: Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---

# Åsidosätt faktureringshastigheter för jobbroller på projektnivå

{{highlighted-preview}}

Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.

I den här artikeln beskrivs hur du kan åsidosätta faktureringstaxorna för systemjobbroller för ett projekt.

Allmän information om hur du åsidosätter faktureringssatser för jobbroller för projekt och beräknar projektintäkter finns i [Översikt över åsidosatta faktureringssatser och beräkning av intäkter för ett projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Mer information om vilken jobbroll som används för att beräkna intäkter för projektet finns i avsnittet [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) och i avsnittet [Inkomstberäkningar för aktiviteter baserade på användar- och rolltilldelningar](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td> <p>Så här åsidosätter du en faktureringsfrekvens för en jobbroll för ett projekt: Alla Workfront- eller arbetsflödespaket</p>
        <p>Så här använder du attribut för jobbrollen: Ultimate för arbetsflöde</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Administrativ åtkomst för jobbroller</p></td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för det projekt som innehåller Redigera ekonomiska data </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åsidosätt faktureringshastigheter för jobbroller på projektnivå

När du åsidosätter faktureringsfrekvensen för ett jobb i ett projekt kan du tilldela giltighetsdatum och varje datumintervall har olika hastigheter. Om du inte tilldelar giltighetsdatum används den åsidosättning av faktureringssatsen som du anger för hela projektets varaktighet för att beräkna intäkten.

Du kan lägga till nya faktureringstariffer i en projektmall och dessa blir projektfaktureringstariffer när du skapar projektet från den mallen. Mer information om hur du redigerar mallar finns i [Redigera projektmallar](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Du kan inte åsidosätta användarnas faktureringstaxor för ett projekt om du inte har Workflow Ultimate-paketet.

Så här åsidosätter du en faktureringstaxa för ett projekt:

1. Gå till det projekt som du vill åsidosätta faktureringstariffer för.
1. Klicka på **Faktureringstariffer** i den vänstra panelen.

   eller

   <span class="preview">Klicka på **Kurser** i den vänstra panelen och klicka på fliken **Fakturering** om den inte redan är markerad.</span>

1. Klicka på **Lägg till faktureringsränta** > **Ny faktureringsränta**.

   eller

   <span class="preview">Klicka på **Lägg till faktureringsfrekvens > Ny faktureringsfrekvens för jobbroll**.</span>

   Rutan Ny faktureringsränta öppnas.

1. I fältet **Jobbroll** väljer du den jobbroll du vill ändra faktureringsfrekvensen för.

1. <span class="preview">(Valfritt) Välj eventuella attribut för faktureringsfrekvensen, till exempel byrå eller plats.</span>

   <span class="preview">Systemadministratören definierar tariffattribut i inställningsområdet.</span>

1. Välj **Valuta** för åsidosättning av faktureringsfrekvens.
1. I fältet **Faktureringsgrad** anger du åsidosättning av faktureringsfrekvens och klickar sedan på **Spara** för att åsidosätta faktureringssatsen en gång

   eller

   Klicka på **Lägg till ränta** om du vill lägga till fler åsidosättningar av faktureringsfrekvens.

1. (Villkorligt) Ange följande information för varje rad om åsidosättning av gällande faktureringsränta för datum:

   * **Faktureringstakt**: Värdet för faktureringstakten från början av projektet till första datumet för den första åsidosättningen.
   * **Startdatum**: Det datum då åsidosättningen av faktureringstariff börjar.
   * **Slutdatum**: Det datum då faktureringstakten åsidosätts slutar.

   ![Faktureringstariffer med åsidosättningsdatum](assets/new-job-role-billing-rate-on-project2.png)

   Workfront tillämpar rollfrekvensen för åsidosättningsjobb på de timmar som inträffar under dessa tidsramar vid beräkning av projektets intäkter.

   I Workfront kan du lämna luckor mellan åsidosättandetidsramar, men du får en varning som bekräftar att detta är avsiktligt.

   Du behöver inte ange ett startdatum för den första åsidosättningsfrekvensen eller ett slutdatum för den senaste åsidosättningsfrekvensen.

   Om du bara anger en åsidosättning av faktureringssatsen gäller den avgiften för hela projektperioden. Om du lägger till flera datumgiltiga åsidosättningar förutsätter Workfront att den första åsidosättningen gäller alla timmar före slutdatumet och att den sista åsidosättningen gäller alla timmar efter startdatumet.

   Workfront antar att den första åsidosättandefrekvensen används för alla timmar med ett datum som är äldre än slutdatumet för den första åsidosättningen och att den senaste åsidosättandefrekvensen används för alla timmar med ett datum som är senare än startdatumet för den senaste åsidosättningen.

   Om en timme loggas före projektets planerade startdatum används den första faktureringstakten.

   Om en timme loggas efter projektets planerade slutförandedatum används den sista faktureringstakten.

1. Klicka på **Spara**.

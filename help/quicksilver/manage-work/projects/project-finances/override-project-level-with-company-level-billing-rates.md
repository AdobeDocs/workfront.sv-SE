---
product-area: projects
navigation-topic: financials
title: Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå
description: Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Du kan konfigurera ett projekt så att det använder faktureringstariffer på företagsnivå i stället för faktureringstariffer på projektnivå.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivera alternativet Åsidosätt faktureringstariffer på företagsnivå

När ett företag är associerat med ett projekt och det här alternativet är aktiverat åsidosätter ändringar av faktureringstarifferna på företagsnivå den faktureringstaxa som angetts för projektet.

När en användare manuellt beräknar om budgeten för projektet tillämpas eventuella ändringar av faktureringstarifferna på företagsnivå. Historiska intäktsberäkningar åsidosätts också såvida de inte markeras som fakturerade.

1. Gå till ett projekt.
1. Klicka på menyn **Mer** ![Mer ](assets/qs-more-icon-on-an-object.png) bredvid namnet på projektet i sidhuvudet och klicka sedan på **Redigera**.
1. I avsnittet **Ekonomi** aktiverar du alternativet **Tillåt faktureringstariffer på företagsnivå för att åsidosätta faktureringstariffer på projektnivå**.

   >[!CAUTION]
   >
   >Om du aktiverar det här alternativet åsidosätts historiska intäktsberäkningar om de inte markeras som fakturerade. Du kan bevara de historiska intäktsberäkningarna genom att skapa en faktureringspost. Mer information finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Klicka på **Spara ändringar**.

## Uppdatera faktureringspriser på företagsnivå och tillämpa dem på ett projekt

När du har aktiverat alternativet för åsidosättning av faktureringsräntor på företagsnivå för ett projekt, gäller ändringar av företagets faktureringssatser för projektet när ekonomin beräknas om.

>[!NOTE]
>
>Användare måste ha tillgång till företag på sin åtkomstnivå för att kunna uppdatera faktureringspriserna på företagsnivå.

{{step-1-to-setup}}

1. Klicka på **Företag**.
1. Klicka på namnet på det företag som är associerat med det projekt för vilket du aktiverat åsidosättning av faktureringspriser på företagsnivå.
1. Klicka på **Faktureringstariffer** i den vänstra panelen.
1. Uppdatera **Företagets faktureringsfrekvens** och start-/slutdatum för en befintlig jobbroll och tryck sedan på Retur.

   Om du vill lägga till ett nytt giltighetsdatum för företagsfaktureringstariff väljer du en faktureringsfrekvens för jobbrollen och klickar på **Redigera**. Mer information om giltighetsdatum för företagsfaktureringstariffer finns i [Åsidosätt faktureringstariffer för jobbroller på företagsnivå](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Gör något av följande om du vill uppdatera företagsräntor för ett eller flera projekt:

   * Flera projekt:

      1. Gå till en lista med projekt.
      1. Markera kryssrutan i linje med de projekt som du vill uppdatera.
      1. Klicka på **Redigera**.
      1. Aktivera alternativet **Omberäkna kostnader och intäkter** i avsnittet Inställningar.
      1. Klicka på **Spara ändringar**.

   * Ett projekt:

      1. Gå till det projekt där du aktiverade åsidosättning av faktureringstariffer på företagsnivå.
      1. Klicka på menyn **Mer** ![Mer](assets/qs-more-icon-on-an-object.png) bredvid projektnamnet i rubriken och klicka sedan på **Beräkna om ekonomi**.

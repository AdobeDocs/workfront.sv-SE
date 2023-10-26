---
product-area: projects
navigation-topic: financials
title: Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå
description: Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Du kan konfigurera ett projekt så att det använder faktureringstariffer på företagsnivå i stället för faktureringstariffer på projektnivå.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Aktivera alternativet Åsidosätt faktureringstariffer på företagsnivå

När ett företag är associerat med ett projekt och det här alternativet är aktiverat åsidosätter ändringar av faktureringstarifferna på företagsnivå den faktureringstaxa som angetts för projektet.

När en användare manuellt beräknar om budgeten för projektet tillämpas eventuella ändringar av faktureringstarifferna på företagsnivå. Historiska intäktsberäkningar åsidosätts också såvida de inte markeras som fakturerade.

1. Gå till ett projekt.
1. Klicka på **Mer** meny ![](assets/qs-more-icon-on-an-object.png) bredvid namnet på projektet i sidhuvudet och klicka sedan på **Redigera**.
1. I **Ekonomi** -sektion, aktivera **Tillåt faktureringstariffer på företagsnivå att åsidosätta faktureringstariffer på projektnivå**.

   >[!CAUTION]
   >
   >Om du aktiverar det här alternativet åsidosätts historiska intäktsberäkningar om de inte markeras som fakturerade. Du kan bevara de historiska intäktsberäkningarna genom att skapa en faktureringspost. Mer information finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Klicka **Spara ändringar**.

## Uppdatera faktureringspriser på företagsnivå och tillämpa dem på ett projekt

När du har aktiverat alternativet för åsidosättning av faktureringsräntor på företagsnivå för ett projekt, gäller ändringar av företagets faktureringssatser för projektet när ekonomin beräknas om.

>[!NOTE]
>
>Användare måste ha tillgång till företag på sin åtkomstnivå för att kunna uppdatera faktureringspriserna på företagsnivå.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar**.
1. Klicka **Företag**.
1. Klicka på namnet på det företag som är associerat med det projekt för vilket du aktiverat åsidosättning av faktureringspriser på företagsnivå.
1. Klicka **Faktureringstaxor** till vänster.
1. Uppdatera **Företagets faktureringstakt** och start-/slutdatum för en befintlig jobbroll och tryck sedan på Retur.

   Om du vill lägga till ett nytt giltighetsdatum för företagsfaktureringstariff väljer du en faktureringssats för jobbrollen och klickar på **Redigera**. Mer information om aktuella företagsfaktureringspriser finns i [Åsidosätt faktureringssatser för jobbroller på företagsnivå](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Gör något av följande om du vill uppdatera företagsräntor för ett eller flera projekt:

   * Flera projekt:

   1. Gå till en lista med projekt.
   1. Markera kryssrutan i linje med de projekt som du vill uppdatera.
   1. Klicka **Redigera**.
   1. I avsnittet Inställningar aktiverar du **Omberäkna kostnader och intäkter** alternativ.
   1. Klicka **Spara ändringar**.

   * Ett projekt:

      1. Gå till det projekt där du aktiverade åsidosättning av faktureringstariffer på företagsnivå.
      1. Klicka på **Mer** meny ![](assets/qs-more-icon-on-an-object.png) bredvid projektnamnet i rubriken och klicka sedan på **Beräkna om ekonomi**.

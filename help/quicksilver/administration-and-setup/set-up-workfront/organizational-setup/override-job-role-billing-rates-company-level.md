---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Åsidosätt faktureringssatser för jobbroller på företagsnivå
description: När en jobbroll skapas kan du välja en timfaktureringsfrekvens för den rollen. Du kan skapa en timtaxa som är specifik för ett företag.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Åsidosätt faktureringssatser för jobbroller på företagsnivå

{{highlighted-preview}}

När en jobbroll skapas kan du välja en timfaktureringsfrekvens för den rollen. <span class="preview">Du kan skapa flera faktureringspriser per timme som är specifika för ett företag. Varje faktureringstaxa gäller för ett visst datumintervall.</span>

På projektnivå kan du aktivera ett alternativ för att tillåta faktureringstariffer på företagsnivå att åsidosätta projektnivåpriser. Mer information finns i [Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till företag om du inte är systemadministratör</p> <p>[!UICONTROL Edit] tillgång till finansiella uppgifter</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Åsidosätta eller ändra en fastställd faktureringsfrekvens som används för en specifik jobbroll

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Companies]**.
1. Leta reda på företaget där jobbrollen är tilldelad.
1. <span class="preview">Klicka på företagsnamnet i listan.</span>
1. <span class="preview">Klicka **[!UICONTROL Billing Rates]** i den vänstra panelen.</span>
1. <span class="preview">Klicka **[!UICONTROL Add Billing Rate]>[!UICONTROL New Billing Rate]** eller välj en befintlig frekvens att redigera.</span>
1. <span class="preview">I [!UICONTROL New Billing Rate] väljer du [!UICONTROL **Jobbroll**] för att definiera faktureringstaxan för.</span>

   <span class="preview">The [!UICONTROL **Standardfaktureringshastighet**] visar systemnivåfrekvensen för den här jobbrollen.</span>

   <span class="preview">![Ny dialogruta för faktureringstakt](assets/date-effective-billing-rates-for-company.png)</span>

1. <span class="preview">I [!DNL **Faktureringstariffer 1**] anger du faktureringstaxan. Klicka sedan på [!UICONTROL **Spara**] för att åsidosätta faktureringstakten en gång.</span>

   <span class="preview">eller</span>

   <span class="preview">Klicka [!UICONTROL **Lägg till frekvens**] för att lägga till fler faktureringstariffer med giltighetsdatum.</span>

1. <span class="preview">(Villkorligt) Om du lägger till mer än en faktureringsavgift anger du följande information:</span>

   * <span class="preview">**[!UICONTROL Billing Rates 1], 2 osv.**: Värdet på faktureringssatsen för tidsperioden.</span>
   * <span class="preview">**[!UICONTROL Start Date]**: Det datum då tariffen börjar gälla.</span>
   * <span class="preview">**[!UICONTROL End Date]**: Datumet då tariffen upphör.</span>

     <span class="preview">Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum. Vissa datum läggs till automatiskt. Om t.ex. Faktureringstariff 1 inte har något slutdatum och du lägger till Faktureringstariff 2 med startdatumet 1 maj 2023, läggs slutdatumet 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.</span>

1. <span class="preview">Klicka [!UICONTROL **Spara**].</span>

   >[!NOTE]
   >
   >Jobbrollssatser som ändras i projektet påverkar bara det projektet. Kurser som ändras på företagsnivå påverkar alla projekt. Mer information finns i [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

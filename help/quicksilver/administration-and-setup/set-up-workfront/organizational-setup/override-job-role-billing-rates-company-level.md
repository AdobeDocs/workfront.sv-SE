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
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Åsidosätt faktureringssatser för jobbroller på företagsnivå

När en jobbroll skapas kan du välja en timfaktureringsfrekvens för den rollen. Du kan skapa flera faktureringspriser per timme som är specifika för ett företag. Varje faktureringstaxa gäller för ett visst datumintervall.

På projektnivå kan du aktivera ett alternativ för att tillåta faktureringstariffer på företagsnivå att åsidosätta projektnivåfrekvenser. Mer information finns i [Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

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
   <td> <p>Administrativ åtkomst till företag om du inte är systemadministratör</p> <p>[!UICONTROL Edit] tillgång till finansiella uppgifter</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Åsidosätta eller ändra en fastställd faktureringsfrekvens som används för en specifik jobbroll

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Companies]**.
1. Leta reda på företaget där jobbrollen är tilldelad.
1. Klicka på företagsnamnet i listan.
1. Klicka på **[!UICONTROL Billing Rates]** i den vänstra panelen.
1. Klicka på **[!UICONTROL Add Billing Rate]>[!UICONTROL New Billing Rate]** eller välj en befintlig frekvens att redigera.
1. I dialogrutan [!UICONTROL New Billing Rate] väljer du en [!UICONTROL **jobbroll**] för att definiera faktureringsfrekvensen.

   [!UICONTROL **Standardfaktureringshastighet**] visar systemnivåfrekvensen för den här jobbrollen.

   ![Dialogrutan Ny faktureringshastighet](assets/date-effective-billing-rates-for-company.png)

1. I fältet [!DNL **Faktureringstariffer 1**] anger du faktureringstaxan. Klicka sedan på [!UICONTROL **Spara**] för att åsidosätta faktureringstakten en gång.

   eller

   Klicka på [!UICONTROL **Lägg till ränta**] om du vill lägga till fler faktureringstariffer med giltighetsdatum.

1. (Villkorligt) Om du lägger till mer än en faktureringsavgift anger du följande information:

   * **[!UICONTROL Billing Rates 1], 2 osv.**: Värdet för faktureringssatsen för tidsperioden.
   * **[!UICONTROL Start Date]**: Det datum då tariffen börjar gälla.
   * **[!UICONTROL End Date]**: Datumet då hastigheten slutar.

     Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum. Vissa datum läggs till automatiskt. Om t.ex. Faktureringstariff 1 inte har något slutdatum och du lägger till Faktureringstariff 2 med startdatumet 1 maj 2023, läggs slutdatumet 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.

1. Klicka på [!UICONTROL **Spara**].

   >[!NOTE]
   >
   >Jobbrollsatser som ändras i projektet påverkar bara det projektet. Kurser som ändras på företagsnivå kommer att påverka alla projekt. Mer information finns i [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

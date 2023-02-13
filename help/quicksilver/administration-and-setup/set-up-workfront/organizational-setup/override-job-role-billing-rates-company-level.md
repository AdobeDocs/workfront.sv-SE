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
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Åsidosätt faktureringssatser för jobbroller på företagsnivå

När en jobbroll skapas kan du välja en timfaktureringsfrekvens för den rollen. Du kan skapa en timtaxa som är specifik för ett företag.

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
1. Klicka **[!UICONTROL Edit Company]** i det övre högra hörnet.
1. I **[!UICONTROL Billing Rates]** väljer du den jobbroll du vill redigera och anger den nya faktureringssatsen för den jobbrollen i **[!UICONTROL Company Billing Rate]** box.

   >[!NOTE]
   >
   >Jobbrollssatser som ändras i projektet påverkar bara det projektet. Kurser som ändras på företagsnivå påverkar alla projekt. Mer information finns i [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

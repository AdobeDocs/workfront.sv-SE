---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Hantera tariffkort
description: Med tariffkort kan du definiera flera faktureringspriser per roll, baserat på plats.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Hantera tariffkort

{{highlighted-preview-article-level}}

Med tariffkort kan du definiera flera faktureringspriser per roll, baserat på plats. Du kan ha en jobbroll som Designer baserad i Paris och en andra Designer baserad i New York, där alla har olika faktureringstaxor. Det krävs dock ingen plats för jobbroller på ett tariffkort. En faktureringsfrekvens för en jobbroll (och eventuell plats) på ett kurskort kan även innehålla giltighetsdatum.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Äldre plan: [!UICONTROL Plan]</p>
       <p>Aktuell plan: [!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till [!UICONTROL Financial Data]</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Om du vill redigera ett tariffkort som delas med dig måste du ha behörigheten Hantera för tariffkortet.</td> 
  </tr> 
 </tbody> 
</table>

## Lägg till ett tariffkort

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen [!UICONTROL **Klassificeringskort**].
1. Klicka [!UICONTROL **Nytt tariffkort**] anger du namnet och beskrivningen för tariffkortet i listan.
1. Om du vill lägga till faktureringstariffer klickar du på priskortets namn i listan.
1. På kortskärmen klickar du på [!UICONTROL **Ny faktureringstaxa**].
1. Välj en [!UICONTROL **Jobbroll**] för att definiera faktureringstaxor för.

   Standardfaktureringshastighet visar systemnivåfrekvensen för den här jobbrollen.

   ![Ny dialogruta för faktureringstakt](assets/location-rate-for-rate-card.png)

1. Välj en [!UICONTROL **Valuta**] för jobbrollen.
1. (Valfritt) Välj en [!UICONTROL **Plats**] för jobbrollen.
1. I [!UICONTROL **Faktureringsränta 1**] anger du faktureringstakten för den här platsen. Klicka sedan på [!UICONTROL **Spara**] för att åsidosätta faktureringstakten en gång.

   eller

   Klicka [!UICONTROL **Lägg till frekvens**] för att lägga till mer platsspecifika faktureringspriser med giltighetsdatum.

1. (Villkorligt) Om du lägger till mer än en faktureringstaxa för den här platsen anger du följande information:

   * **[!UICONTROL Billing Rate 1], 2 osv.:** Värdet på faktureringssatsen för tidsperioden.
   * **[!UICONTROL Start Date]:** Det datum då prisåsidosättningen börjar.
   * **[!UICONTROL End Date]:** Datumet då tariffåsidosättningen upphör.

     Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum. Vissa datum läggs till automatiskt. Om t.ex. Faktureringstariff 1 inte har något slutdatum och du lägger till Faktureringstariff 2 med startdatumet 1 maj 2023, läggs slutdatumet 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.

1. Klicka [!UICONTROL **Spara**].
1. (Valfritt) Om du vill lägga till en annan faktureringsfrekvens, antingen för samma jobbroll på en annan plats eller för en separat jobbroll, klickar du på [!UICONTROL **Ny faktureringstaxa**].

## Kopiera ett priskort

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen [!UICONTROL **Klassificeringskort**].
1. Markera kryssrutan bredvid Betygsätt kort i listan och klicka på **Kopiera** icon ![Kopiera, ikon](assets/copy-icon.png).

   Ett dubbletttariffkort läggs till. Klicka på kortnamnet i listan för att ändra namnet.

## Ta bort ett tariffkort

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen [!UICONTROL **Klassificeringskort**].
1. Markera kryssrutan invid betygskortet i listan och klicka på **Ta bort** icon ![Ikonen Ta bort](assets/delete.png).

   >[!NOTE]
   >
   >Ett tariffkort som är kopplat till ett projekt tas bort från projektet.

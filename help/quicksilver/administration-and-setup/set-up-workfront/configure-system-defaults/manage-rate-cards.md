---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Hantera tariffkort
description: Med tariffkort kan du definiera flera faktureringspriser per roll, baserat på plats.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '660'
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
   <td><p>Ny plan: [!UICONTROL Standard] </p>
       <p>eller</p> 
       <p>Aktuell plan: [!UICONTROL Plan] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till [!UICONTROL Financial Data]</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
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
1. Klicka [!UICONTROL **Nytt tariffkort**] skriver du ett namn för tariffkortet i dialogrutan [!UICONTROL New rate card] i stället för&quot;Namnlöst tariffkort&quot;.
1. (Valfritt) Lägg till en [!UICONTROL **Beskrivning**].
1. (Valfritt) Om du vill bifoga ett anpassat formulär till tariffkortet klickar du på [!UICONTROL **Lägg till anpassat formulär**] i det övre högra hörnet och välj ett anpassat formulär i listan som visas.

   Mer information om hur du bifogar ett anpassat formulär finns i [Lägga till ett anpassat formulär i ett objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicka [!UICONTROL **Roller och hastigheter för jobb**] i den vänstra navigeringspanelen.
1. På skärmen Roller och tariffer för jobbjobb klickar du på [!UICONTROL **Lägg till jobbroll**].
1. I dialogrutan väljer du [!UICONTROL **Jobbroll**] för att definiera faktureringstaxor för.

   Standardfaktureringshastigheten visar systemnivåfrekvensen för den här jobbrollen, om en sådan har definierats.

   ![Ny dialogruta för faktureringstakt](assets/location-rate-for-rate-card.png)

1. Välj en [!UICONTROL **Valuta**] för jobbrollen.
1. (Valfritt) Välj en [!UICONTROL **Plats**] för jobbrollen.
1. I [!UICONTROL **Faktureringsränta 1**] anger du faktureringstakten för den här platsen. Klicka sedan på [!UICONTROL **Spara**] om du vill åsidosätta faktureringstakten en gång.

   eller

   Klicka [!UICONTROL **Lägg till frekvens**] för att lägga till mer platsspecifika faktureringspriser med giltighetsdatum.

1. (Villkorligt) Om du lägger till mer än en faktureringstaxa för den här platsen anger du följande information:

   * **[!UICONTROL Billing Rate 1], 2 osv.:** Värdet på faktureringssatsen för tidsperioden.
   * **[!UICONTROL Start Date]:** Det datum då prisåsidosättningen börjar.
   * **[!UICONTROL End Date]:** Datumet då tariffåsidosättningen upphör.

     Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum. Vissa datum läggs till automatiskt. Om t.ex. Faktureringstariff 1 inte har något slutdatum och du lägger till Faktureringstariff 2 med startdatumet 1 maj 2023, läggs slutdatumet 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.

1. Klicka [!UICONTROL **Spara**].
1. (Valfritt) Om du vill lägga till en annan faktureringsfrekvens, antingen för samma jobbroll på en annan plats eller för en separat jobbroll, klickar du på [!UICONTROL **Lägg till jobbroll**].
1. (Valfritt) Om du vill redigera ett tariffkort klickar du på kortnamnet i listan Klassificeringskort i Inställningar. Om du vill redigera en faktureringsfrekvens klickar du på [!UICONTROL **Roller och hastigheter för jobb**] i den vänstra navigeringspanelen på hastighetskortet. Välj sedan hastigheten och klicka på **Redigera** icon ![Ikonen Redigera](assets/edit-icon.png).

## Kopiera ett priskort

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen [!UICONTROL **Klassificeringskort**].
1. Markera kryssrutan bredvid tariffkortet i listan och klicka på **Kopiera** icon ![Kopiera, ikon](assets/copy-icon.png).
1. Ange ett namn för tariffkortet i dialogrutan [!UICONTROL Copy rate card] i stället för&quot;Namnlöst tariffkort&quot;. Klicka sedan på **Spara**.

   Det nya tariffkortet sparas. Redigera tariffkortsinformation, jobbroller och tariffer efter behov.

## Ta bort ett helt tariffkort

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen [!UICONTROL **Klassificeringskort**].
1. Markera kryssrutan bredvid tariffkortet i listan och klicka på **Ta bort** icon ![Ikonen Ta bort](assets/delete.png).

   >[!NOTE]
   >
   >Ett tariffkort som är kopplat till ett projekt tas bort från projektet.

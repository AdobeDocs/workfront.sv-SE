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
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Hantera tariffkort

{{highlighted-preview-article-level}}

Med tariffkort kan du definiera flera faktureringspriser per roll, baserat på plats. Du kan vara Designer-baserad i Paris och en andra Designer-baserad i New York, var och en med olika faktureringstaxor. Det krävs dock ingen plats för jobbroller på ett tariffkort. En faktureringsfrekvens för en jobbroll (och eventuell plats) på ett kurskort kan även innehålla giltighetsdatum.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Redigera åtkomst till [!UICONTROL Financial Data]</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Om du vill redigera ett tariffkort som delas med dig måste du ha behörigheten Hantera för tariffkortet.</td> 
  </tr> 
 </tbody> 
</table>

+++

## Lägg till ett tariffkort

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Klicka på [!UICONTROL **Nytt tariffkort**] och skriv ett namn på tariffkortet i rutan [!UICONTROL New rate card] för att ersätta&quot;Namnlöst tariffkort&quot;.
1. (Valfritt) Lägg till en [!UICONTROL **beskrivning**] på skärmen Värdekortsinformation.
1. (Valfritt) Om du vill bifoga ett anpassat formulär till tariffkortet klickar du på fältet [!UICONTROL **Lägg till anpassat formulär**] i det övre högra hörnet och väljer ett anpassat formulär i listan som visas.

   Mer information om hur du bifogar ett anpassat formulär finns i [Lägga till ett anpassat formulär till ett objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicka på [!UICONTROL **Jobbroller och hastigheter**] i den vänstra navigeringspanelen.
1. Klicka på [!UICONTROL **Lägg till jobbroll**] på skärmen Roller och hastigheter för jobbjobb.
1. I dialogrutan väljer du en [!UICONTROL **jobbroll**] för att definiera faktureringstaxor för.

   Standardfaktureringshastigheten visar systemnivåfrekvensen för den här jobbrollen, om en sådan har definierats.

   ![Dialogrutan Ny faktureringshastighet](assets/location-rate-for-rate-card.png)

1. Välj en [!UICONTROL **Valuta**] för jobbrollen.
1. (Valfritt) Välj en [!UICONTROL **plats**] för jobbrollen.
1. I fältet [!UICONTROL **Faktureringstakt 1**] anger du faktureringstakten för den här platsen. Klicka sedan på [!UICONTROL **Spara**] för att åsidosätta faktureringstakten en gång.

   eller

   Klicka på [!UICONTROL **Lägg till ränta**] om du vill lägga till fler platsspecifika faktureringspriser med giltighetsdatum.

1. (Villkorligt) Om du lägger till mer än en faktureringstaxa för den här platsen anger du följande information:

   * **[!UICONTROL Billing Rate 1], 2 osv.:** Värdet på faktureringssatsen för tidsperioden.
   * **[!UICONTROL Start Date]:** Datumet då hastighetsåsidosättningen börjar.
   * **[!UICONTROL End Date]:** Datumet då hastighetsåsidosättningen upphör.

     Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum. Vissa datum läggs till automatiskt. Om t.ex. Faktureringstariff 1 inte har något slutdatum och du lägger till Faktureringstariff 2 med startdatumet 1 maj 2023, läggs slutdatumet 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.

1. Klicka på [!UICONTROL **Spara**].
1. (Valfritt) Om du vill lägga till en annan faktureringsfrekvens, antingen för samma jobbroll på en annan plats eller för en separat jobbroll, klickar du på [!UICONTROL **Lägg till jobbroll**].
1. (Valfritt) Om du vill redigera ett tariffkort klickar du på kortnamnet i listan Klassificeringskort i Inställningar. Om du vill redigera en faktureringsfrekvens klickar du på [!UICONTROL **Jobbroller och -hastigheter**] i den vänstra navigeringspanelen på tariffkortet. Markera sedan hastigheten och klicka på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

## Kopiera ett priskort

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Markera kryssrutan bredvid tariffkortet i listan och klicka på ikonen **Kopiera** ![Kopiera](assets/copy-icon.png) .
1. Skriv in ett namn för tariffkortet i rutan [!UICONTROL Copy rate card] om du vill ersätta&quot;Kort med namnlös hastighet&quot;. Klicka sedan på **Spara**.

   Det nya tariffkortet sparas. Redigera tariffkortsinformation, jobbroller och tariffer efter behov.

## Ta bort ett helt tariffkort

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Markera kryssrutan bredvid tariffkortet i listan och klicka på ikonen **Ta bort** ![Ta bort](assets/delete.png) .

   >[!NOTE]
   >
   >Ett tariffkort som är kopplat till ett projekt tas bort från projektet.

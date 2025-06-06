---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Lägg till ett Outlook-e-postmeddelande som en uppgift i din arbetslista
description: Du kan konvertera [!DNL Outlook] e-postmeddelanden till [!DNL Adobe Workfront] aktiviteter. När ett e-postmeddelande har konverterats är uppgiften tillgänglig i din arbetslista i hemområdet.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Lägg till ett [!DNL Outlook]-e-postmeddelande som en uppgift i din arbetslista

>[!IMPORTANT]
>
>[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.
>
>* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**
>
>Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**


Du kan konvertera [!DNL Outlook] e-postmeddelanden till [!DNL Adobe Workfront] uppgifter. När ett e-postmeddelande har konverterats är uppgiften tillgänglig i listan [!UICONTROL Work] i området [!UICONTROL Home].

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

[!DNL Workfront]-administratören måste aktivera [!DNL Outlook for Office] med [!DNL Workfront] innan du kan använda den här integreringen.

## Lägg till ett [!DNL Outlook]-e-postmeddelande som en uppgift i din arbetslista

1. Markera det e-postmeddelande i [!DNL Outlook] som du vill konvertera till en uppgift.
1. Klicka på ikonen **[!DNL Workfront]** i det övre högra hörnet av e-postmeddelandet för att visa tillägget [!DNL Workfront].\
   Du kan behöva klicka på den nedåtriktade pilen i det övre högra hörnet av ditt e-postmeddelande för att komma åt ikonen [!DNL Workfront].

1. Klicka på ikonen **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) för att visa en lista över tillgängliga [!DNL Workfront]-alternativ.\


1. Klicka på **[!UICONTROL Add to Work]**.\

1. Avmarkera fältet **[!UICONTROL Add to Project]**.
1. (Valfritt) Du kan uppdatera följande information från e-postmeddelandet innan det sparas som en uppgift:

   * **[!UICONTROL Task Name]:** Som standard är aktivitetsnamnet samma som e-postmeddelandets ämne. Du kan ändra aktivitetsnamnet efter behov.
   * **[!UICONTROL Description]:** Beskrivningen är som standard densamma som e-postbrödtexten. Du kan ändra beskrivningen efter behov.
   * **[!UICONTROL Attachments]:** Alla e-postbilagor sparas i aktivitetens [!UICONTROL Documents]-område. Du kan ta bort eventuella bilagor innan du sparar e-postmeddelandet som en uppgift.

1. Klicka på **[!UICONTROL Add]**.\
   Uppgiften läggs till i [!UICONTROL Work List] i hemområdet utan implementeringsdatum.

1. (Valfritt) Klicka på **[!UICONTROL View in Workfront]** om du vill visa uppgiften i programmet [!DNL Workfront] på en ny flik.

1. (Valfritt) Navigera tillbaka till [!DNL Outlook] och markera det ursprungliga e-postmeddelandet.\
   Längst upp på tilläggspanelen [!DNL Workfront] kan du se bekräftelsen med en länk att e-postmeddelandet har lagts till i Workfront som en uppgift. Länken innehåller datumet då den konverterades.\

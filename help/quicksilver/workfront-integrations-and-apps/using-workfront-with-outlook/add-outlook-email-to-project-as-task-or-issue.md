---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Lägg till ett Outlook-e-postmeddelande i ett projekt som en uppgift eller ett problem
description: Du kan konvertera e-postmeddelanden till  [!DNL Adobe Workfront]  uppgifter eller problem. När ett e-postmeddelande har konverterats visas uppgiften eller problemet i det projekt som väljs när du konverterar det.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Lägg till ett [!DNL Outlook]-e-postmeddelande i ett projekt som en aktivitet eller ett problem

>[!IMPORTANT]
>
>[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.
>
>* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**
>
>Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**

Du kan konvertera e-postmeddelanden till [!DNL Adobe Workfront] uppgifter eller problem. När ett e-postmeddelande har konverterats visas uppgiften eller problemet i det projekt som väljs när du konverterar det.

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

## Lägg till ett [!DNL Outlook]-e-postmeddelande i ett projekt som en aktivitet eller ett problem

1. Markera det e-postmeddelande i [!DNL Outlook] som du vill konvertera till en aktivitet eller ett problem.
1. Klicka på ikonen **[!DNL Workfront]** i det övre högra hörnet av e-postmeddelandet för att visa Workfront-tillägget.

   Du kan behöva klicka på den nedåtriktade pilen i det övre högra hörnet av ditt e-postmeddelande för att komma åt ikonen [!DNL Workfront].

1. Klicka på ikonen **[!UICONTROL Menu]** ![ o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) för att visa listan med tillgängliga [!DNL Workfront]-alternativ.



1. Klicka på **[!UICONTROL Add to Work]**.

1. Markera fältet **[!UICONTROL Add to Project]**.
1. Börja skriva namnet på ett projekt i fältet **[!UICONTROL Project]** och markera det när det visas i listan.
1. Markera alternativknappen **[!UICONTROL Task]** om du vill lägga till en aktivitet i det markerade projektet.

   eller

   Markera alternativknappen **[!UICONTROL Issue]** om du vill lägga till ett problem i det valda projektet.

1. (Valfritt) Ange vem den här aktiviteten eller problemet har tilldelats i fältet **[!UICONTROL Assign this to]**.

   >[!TIP]
   >
   >Du kan tilldela en uppgift eller utgåva till ett team om du vill att flera personer ska vara medvetna om den. Om teamets medlemmar har aktiverat sina e-postmeddelanden får de ett e-postmeddelande om den nya uppgiften eller det nya problemet.


1. (Valfritt) Ange **[!UICONTROL Due by date]**. Detta blir [!UICONTROL Planned Completion Date] för aktiviteten eller problemet.
1. (Valfritt) Uppdatera följande information från e-postmeddelandet innan det sparas som en uppgift eller ett problem (obligatoriska fält föregås av en asterisk).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Task or Issue Name]</td>
        <td>Som standard är aktivitetsnamnet samma som e-postmeddelandets ämne. Du kan ändra aktivitetsnamnet efter behov.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Description]</td>
        <td>Beskrivningen är som standard densamma som e-postbrödtexten. Du kan ändra beskrivningen efter behov.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Attachments]</td>
        <td>Eventuella e-postbilagor sparas i området [!UICONTROL Documents] för uppgiften eller utgåvan. Du kan ta bort eventuella bilagor innan du sparar e-postmeddelandet som en uppgift eller ett problem.</td>
      </tr>
   </table>

1. Klicka på **[!UICONTROL Add]**.

   Uppgiften eller utgåvan läggs till i det angivna projektet

1. (Valfritt) Klicka på **[!UICONTROL View in [!DNL Workfront]]** om du vill visa uppgiften i programmet [!DNL Workfront] på en ny flik.

1. (Valfritt) Gå tillbaka till [!DNL Outlook] och välj det konverterade e-postmeddelandet.

   Längst upp på tilläggspanelen [!DNL Workfront] kan du se bekräftelsen med en länk att e-postmeddelandet har lagts till i [!DNL Workfront] som en uppgift eller ett problem. Länken innehåller datumet då den konverterades.




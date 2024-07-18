---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Uppdatera ett befintligt objekt från ett Outlook-e-postmeddelande
description: Du kan uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett Outlook-e-postmeddelande.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 16acba0f1981b75ca141a36d096fb6f5d37c40d1
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Uppdatera ett befintligt objekt från ett [!DNL Outlook]-e-postmeddelande

Du kan uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett [!DNL Outlook]-e-postmeddelande.

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

## Uppdatera ett befintligt objekt från ett [!DNL Outlook]-e-postmeddelande

1. I [!DNL Outlook] markerar du det e-postmeddelande som innehåller den information som du vill inkludera i en [!DNL Adobe Workfront update].
1. Klicka på ikonen **[!DNL Workfront]** i det övre högra hörnet av e-postmeddelandet för att visa Workfront-tillägget.\
   Du kan behöva klicka på den nedåtriktade pilen i det övre högra hörnet av ditt e-postmeddelande för att komma åt ikonen [!DNL Workfront].

1. Klicka på ikonen **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) för att visa listan med tillgängliga [!DNL Workfront]-alternativ.\


1. Klicka på **[!UICONTROL Update]i Workfront**.\
   Du kan uppdatera följande information från e-postmeddelandet innan det sparas som en uppgift:

   * **[!UICONTROL Type]**: Välj den typ av objekt som du uppdaterar. Du kan välja **[!UICONTROL Project]**, **[!UICONTROL Task]** eller **[!UICONTROL Issue]**. Objektet du väljer avgör vilka resultat som visas i fältet **[!UICONTROL Name]** nedan. Om du är osäker på objekttypen väljer du **[!UICONTROL All]** om du vill söka efter projekt, uppgifter och utgåvor samtidigt.

   * **[!UICONTROL Name]**: Börja skriva namnet på projektet, aktiviteten eller problemet som du vill uppdatera. Klicka på namnet när det visas i listrutan.
   * **[!UICONTROL Update]**: Uppdateringen är som standard densamma som brödtexten för e-post. Du kan ändra uppdateringen efter behov.\

     [!UICONTROL update] visas som uppdateringsstatus i Workfront.

   * **[!UICONTROL Attachments]**: Alla e-postbilagor sparas i aktivitetens [!UICONTROL Documents]-område. Du kan ta bort alla bifogade filer innan du skickar in uppdateringen.

1. (Valfritt) Klicka på **[!UICONTROL Include Others]**, börja skriva namnet på de användare som du vill ta med i uppdateringen och klicka sedan på namnet när det visas i listrutan.\
   Upprepa den här processen om du vill inkludera fler användare och klicka sedan på **[!UICONTROL Done]**.\
   Som standard får den användare du svarar ett meddelande oavsett om du tar med dem eller inte.\

1. (Valfritt) Klicka på ikonen **[!UICONTROL Lock]** om du vill begränsa uppdateringen till användare i ditt företag. När uppdateringen är låst kan användare utanför företaget inte se uppdateringen.

   * **[!UICONTROL Unlocked]:** Alla användare med åtkomst till projektet, aktiviteten eller problemet där uppdateringen finns kan visa uppdateringen.\

     Uppdateringen är som standard olåst.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Locked]:** Endast användare i ditt företag kan visa uppdateringen.\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Klicka på **[!UICONTROL Update]**.
1. (Valfritt) Klicka på **[!UICONTROL View in Workfront]** om du vill visa det uppdaterade objektet med [!DNL Workfront]-integreringen i [!UICONTROL Outlook].

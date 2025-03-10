---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Överföra XD ritytor som dokument till Workfront
description: Du kan överföra ritytorna som dokument för snabb granskning och godkännande eller bara lagra dem i Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---


# Överför [!DNL XD] ritytor som dokument till [!DNL Workfront]

Du kan överföra ritytorna som dokument för snabb granskning och godkännande eller bara lagra dem i [!DNL Adobe Workfront].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till [!UICONTROL Documents]</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL View] åtkomst eller högre till objektet där du vill överföra ett dokument.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

* Du måste installera plugin-programmet [!DNL Adobe Workfront for XD] innan du kan överföra XD ritytor som dokument till Workfront.

Instruktioner finns i [Installera [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Lägg till ett nytt dokument

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Menyikon](assets/menu-350x440.png)

1. Gå till den arbetsuppgift där du vill överföra ett dokument.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument ](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New File]** längst ned i plugin-programmet.
1. Markera den rityta som du vill överföra.

   >[!TIP]
   >
   >Om du vill markera mer än en rityta klickar du och drar musen över de ritytor du vill använda.
1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.
1. Välj **[!UICONTROL Asset Type]** i listrutan:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Export Format]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Ritytorna överförs som en PNG-fil till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Ritytorna överförs som en JPG till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Ritytorna överförs som SVG till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Välj om du vill att de markerade ritytorna ska överföras som en <strong>fil med ett PDF </strong> eller <strong>flera PDF </strong> . Ritytorna överförs som ett PDF till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Klicka på **[!UICONTROL Upload]**.\
   Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.

## Lägg till en ny version

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Menyikon](assets/menu-350x440.png)

1. Gå till den arbetsuppgift där du vill överföra ett dokument.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument ](assets/documents.png) i navigeringsfältet.

1. Klicka på dokumentet som du vill lägga till en ny version i.
1. Klicka på **[!UICONTROL New version]** längst ned i plugin-programmet.
1. Markera de ritytor som du vill överföra.

   >[!NOTE]
   >
   >Om du vill överföra en ny version av en SVG, PNG eller JPG kan du bara överföra en rityta.

1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

1. Välj **[!UICONTROL Asset Type]** i listrutan:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Exportformat</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Ritytan överförs som en PNG-fil till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Ritytan överförs som en JPG till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Ritytan överförs som ett SVG till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Ritytorna överförs som PDF till arbetsobjektets [!UICONTROL Documents]-flik i [!DNL Workfront].</p>
      <p><strong>Obs!</strong>: Du kan bara överföra en rityta för en ny dokumentversion.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Klicka på **[!UICONTROL Upload]**.\
   Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.

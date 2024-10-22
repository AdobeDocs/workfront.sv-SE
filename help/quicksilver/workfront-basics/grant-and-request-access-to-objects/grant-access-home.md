---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: Bevilja åtkomst till objekt i Hem-området
description: Användare kan begära åtkomst till objekt i Adobe Workfront. Mer information om hur du begär åtkomst finns i Begär åtkomst till objekt.
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Bevilja åtkomst till objekt i Hem-området

<!--Audited: 10/2024-->

Användare kan begära åtkomst till objekt i Adobe Workfront.

Mer information om hur du begär åtkomst finns i [Begär åtkomst till objekt](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).

Om du är ägare till ett objekt kan du bevilja eller neka åtkomst till objekt från Hem-området.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p> 
   <p>Aktuell: Arbete eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller högre till projekt, uppgifter, utgåvor eller dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för projekt, uppgifter, utgåvor eller dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bevilja åtkomst till objekt i Hem-området

1. Klicka på **huvudmenyn** ![](assets/dots-main-menu.png) i det övre högra hörnet av skärmen eller på **huvudmenyn** ![](assets/lines-main-menu.png) i det övre vänstra hörnet, om det är tillgängligt, och klicka sedan på **Hem**
eller
Klicka på ikonen **Hem** ![](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmenyn** ![](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Gör följande:

   1. Gå till widgeten **Mina godkännanden** och leta upp begäran om mer åtkomst. Klicka sedan på **Bevilja åtkomst**.

      ![](assets/request-for-access-to-project-in-new-home-approvals-widget.png)

   1. (Valfritt) Om du vill ge en annan åtkomstnivå än den som begärts klickar du på listrutan till vänster om knappen Bevilja åtkomst och väljer den nya åtkomsten. Klicka sedan på **Bevilja åtkomst**.

      Åtkomstbegäran beviljas och tas bort från listan över godkännandebegäranden.

1. (Valfritt) Klicka på **Ignorera** om du vill neka åtkomst. Åtkomstbegäran beviljas inte och begäran tas bort från listan över godkännandebegäranden.

## Konfigurera e-postmeddelanden för åtkomstbegäranden

Du kan konfigurera om du ska få e-postmeddelanden för åtkomstbegäranden. Workfront-administratören kan inaktivera den här funktionen (enligt beskrivningen i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

1. Gå till din användarprofil genom att göra något av följande:

   * Klicka på **Huvudmenyn** ![](assets/dots-main-menu.png) i skärmens övre högra hörn och klicka sedan på ditt namn.
   * Klicka på Adobe **Huvudmenyn** ![](assets/adobe-blue-main-menu.png) i det övre högra hörnet, om det är tillgängligt, och klicka sedan på **Workfront-profil**.

1. Klicka på menyn **Mer** ![](assets/more-icon.png) till höger om ditt namn i sidhuvudet och klicka sedan på **Redigera**.
1. Klicka på **Meddelanden** och markera eller avmarkera **Någon begär åtkomst från mig** i avsnittet **Åtgärd krävs**, beroende på om du vill få e-postmeddelanden när en annan användare begär åtkomst från dig eller inte.

   Du kan aktivera ett dagligt eller omedelbart meddelande.

1. Klicka på **Spara ändringar**.

<!--1. (Conditional) From the legacy Home area, do the following: 
   
   1. In the **Work List**, select the access request you want to manage in the **Approvals** section.  

   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

   The request displays on the right of the Work List. 

   1. In the upper-right corner, click the grant access button.  
   Depending on the type of access requested, the button name changes. For example, if the requestor asks for View access, the button says **Grant View Access**.  
   ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

   1. (Optional) To grant a different level of access than requested, click the arrow next to the grant access button and select the new access, then click **Grant < Permission level > Access >**.  
   A message appears confirming access was granted.  
   
   1. (Optional) Click **Ignore** to deny access.  
   A message appears confirming access was ignored.-->

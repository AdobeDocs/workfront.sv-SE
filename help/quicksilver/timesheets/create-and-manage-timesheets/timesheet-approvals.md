---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Godkänn en tidrapport
description: Processen att godkänna tidrapporter ger cheferna insyn i arbetstiden för sina direkta rapporter. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att tillräckligt många timmar har registrerats för perioden.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Godkänn en tidrapport

Processen att godkänna tidrapporter ger cheferna insyn i arbetstiden för sina direkta rapporter. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att tillräckligt många timmar har registrerats för perioden.

Adobe Workfront ger möjlighet att konfigurera tidrapportgodkännanden som stöds i det här området.

Information om hur du skickar in en tidrapport finns i [Skicka en tidrapport för godkännande](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan eller licenstyp du har.

## Utse godkännare av tidrapporter

Tidrapporter brukar godkännas av personalchefer eller personal. (Tidrapporter godkänns normalt inte av projektledare.)

En tidrapportgodkännare definieras när du skapar tidrapportprofilen. Du måste ha en planlicens för att kunna utses till godkännare.

Mer information om hur du anger godkännare av tidrapporter finns i avsnittet [Skapa eller redigera en tidrapportprofil](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) i artikeln [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Godkänn en tidrapport

Du kan godkänna alla tidrapporter som har skickats in där du har utsetts till godkännare. När en tidrapport skickas för godkännande visas tidrapporten i området **Godkännanden** på **Hem**  sida. Mer information finns i [Godkänna arbete](../../review-and-approve-work/manage-approvals/approving-work.md).

Om Workfront-administratören har aktiverat händelsehanterarna Godkännande av tidrapport för användare och Avvisning av tidrapport för användare, meddelas du när tidrapporten har godkänts eller avvisats. Mer information om hur du aktiverar händelsemeddelanden finns i [Händelsemeddelandetyper](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Så här godkänner du en tidrapport:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.
1. Klicka på **Tidrapporter**.
1. Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du har godkänt

   eller

   Välj filtret **Mina tidrapportgodkännanden** högst upp i tidrapportlistan.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Alternativet Mina tidrapportgodkännanden visas inte längst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtret Mina tidrapportgodkännanden från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   >
   >   
   >   
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Valfritt) Klicka på ikonen **sök** ![](assets/search-icon.png) högst upp i tidrapportlistan och skriv ett nyckelord för att hitta en viss tidrapport. Du kan söka efter en tidsram, en ägare eller en godkännare.
1. Klicka på tidsramen för den tidrapport som du vill godkänna. Tidrapporten öppnas.

   >[!TIP]
   >
   >Tidrapporter som väntar på godkännande har statusen [!UICONTROL Submitted].


1. Klicka på **Godkänn**

   eller

   Om du vill avvisa tidrapporten klickar du på **Avvisa** i det nedre vänstra hörnet av tidrapporten.

   Om det godkänns ändras tidrapportens status till **Stängd**.

   Om den avvisas ändras tidrapportens status till **Avvisad**.

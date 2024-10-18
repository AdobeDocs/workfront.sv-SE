---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Godkänn en tidrapport
description: Processen att godkänna tidrapporter ger cheferna insyn i arbetstiden för sina direkta rapporter. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att tillräckligt många timmar har registrerats för perioden.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 9d0caff0381ee50bf8dd7060bebafb5354c0f0d8
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Godkänn en tidrapport

<!--Audited: 8/2024-->

Processen att godkänna tidrapporter ger cheferna insyn i arbetstiden för sina direkta rapporter. Godkännarna kan verifiera att all registrerad tid har allokerats i rätt områden och att tillräckligt många timmar har registrerats för perioden.

Adobe Workfront ger möjlighet att konfigurera tidrapportgodkännanden som stöds i det här området.

Information om hur du skickar in en tidrapport finns i [Skicka en tidrapport för godkännande](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td> <p>Nytt: Standard</p>
   <p>Aktuell: Planera </p> 
   <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till tidrapporter och timmar </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utse godkännare av tidrapporter

Tidrapporter brukar godkännas av personalchefer eller personal. Tidrapporter godkänns vanligtvis inte av projektledare. Projektledare kan godkänna tidsinloggade projekt, men team- eller personalchefer bör godkänna tidrapporter.

En tidrapportgodkännare definieras när du skapar tidrapportprofilen. Du måste ha en planlicens för att kunna utses till godkännare.

Mer information om hur du anger godkännare av tidrapporter finns i avsnittet [Skapa eller redigera en tidrapportprofil](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) i artikeln [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Godkänn en tidrapport

Du kan godkänna alla tidrapporter som har skickats in där du har utsetts till godkännare. När en tidrapport skickas för godkännande visas tidrapporten i widgeten **Mina godkännanden** i området **Hem** . Mer information finns i [Godkänna arbete](../../review-and-approve-work/manage-approvals/approving-work.md).

Om följande meddelandeinställningar finns på plats får den användare som skickar tidrapporten för godkännande ett e-postmeddelande när en tidrapport har godkänts:

* Workfront-administratören har aktiverat tidrapportgodkännande för användare och händelsehanterare för avvisning av tidrapport. Mer information om hur du aktiverar händelsemeddelanden finns i [Händelsemeddelandetyper](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* Min tidrapport har godkänts för personligt meddelande på användarens profilsida. Mer information finns i [Ändra dina egna e-postmeddelanden](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Godkänn en tidrapport från området Tidrapporter

{{step1-to-timesheets}}

Området **Tidrapporter** öppnas.

1. (Villkorligt) Om den senaste gången du öppnade öppnas klickar du på **Tillbaka till tidrapporter** i skärmens övre vänstra hörn.

1. Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du har godkänt

   eller

   Välj filtret **Mina tidrapportgodkännanden** högst upp i tidrapportlistan.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Alternativet Mina tidrapportgodkännanden visas inte längst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtret Mina tidrapportgodkännanden från antingen listkontrollerna i inställningsområdet eller från layoutmallen.
   >
   >Mer information finns i [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
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

### Godkänn en tidrapport från hemområdet

{{step1-to-home}}

Hemområdet öppnas.

1. Kontrollera att widgeten **Mina godkännanden** har lagts till i din hemsida. Mer information finns i [Lägg till, redigera och ta bort widgetar i Nytt hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).
1. Hitta ett godkännande av tidrapporten i widgeten Mina godkännanden.
1. (Valfritt) Expandera den nedrullningsbara menyn till höger om knapparna Godkänn eller Avvisa för att lägga till en kommentar om ditt beslut och klicka sedan på **Lägg till**.
1. Klicka på någon av följande knappar för att fatta ditt beslut om godkännande:

   * Godkänn
   * Avvisa

   Godkännandet tas bort från widgeten **Mina godkännanden**.



---
user-type: administrator
product-area: system-administration
navigation-topic: start-with-workfront-administration
title: Skicka meddelanden
description: Som Adobe Workfront-administratör kan du använda meddelandesidan för att skicka meddelanden till användare.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 413e3051-fcb5-44d7-b6bd-6b05d39935e8
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Skicka meddelanden

Som Adobe Workfront-administratör kan du använda meddelandesidan för att skicka meddelanden till användare.

Meddelanden från Workfront innehåller vanligtvis information om nya funktioner och releaser, processändringar och så vidare.

Mer information om hur du visar meddelanden finns i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara Workfront-administratör. </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skicka meddelanden till användare

Du kan använda sidan **Meddelanden** för att kommunicera med användare i ditt Workfront-system genom att vidarebefordra meddelanden som skickas från Workfront och genom att skriva nya meddelanden. Du kan skicka meddelanden till specifika användare, grupper, team eller företag i Workfront.

* [Vidarebefordra Workfront-meddelanden till användare](#forward-workfront-announcements-to-users)
* [Skapa nya meddelanden](#compose-new-announcements)

### Vidarebefordra Workfront-meddelanden till användare {#forward-workfront-announcements-to-users}

Du kan enkelt vidarebefordra meddelanden som du får från Workfront till användare i ditt system.

1. Gå till sidan Meddelanden genom att klicka på ikonen **Meddelande** i det övre högra hörnet av Workfront-gränssnittet och sedan på **Alla meddelanden**.

   ![Alla meddelanden](assets/announcement-access-350x212.png)

1. Markera meddelandet som du vill vidarebefordra på sidan **Meddelanden**.
1. Klicka på **Vidarebefordra**.
1. I rutan **Skicka till** börjar du skriva namnet på en användare, grupp, team eller företag som du vill ska få meddelandet. Klicka sedan på namnet när det visas i listrutan. Upprepa den här processen om du vill lägga till flera användare, grupper, team eller företag.

   eller

   Om du vill vidarebefordra meddelandet till alla användare i systemet börjar du med att skriva **Alla** och klickar sedan på meddelandet när det visas i listrutan.

1. Fortsätt med steg 3 i [Skapa nya meddelanden](#compose-new-announcements).

### Skapa nya meddelanden {#compose-new-announcements}

1. Gå till sidan Meddelanden genom att klicka på ikonen **Meddelande** i det övre högra hörnet av Workfront-gränssnittet och sedan på **Alla meddelanden**.

   ![Alla meddelanden](assets/announcement-access-350x212.png)

1. Klicka på **Nytt meddelande på sidan** Meddelanden **.**

1. I rutan **Skicka till** börjar du skriva namnet på en användare, grupp, team eller företag som du vill ska få meddelandet. Klicka sedan på namnet när det visas i listrutan. Upprepa den här processen om du vill lägga till flera användare, grupper, team eller företag.

   Som standard fylls **Alla** i automatiskt i det här fältet när ett nytt meddelande skickas. Om du inte vill att alla användare i systemet ska få meddelandet tar du bort **Alla** från listan.

1. Ange följande ytterligare information:

   | Ämne | Ange ett ämne för meddelandet. |
   |---|---|
   | Skriv meddelandet här | Ange innehållet i meddelandet. Med meddelanderedigeraren kan du inkludera vanliga märkord, t.ex. fet, kursiv stil, understrykning, punktlistor och numrerade listor samt hyperlänkar. |
   | Bifogade filer | Klicka på **Lägg till bifogad fil** och bläddra sedan till och markera filen som du vill bifoga i meddelandet. |

   {style="table-layout:auto"}

1. (Valfritt) Klicka på **Spara som utkast** om du vill spara meddelandet (inklusive mottagarlistan, ämnet och bifogade filer) som ett utkast.

1. (Valfritt) Om du vill visa ett utkast klickar du på **Utkast** i området **Meddelanden**.

1. Klicka på **Skicka.**

   Användare kan nu visa meddelandet som beskrivs i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Begränsa de typer av Workfront-meddelanden du får

Om du är Workfront-administratör kan du avbryta prenumerationen på vissa typer av meddelanden.

Som standard får du alla meddelanden som skickas från Workfront. Detta är den rekommenderade konfigurationen.

1. På sidan **Meddelanden** klickar du på **Inställningar.**
1. Välj de ämnen som du inte längre vill ta emot meddelanden för.
1. Klicka på **Spara inställningar.**

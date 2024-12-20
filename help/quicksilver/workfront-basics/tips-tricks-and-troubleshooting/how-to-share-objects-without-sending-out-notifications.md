---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Dela objekt utan att generera meddelanden
description: Ta reda på hur du kan dela objekt och förhindra att meddelanden skickas om den här ändringen. Detta är särskilt användbart när du delar flera objekt samtidigt.
author: Alina
feature: Get Started with Workfront
source-git-commit: b14dd633edec3e9746f7f1412445b74bcd37a676
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---


# Dela objekt utan att generera meddelanden

<!--Audited: 12/2024-->

När du delar ett objekt i Adobe Workfront får de personer som du delar objektet med ett e-postmeddelande om delningen.

Det är viktigt att du är medveten om den här ändringen genom att få ett e-postmeddelande när någon delar ett objekt med dig. För många meddelanden kan dock vara för förvirrande för användarna. Om du vill dela ett stort antal objekt med användare samtidigt kan du undvika förvirring genom att tillfälligt inaktivera meddelanden.

Användarna får e-postmeddelanden när följande inställningar är aktiverade samtidigt:

* Ett eller båda av följande händelsemeddelanden är aktiverade på system- eller gruppnivå:

   * Objektdelning till användare
   * Objektdelning till team är aktiverat på system- eller gruppnivå.
* Ett eller båda av följande e-postmeddelanden är aktiverade i användarens profil:

   * Någon delar objekt med mig
   * Någon delar ett objekt med mitt team

Om du behöver dela flera objekt med flera personer (flera), men inte vill att de ska få e-postmeddelanden om den här ändringen, gör du följande:

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna dela objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Ny licens: Standard</p> 
   eller
   <p>Aktuell licens: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p>
   <p>Redigera åtkomst för användare</p>
   <p><b>ANMÄRKNING</b></p>
   <p> Du måste vara system- eller gruppadministratör för att kunna kontrollera statusen för händelseaviseringar för systemet eller gruppen</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela objekt utan att generera meddelanden

1. Kontrollera att följande **Händelsemeddelanden** är aktiverade på system- eller gruppnivå:

   * **Objektdelning till användare**
   * **Objektdelning till team är aktiverat på system- eller gruppnivå**.

   Mer information finns i [Konfigurera händelsemeddelanden för alla i systemet](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Om dessa händelsemeddelanden inte är aktiverade skickas inga meddelanden om att dela ett objekt till användarna. Om det ena eller båda är aktiverade fortsätter du med följande steg.

{{step-1-to-users}}

1. Markera flera användare i listan och klicka sedan på **Meddelanden** > **Diverse**.
1. Inaktivera ett eller båda av följande meddelanden (beroende på vilka som är aktiverade från system- eller gruppnivå):

   * **Någon delar ett objekt med mig**
   * **Någon delar ett objekt med mitt team**

   Se till att alla valda användare har dessa meddelanden markerade innan du inaktiverar dem. På så sätt kan du aktivera dem flera gånger för alla när du har delat objekten.

1. Klicka på **Spara ändringar**.
1. Gå till en lista med objekt som du vill dela och markera objekten. Klicka sedan på ikonen **Dela** längst upp i listan.

   Mer information om att dela flera objekt samtidigt finns i [Dela ett objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

1. Gå tillbaka till listan över användare som du har inaktiverat meddelanden för och välj samma användare.
1. Markera samma användare i listan och klicka sedan på **Meddelanden** > **Diverse**.
1. Aktivera ett eller båda av följande meddelanden (beroende på vilka som är aktiverade från system- eller gruppnivå):

   * **Någon delar ett objekt med mig**
   * **Någon delar ett objekt med mitt team**

1. Klicka på **Spara ändringar**.

   Objekten delades med de valda användarna och ingen av dem fick några e-postmeddelanden om den här ändringen.







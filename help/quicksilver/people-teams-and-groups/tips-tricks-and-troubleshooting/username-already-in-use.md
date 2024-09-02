---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Användarnamnet används redan
description: Läs de här tipsen när du får ett felmeddelande om att användarnamnet redan används.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Användarnamnet används redan

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Systemadministratör</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fråga

När du skapar en ny användare visas ett [!UICONTROL Whoops]-fel som anger att användarnamnet redan används. Det finns inga andra förekomster av det här e-postmeddelandet i systemet. Varför visas detta?

## Lösning

Detta kan bero på att användarnamnet eller e-postadressen inte är unik i den aktuella [!DNL Adobe Workfront]-instansen. Användare kan ha samma användarnamn eller e-postadress i olika instanser. Användare A kan till exempel ha följande e-postadresser kopplade till ett [!DNL Workfront]-konto: usera@company1.com och usera@company2.com.

>[!NOTE]
>
>Den primära [!DNL Workfront]-administratören kan inte ha samma användarnamn eller e-postadress om de finns i separata Workfront-instanser i samma kluster.
>
>Om instanserna finns i olika kluster kan den primära administratören ha samma användarnamn eller e-postadress. Du kan visa klustret som din instans är på under [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Customer Info].

### Kontrollera om ditt användarnamn är unikt i din instans

Kontrollera att användarnamnet och e-postadressen är unika i den aktuella [!DNL Workfront]-instansen:

{{step-1-to-users}}

1. I listan med personer kan du kontrollera i kolumnen **[!UICONTROL Email]** för att se till att det inte finns några dubbla e-postmeddelanden.
1. Lägg till en kolumn för användarnamn i vyn.

   1. Klicka på **[!UICONTROL Customize View]** i listrutan **[!UICONTROL View]**.
   1. Klicka på **[!UICONTROL Add Column]**.
   1. Skriv *[!UICONTROL username]* i sökfältet.
   1. Välj **[!UICONTROL User]** > **[!UICONTROL Username]**.
   1. Spara vyn.\
      Detta resulterar i en vy där användarnamnen visas där du kan leta efter kopian.

1. Kontrollera i kolumnen **[!UICONTROL Username]** i listan över personer att det inte finns några dubbletter av användarnamn.

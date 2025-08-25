---
title: Konfigurera  [!DNL Workfront] och [!DNL Frame.io] integreringen
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Som  [!DNL Adobe Workfront] administratör kan du integrera [!DNL Workfront] med [!DNL Frame.io] och ge din organisation ett smidigt sätt att granska och godkänna resurser.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
hide: true
hidefromtoc: true
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Konfigurera integreringen [!DNL Workfront] och [!DNL Frame.io]

Workfront-administratören aktiverar integreringen mellan Workfront och Frame.io genom att konfigurera standardkontot för Frame.io under Konfigurera och sedan ange Frame.io-användare i Workfront. Detta gör att projektsamordnaren kan planera och initiera arbetet med Workfront-projekt samt granska och godkänna arbetsflöden.


## Åtkomstkrav

>[!IMPORTANT]
>
>Den här funktionen är bara tillgänglig för organisationer som har anslutit till [!DNL Adobe Admin Console].

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plan</td>
   <td>Alla</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licenser
   </td>
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>Nytt: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>

</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera ett standardkonto för [!DNL Frame.io] [!BADGE Kommer snart]{type=Informative}

När ett standardkonto för [!DNL Frame.io] har konfigurerats har projekt som skapats i [!DNL Workfront] ett spegelprojekt skapats i Frame.io.

>[!IMPORTANT]
>
>Den här funktionen kommer snart. För närvarande läggs Frame.io-konton till manuellt av Workfront-teamet. Kontakta din Adobe-kontorepresentant om du behöver hjälp.

## Konfigurera ett enskilt Frame.io-konto med en Workfront-grupp

Du kan ansluta en enda Workfront-grupp med ett enda Frame.io-konto som skiljer sig från standardkontot.

Så här konfigurerar du ett Frame.io-konto med en Workfront-grupp:

{{step-1-to-setup}}

1. Klicka på **Grupper** i den vänstra panelen.
1. Välj en befintlig grupp eller klicka på **Skapa grupp**.
1. Klicka på **Anslut till bildruta.io** i den vänstra panelen.
1. Ange API-utvecklartoken.
1. Klicka på **Initiera anslutning**.
1. (Villkorligt) Om du är administratör för mer än ett Frame.io-konto väljer du det konto som du vill använda.

## Aktivera Frame.io-användare

Workfront-användare som regelbundet använder Frame.io bör markeras som Frame.io-användare. Workfront-administratörer kan ange Frame.io-användare i Workfront användarprofil.

>[!TIP]
>
>Vi rekommenderar att användare som regelbundet arbetar med kreativa verktyg kan aktivera och överföra material för granskning och godkännande som Frame.io-användare.

När en användare har markerats som en Frame.io-användare i Workfront och läggs till i ett projekt:

* De läggs till som medarbetare i Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* De kan skicka material från Frame.io till Workfront för granskning och godkännande.
* De kan visa information i den enkelriktade synkroniseringsmappen från Workfront. [!BADGE Kommer snart]{type=Informative}

Så här aktiverar du användare av Frame.io:

{{step-1-to-users}}

1. Markera en eller flera användare och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .
1. Aktivera kryssrutan Lägg till i projekt i Frame.io i åtkomstavsnittet och välj sedan **Yes** i listrutan.
   ![Lägg till i bildruteprojekt](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Om den här rutan inte är markerad behåller användaren åtkomst till tidigare tilldelningar och läggs till i Frame.io-projekt som flyttas framåt.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->

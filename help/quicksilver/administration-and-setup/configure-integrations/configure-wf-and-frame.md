---
title: Konfigurera [!DNL Workfront] och [!DNL Frame.io] integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Som en [!DNL Adobe Workfront] administratör kan du integrera [!DNL Workfront] med [!DNL Frame.io] och ge organisationen ett smidigt sätt att granska och godkänna resurser.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---


# Konfigurera [!DNL Workfront] och [!DNL Frame.io] integration

Workfront-administratören aktiverar integreringen mellan Workfront och Frame.io genom att konfigurera standardkontot för Frame.io under Konfigurera och sedan ange Frame.io-användare i Workfront. Detta gör att projektsamordnaren kan planera och initiera arbetet med Workfront-projekt samt granska och godkänna arbetsflöden.


## Åtkomstkrav

>[!IMPORTANT]
>
>Den här funktionen är bara tillgänglig för organisationer som har anslutit sig till [!DNL Adobe Admin Console].

Du måste ha följande:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenser</strong>
   </td>
   <td>Aktuell: [!UICONTROL Plan] <br>
   Nytt: [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong>Konfigurationer på åtkomstnivå</strong>
   </td>
   <td>Du måste vara en [!DNL Workfront] administratör.
   </td>
  </tr>

</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Konfigurera en standardinställning [!DNL Frame.io] konto [!BADGE Kommer snart]{type=Informative}

En gång som standard [!DNL Frame.io] konto har konfigurerats, projekt har skapats i [!DNL Workfront] har ett spegelprojekt skapat i Frame.io.

>[!IMPORTANT]
>
>Den här funktionen kommer snart. För närvarande läggs Frame.io-konton till manuellt av Workfront-teamet. Kontakta din kontorepresentant på Adobe om du behöver hjälp.

## Konfigurera ett enskilt Frame.io-konto med en Workfront-grupp

Du kan ansluta en enda Workfront-grupp med ett enda Frame.io-konto som skiljer sig från standardkontot.

Så här konfigurerar du ett Frame.io-konto med en Workfront-grupp:

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen **Grupper**.
1. Välj en befintlig grupp eller klicka på **Skapa grupp**.
1. Klicka på i den vänstra panelen **Anslut till bildruta.io**.
1. Ange API-utvecklartoken.
1. Klicka **Initiera anslutning**.
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

1. Markera en eller flera användare och klicka sedan på **Redigera** icon ![](assets/edit-icon.png).
1. Aktivera kryssrutan Lägg till i projekt i bildruta.io i Access-avsnittet och markera sedan **Ja** i listrutan.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Om den här rutan inte är markerad behåller användaren åtkomst till tidigare tilldelningar och läggs till i Frame.io-projekt som flyttas framåt.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->


---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installera [!DNL Adobe Workfront] för [!DNL Jira]
description: Du kan använda  [!DNL Adobe Workfront] for [!DNL Jira] för att integrera dina [!DNL Jira] och [!DNL Workfront] system.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Installera [!DNL Adobe Workfront for Jira]

Du kan använda [!DNL Adobe Workfront for Jira] för att integrera dina [!DNL Jira]- och [!DNL Workfront]-system.

När du har installerat tillägget kan du definiera arbetsflöden som skapar [!DNL Jira] utgåvor automatiskt när [!DNL Workfront] arbetsobjekt skapas. Objekten i båda programmen länkas och en del av deras information kan uppdateras automatiskt i båda systemen.

Alla användare i [!DNL Workfront] och [!DNL Jira] kan dra nytta av den här integreringen. De behöver bara en licens för det system där de arbetar mest, inte för båda systemen.

Det här tillägget är tillgängligt för versionerna [!UICONTROL Server] och [!UICONTROL OnDemand] (eller [!UICONTROL Cloud]) av programvaran [!DNL Jira]. Det här tillägget är inte tillgängligt för [!DNL Data Center]-versionen av programvaran [!DNL Jira].

En lista över [!DNL Jira] versioner som [!DNL Workfront for Jira] stöder finns på [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) på Atlassian Marketplace.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> 
   <p>Nytt: Alla</p>
   <p>Aktuell: [!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Översikt över licenser för Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nytt: Standard</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt! Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Du måste vara en [!DNL Workfront]-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installera [!DNL Workfront] för [!DNL Jira]

Installation av [!DNL Workfront] för [!DNL Jira] OnDemand är identisk med installation på en [!DNL Jira]-serverinstans.

Du måste vara administratör för [!DNL Jira] för att kunna installera tillägget [!DNL Workfront].

Om du inte är administratör för [!DNL Jira] kan du bläddra efter tillägget [!DNL Workfront] och begära att det installeras. Din begäran skickas till administratören för [!DNL Jira] för godkännande och installation.

Mer information om hur du begär att ett tillägg ska installeras i ditt [!DNL Jira]-program finns i [Hantera användarförfrågningar för tillägg.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Installera [!DNL Workfront for Jira]:

1. Logga in på [!DNL Jira] som [!DNL Jira]-administratör.
1. Hitta tillägget **[!DNL Workfront for Jira]** i [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Klicka på **[!UICONTROL Get it now]** för att installera den.

   När installationen är klar kan du logga in på [!DNL Workfront] från [!DNL Jira] och konfigurera integreringen.

   Mer information finns i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Överväganden för en [!DNL Jira Server]-installation

>[!NOTE]
>
>Dessa krav gäller inte för programversionen [!UICONTROL OnDemand] ([!UICONTROL Cloud]) av [!DNL Jira].

Även om installationen av [!DNL Workfront]-tillägget i de två [!DNL Jira]-miljöerna liknar varandra måste du tänka på följande när du arbetar med en [!DNL Jira Server]-installation:

* När tillägget konfigureras i [!DNL Jira] kanske adressen som anges i fältet **[!DNL JIRA Base URL]** inte är samma URL som du använder för att komma åt [!DNL Jira] på din privata server. **[!DNL JIRA Base URL]** måste vara en offentligt tillgänglig adress som är ansluten till din privata server med NAT- eller omvända proxyprotokoll, så att [!DNL Workfront] kan komma åt den för att göra förfrågningar till servern.

* Du måste använda SSL-kryptering för att säkra kommunikationen mellan [!DNL Jira] och [!DNL Workfront]. När du aktiverar SSL måste du ha en fullständig SSL-certifikathög från en certifikatutfärdare. Vi stöder inte självsignerade certifikat.
* Du måste se till att domänen [!DNL jira.workfront.com] är tillgänglig från dina företagsservrar. Den fungerar som en mellanliggande programmiljö mellan [!DNL Workfront] och [!DNL Jira] och krävs för att tilläggsprogrammet ska fungera.

  Du måste också lägga till följande statiska IP-adresser till tillåtelselista på brandväggen för utgående och inkommande anslutningar.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Mer information om hur du konfigurerar brandväggen för optimal funktionalitet med [!DNL Workfront] finns i [Konfigurera brandväggen](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

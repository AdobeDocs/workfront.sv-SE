---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installera [!DNL Adobe Workfront] for [!DNL Jira]
description: Du kan använda [!DNL Adobe Workfront] for [!DNL Jira] integrera [!DNL Jira] och [!DNL Workfront] system.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Installera [!DNL Adobe Workfront for Jira]

Du kan använda [!DNL Adobe Workfront for Jira] integrera [!DNL Jira] och [!DNL Workfront] system.

När du har installerat tillägget kan du definiera arbetsflöden som skapar [!DNL Jira] automatiskt när [!DNL Workfront] arbetsobjekt skapas. Objekten i båda programmen länkas och en del av deras information kan uppdateras automatiskt i båda systemen.

Alla användare i [!DNL Workfront] och [!DNL Jira] kan dra nytta av den här integreringen. De behöver bara en licens för det system där de arbetar mest, inte för båda systemen.

Det här tillägget är tillgängligt för [!UICONTROL Server] och [!UICONTROL OnDemand] (eller [!UICONTROL Cloud]) versioner av [!DNL Jira] Programvara. Det här tillägget är inte tillgängligt för [!DNL Data Center] version av [!DNL Jira] Programvara.

För en lista med [!DNL Jira] versioner som [!DNL Workfront for Jira] för närvarande stöds, se [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) på Atlassian Marketplace.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licensöversikt</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt: Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] att ägna sig åt den här integreringen, i stället för att använda befintliga integreringar som kan vara kopplade till användarna.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Installera [!DNL Workfront] for [!DNL Jira]

Installerar [!DNL Workfront] for [!DNL Jira] OnDemand är identiskt med att installera det på en [!DNL Jira] Serverinstans.

Du måste vara en [!DNL Jira] administratör för att installera [!DNL Workfront] tillägg.

Om du inte är en [!DNL Jira] -administratör kan du bläddra efter [!DNL Workfront] tillägg och begära att det installeras. Din förfrågan skickas till [!DNL Jira] administratör för godkännande och installation.

Mer information om hur du begär ett tillägg som ska installeras på din [!DNL Jira] program, se [Hantera användarförfrågningar för tillägg.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Installera [!DNL Workfront for Jira]:

1. Logga in på [!DNL Jira] som [!DNL Jira] administratör.
1. Hitta **[!DNL Workfront for Jira]** tillägg i [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Klicka **[!UICONTROL Get it now]** för att installera den.

   När installationen är klar kan du logga in på [!DNL Workfront] från [!DNL Jira] och konfigurera integreringen.
   [!DNL ]
Mer information finns i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Att tänka på vid [!DNL Jira Server] installation

>[!NOTE]
>
>Dessa krav gäller inte för [!UICONTROL OnDemand] ([!UICONTROL Cloud]) version av [!DNL Jira] Programvara.

Även om du installerar [!DNL Workfront] i de två [!DNL Jira] miljöer liknar varandra måste du tänka på följande när du arbetar med en [!DNL Jira Server] installation:

* När tillägget konfigureras i [!DNL Jira], den adress som anges i **[!DNL JIRA Base URL]** fältet får inte vara samma URL som du använder för att komma åt [!DNL Jira] på din privata server. The **[!DNL JIRA Base URL]** måste vara en offentligt tillgänglig adress som är ansluten till din privata server med NAT- eller omvända proxyprotokoll, så [!DNL Workfront] kan komma åt den för att göra förfrågningar till servern.

* Du måste använda SSL-kryptering för att säkra kommunikationen mellan [!DNL Jira] och [!DNL Workfront]. När du aktiverar SSL måste du ha en fullständig SSL-certifikathög från en certifikatutfärdare. Vi stöder inte självsignerade certifikat.
* Du måste se till att [!DNL jira.workfront.com] domänen är tillgänglig från företagets servrar. Den fungerar som en mellanliggande programmiljö mellan [!DNL Workfront] och [!DNL Jira] och krävs för att tilläggsprogrammet ska fungera.

   Du måste också lägga till följande statiska IP-adresser till tillåtelselista på brandväggen för utgående och inkommande anslutningar.

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   Mer information om hur du konfigurerar brandväggen för optimal funktionalitet med [!DNL Workfront], se [Konfigurera brandväggen](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

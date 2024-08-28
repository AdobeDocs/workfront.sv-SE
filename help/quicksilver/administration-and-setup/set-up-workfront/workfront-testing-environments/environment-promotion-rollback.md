---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Återställa ett paket med miljökampanjer
description: Funktionen för att främja miljön är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Lär dig hur du återställer ett installerat kampanjpaket från en målmiljö.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 84a72ab4547a582707351948052fdd59cc57a9d5
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Återställa ett paket med miljökampanjer

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

När du har installerat ett paket kan du återställa det. Detta tar bort de ändringar som paketet gjorde i målmiljön och återställer de berörda objekten till deras tidigare konfigurationer.

Du kan återställa ett kampanjpaket inom 24 timmar efter att det installerats. Efter 24 timmar är återställningsfunktionen inte längre tillgänglig för den installationen.

## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> <p>Nytt: Prime eller Ultimate</p><p>eller</p><p>Aktuell: Inte tillgänglig</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenser</strong>
   </td>
   <td> <p>[!UICONTROL Standard]</p><p>eller</p><p>Aktuell: Inte tillgänglig</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

* Ett miljömarknadsföringspaket måste installeras innan det kan återställas.

  Instruktioner finns i [Installera ett uppgraderingspaket för miljö](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Kontrollera om en specifik paketdistribution kan återställas

Om du vill veta om en specifik paketdistribution kan återställas bör du tänka på följande:

* Det måste ha gått mindre än 24 timmar sedan paketet installerades.
* Endast den senaste paketdistributionen kan återställas.
* En misslyckad distribution kan återställas.
* Återställningar kan inte återställas.


## Återställa ett installerat miljöerbjudande

1. Gå till miljön där paketet installerades.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Välj **Miljökampanj** i den vänstra navigeringen.
1. Markera det paket som du vill återställa och klicka på **Distributioner**.
1. Håll muspekaren över den distribution (installation) som du vill återställa och klicka sedan på Återställ när den visas till höger om distributionsraden.

   eller

   Klicka på den distribution som du vill återställa och klicka sedan på **Återställ paket** i skärmens övre högra hörn.

   >[!IMPORTANT]
   >
   >Distributionen måste ha skett inom 24 timmar innan du återställer den. Installationer som är äldre än 24 timmar kan inte återställas.

1. (Valfritt) I området Förhandsvisa återställning kan du visa de ändringar som kommer att göras när distributionen återställs.
1. Klicka på **Återställ** i skärmens övre högra hörn.








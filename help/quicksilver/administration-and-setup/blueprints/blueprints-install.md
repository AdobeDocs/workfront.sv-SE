---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Installera en plan
description: Du kan installera en plan i din produktionsmiljö eller i en sandlådemiljö.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Installera en plan

Du kan installera en plan i din produktionsmiljö eller i en sandlådemiljö.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront]-licens</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Var ska jag installera en plan? {#where-should-i-install-a-blueprint}

Du kan installera ditt paket i följande miljöer:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produktion</strong></td>
        <td>Produktionen är er livemiljö.</td>
    </tr>
    <tr>
        <td><strong>Förhandsgranska sandlåda</strong></td>
        <td>Sandbox Preview är en testmiljö som fungerar som en kopia av din livemiljö och uppdateras varje helg av Workfront. Alla supportpaket har tillgång till förhandsvisningen av sandlådan. Mer information finns i <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Sandlådemiljö för [!DNL Adobe Workfront] förhandsvisning</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>Sandlådan för anpassad uppdatering är en separat testmiljö som uppdateras manuellt av dig. Det finns en extra kostnad för att hämta den anpassade uppdateringssandlådan. Mer information finns i <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">Anpassad sandlådemiljö för uppdatering [!DNL Adobe Workfront] </a>.</td>
    </tr>
</table>

>[!TIP]
>
>Vi rekommenderar att du först installerar ritningen i en sandlådemiljö. På så sätt kan du testa innehållet i ritningen och se till att den passar organisationen utan att göra ändringar i livedata.

>[!NOTE]
>
>Vissa utkast är bara tillgängliga för installation i förhandsvisningsmiljön i testsyfte. Om du har tillgång till innehåll som bara är för förhandsgranskning i din produktionsmiljö, i sandlåda 1 eller i sandlåda 2, är installationsknappen inte aktiv, och du kan se ett varningsmeddelande.\
>Dessutom är möjligheten att växla mellan olika miljöer begränsad vid åtkomst till innehåll som bara är för förhandsgranskning, även när du befinner dig i förhandsvisningsmiljön.

## Installera ritningen

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront och klicka sedan på **[!UICONTROL Blueprints]**.
1. Hitta den plan du vill installera. Du kan filtrera efter användningsfall, mognadsnivå, installationsstatus och typ till höger.
1. (Valfritt) Klicka på **[!UICONTROL Details]** om du vill veta hur ritningen fungerar.
1. Klicka på **[!UICONTROL Install]**.
1. Välj om du vill installera i din produktionsmiljö eller i en sandlådemiljö.\
   Mer information finns i [Var ska jag installera en plan?avsnittet ](#where-should-i-install-a-blueprint) i den här artikeln.
1. På sidan [!UICONTROL Configure] kan du göra något av följande:

   * Installera ritningen som den är. För ritningstyper som inte kräver någon konfiguration är detta det enda alternativet. För ritningstyper som behöver konfigureras kan du välja att installera ritningen nu och konfigurera den senare. Klicka på **[!UICONTROL Install as is]**.
   * Konfigurera ritningen före installation, för ritningar som behöver konfigureras. Gör dina konfigurationsval och klicka på **[!UICONTROL Install blueprint]**.\

     Mer information finns i [Konfigurera en plan](../../administration-and-setup/blueprints/configure-template-package.md).
När installationen är klar visas ett meddelande med en lista över de specifika objekt (t.ex. roller, team eller grupper) som har installerats med planen och eventuella objekt som inte gick att installera.

När du har installerat ritningen kan ytterligare åtgärder behövas för att den ska kunna distribueras helt. Mer information finns i [Åtgärder som ska vidtas efter att en plan har installerats](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

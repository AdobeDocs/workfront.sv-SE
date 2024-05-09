---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installera Desktop Proofing Viewer för din organisation
description: Desktop Proofing Viewer, som huvudsakligen är avsedd för korrektur av interaktivt innehåll, är ett program som måste installeras på varje användares dator. Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du utföra den här installationen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Installera Desktop Proofing Viewer för din organisation

<!--Audited: 05/2024-->

Desktop Proofing Viewer, som huvudsakligen är avsedd för korrektur av interaktivt innehåll, är ett program som måste installeras på varje användares dator. Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du utföra den här installationen.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Premium eller Select</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administratör måste väljas i din behörighetsprofil för korrektur. Mer information finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurera en användares språkkontroll</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Systemkrav

Desktop Proofing Viewer stöds i följande operativsystem:

* Windows 7 och senare, 32- och 64-bitars
* Mac OS X 10.9 och senare, 64 bitar

## Förutsättningar

Om du vill att användare ska kunna använda Desktop Proofing Viewer måste du konfigurera systemet så att Desktop Proofing Viewer startas som standardvy för interaktiva korrektur före installationen.

## Konfigurera Desktop Proofing Viewer som standard för interaktiva korrektur

När du har installerat Desktop Proofing Viewer för din organisation kan du ange det som standardvisningsprogram för interaktiva korrektur.

{{step1-to-proofing}}

1. Klicka **Kontoinställningar** i det övre högra hörnet av Workfront Proof och klicka sedan på **Inställningar** -fliken.

1. Under **Korrekturinställningar**, i slutet av **Desktop Proofing Viewer for Interactive proofing** rad, klicka **Inställningar**.

   ![Korrekturinställningar](assets/proof-defaults.png)

1. Klicka **Aktiverad och standard** och sedan klicka **Spara**.

## Installera Desktop Proofing Viewer för dina användare

* [Installera Desktop Proofing Viewer på Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Installera Desktop Proofing Viewer i Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Installera Desktop Proofing Viewer på Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Hämta appen genom att göra något av följande på användarens dator:

   * Om du använder produktionsmiljön klickar du på [Mac Production Download for the Desktop Proofing Viewer](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * Om du använder förhandsvisningsmiljön klickar du på [Mac Preview Download for the Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. Öppna filen som du just laddat ned för att starta installationen.
1. I installationsrutan som visas klickar du på **Fortsätt** och sedan klicka **Installera**.

   ![Installationsruta](assets/install-wf-proof-box.png)

1. Se till att alla användare slutför installationen genom att öppna ett interaktivt korrektur från dokumentområdet i Workfront.

### Installera Desktop Proofing Viewer i Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Hämta appen genom att göra något av följande på användarens dator:

   * I produktionsmiljön klickar du på [Windows Production-nedladdning för Desktop Proofing Viewer](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * I förhandsgranskningsmiljön klickar du på [Windows Preview-hämtning för Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Öppna filen som du just laddat ned för att starta installationen.
1. I säkerhetsvarningsrutan som visas klickar du på **Kör**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   Desktop Proofing Viewer installeras och körs.

1. (Villkorligt) Om du installerar programmet med Internet Explorer uppdaterar du startsidan i webbläsaren när programmet har installerats.
1. Se till att alla användare slutför installationen genom att öppna ett interaktivt korrektur från dokumentområdet i Workfront.

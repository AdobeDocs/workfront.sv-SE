---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: inaktivera,offentlig,dela,korrektur,offentlig,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Inaktivera delning av korrektur via offentlig URL eller inbäddningskod
description: Du kan inaktivera möjligheten att dela ett korrektur med en offentlig URL eller bädda in kod som korrektur eller som bevis för enskilda användare.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Inaktivera delning av korrektur via offentlig URL eller inbäddningskod

Du kan inaktivera möjligheten att dela ett korrektur med en offentlig URL eller bädda in kod som korrektur eller som bevis för enskilda användare.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Inaktivera per korrektur

Du måste vara korrekturägare eller skapare, eller också måste du ha rollen som författare eller moderator.

1. Klicka på **Dokument** i den vänstra panelen i det projekt som innehåller korrekturet.
1. Håll pekaren över korrekturet och välj **Dokumentinformation** .
1. I den vänstra panelen klickar du på **Inställningar för språkgranskning** och inaktiverar sedan kryssrutan **Tillåt delning av korrektur via offentlig URL eller bädda in kod** .

   ![](assets/proofing-viewer-settings-350x200.png)

1. Klicka på **Spara**.

## Inaktivera per användare

Du kan inaktivera inställningen för publikt korrektur för enskilda användare i din Workfront-instans. Du måste ha en behörighetsprofil för administratör för att kunna göra den här ändringen.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Korrektur**.
1. Klicka på **Kontoinställningar** i det övre högra hörnet.
1. Klicka på fliken **Användare** och sedan på namnet på en användare.
1. Inaktivera kryssrutan **Offentlig delning** i avsnittet **Standardkorrekturinställningar**.

   ![](assets/default-proof-settings--public-sharing-350x210.png)

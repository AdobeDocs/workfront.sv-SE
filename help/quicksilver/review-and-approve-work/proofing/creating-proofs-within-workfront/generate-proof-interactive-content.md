---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett korrektur för interaktivt innehåll i en ZIP-fil
description: Du kan generera ett korrektur för interaktivt innehåll som inte finns på webbplatsen och som lagras i en ZIP-fil. Exempel på den här typen av webbinnehåll är bl.a. annonser med direktuppspelad video eller ljud, HTML-animeringar och interaktiva banners.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Skapa ett korrektur för interaktivt innehåll i en ZIP-fil

Du kan generera ett korrektur för interaktivt innehåll som inte finns på webbplatsen och som lagras i en ZIP-fil. Exempel på den här typen av webbinnehåll är bl.a. annonser med direktuppspelad video eller ljud, HTML-animeringar och interaktiva banners.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Gammal plan: Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Skapa ett korrektur för interaktivt innehåll i en ZIP-fil

När du lägger till interaktivt innehåll i en ZIP-fil till ett korrektur skapar Adobe Workfront ett korrektur av de zippade dokumenten. Beroende på filstorleken kan överföringstiden variera. Det tar längre tid att skapa större filer. Du kan navigera bort från sidan och Workfront fortsätter att skapa filen. Den maximala filöverföringsstorleken är 4 GB. 

1. Förbered innehållet genom att skapa en paketerad ZIP-fil.

   ZIP-filen måste uppfylla följande krav:

   * Alla resurser, som CSS, JavaScript, videor, ljud och bilder, ska inkluderas i paketfilen.
   * Kontrollera att huvudfilen (till exempel index.html, index.htm) finns i rotmappen och att det är den enda .html/.htm-filen som lagras där.

     Om huvudfilen inte placeras i rotmappen söker Workfront igenom mappen för att hitta huvudfilen.

   * Största paketstorlek är 500 MB.
   * När det gäller ZIP-filer som skapats i iOS identifierar verktyget automatiskt rätt mapp där innehållet placeras.

1. Gå till projektet, aktiviteten eller utgåvan där du vill överföra ZIP-filen.
1. Klicka på **Dokument** i den vänstra panelen.
1. Klicka på **Lägg till ny** och sedan på **Korrektur** på den meny som visas.
1. I avsnittet **Lägg till filer** drar och släpper du eller bläddrar efter den ZIP-fil du behöver.
1. Klicka på **Skapa korrektur** om du vill skapa ett enkelt korrektur utan någon granskningsprocess.\
   eller\
   Fortsätt genom att konfigurera ett avancerat korrektur:

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

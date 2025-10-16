---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett korrektur för interaktivt innehåll i en ZIP-fil
description: Du kan generera ett korrektur för interaktivt innehåll som inte finns på webbplatsen och som lagras i en ZIP-fil. Exempel på den här typen av webbinnehåll är bl.a. annonser med direktuppspelad video eller ljud, HTML-animationer och interaktiva banners.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Skapa ett korrektur för interaktivt innehåll i en ZIP-fil

Du kan generera ett korrektur för interaktivt innehåll som inte finns på webbplatsen och som lagras i en ZIP-fil. Exempel på den här typen av webbinnehåll är bl.a. annonser med direktuppspelad video eller ljud, HTML-animationer och interaktiva banners.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Standard</p>
   <p>Arbete eller plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

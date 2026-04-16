---
title: Bevilja åtkomst till varumärkesbehörigheter
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du konfigurera varumärkesbehörigheter genom att skapa en användargrupp i Admin Console och tilldela GenStudio systemhanterarproduktprofil.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Ge åtkomst till varumärkesbehörigheter

Användarna får behörighet att skapa, redigera och publicera varumärket för Adobe GenStudio systemhanterare när de läggs till i en användargrupp.

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
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console-behörigheter</td> 
   <td> <p>Du måste vara systemadministratör i Adobe Admin Console.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Krav

* Enhetliga godkännanden måste vara aktiverat för din Workfront-instans.

* Din organisation måste ha GenStudio Foundation.
   * Content Reviewer i Workfront innehåller de funktioner som är tillgängliga i GenStudio Foundation för granskning och godkännande av resurser. Du behöver inte komma åt GenStudio Foundation direkt för att slutföra arbetet. Din åtkomst till GenStudio Foundation-funktioner via Content Reviewer följer villkoren i ditt Workfront-avtal.
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands.
Mer information om hur du signerar avtalet finns i [Signera Adobe Gen AI-avtalet](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## &#x200B;1. Konfigurera varumärkesbehörigheter i Admin Console

### Steg 1: Skapa en användargrupp

Skapa en ny användargrupp i Admin Console som hanterar behörigheter för att skapa och redigera varumärken.

### Steg 2: Tilldela en produktprofil till användargruppen

Det berättigande som är kopplat till den tilldelade profilen ger alla användare i gruppen GenStudio Brands behörigheter (skapa, uppdatera och ta bort varumärken).

Tilldela en profil:

1. Navigera till den nya användargruppen.
1. Klicka på fliken **Tilldelade produktprofiler**.
1. Klicka på **Tilldela profil**.
1. På popup-menyn väljer du **Adobe GenStudio** i produktlistan och klickar sedan på **Använd**.
1. Välj profilen för **Adobe GenStudio Foundation-redigerare**.
1. Klicka på **Använd**.
1. Klicka på **Spara**.

### Steg 3: Lägg till användare i användargruppen

Om du vill tilldela användarbehörigheter för att skapa, redigera och publicera varumärken lägger du till dem i användargruppen.

>[!NOTE]
>
>Du måste lägga till minst en användare innan du lägger till gruppen i ett projekt enligt beskrivningen i steg 4.

Så här lägger du till användare:

1. Gå till **Admin Console** > **Användare** > **Användargrupper**.
1. Välj användargrupp.
1. Lägg till användare efter användarnamn eller e-postadress.
1. Välj bland förslag på matchningar för befintliga användare.

### Steg 4: Skapa ett varumärkesprojekt

Ett projekt ger en lagringsplats där användarna kan spara varumärkesresurser.

Så här skapar du ett projekt:

1. Gå till fliken **Lagring** i Admin Console.
1. Klicka på **Projekt**.
1. Klicka på **Skapa projekt**.
1. Ange projektnamnet **Adobe GenStudio Brands** på popup-menyn.

   >[!IMPORTANT]
   >
   >Ange projektnamnet exakt som det visas. Lägg inte till extra blanksteg eller ändra skiftläget.

1. Klicka på **Skapa**.

### Steg 5: Bjud in användargruppen till projektet

Lägg till användargruppen i varumärkesprojektet så att de kan komma åt och hantera resurser.

1. Lägg till användargruppen som du skapade i popup-fönstret **Bjud in till projekt** .
1. Välj **Kan redigera**-behörigheter.
1. Klicka på **Bjud in**.

### Resultat

Användare i gruppen har nu behörighet att skapa, redigera och publicera varumärkesresurser i Workfront.

## &#x200B;2. Bevilja åtkomst till varumärken i Workfront åtkomstnivåer

Du måste slutföra alla steg i föregående avsnitt innan du ger enskilda användare åtkomst till varumärken på Workfront åtkomstnivåer.

>[!IMPORTANT]
>
>* Endast användare som är tilldelade användargruppen med GenStudio systemhanterarproduktprofil i Admin Console kan skapa, redigera och publicera varumärken i Workfront, även om andra användare har tillgång till varumärken som är aktiverade i sina åtkomstnivåinställningar.
>* Användare som läggs till på åtkomstnivån med åtkomst till varumärken aktiverad men som inte lagts till i användargruppen i Admin Console kan bara visa varumärken.


Så här ger du varumärken i Workfront åtkomst:

{{step-1-to-setup}}

1. Klicka på **Åtkomstnivåer** i den vänstra panelen.
1. Hitta den åtkomstnivå som du vill redigera och klicka sedan på redigeringsikonen ![redigeringsikonen](assets/edit-icon.png) för att redigera den.

   eller

   Klicka på **Ny åtkomstnivå** om du vill skapa en ny åtkomstnivå. Mer information om hur du skapar åtkomstnivåer finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Bläddra ned till **Ange ytterligare begränsningar** och välj sedan **Tillåt användare att komma åt varumärken**.
   ![tillåt åtkomst till varumärkesinställningen](assets/access-for-brands.png)
1. Klicka på **Spara**.

När du har konfigurerat varumärken kan du skapa en Content Reviewer som granskar resurser mot varumärkesriktlinjerna i arbetsflödet för granskning och godkännande. Mer information finns i [Konfigurera AI-medarbetare](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

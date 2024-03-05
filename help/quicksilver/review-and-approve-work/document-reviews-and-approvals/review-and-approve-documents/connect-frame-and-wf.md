---
product-area: projects
navigation-topic: approvals
title: Connect Workfront and Frame.io
description: Workfront använder Frame.io i gransknings- och godkännandeprocessen för att möta personer där de vill arbeta. Projekthanteringen och godkännandeprocessen hanteras i Workfront och granskningsprocessen görs i Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: cf8501ff21dc9f3a3c66d8e98555986f18aeaa80
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Connect Workfront and Frame.io

Workfront använder Frame.io i gransknings- och godkännandeprocessen för att möta personer där de vill arbeta. Projekthanteringen och godkännandeprocessen hanteras i Workfront och granskningsprocessen slutförs i Frame.io. Du måste slutföra alla följande avsnitt för att kunna konfigurera integreringen:

* [Koppla en Workfront-grupp till ett Frame.io-team](#connect-a-workfront-group-to-a-frameio-team)
* [Skapa ett Workfront-projekt och lägg till en ansluten grupp](#create-a-workfront-project-and-add-a-connected-group)

Innehållet i den här artikeln hänvisar till den uppdaterade funktionen för dokumentgodkännande som bara är tillgänglig för specifika konton. Mer information om standardgodkännandeprocesser finns i artiklarna i [Arbetsgodkännanden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Åtkomstkrav

* Din organisation måste vara manuellt registrerad för att kunna använda de funktioner som beskrivs i den här artikeln. Mer information finns i [Adobe Workfront och Frame.io native integration alpha: översikt](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).


## Koppla en Workfront-grupp till ett Frame.io-team

Vi förbättrar aktivt den här funktionen för allmän tillgänglighet i maj.

### Förutsättningar

* Skapa ett Frame.io-team för att mappa till en Workfront-grupp.
* Hitta API-utvecklartoken för teamet. Mer information finns i [Tokens för utvecklare](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) på utvecklingswebbplatsen Frame.io.

### Koppla en Workfront-grupp till ett Frame.io-team

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen **Grupper**.
1. Välj en befintlig grupp eller klicka på **Skapa grupp**.
1. Klicka på i den vänstra panelen **Anslut till bildruta.io**.
   ![](assets/connect-frame-group.png)
1. Ange API-utvecklartoken.
1. Klicka **Initiera anslutning**.
1. (Villkorligt) Om du är administratör för mer än ett Frame.io-konto väljer du det konto som du vill använda.

## Skapa ett Workfront-projekt och lägg till en ansluten grupp

När du har anslutit en Workfront Group till ett Frame.io-team måste du skapa ett projekt med den anslutna gruppen.

### Förutsättningar

* Du måste ha en Workfront-grupp ansluten till ett Frame.io-team enligt beskrivningen i föregående avsnitt.

### Skapa ett Workfront-projekt och lägg till en ansluten grupp

{{step1-to-projects}}

1. Skapa ett nytt projekt från grunden eller en mall. Mer information om hur du skapar ett projekt finns i [Skapa ett projekt](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. I den vänstra panelen hittar du **Projektinformation**.

1. Hitta **Grupp** till höger på skärmen och ta bort gruppen Standard.

1. I listrutan hittar du önskad grupp. Grupper som är anslutna till Frame.io visar ikonen Frame.io.
   ![](assets/add-frame-group.png)

1. Gör eventuella andra ändringar av projektkonfigurationen.

1. Klicka **Spara ändringar**.

1. Fortsätt till nästa avsnitt.

### Lägg till en uppgift och ange integreringsstatusen till Aktiv

>[!NOTE]
>
>Underaktiviteter stöds för närvarande inte i anslutna Frame.io-projekt.


1. Skapa de uppgifter du behöver fylla i i Frame.io

1. Välj de uppgifter du behöver och klicka sedan på **Redigera**.

1. Bläddra till **Anpassad Forms** och hitta Frame.io-integreringsformuläret.

   >[!IMPORTANT]
   >
   >En ansluten Frame.io-grupp måste tilldelas i området Projektinformation för att formuläret ska visas. Mer information finns i [Skapa ett Workfront-projekt och lägg till en ansluten grupp](#create-a-workfront-project-and-add-a-connected-group) i den här artikeln.


1. Aktivera **Aktivitetens integreringsstatus** och välj **Aktiv**.
   ![](assets/frame-custom-form.png)

1. Klicka **Spara ändringar**. En Frame.io-ikon visas bredvid projektnamnet.

1. Tilldela användare eller team till uppgifter.

   >[!NOTE]
   >
   >Användare eller team som läggs till i uppgifterna läggs också till i Frame.io-projektet.

1. Ladda upp alla dokument och all annan information i projektdokumentområdet.

Projektet är fortfarande inte anslutet, du måste fortsätta till nästa avsnitt för att slutföra integreringen.

### Aktivera projektet i Frame.io

1. Ändra projektstatus från **Planering** till **Aktuell** eller en anpassad status som är lika med aktuell. Integreringen slutförs och projektet, åtgärderna och eventuella dokument i Frame.io genereras.

Ikonen Frame.io bredvid projektnamnet visas med en lila signal om att integreringen lyckades. Användarna får ett e-postmeddelande med en inbjudan till Frame.io-projektet.

>[!IMPORTANT]
>
>När projektet har anslutits för Frame.io återspeglas ändringar som görs i projektgruppen inte i Frame.io.



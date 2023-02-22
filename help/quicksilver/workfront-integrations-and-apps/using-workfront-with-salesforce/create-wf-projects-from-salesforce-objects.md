---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt
description: Efter installation [!DNL Adobe Workfront] för Salesforce kan du definiera utlösare som skapar [!DNL Workfront] projekt när vissa kriterier uppfylls [!DNL Salesforce] Affärsmöjligheter och konton.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt

Efter installation [!DNL Adobe Workfront] för Salesforce kan du definiera utlösare som skapar [!DNL Workfront] projekt när vissa kriterier uppfylls [!DNL Salesforce] [!UICONTROL Opportunities] och [!UICONTROL Accounts].

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda de funktioner som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Att skicka in [!DNL Workfront] begäran från en [!DNL Salesforce] [!UICONTROL Opportunity] eller Konto kontrollerar att du har följande i din miljö:

* Dina [!DNL Workfront] administratören har installerat [!DNL Workfront for Salesforce].\
   Mer information om installation [!DNL Workfront for Salesforce], se [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Dina [!DNL Workfront] administratören har lagt till [!DNL Workfront] till [!UICONTROL Opportunity] och Sidlayouter för konto.\
   Mer information om hur du lägger till [!DNL Workfront] till en sidlayout, se [Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Du har en [!DNL Workfront] kontot och du kan logga in på det från [!DNL Workfront] -avsnittet i [!UICONTROL Opportunity] eller Konto .

## Konfigurera skapande av [!DNL Workfront] Projekt från [!DNL Salesforce]

* [Så här skapar du projekt automatiskt](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Konfigurera utlösare](#configuring-triggers-configuring-triggers)
* [Om projektnamn](#understanding-project-names-understanding-project-names)

### Så här skapar du projekt automatiskt {#understanding-the-automatic-creation-of-projects}

Som [!DNL Salesforce] systemadministratör kan du definiera utlösare som automatiskt kan skapa projekt i [!DNL Workfront] när följande saker händer i [!DNL Salesforce]:

* The [!UICONTROL Stage] av [!UICONTROL Opportunity] uppdateras.
* The [!UICONTROL Type] för ett konto uppdateras.

Utlösare kan bara konfigureras efter att du har installerat [!DNL Workfront for Salesforce].  \
Mer information om installation [!DNL Workfront for Salesforce], se [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Tänk på följande när du konfigurerar utlösare för att skapa automatiskt [!DNL Workfront] projekt när [!DNL Salesforce] objekt skapas eller uppdateras:

* Du måste vara en [!DNL Salesforce] och [!DNL Workfront] systemadministratör för att konfigurera utlösare.
* När du har konfigurerat utlösarna kan alla som uppdaterar [!UICONTROL Stage] av [!UICONTROL Opportunity] eller [!UICONTROL Type] av ett konto kan göra att en [!DNL Workfront] projekt. Detta inkluderar [!DNL Salesforce] användare som inte har [!DNL Workfront] konto.
* Det finns ingen gräns för hur många utlösare du kan ha.
* Du kan inte skapa flera utlösare baserat på samma villkor. Utlösare är unika som standard.
* När projektet har skapats länkas det automatiskt till affärsmöjligheten eller kontot där det skapades. Länken kan inte brytas när den har upprättats.
* En affärsmöjlighet eller ett konto kan länkas till flera projekt i [!DNL Workfront] när ett utlöst villkor har uppfyllts flera gånger under affärsmöjlighetens eller kontots livstid.

   Om du till exempel definierar mer än en [!UICONTROL Stage] för [!UICONTROL Opportunity] för att utlösa ett projekt skapas ett projekt för varje definierad fas som affärsmöjligheten når, så länge affärsmöjligheten varar. Om du uppdaterar [!UICONTROL Stage] av [!UICONTROL Opportunity] från en definierad fas till en annan och sedan uppdatera den till den definierade fasen, skapas ett andra projekt för andra gången du uppdaterar [!UICONTROL Stage] till samma definierade fas.

* Ett projekt i [!DNL Workfront] kan bara länkas till en affärsmöjlighet eller ett konto i [!DNL Salesforce] vid en given tidpunkt, men inte till båda samtidigt.

### Konfigurera utlösare {#configuring-triggers}

När du har konfigurerat utlösarna skapas [!DNL Workfront] projekt är aktiverade för båda [!UICONTROL Salesforce Classic] eller [!DNL Lightning Experience] ramverk.

Så här konfigurerar du utlösare i [!UICONTROL Salesforce]:

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. (Villkorligt) i [!DNL Salesforce Classic], klicka **[!UICONTROL Setup]** och under **[!UICONTROL Build]** sektion, expandera **[!UICONTROL Lightning Bolt]**.

   eller

   I [!DNL Salesforce] Lightning Experience, klicka på **[!UICONTROL Setup]icon** sedan **[!UICONTROL Setup]** och under **[!UICONTROL PLATFORM TOOLS]** expandera **[!UICONTROL Apps]**.

1. Klicka på **[!UICONTROL Installed Packages]**.

   Observera att **[!DNL Workfront]** paketet har installerats.

1. Klicka **[!UICONTROL Configure]** nästa **[!DNL Workfront]**.

1. Logga in på [!DNL Workfront] som systemadministratör.

   The **[!UICONTROL Triggers]** visas.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Klicka på **[!UICONTROL New Trigger]**.
1. Från **[!UICONTROL [!DNL Salesforce] Object]** nedrullningsbar meny, välja **[!UICONTROL Opportunity]**.

   Detta är ett obligatoriskt fält.

1. (Villkorligt) Ange följande:

   1. Från **[!UICONTROL Stage]** väljer du en **[!UICONTROL Stage]**.\

      När en affärsmöjlighet når [!UICONTROL Stage] anges här, skapas ett projekt i [!DNL Workfront]. Detta är ett obligatoriskt fält.

   1. I **[!UICONTROL Portfolio or Program]** fält, börja skriva namnet på Portfolio eller programmet där du vill att projektet ska placeras [!DNL Workfront]markerar du den när den visas i listan.\

      Om du inte anger ett Portfolio eller ett program skapas det nya projektet och läggs till i [!UICONTROL Projects I Own] lista över den användare som är inloggad på [!DNL Workfront] när utlösarna konfigureras. Användaren är också projektägare för det nya projektet.

   1. Börja skriva namnet på en mall som du vill associera med den nya mallen [!DNL Workfront] och sedan markera det när det visas i listan.\

      Detta är ett obligatoriskt fält.


      >[!NOTE]
      >
      >Om du har angett en mallägare i mallen som du tänker använda för den här integreringen blir det projektägaren för det nya projektet. De nya projekten visas under [!UICONTROL Projects I Own] lista över den användare som är ägare till det nya projektet, enligt mallen.

   1. (Valfritt) Välj **[!UICONTROL Create a new project for each sold product type]fält** om du vill skapa ett nytt projekt för varje typ av produkt som säljs i ett och samma projekt.
   1. (Villkorligt) Välj en **[!UICONTROL Product]** i **[!UICONTROL Product]** nedrullningsbar meny.

      Detta är ett obligatoriskt fält.

   1. (Villkorligt) Börja skriva namnet på en **[!UICONTROL Template]** som du vill associera med den nya [!DNL Workfront] projektet om den angivna produkten finns på [!UICONTROL Opportunity]. Markera den när den visas i listan.

      Detta är ett obligatoriskt fält.

      Projektet som skapades när en ny produkt lades till i [!DNL Salesforce] affärsmöjligheten placeras i samma Portfolio eller program som valts ut för affärsmöjligheten.

      >[!IMPORTANT]
      >
      >Projektet skapas endast när scenen uppdateras på [!UICONTROL Opportunity]. Ett unikt projekt skapas för varje produkt som anges när scenfältet uppdateras, och inte när produkterna läggs till i [!UICONTROL Opportunities].

1. (Valfritt) Klicka på **[!UICONTROL New Trigger]**.
1. (Valfritt) Från **[!UICONTROL [!DNL Salesforce] Object]** väljer du **Konto **.

   Detta är ett obligatoriskt fält.
1. (Villkorligt) Ange följande:

   1. Välj en **[!UICONTROL Type]** från **[!UICONTROL Type]** nedrullningsbar meny.

      När ett **Konto ** anges som **[!UICONTROL Type]** anges här i [!DNL Salesforce], a **[!UICONTROL Project]** skapas i [!DNL Workfront].

      Detta är ett obligatoriskt fält.

   1. (Valfritt) Börja skriva namnet på en **[!UICONTROL Portfolio]** eller **[!UICONTROL Program]** där du vill att projektet ska placeras [!DNL Workfront] i **[!UICONTROL Portfolio or Program]** markerar du det när det visas i listan.

      Om du inte anger ett Portfolio eller ett program skapas det nya projektet och läggs till i **[!UICONTROL Projects I Own]** lista över den användare som är inloggad på [!DNL Workfront] från [!DNL Salesforce]. Användaren är också projektägare för det nya projektet.

   1. Börja skriva namnet på en **[!UICONTROL Template]** som du vill associera med den nya [!DNL Workfront] och sedan markera det när det visas i listan.

      Detta är ett obligatoriskt fält.

      >[!NOTE]
      >
      >Om du har angett en mallägare i mallen som du tänker använda för den här integreringen blir det projektägaren för det nya projektet. De nya projekten visas under **[!UICONTROL Projects I Own]** lista över den användare som är ägare till det nya projektet, enligt mallen.
   ![salesforce_triggers_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Klicka på **[!UICONTROL Save]**.

   [!DNL Workfront] projekt genereras nu varje gång någon av utlösarna uppfylls.

### Om projektnamn {#understanding-project-names}

Beroende på vilken utlösare som genererade projekten, namnen på projekten i [!DNL Workfront] kan följa något av dessa mönster:

* Om projektet skapas baserat på en affärsmöjlighet eller kontoutlösare är projektets namn: *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Om projektet skapas baserat på en utlösare som även innehåller en ny produkt, är projektets namn: *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Visa [!DNL Workfront] projekt

Om [!DNL Workfront] administratören lade till [!DNL Workfront] till [!UICONTROL Opportunity] eller Sidlayouten Konto kan du se projekt som skapats automatiskt i [!UICONTROL Projects] -fliken i det här avsnittet.\
Mer information om hur du lägger till [!DNL Workfront] till sidlayouten i ett [!UICONTROL Opportunity] eller Konto, se [Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Du måste ha en [!DNL Workfront] och loggas in på [!DNL Workfront] för att visa [!UICONTROL Projects] -fliken.

Visa projekt som skapats från en [!UICONTROL Opportunity] eller Konto:

1. Gå till en [!UICONTROL Opportunity] eller Konto .
1. Gå till **[!DNL Workfront]** -avsnitt.

   >[!NOTE]
   >
   >Beroende på hur [!DNL Workfront] administratören konfigurerade det här avsnittet. Det kan ha ett annat namn.

1. Välj **[!UICONTROL Projects]** -fliken.

   Alla projekt som skapas av definierade utlösare visas på den här fliken. Alla användare i [!DNL Salesforce] som även har en [!DNL Workfront] konto och vem som kan ha behörighet att se dessa projekt i [!DNL Workfront] kan även se dem i [!DNL Salesforce] för [!UICONTROL Opportunity] eller kontot som genererade dem.

   Du kan visa följande information om de projekt som har skapats av integreringen:

   * Projektnamn
   * Referensnummer
   * Anmälningsdatum
   * Ägarens namn
   * Status
   * Villkor
   * Planerat slutförandedatum
   * Procent färdigt

      När den här informationen uppdateras i [!DNL Workfront]kan du se fälten som uppdateras i den här listan.

1. (Valfritt) Klicka på namnet på ett projekt för att öppna det i Workfront.
1. (Valfritt) Klicka på [!UICONTROL **[!UICONTROL Go to Salesforce]**] i [!UICONTROL Project Details] -området eller projektrubriken för att komma åt [!UICONTROL Opportunity] eller kontot där projektet kom från. Systemadministratören eller gruppadministratören måste lägga till [!UICONTROL Integrations] till layoutmallen för att hitta den i projektrubriken.

   >[!NOTE]
   >
   >The [!UICONTROL Go to Salesforce] länk är synlig för alla [!DNL Workfront] -användare som kan visa projektet. Du måste ha en [!DNL Salesforce] för att kunna gå till [!DNL Salesforce] Möjligheter eller konto som projektet skapades från.

---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt
description: När du har installerat [!DNL Adobe Workfront] för Salesforce kan du definiera utlösare som skapar [!DNL Workfront] projekt när vissa villkor uppfylls för  [!DNL Salesforce] säljprojekt och konton.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce]-objekt

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Integreringen av Workfront för Salesforce kommer inte att vara tillgänglig efter den **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Salesforce.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Salesforce finns i [Salesforce-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

När du har installerat [!DNL Adobe Workfront] för Salesforce kan du definiera utlösare som skapar [!DNL Workfront]-projekt när vissa villkor uppfylls för [!DNL Salesforce] [!UICONTROL Opportunities] och [!UICONTROL Accounts].

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
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Skicka en [!DNL Workfront]-begäran från ett [!DNL Salesforce] [!UICONTROL Opportunity] eller konto
Kontrollera att du har följande i din miljö:

* [!DNL Workfront]-administratören har installerat [!DNL Workfront for Salesforce].\
   Mer information om att installera [!DNL Workfront for Salesforce] finns i [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Din [!DNL Workfront]-administratör har lagt till avsnittet [!DNL Workfront] i din [!UICONTROL Opportunity] och ditt konto
sidlayouter.\
   Mer information om hur du lägger till avsnittet [!DNL Workfront] i en sidlayout finns i [Konfigurera avsnittet  [!DNL Adobe Workfront] för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Du har ett [!DNL Workfront]-konto och du kan logga in på det från avsnittet [!DNL Workfront] i ditt [!UICONTROL Opportunity]- eller konto
.

## Konfigurerar skapande av [!DNL Workfront] projekt från [!DNL Salesforce]

* [Så här skapar du projekt automatiskt](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Konfigurera utlösare](#configuring-triggers-configuring-triggers)
* [Förstå projektnamn](#understanding-project-names-understanding-project-names)

### Så här skapar du projekt automatiskt {#understanding-the-automatic-creation-of-projects}

Som [!DNL Salesforce]-systemadministratör kan du definiera utlösare som automatiskt kan skapa projekt i [!DNL Workfront] när följande saker händer i [!DNL Salesforce]:

* [!UICONTROL Stage] för en [!UICONTROL Opportunity] har uppdaterats.
* [!UICONTROL Type] för ett konto
uppdateras.

Utlösare kan bara konfigureras efter att du har installerat [!DNL Workfront for Salesforce].  \
Information om hur du installerar [!DNL Workfront for Salesforce] finns i [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Tänk på följande när du konfigurerar utlösare för att automatiskt skapa [!DNL Workfront] projekt när [!DNL Salesforce] objekt skapas eller uppdateras:

* Du måste vara [!DNL Salesforce] och [!DNL Workfront]-systemadministratör för att kunna konfigurera utlösare.
* När du har konfigurerat utlösarna kan alla som uppdaterar [!UICONTROL Stage] för ett [!UICONTROL Opportunity] eller [!UICONTROL Type] för ett konto
kan utlösa att ett [!DNL Workfront] -projekt skapas. Detta inkluderar [!DNL Salesforce] användare som inte har något [!DNL Workfront]-konto.
* Det finns ingen gräns för hur många utlösare du kan ha.
* Du kan inte skapa flera utlösare baserat på samma villkor. Utlösare är unika som standard.
* När projektet har skapats länkas det automatiskt till affärsmöjligheten eller kontot där det skapades. Länken kan inte brytas när den väl har upprättats.
* En affärsmöjlighet eller ett konto kan länkas till flera projekt i [!DNL Workfront] när ett utlöst villkor har uppfyllts flera gånger under affärsmöjlighetens eller kontots livstid.

  Om du till exempel definierar mer än en [!UICONTROL Stage] för en [!UICONTROL Opportunity] som ska utlösa ett projekt, skapas ett projekt för varje definierad fas som affärsmöjligheten når under affärsmöjlighetens livstid. Om du uppdaterar [!UICONTROL Stage] för en [!UICONTROL Opportunity] från en definierad fas till en annan och sedan uppdaterar den tillbaka till den definierade scenen skapas ett andra projekt för andra gången du uppdaterar fältet [!UICONTROL Stage] till samma definierade fas.

* Ett projekt i [!DNL Workfront] kan bara länkas till en affärsmöjlighet eller ett konto i [!DNL Salesforce] vid en given tidpunkt, men inte till båda samtidigt.

### Konfigurera utlösare {#configuring-triggers}

När du har konfigurerat utlösarna aktiveras processen för att skapa [!DNL Workfront]-projekt för både [!UICONTROL Salesforce Classic]- och [!DNL Lightning Experience]-ramverk.

Konfigurera utlösare i [!UICONTROL Salesforce]:

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. (Villkorligt) Klicka på [!DNL Salesforce Classic] i **[!UICONTROL Setup]** och expandera **[!UICONTROL Build]** under avsnittet **[!UICONTROL Lightning Bolt]**.

   eller

   I [!DNL Salesforce] Lightning Experience klickar du på ikonen **[!UICONTROL Setup]**, sedan på **[!UICONTROL Setup]** och under **[!UICONTROL PLATFORM TOOLS]** expandera **[!UICONTROL Apps]**.

1. Klicka på **[!UICONTROL Installed Packages]**.

   Observera att paketet **[!DNL Workfront]** har installerats.

1. Klicka på **[!UICONTROL Configure]** bredvid **[!DNL Workfront]**.

1. Logga in på [!DNL Workfront] som systemadministratör.

   Sidan **[!UICONTROL Triggers]** visas.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Klicka på **[!UICONTROL New Trigger]**.
1. Välj **[!UICONTROL [!DNL Salesforce] Object]** i listrutan **[!UICONTROL Opportunity]**.

   Detta är ett obligatoriskt fält.

1. (Villkorligt) Ange följande:

   1. Välj en **[!UICONTROL Stage]** i listrutan **[!UICONTROL Stage]**.\

      När en affärsmöjlighet når den [!UICONTROL Stage] som anges här skapas ett projekt i [!DNL Workfront]. Detta är ett obligatoriskt fält.

   1. I fältet **[!UICONTROL Portfolio or Program]** börjar du skriva namnet på en Portfolio eller ett program där du vill att projektet ska placeras i [!DNL Workfront] och markerar det sedan när det visas i listan.\

      Om du inte anger en Portfolio eller ett program skapas det nya projektet och läggs till i listan [!UICONTROL Projects I Own] för användaren som är inloggad på [!DNL Workfront] när utlösarna konfigureras. Användaren är också projektägare för det nya projektet.

   1. Börja skriva namnet på en mall som du vill associera med det nya [!DNL Workfront]-projektet och markera det sedan när det visas i listan.\

      Detta är ett obligatoriskt fält.


      >[!NOTE]
      >
      >Om du har angett en mallägare i mallen som du tänker använda för den här integreringen blir det projektägaren för det nya projektet. De nya projekten visas i listan [!UICONTROL Projects I Own] för den användare som är ägare av det nya projektet, enligt mallen.

   1. (Valfritt) Välj fältet **[!UICONTROL Create a new project for each sold product type]** om du vill skapa ett nytt projekt för varje typ av produkt som säljs inom ett affärstillfälle.
   1. (Villkorligt) Välj en **[!UICONTROL Product]** i listrutan **[!UICONTROL Product]**.

      Detta är ett obligatoriskt fält.

   1. (Villkorligt) Börja skriva namnet på **[!UICONTROL Template]** som du vill associera med det nya [!DNL Workfront]-projektet om den angivna produkten finns i [!UICONTROL Opportunity]. Markera den när den visas i listan.

      Detta är ett obligatoriskt fält.

      Det projekt som skapas när en ny produkt läggs till i affärsmöjligheten [!DNL Salesforce] placeras i samma Portfolio eller Program som valts för affärsmöjligheten.

      >[!IMPORTANT]
      >
      >Projektet skapas endast när scenen uppdateras på [!UICONTROL Opportunity]. Ett unikt projekt skapas för varje produkt som anges när scenfältet uppdateras, och inte när produkterna läggs till i [!UICONTROL Opportunities].

1. (Valfritt) Klicka på **[!UICONTROL New Trigger]**.
1. (Valfritt) Välj **Konto i listrutan &#x200B;** [!UICONTROL [!DNL Salesforce] Object]**
**.

   Detta är ett obligatoriskt fält.
1. (Villkorligt) Ange följande:

   1. Välj en **[!UICONTROL Type]** i listrutan **[!UICONTROL Type]**.

      Vid ett **konto
**&#x200B; anges som &#x200B;** [!UICONTROL Type] **&#x200B; som anges här i [!DNL Salesforce], en &#x200B;** [!UICONTROL Project]** skapas i [!DNL Workfront].

      Detta är ett obligatoriskt fält.

   1. (Valfritt) Börja skriva namnet på **[!UICONTROL Portfolio]** eller **[!UICONTROL Program]** där du vill att projektet ska placeras i [!DNL Workfront] i fältet **[!UICONTROL Portfolio or Program]** och markera det sedan när det visas i listan.

      Om du inte anger en Portfolio eller ett program skapas det nya projektet och läggs till i listan **[!UICONTROL Projects I Own]** för användaren som är inloggad på [!DNL Workfront] från [!DNL Salesforce]. Användaren är också projektägare för det nya projektet.

   1. Börja skriva namnet på **[!UICONTROL Template]** som du vill associera med det nya [!DNL Workfront]-projektet och markera det sedan när det visas i listan.

      Detta är ett obligatoriskt fält.

      >[!NOTE]
      >
      >Om du har angett en mallägare i mallen som du tänker använda för den här integreringen blir det projektägaren för det nya projektet. De nya projekten visas i listan **[!UICONTROL Projects I Own]** för den användare som är ägare av det nya projektet, enligt mallen.

   ![salesforce_triggers_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Klicka på **[!UICONTROL Save]**.

   [!DNL Workfront] projekt genereras nu varje gång någon av utlösarna uppfylls.

### Förstå projektnamn {#understanding-project-names}

Beroende på vilken utlösare som genererade projekten kan projektnamnen i [!DNL Workfront] följa något av följande mönster:

* Om projektet skapas baserat på en affärsmöjlighet eller kontoutlösare är projektets namn: *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Om projektet skapas baserat på en affärsmöjlighetsutlösare som även innehåller en ny produkt, är projektets namn: *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Visa [!DNL Workfront] projekt

Om [!DNL Workfront]-administratören har lagt till avsnittet [!DNL Workfront] i din [!UICONTROL Opportunity] eller ditt konto
sidlayout kan du se de projekt som skapas automatiskt på fliken [!UICONTROL Projects] i det här avsnittet.\
Mer information om hur du lägger till avsnittet [!DNL Workfront] i sidlayouten för ett [!UICONTROL Opportunity] eller konto
, se [Konfigurera  [!DNL Adobe Workfront] avsnittet för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md) .

Du måste ha ett [!DNL Workfront]-konto och vara inloggad på [!DNL Workfront] för att kunna visa fliken [!UICONTROL Projects].

Så här visar du projekt som skapats från ett [!UICONTROL Opportunity] eller konto
:

1. Gå till ett [!UICONTROL Opportunity] eller konto
.
1. Gå till avsnittet **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Beroende på hur administratören för [!DNL Workfront] konfigurerade det här avsnittet kan det ha ett annat namn.

1. Klicka på fliken **[!UICONTROL Projects]**.  

   Alla projekt som skapas av definierade utlösare visas på den här fliken. Alla användare i [!DNL Salesforce] som också har ett [!DNL Workfront]-konto och som kan ha behörighet att se de här projekten i [!DNL Workfront] kan också se dem i [!DNL Salesforce] för [!UICONTROL Opportunity] eller kontot
som genererade dem.

   Du kan visa följande information om de projekt som har skapats av integreringen:

   * Projektnamn
   * Referensnummer
   * Anmälningsdatum
   * Ägarens namn
   * Status
   * Villkor
   * Planerat slutförandedatum
   * Procent färdigt

     När den här informationen uppdateras i [!DNL Workfront] kan du se fälten uppdaterade i den här listan.

1. (Valfritt) Klicka på namnet på ett projekt för att öppna det i Workfront.
1. (Valfritt) Klicka på [!UICONTROL **[!UICONTROL Go to Salesforce]**] i området [!UICONTROL Project Details] eller projekthuvudet för att komma åt [!UICONTROL Opportunity] eller kontot
där projektet har sitt ursprung. Systemet eller gruppadministratören måste lägga till fältet [!UICONTROL Integrations] i layoutmallen för att kunna hitta det i projekthuvudet.

   >[!NOTE]
   >
   >Länken [!UICONTROL Go to Salesforce] är synlig för alla [!DNL Workfront]-användare som kan visa projektet. Du måste ha ett [!DNL Salesforce]-konto för att kunna gå till [!DNL Salesforce]-säljprojektet eller kontot som projektet skapades från.

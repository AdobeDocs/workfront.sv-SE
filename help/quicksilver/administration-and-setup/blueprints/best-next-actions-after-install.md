---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Åtgärder som ska vidtas efter installation av en skiss
description: I den här artikeln beskrivs vad du bör göra efter att du har installerat en plan i  [!DNL Adobe Workfront] för att fullständigt distribuera den till dina systemanvändare.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 0%

---

# Åtgärder som ska vidtas efter installation av en plan

I den här artikeln beskrivs vad du bör göra efter att du har installerat en plan i [!DNL Adobe Workfront] för att fullständigt distribuera den till systemanvändarna.

* [Rekommendationer för projektmallar](#project-template-recommendations)
* [Rekommendationer för organisationsstruktur](#organizational-structure-recommendations)
* [Instrumentpanelsrekommendationer](#dashboard-recommendations)

## Rekommendationer för projektmallar {#project-template-recommendations}

Det här avsnittet innehåller rekommendationer för de projektmallar som installeras med dina ritningar.

### Tilldela användare till nyligen skapade roller och team {#assign-users-to-newly-created-roles-and-teams}

De roller och/eller team som skapas under processen för planinstallation har inte användare som kopplas till dem automatiskt. Om du inte tilldelar användare till nya roller eller team skapar du arbete för en funktion som ingen kan hämta. I vissa fall kan du behöva skapa nya användare för att kunna fylla i dessa roller och team. Mer information om hur du skapar nya användare finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Använda ett anpassat formulär i mallen och malluppgifterna {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Installationsprocessen kopplar inte projektmallen till några anpassade formulär. Om dina projekt eller uppgifter kräver att specifika formulär eller fält fylls i för att skapa en enhetlig rapportering, eller om ditt digitala begärandeformulär innehåller fält som behöver behållas på projektnivå, rekommenderar vi att du associerar mallen eller malluppgifterna med dessa formulär. Mer information finns i [Lägga till ett anpassat formulär i ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Uppdatera varaktighet för malluppgift och uppskattningar av arbetsinsats {#update-template-task-duration-and-effort-estimates}

Varje aktivitet i mallen innehåller en planerad varaktighet och planerad ansträngningsberäkning. Dessa uppskattningar fungerar som en utgångspunkt för varaktighet och tid för dessa aktiviteter. Organisationens funktioner, färdigheter och tempo är dock unika. Du bör granska varje uppgifts beräknade varaktighet och arbetsinsats för att justera den efter organisationens behov. Mer information finns i [Hantera aktivitetsinformation i [!UICONTROL Task Details Overview]-området](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Koppla en milstolpe och milstolpar {#associate-a-milestone-path-and-milestones}

Installationsprocessen kopplar inte projektmallen till en milstolpe-sökväg. Använd en milstolpe för mallen och använd milstolpar på viktiga uppgifter i mallen för att stödja dina behov av milstolpe-rapportering. Mer information finns i [Associera milstolpar med uppgifter](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Fyll i mallen för ditt team {#roll-out-the-template-to-your-team}

Ta fram utbildningsmaterial för både de arbetsledare som ska använda den här mallen och de medarbetare som ska utföra arbetet i projektmallen.

### Skapa eller uppdatera rapporter och kontrollpaneler {#create-or-update-reports-and-dashboards}

Om lösningen representerar en ny typ av arbete som din organisation inte har utfört tidigare i [!DNL Workfront], kan du behöva skapa nya rapporter och instrumentpaneler för att stödja arbetet. Mer information finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) och [Skapa en kontrollpanel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Om lösningen liknar det arbete som du redan har utfört i [!DNL Workfront] bör du verifiera att arbetet matas in i befintliga rapporter och instrumentpaneler som förväntat. Om den inte matas in i din befintliga rapportering ska du vidta åtgärder för att uppdatera filter eller skapa nya rapporter.

## Rekommendationer för organisationsstruktur {#organizational-structure-recommendations}

Det här avsnittet innehåller rekommendationer för de organisationsstrukturelement som installeras med dina utkast.

### Företag

Efter installation av en plan som innehåller ett företag:

* Lägg till ett anpassat formulär för att förstärka företagets post med användbar information (formuläret och dess detaljer är unika för dig). Mer information finns i [Lägga till ett anpassat formulär i ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Om företaget representerar en kund ska du granska de åsidosättningsfrekvenser som är kopplade till företaget. Mer information finns i [Åsidosätta faktureringstariffer för jobbroller på företagsnivå](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Om företaget representerar en kund och om det finns andra projektmallar som är unika för just den organisationen måste du först associera projektmallarna med det nya företaget. Mer information finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Om företaget representerar en kund eller leverantör ska du associera befintliga användare från den externa organisationen som redan finns i din miljö. Mer information finns i [Skapa och redigera företag](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Om företaget representerar en kund eller leverantör skapar du ytterligare medarbetaranvändare för den externa organisationen som du kan behöva i din miljö för att effektivisera kommunikation, utförande av arbete och godkännanden. Mer information om hur du skapar nya användare finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Uppdatera organisationsschemans relationer för alla användare som nu är kopplade till det nyligen tillagda företaget. Mer information finns i [Skapa direkta rapporter](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) och [Visa organisationsschemat](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Mer information om företag finns i [Skapa och redigera företag](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Instrumentpanelsrekommendationer {#dashboard-recommendations}

Det här avsnittet innehåller rekommendationer för kontrollpaneler och rapporter som installeras med en plan.

### Uppdatera de nya instrumentpanelerna för att lägga till/ta bort rapporter

Kontrollpanelerna som läggs till från en plan har en eller flera rapporter, externa sidor eller kalendrar. Det är troligt att du antingen inte behöver alla rapporter och andra instrumentpanelselement, eller att du måste utöka instrumentpanelen med befintliga rapporter, externa sidor och kalendrar innan den kan delas med andra. Mer information finns i [Lägga till en rapport på en instrumentpanel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Uppdatera nyskapade rapporter för att lägga till/ta bort kolumner eller filtervillkor

Rapporterna som distribueras via en instrumentpanelsplan har inte alla kolumner eller filtervillkor som stöder konfigurationen av [!DNL Workfront]. Du förväntas göra vissa justeringar av rapporterna så att de passar dina standarder. Om du vill skapa konsekvens med andra rapporter i miljön kanske du vill lägga till en kolumn som du inkluderar i alla rapporter för objektet som visas, eller lägga till filtervillkor som begränsar resultaten till en viss projekttyp eller användargrupp. Mer information finns i [Skapa eller redigera vyer](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) och [Skapa eller redigera filter](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Dela paneler och rapporter med användare

Om du inte tänker placera kontrollpanelen i en layoutmall bör du dela kontrollpanelen med de personer som tycker att den är användbar. Mer information finns i [Dela en instrumentpanel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) och [Dela en rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Lägga till kontrollpaneler i layoutmallar

Det bästa sättet att göra information tillgänglig för andra är att lägga till kontrollpaneler i layoutmallar. Identifiera layoutmallarna för de personer som skulle ha nytta av att regelbundet granska kontrollpanelen och lägga till den nya kontrollpanelen i layoutmallarna. Mer information finns i [Skapa och hantera layoutmallar](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Uppdatera andra instrumentpaneler och rapporter

Genom att en ny kontrollpanel och dess rapporter introduceras kan andra befintliga kontrollpaneler och rapporter kasseras och justeras. Ta dig tid att granska era befintliga rapporter för att identifiera överflödiga och motsägelsefulla rapporter.

### Distribuera anpassade data till relevanta formulär

Vissa rapporter som ingår i en kontrollpanelsöversikt har anpassade datafält i antingen vyn, filtret eller grupperingen av rapporten. I vissa fall har designen även ett formulär som dessa fält är kopplade till. I de flesta fall används emellertid inte anpassade fält i anpassade formulär. För att kolumnerna, filtren eller grupperingarna ska fungera på rätt sätt måste dessa fält kopplas till formulär som är kopplade till en användar-, projekt-, uppgift- eller annan objektpost. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

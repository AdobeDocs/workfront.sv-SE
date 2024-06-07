---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över projektets faktiska slutförandedatum
description: Projekt, uppgifter och utgåvor har ett faktiskt slutförandedatum i Adobe Workfront. Detta är det datum då projektet, aktiviteten eller utgåvan markerades som slutförd.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Översikt över projektets faktiska slutförandedatum

Projekt, uppgifter och utgåvor har ett faktiskt slutförandedatum i Adobe Workfront. Detta är det datum då projektet, aktiviteten eller utgåvan markerades som slutförd.

## Faktiska slutförandedatum

Faktiskt slutförandedatum representerar realdatum och realtid när arbetet är slutfört. När en uppgift eller ett problem har markerats som Klar eller Fullständig anger Workfront automatiskt datumet för statusändringen för objektet som faktiskt slutförandedatum för uppgiften eller problemet. Om det datumet inte är en korrekt återgivning av när uppgiften eller problemet faktiskt slutfördes, kan du redigera det faktiska slutförandedatumet manuellt.

Du kan till exempel markera en uppgift eller ett problem Klar på måndag, men du vet att arbetet slutfördes föregående fredag. När du har markerat uppgiften eller problemet som färdigt kan du manuellt uppdatera aktivitetens eller utställningens verkliga slutförandedatum till föregående fredag för att återspegla det verkliga slutförandet.

Du kan inte redigera det faktiska slutförandedatumet för ett projekt manuellt, men du kan ändra status manuellt för ett projekt, vilket kan utlösa en ändring av projektets faktiska slutförandedatum.

Det faktiska slutförandedatumet för ett projekt anges på följande sätt:

* Genom att manuellt uppdatera projektets status: Om projektets slutföringsläge är inställt på Manuellt och du manuellt ändrar status för projektet till Fullständigt, utlöser detta projektets faktiska slutförandedatum som ska uppdateras till datumet och tiden för den senaste slutförda uppgiften.
* När den sista uppgiften i projektet slutförs automatiskt: Om projektets slutföringsläge är inställt på Automatiskt och du markerar den sista uppgiften som Fullständig eller uppdaterar det faktiska slutförandedatumet för den senaste uppgiften, uppdateras även projektets verkliga slutförandedatum med det datumet.

  Mer information om hur du ställer in ett projekts slutföringsläge finns i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront använder det faktiska slutförandedatumet från projektets uppgift som slutfördes sist som det faktiska slutförandedatumet för hela projektet.

En Workfront- eller gruppadministratör avgör om Workfront använder dagens datum, det planerade slutförandedatumet för en uppgift eller ett problem när dessa är inställda på Fullständigt eller Stängt. Mer information om hur du anger inställningar för åtgärder och problem finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Hitta faktiska slutförandedatum

Faktiskt slutförandedatum finns i följande områden i Workfront:

* Områdena Projekt, Uppgift och Utleveransinformation
* Redigera projekt-, uppgifts- och problemrutor
* Området Projekt, Uppgift och Utgåva uppdateringar som en systemuppdatering.
* Projekt-, uppgifts- eller utgivningslistor eller rapporter.

Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

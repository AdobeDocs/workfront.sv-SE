---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Översikt över knappen Arbeta på den och Klar
description: När du har tilldelats en uppgift eller ett problem kan du använda en sammanhangsberoende knapp som ändrar namn och funktion beroende på hur du är inblandad i arbetsuppgiften.
author: Becky and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Översikt över knappen Arbeta på den och Klar

När du har tilldelats en uppgift eller ett problem kan du använda en sammanhangsberoende knapp som ändrar namn och funktion beroende på hur du är inblandad i arbetsuppgiften.

Med hjälp av kontextknappen för att acceptera eller slutföra arbetsobjekt kan du låta Adobe Workfront uppdatera flera fält på objekten utan att behöva uppdatera dem manuellt.

Knapparna Work On It (Arbeta på) och Done (Klar) är synliga för användare som har:

* En standardlicens (ny) eller en plan- eller arbetslicens (aktuell)
* Begränsad redigeringsåtkomst eller högre för uppgiften eller problemet

>[!NOTE]
>
>Knappen Klar visas som Markera som färdig i alla områden av Workfront.

## Arbeta med knappnamnen och Klar

Beroende på vilket område av Workfront du kommer åt uppgiften eller utgåvan från kan du ändra namn med knappen Arbeta på den eller Klar, enligt följande scenarier:

* När uppgiften eller utgåvan först tilldelas dig och statusen är Ny visas knappen Arbeta på den.

  ![Knappen Arbeta på den](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >Du kan ersätta knappen Arbeta med knappen Start. Mer information om hur du ersätter knappen Arbeta på den med knappen Start finns i [Ersätta knappen Arbeta på den med knappen Start](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* När du har klickat på Work On It accept ändras knappen till Mark as done. Mer information om var du kan komma åt knappen Arbeta på den finns i avsnittet [Hitta knappen Arbeta på det och Klar](#locate-the-work-on-it-and-done-button) i den här artikeln.

  ![Knappen Markera som färdig](assets/nwe-mark-as-done-button-350x122.png)


<!--If you are not the only one assigned to the task or issue and you are accessing your work item from the My Work widget in the Home area, the button changes to Done with my part.

  ![Home left Done with my part button](assets/home-left-done-with-my-part-button-350x184.png)-->

## Leta reda på knappen Arbeta på och Klart {#locate-the-work-on-it-and-done-button}

Du kan hitta knappen Arbeta med och Klar i följande områden i Workfront:

* Hem-området i widgeten Mitt arbete

  Mer information om hur du markerar ett objekt som Klar i hemområdet finns i [Markera ett objekt som Klar i hemområdet](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* I huvudet på uppgiften eller utgåvan

  Mer information om objektrubrikerna finns i [Nya objektrubriker](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* På aktivitets- eller ärendesammanfattningspanelen

  Mer information om hur du använder panelen Sammanfattning finns i [Översikt över sammanfattning](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Översikt över fält som uppdateras automatiskt när du klickar på knapparna Work On It eller Done

Fördelen med att använda knapparna Work On It (Arbeta på) och Done (Klar) är att du kan låta Workfront automatiskt uppdatera information om arbetsuppgiften som du har tilldelats.

* [Knappen Arbeta på den](#work-on-it-button)
* [Startknapp](#start-button)
* [Knappen Klar](#the-done-button)

### Knappen Arbeta på den {#work-on-it-button}

När du klickar på Arbeta på det uppdateras även följande objekt:

* Tilldelningsstatusuppdateringar från Begärd till aktuell

  >[!TIP]
  >
  >Fältet Tilldelningsstatus visas bara i rapporter och listor. Mer information om fältet Tilldelningsstatus finns i [Ordlistan för Adobe Workfront-terminologi](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Bekräftelsedatum

  Mer information om implementeringsdatumet finns i [Genomför datumöversikt](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Knappen Start {#start-button}

Om du har tillgång till redigeringsteam kan du ersätta knappen Arbeta med knappen Start för ett team. När användare med det teamet som hemteam klickar på knappen Start för objekt som de har tilldelats, uppdateras ytterligare fält på deras arbetsobjekt automatiskt. Mer information om hur du ersätter knappen Arbeta på den med knappen Start finns i [Ersätt knappen Arbeta på den med knappen Start](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Förutom de fält som uppdateras när du klickar på knappen Work On It (Arbeta på det) uppdateras följande fält automatiskt för en uppgift eller ett problem när du klickar på Start:

* Status
* Faktiskt startdatum

  Mer information om det faktiska startdatumet finns i [Översikt över projektets faktiska startdatum](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Faktiskt slutförandedatum om knappen Start är associerad med en status som är lika med Fullständigt eller Stängt.

  Mer information om det faktiska slutförandedatumet finns i [Översikt över projektets faktiska slutförandedatum](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Om du klickar på Ångra återställs arbetsposten till ursprunglig status och det faktiska startdatumet tas bort.
>
>Knappen Ångra är inte tillgänglig i följande områden:
>
>* Teamförfrågningar
>* Aktivitetshuvud
>

### Knappen Klar {#the-done-button}

Om du har tillgång till redigeringsteam kan du konfigurera Klar-knappen för ett team så att de kan uppdatera uppgiften eller utfärda statusvärden när du markerar ett objekt som slutfört. När användare med det teamet som hemteam klickar på knappen Markera som slutförd för sina objekt uppdateras följande fält automatiskt för en uppgift eller ett problem:

* Status
* Uppdateringar av tilldelningsstatus från Arbeta till Klart
* Faktiskt slutförandedatum

Mer information om hur du konfigurerar Klar-knappen för ett team finns i följande artiklar:

* [Konfigurera Klar-knappen för uppgifter](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Konfigurera Klar-knappen för problem](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)

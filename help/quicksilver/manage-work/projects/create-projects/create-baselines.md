---
product-area: projects
navigation-topic: create-projects
title: Skapa projektbaslinjer
description: En baslinje är en ögonblicksbild av ett projekt som representerar viktig information som ingår i den ursprungliga projektplanen eller vid någon tidpunkt under projektets löptid.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Skapa projektbaslinjer

<!-- Audited: 08/2025 -->

En baslinje är en ögonblicksbild av ett projekt som representerar viktig information som ingår i den ursprungliga projektplanen eller vid någon tidpunkt under projektets löptid.

Du kan använda baslinjen för att jämföra informationen från den aktuella planen med den ursprungliga planen eller någon annan tidpunkt för att identifiera problemuppgifter, krypning av omfång och andra trender över tiden.

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
    <td><p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till projektet eller högre för att visa baslinjer</p> <p>Hantera behörigheter för projektet för att skapa baslinjer</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
    <td><p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på när du arbetar med baslinjer

* Du kan ta en ögonblicksbild av förloppet för ett projekt flera gånger under projektets livstid och skapa flera baslinjer.
* Du kan visa information som ingår i ett projekts baslinjer genom att skapa en baslinje eller genom att skapa en baslinjerapport.
* När du skapar en baslinje hämtas uppgiftsinformationen också till baslinjeuppgifterna för den baslinjen.
* Du kan visa information om baslinjeaktiviteter genom att skapa en rapport för baslinjeaktiviteter.

>[!IMPORTANT]
>
>En baslinje tar en ögonblicksbild av projektets namn, datum och ekonomiska information. Baslinjen inkluderar inte värdena för anpassade fält i projektet. Information om finansiell information som ingår i baslinjen finns i [Projektfinanser ingår i projektbaslinjer](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Skapa en baslinje

Du kan skapa en baslinje på följande sätt:

* **Automatiskt**: Din Workfront-administratör eller en gruppadministratör ställer in projektinställningen för Workfront så att en baslinje skapas automatiskt när ett projekt blir Aktuell. När den här inställningen är aktiverad skapas en baslinje när projektstatusen blir Aktuell. När den här inställningen inte är aktiverad måste du skapa baslinjer manuellt.

  Mer information om hur du konfigurerar projektinställningar och ställer in automatisk baslinje finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >Om du aktiverar den här inställningen skapas automatiskt en baslinje för ett projekt varje gång ett projekts status ändras till Aktuell. Den första skapade baslinjen är standardbaslinjen. Du måste skapa alla andra baslinjer manuellt under projektets livslängd.

* **Manuellt**: Du kan skapa nya baslinjer för projektet efter behov medan projektet fortskrider. Du kan sedan jämföra baslinjer för att se hur projektet fortskrider över tid.

Så här skapar du en baslinje:

1. Gå till ett projekt.
1. Klicka på **Baslinjer** i den vänstra panelen.

   ![Avsnittet Baslinjer i projekt](assets/baselines-section-on-project-with-header.png)

1. Klicka på **Ny baslinje.**
1. Ange namnet på baslinjen.
1. (Valfritt) Om det här är den första baslinjen kanske du vill välja den som standard.
1. Klicka på **Spara**.

   Som standard visas följande information om den baslinje du skapade:

   * Originalnamn
   * Ingångsdatum för baslinje
   * Planerat startdatum för projektet när baslinjen skapades
   * Projektets planerade startdatum när baslinjen skapades
   * Projektets faktiska varaktighet när baslinjen skapades
   * % färdigt för projektet när baslinjen skapades
   * Indikator för standardbaslinje som visar om en baslinje är standardbaslinjen för projektet

     >[!TIP]
     >
     >Du kan inte visa information från två baslinjer samtidigt i samma vy eller rapport. Du kan bara visa information från en viss baslinje och standardbaslinjen i samma rapport. Du kan ändra vilken baslinje du anser vara standardbaslinje när som helst under projektets livslängd.

1. (Valfritt) Klicka på knappen **Visa** och skapa sedan en ny vy eller redigera den aktuella vyn för att lägga till fält i vyn och jämföra ytterligare information mellan baslinjer. Mer information finns i [Skapa eller redigera vyer i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Skapa en rapport för en baslinje eller en baslinjeaktivitet

Om du vill visa baslinjeinformation kan du även skapa en rapport för baslinje- eller baslinjeaktiviteter. På så sätt kan du visa valfritt antal fält om baslinjerna eller baslinjeåtgärderna för att jämföra dem i en vy.

>[!TIP]
>
>Du måste skapa en baslinje innan du kan skapa en uppgiftsrapport för baslinje eller baslinje.

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Vi rekommenderar att du lägger till en projektnamnsgruppering i din rapport över baslinje- eller baslinjeaktiviteter så att det blir enklare att läsa.

Mer information om hur du skapar en gruppering finns i [Skapa grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

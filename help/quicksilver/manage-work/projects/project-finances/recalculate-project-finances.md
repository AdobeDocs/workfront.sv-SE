---
title: Beräkna om projektfinansiering
product-area: projects
navigation-topic: financials
description: Ekonomer beräknas för ett projekt i takt med att förändringar sker i de timmar som är registrerade för projektet eller i de satser som används för att beräkna kostnader och intäkter.
author: Lisa
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '1609'
ht-degree: 0%

---

# Beräkna om projektekonomi

Ekonomer beräknas för ett projekt i takt med att förändringar sker i de timmar som är registrerade för projektet eller i de satser som används för att beräkna kostnader och intäkter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller att beräkna ekonomi i Adobe Workfront

Ekonomer beräknas för projekt på följande sätt:

* Du kan manuellt beräkna om kostnader och intäkter för ett projekt genom att använda alternativet Beräkna om finansiering för ett projekt.
* Dessutom utlöser vissa åtgärder en automatisk omberäkning.

När hastigheten för en användare eller roll ändras under ett projekts livslängd kan följande inträffa:

* När ändringen görs används den uppdaterade tariffen från och med den tidpunkten när timmar loggas och den ekonomiska informationen beräknas. Om du ändrar hastigheten påverkas inte hur saker och ting beräknades innan ändringen gjordes. För alla befintliga loggade timmar används den gamla kursen för att beräkna ekonomisk information.
* Du kan tvinga Adobe Workfront att använda den nya avgiften retroaktivt för alla timmar som har loggats hittills genom att använda alternativet Beräkna om finansiering. Detta tvingar Workfront att retroaktivt beräkna alla tidigare angivna timmar, planerade kostnader och intäkter i enlighet med den nya tariffinformationen.

Rapporttypen Project (Financial Data) utför inte automatiskt en omberäkning av dina ekonomiska data. Om du vill uppdatera data i den här rapporttypen måste du manuellt beräkna om ekonomin för enskilda projekt.

>[!CAUTION]
>
>Innan du manuellt beräknar om ekonomin för ett visst projekt kanske du vill bevara alla ekonomiska data som redan har beräknats till en tidigare sats. Vi rekommenderar att du endast använder alternativet Beräkna om ekonomi när du är säker på att du inte gör ändringar i befintlig information, eller bara när sådana ändringar är önskade.

## Bevara ekonomiska data för uppgifter med befintliga timmar {#preserve-financial-data-for-tasks-with-existing-hours}

När ekonomiska data för ett projekt beräknas om beräknar Workfront retroaktivt alla tidigare loggade timmar, planerade, faktiska kostnader samt planerade och faktiska intäkter, i enlighet med ny eller uppdaterad finansiell information.

* [Bevara projektintäkter](#preserve-project-revenue)
* [Bevara projektkostnad](#preserve-project-cost)

### Bevara projektintäkter  {#preserve-project-revenue}

Inkomstnivåerna kan ändras under ett projekts hela livstid.

Mer information om faktureringstariffer och intäkter finns i artikeln [Översikt över fakturering och intäkter](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Inkomstnivåerna kan ändras på följande nivåer:

* Systemnivån (för jobbroller)\
  Mer information om hur du skapar jobbroller med faktureringsfrekvenser på systemnivå finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Användarnivån\
  Mer information om hur du ändrar faktureringsinformation för användare finns i artikeln [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Företagsnivå (för jobbroller)\
  Mer information finns i [Åsidosätta faktureringstariffer för jobbroller på företagsnivå](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Projektnivån (för jobbroller)\
  Mer information om hur du åsidosätter rollfrekvenser för jobb på projektnivå finns i artikeln [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

En användares faktureringstakt ändras till exempel under ett projekt från 50 till 75 USD per timme och du vill att alla befintliga data ska fortsätta att beräknas till den gamla avgiften ($50 och timme). När projektets ekonomi beräknas om kommer dock befintliga finansiella uppgifter att uppdateras för att återspegla den nya faktureringstakten (75 USD i timmen).

* [Bevara projektintäkter genom att skapa en faktureringspost](#preserve-project-revenue-by-creating-a-billing-record)
* [Bevara projektintäkter genom att använda flera åsidosättningar av faktureringsgrad](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Bevara projektintäkt genom att skapa en faktureringspost {#preserve-project-revenue-by-creating-a-billing-record}

När faktureringspriserna ändras på någon nivå som nämns ovan kan du behålla befintliga intäkter som redan har beräknats i projektet genom att undvika att använda det manuella alternativet för att beräkna om finansiering eller genom att låsa den tid som registrerats i projektet och beräkna med den gamla avgiften i en faktureringspost med statusen Fakturerad.

När du inte beräknar om ekonomin i projektet eller när du låser timmarna som är inloggade i en fakturerad faktureringspost, kommer timmarna som loggas efter prisändringen att beräknas med den nya avgiften, och timmarna som loggas innan kostnadstariffen ändras kommer att beräknas med den gamla kursen.

Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Bevara projektintäkter genom att använda flera åsidosättningar av faktureringsgrad {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

När faktureringstarifferna ändras för jobbroller på projektnivå kan du behålla befintliga intäkter som redan har beräknats i projektet genom att använda flera åsidosättningar av faktureringsfrekvenser som är låsta inom en angiven tidsram.

Mer information om hur du använder flera åsidosättningar av faktureringstariffer finns i artikeln [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Detta gäller endast faktureringstariffer för jobbroller som ändras på projektnivå.

### Bevara projektkostnad {#preserve-project-cost}

Kostnadstarifferna kan ändras på följande nivåer:

* Systemnivå (för jobbroller)\
  Mer information om hur du skapar jobbroller med kostnadstariffer på systemnivå finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Användarnivå\
  Mer information om hur du ändrar information om kostnadstariff för användare finns i artikeln [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

När faktureringspriserna ändras på någon nivå som nämns ovan kan du behålla befintliga kostnader som redan har beräknats i projektet genom att låsa den tid som registrerats i projektet och beräkna med den gamla avgiften i en faktureringspost med statusen Fakturerad. Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

Du kan också undvika att använda alternativet för manuell omberäkning av ekonomi om du inte vill skapa en faktureringspost, vilket beskrivs i avsnittet [Beräkna finanser manuellt för ett projekt](#manually-recalculate-finances-for-a-project) i den här artikeln.

När du inte beräknar om ekonomin i projektet eller när du låser timmarna som är inloggade i en fakturerad faktureringspost, kommer timmarna som loggas efter prisändringen att beräknas med den nya avgiften, och timmarna som loggas innan kostnadstariffen ändras kommer att beräknas med den gamla kursen.

## Omberäkna finanser för ett projekt manuellt {#manually-recalculate-finances-for-a-project}

Om dina priser ändras under ett projekts livslängd och du vill att dina kostnads- och intäktsberäkningar ska återspegla de nya kostnaderna, måste du manuellt beräkna om projektets ekonomi.

>[!NOTE]
>
>Du kan förhindra att intäktsvärden uppdateras för att återspegla de nya satserna när du manuellt beräknar om ekonomi genom att följa stegen i avsnittet [Bevara ekonomiska data för aktiviteter med befintliga timmar](#preserve-financial-data-for-tasks-with-existing-hours) i den här artikeln. Kostnadsvärdena uppdateras alltid för att återspegla de nya kostnaderna när du manuellt beräknar om budgeten för ett projekt.

Du kan beräkna om ekonomin för projekt i Workfront från projektsidan eller från en projektlista eller rapport.

Du kan beräkna om ekonomin samtidigt som du redigerar dem i grupp. Mer information finns i avsnittet [Beräkna finanser manuellt i bulk](#manually-recalculate-finances-in-bulk) i den här artikeln.

1. Gå till projektet där du vill beräkna om ekonomin och klicka på ikonen **Mer** ![Mer meny](assets/qs-more-icon-on-an-object.png) till höger om projektnamnet.

   ![Fler listrutor på projektnivå](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   eller

   Gå till en projektlista eller rapport och välj ett eller flera projekt och klicka sedan på ikonen **Mer** ![Mer-menyn](assets/qs-more-icon-on-an-object.png) överst i listan.

   ![Beräkna om uttryck](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du beräknar om deras ekonomi i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden, tilldelningar eller ett stort antal anpassade fält.

1. Klicka på **Beräkna om ekonomi**.

   Alla planerade kostnader och intäkter för projektet beräknas om med ny information.

   Du bör få en bekräftelse högst upp i webbläsaren på att projektets ekonomi har beräknats korrekt.
Befintliga kostnadsvärden och vissa intäktsvärden som inte har låsts uppdateras för att återspegla de nya tarifferna.

## Manuellt beräkna flera ekonomier åt gången{#manually-recalculate-finances-in-bulk}

Du kan manuellt beräkna om ekonomin för flera projekt genom att redigera dem i grupp. Detta gör att projektintäkterna beräknas om retroaktivt.

>[!IMPORTANT]
>
>Du kan förhindra att intäktsvärden uppdateras för att återspegla de nya satserna när du manuellt beräknar om ekonomi genom att följa stegen i avsnittet [Bevara ekonomiska data för aktiviteter med befintliga timmar](#preserve-financial-data-for-tasks-with-existing-hours) i den här artikeln. Kostnadsvärdena uppdateras alltid för att återspegla de nya kostnaderna när du manuellt beräknar om projektbudgeten.

Så här beräknar du om ekonomin för flera projekt manuellt:

1. Gå till en lista med projekt.
1. Markera flera projekt i listan och klicka sedan på ikonen **Mer** ![Mer ](assets/qs-more-icon-on-an-object.png) överst i listan.

   ![Beräkna om uttryck](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du redigerar dem i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden, tilldelningar eller ett stort antal anpassade fält.

1. Klicka på **Beräkna om ekonomi**.

   Alla planerade kostnader och intäkter för de valda projekten beräknas om med ny information.

   Du bör få en bekräftelse högst upp i webbläsaren på att projektens ekonomi har beräknats korrekt.

## Åtgärder som utlöser en automatisk omberäkning av ekonomin

Följande åtgärder utlöser en ekonomisk omberäkning av projekt i Workfront:

* Ändra aktivitetsstatus
* Flytta en aktivitet med timmar till ett annat projekt
* Ändra projektstatus från Fullständig till aktiv status

>[!NOTE]
>
>När du ändrar projektstatus beräknas endast de planerade värdena om.

Du kan även beräkna om ekonomi manuellt på menyn **Mer** ![Mer](assets/qs-more-menu.png) på projektnivå genom att klicka på **Beräkna om ekonomi**.

---
title: Beräkna om projektekonomi
product-area: projects
navigation-topic: financials
description: Ekonomer beräknas för ett projekt i takt med att förändringar sker i de timmar som är registrerade för projektet eller i de satser som används för att beräkna kostnader och intäkter.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# Beräkna om projektekonomi

Ekonomer beräknas för ett projekt i takt med att förändringar sker i de timmar som är registrerade för projektet eller i de satser som används för att beräkna kostnader och intäkter.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när det gäller att beräkna ekonomi i Adobe Workfront

Ekonomer beräknas i Förbättrad analys på följande sätt:

* Du kan manuellt beräkna om kostnader och intäkter för ett projekt genom att använda alternativet Beräkna om finansiering för ett projekt.
* Dessutom utlöser vissa åtgärder en automatisk omberäkning.

När hastigheten för en användare eller roll ändras under ett projekts livslängd kan följande inträffa:

* När ändringen görs används den uppdaterade tariffen från den tidpunkten när timmar loggas och den ekonomiska informationen beräknas. Om du ändrar hastigheten påverkas inte hur saker och ting beräknades innan ändringen gjordes. För alla befintliga loggade timmar används den gamla kursen för att beräkna ekonomisk information.
* Du kan tvinga Adobe Workfront att använda den nya avgiften retroaktivt för alla timmar som har loggats hittills genom att använda alternativet Beräkna om finansiering. Detta tvingar Workfront att retroaktivt beräkna alla tidigare angivna timmar, planerade kostnader och intäkter i enlighet med den nya tariffinformationen.

>[!CAUTION]
>
>Innan du manuellt beräknar om ekonomin för ett visst projekt kanske du vill bevara alla ekonomiska data som redan har beräknats till en tidigare sats. Vi rekommenderar att du endast använder alternativet Beräkna om ekonomi när du är säker på att du inte gör ändringar i befintlig information, eller bara när sådana ändringar är önskade.

## Bevara ekonomiska data för uppgifter med befintliga timmar {#preserve-financial-data-for-tasks-with-existing-hours}

När ekonomiska data för ett projekt beräknas om beräknar Workfront retroaktivt alla tidigare loggade timmar, planerade, faktiska kostnader samt planerade och faktiska intäkter, i enlighet med ny eller uppdaterad finansiell information.

* [Bevara projektintäkter](#preserve-project-revenue)
* [Bevara projektkostnad](#preserve-project-cost)

### Bevara projektintäkter  {#preserve-project-revenue}

Inkomstnivåerna kan ändras under ett projekts hela livstid.

Mer information om faktureringstariffer och intäkter finns i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Inkomstnivåerna kan ändras på följande nivåer:

* Systemnivån (för jobbroller)\
   Mer information om hur du skapar jobbroller med faktureringssatser på systemnivå finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Användarnivån\
   Mer information om hur du ändrar faktureringsinformation för användare finns i artikeln [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Företagsnivå (för jobbroller)\
   Mer information finns i [Åsidosätt faktureringssatser för jobbroller på företagsnivå](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Projektnivån (för jobbroller)\
   Mer information om hur du åsidosätter rollfrekvenser för jobb på projektnivå finns i artikeln [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

En användares faktureringstaxa ändras till exempel under ett projekt från 50 till 75 USD per timme och du vill att alla befintliga data ska fortsätta att beräknas till den gamla taxan ($50 och timme). När projektets ekonomi beräknas om kommer dock befintliga finansiella uppgifter att uppdateras för att återspegla den nya faktureringstakten (75 USD i timmen).

* [Bevara projektintäkt genom att skapa en faktureringspost](#preserve-project-revenue-by-creating-a-billing-record)
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
   Mer information om hur du skapar jobbroller med kostnadsnivåer på systemnivå finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Användarnivå\
   Mer information om hur du ändrar kostnadstariffen för användare finns i artikeln [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

När faktureringspriserna ändras på någon nivå som nämns ovan kan du behålla befintliga kostnader som redan har beräknats i projektet genom att låsa den tid som registrerats i projektet och beräkna med den gamla avgiften i en faktureringspost med statusen Fakturerad. Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

Du kan också undvika att använda alternativet för manuell omberäkning av finansiering om du inte vill skapa en faktureringspost, vilket beskrivs i avsnittet [Omberäkna finanser för ett projekt manuellt](#manually-recalculate-finances-for-a-project) i den här artikeln.

När du inte beräknar om ekonomin i projektet eller när du låser timmarna som är inloggade i en fakturerad faktureringspost, kommer timmarna som loggas efter prisändringen att beräknas med den nya avgiften, och timmarna som loggas innan kostnadstariffen ändras kommer att beräknas med den gamla kursen.

## Omberäkna finanser för ett projekt manuellt {#manually-recalculate-finances-for-a-project}

Om dina priser ändras under ett projekts löptid och du vill att dina kostnads- och intäktsberäkningar ska återspegla de nya kostnaderna, måste du manuellt beräkna om projektets ekonomi.

>[!NOTE]
>
>Du kan förhindra att intäktsvärdena uppdateras för att återspegla de nya räntorna när du manuellt beräknar om finansiering genom att följa stegen i avsnittet [Bevara ekonomiska data för uppgifter med befintliga timmar](#preserve-financial-data-for-tasks-with-existing-hours) i den här artikeln. Kostnadsvärdena uppdateras alltid för att återspegla de nya priserna när du manuellt beräknar om budgeten för ett projekt.

Du kan beräkna om ekonomin för projekt i Workfront från projektsidan eller från en projektlista eller rapport.

Du kan beräkna om ekonomin samtidigt som du redigerar dem i grupp. Mer information finns i [Automatisk omberäkning av flera ekonomi samtidigt i rutan Redigera projekt](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) i den här artikeln.

1. Gå till projektet där du vill beräkna om ekonomin och klicka på **Mer** icon ![](assets/qs-more-icon-on-an-object.png) till höger om projektnamnet

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   eller

   Gå till en projektlista eller rapport och välj ett eller flera projekt. Klicka sedan på **Mer** icon ![](assets/qs-more-icon-on-an-object.png) högst upp i listan.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du beräknar om deras ekonomi i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden, tilldelningar eller ett stort antal anpassade fält.

1. Klicka **Beräkna om ekonomi**.

   Alla planerade kostnader och intäkter för projektet beräknas om med ny information.

   Du bör få en bekräftelse högst upp i webbläsaren på att projektets ekonomi har beräknats korrekt.\
   Befintliga kostnadsvärden och vissa intäktsvärden som inte har låsts uppdateras för att återspegla de nya tarifferna.

## Automatisk omberäkning av flera ekonomi samtidigt i rutan Redigera projekt {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

Du kan manuellt beräkna om ekonomin för flera projekt genom att redigera dem i grupp. Detta gör att projektintäkterna beräknas om retroaktivt.

>[!IMPORTANT]
>
>Du kan förhindra att intäktsvärdena uppdateras för att återspegla de nya räntorna när du manuellt beräknar om finansiering genom att följa stegen i avsnittet [Bevara ekonomiska data för uppgifter med befintliga timmar](#preserve-financial-data-for-tasks-with-existing-hours) i den här artikeln. Kostnadsvärdena uppdateras alltid för att återspegla de nya kostnaderna när du manuellt beräknar om projektbudgeten.

Så här beräknar du om ekonomin för flera projekt manuellt:

1. Gå till en lista med projekt.
1. Markera flera projekt i listan och klicka sedan på **Redigera**.

   >[!TIP]
   >
   >Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du redigerar dem i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden, tilldelningar eller ett stort antal anpassade fält.

1. Klicka **Inställningar** väljer **Omberäkna kostnader och intäkter**.

1. Klicka **Spara ändringar**.

## Åtgärder som utlöser en automatisk omberäkning av ekonomin

Följande åtgärder utlöser en ekonomisk omberäkning av projekt i Workfront:

* Ändra aktivitetsstatus
* Flytta en aktivitet med timmar till ett annat projekt
* Ändra projektstatus från Fullständig till aktiv status

>[!NOTE]
>
>När du ändrar projektstatus beräknas endast de planerade värdena om.

Du kan även beräkna om ekonomi manuellt under **Mer** meny ![](assets/qs-more-menu.png) på projektnivå genom att klicka på **Beräkna om finanser**.

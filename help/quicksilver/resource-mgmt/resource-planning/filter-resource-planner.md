---
product-area: resource-management
navigation-topic: resource-planning
title: Filtrera information i resursplaneraren
description: '''(AL:*Iterate on this article: filtrera efter anpassade data. Andra förbättringar? Specialtecken kan ändras - följ artikeln för att få veta när. Det kom ursprungligen i Beta 3 17.3.)"'
author: Alina
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '2415'
ht-degree: 0%

---

# Filtrera information i resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

Med hjälp av filter kan du ändra vilken information som visas i resursplaneraren utifrån all information som lagras i systemet.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomst till projekt, användare och resurshantering </p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Översikt över filter för resursplanering

För att minimera mängden information som visas i resursplaneraren tillhandahåller Adobe Workfront ett standardfilter med förkonfigurerade villkor. Mer information om standardfiltret finns i avsnittet [Översikt över standardfiltret i resursplaneraren](#overview-of-the-default-filter-in-the-resource-planner) i den här artikeln.

Du kan också skapa anpassade filter. Information om hur du anpassar filter i resursplaneraren finns i avsnittet [Skapa resursplaneringsfilter](#create-resource-planner-filters) i den här artikeln.

Tänk på följande när du använder filter i resursplaneraren:

* De filter du skapar är bara synliga för dig. Du kan dela filter för att göra dem tillgängliga för andra användare.
* Som Workfront-administratör kan du bara se filter som du skapar eller som delas med dig.
* De filtrerade resultaten ändras inte när du väljer en annan vy för resursplaneraren.\
  Mer information om hur du ändrar vyn i resursplaneraren finns i avsnittet Projekt/roll/användarvy i [Översikt över navigering i resursplanering](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* När du använder ett filter ändras inte allokerings- och tillgänglighetsdata i resursplaneraren för projekt, roller eller användare. Ett filter ändrar bara antalet objekt som visas i resursplaneraren.
* Filtreringen gäller för alla objekt som visas i resursplaneraren samtidigt. Om du till exempel filtrerar efter en viss användare visas endast följande resultat i resursplaneraren:

   * Projekt där den användaren är en del av resurspoolen (för projekt- och rollvyerna) eller har en tilldelning i projektet (för användarvyn)
   * Roller som är associerade med användaren i dessa projekt\
     Andra roller eller användare i de projekt som användaren är kopplad till visas inte.

## Översikt över standardfiltret i resursplaneraren {#overview-of-the-default-filter-in-the-resource-planner}

När du öppnar resursplaneraren för första gången använder Workfront standardfiltret. Du kan redigera standardfiltret för att filtrera efter endast de objekt som du vill visa. Mer information om hur du ändrar filter finns i avsnittet [Redigera ett filter i Resursplanering](#edit-a-filter-in-the-resource-planner) i den här artikeln.

Tänk på följande när du använder standardfiltret:

* Standardfiltret hämtar endast information från projekt med följande:

   * Ett planerat slutförandedatum som infaller efter det första datumet i den aktuella månaden
   * Ett planerat startdatum som infaller före den sista dagen i den fjärde månaden från dagens datum
   * Status för aktuell eller planerad

  >[!IMPORTANT]
  >
  >Standardfiltret hämtar information från projekt som alltid inträffar inom fyra månader från och med den första dagen i den aktuella månaden, oavsett vilken tidsram du väljer för visningen i resursplaneraren.

* I användarvyn visas alla användare i systemet, men endast de användare som är associerade med de filtrerade projekten visar timinformation.
* Du kan redigera informationen i standardfiltret utan att spara filtret.
* Du kan duplicera och redigera en kopia av standardfiltret, ändra önskade villkor i det och sedan spara det som ett nytt filter.
* Du kan inte ta bort eller dela standardfiltret.

  ![RP_new_default_fitler_Criteri__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## Skapa resursplaneringsfilter {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

Att skapa ett filter i resursplaneraren är identiskt för alla vyer.

Kontrollera att förutsättningarna för att visa rätt information i resursplaneraren finns innan du skapar ett filter.\
Information om hur du uppfyller de nödvändiga kraven för att arbeta med resursplaneraren finns i avsnittet Krav för att arbeta i resursplaneraren i [Översikt över resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artikel.

Tänk på följande när du skapar ett filter:

* Det finns ingen gräns för hur många objekt du kan filtrera efter samtidigt.
* De tillgängliga fälten som du kan lägga till i en filterändring beroende på vilket objekt i vyn som du använder i resursplaneraren. Du kan till exempel bara filtrera fälten Problem och Aktivitet i användarvyn eftersom dessa objekt bara visas i användarvyn. Om du skapar ett filter för Problem eller Uppgifter i användarvyn och sedan tillämpar det på projekt- eller rollvyerna, ignoreras det eftersom fälten inte finns i projekt- eller rollvyerna. I så fall är filtret inte tillgängligt.

Så här skapar du ett filter i resursplaneraren:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn.

1. Klicka **Resurser**.

   The **Planering** visas som standard.

   Första gången du öppnar resursplaneraren är det som standard <strong>Standardfilter</strong> används.<br>Mer information om standardfiltret finns i <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">Översikt över standardfiltret i resursplaneraren</a> i den här artikeln.

1. Klicka på i det övre vänstra hörnet av . **Filter** -ikon.\
   ![filter_icon.png](assets/filter-icon.png)\
   eller\
   Expandera **Filter** nedrullningsbar meny och klicka **Lägg till nytt filter**.\
   ![](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. Om du vill skapa ett filter med hjälp av de inbyggda villkoren anger du något av följande fält:

   * **Portfolio**: Börja skriva namnet på portföljen som innehåller den information du vill ha med i resursplaneraren och klicka sedan på namnet när det visas i listan.\
     Upprepa den här processen om du vill inkludera information från flera portföljer.

   * **Projektstatus**: Expandera den nedrullningsbara menyn Projektstatus och välj en eller flera projektstatusvärden som är tillgängliga i listan.
   * **Team**: Börja skriva namnet på ett eller flera team som är kopplade till användarna som är tilldelade till uppgifter i de projekt som du vill visa.
   * **Jobbroll**: Börja skriva namnet på en eller flera jobbroller som är kopplade till användarna som är tilldelade till uppgifter i de projekt som du vill visa.
   * **Pooler**: Börja skriva namnet på en eller flera resurspooler som är associerade med projekten (för projektvyn), användarna (för användarvyn) eller associerade med både projekten och användarna (för rollvyn) som du vill visa.
   * **Grupp**: Börja skriva namnet på en eller flera grupper som är kopplade till användarna (i användarvyn) eller projekten (i projekt- och rollvyerna) som du vill visa.

1. Klicka **Lägg till filterregel** börjar du sedan skriva in fältnamnet som du vill filtrera efter i dialogrutan **Typ för att filtrera objekt** box. Om fältet är tillgängligt fylls det i för varje objekt där det kan kopplas.

   >[!IMPORTANT]
   >
   >När du refererar till anpassade fält måste du ange fältnamnet och inte fältetiketten. Fältetiketten visas i ett anpassat formulär som är kopplat till ett objekt. Mer information om skillnaden mellan etiketten och namnet på ett anpassat fält finns i  [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

1. Klicka på fältets namn för att lägga till det i filtret när det visas i listan.\
   Mer information om fälten som visas i listan finns i [Ordlista för Adobe Workfront-terminologi](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (Valfritt) Välj filter och villkorsmodifierare för filtret. Tillgängliga modifierare beskrivs i [Filter- och villkorsmodifierare](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Du kan använda användarbaserade eller datumbaserade jokertecken för att filtrera efter information som är kopplad till den inloggade användaren.\
   Mer information om jokertecken som stöds i filter finns i [Översikt över filtervariabler för jokertecken](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicka **Spara** för att spara filterregeln.
1. (Valfritt) Klicka på **Lägg till filterregel** om du vill lägga till en ny regel för ett annat objekt eller fält.
1. Klicka **Använd** om du vill använda filtret utan att spara det.

   eller

   Klicka **Spara filter** för att spara filtret.\
   ![RP_Apply_or_Save_buttons_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (Villkorligt) När du har klickat **Spara**, ange ett namn för filtret i **Filternamn** i **Spara filter** -dialogrutan. Detta är ett obligatoriskt fält.\
   ![RP_new_save_filter_box_with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >Om filternamnet innehåller specialtecken använder du endast följande tecken:
   >
   >* Komma
   >* Snedstreck
   >* Bindestreck
   >* Understreck

1. Klicka **Spara**.

   Resultaten i resursplaneraren filtreras nu efter informationen som du angav i filterreglerna.

## Använda ett befintligt filter

När du eller någon med åtkomst till resursplaneraren sparar ett filter blir det tillgängligt för alla som använder resursplaneraren.

Så här använder du ett befintligt filter:

1. Gå till Resursplaneraren.
1. Expandera **Filter** listruta.

   I den här menyn kan du se filter som du har skapat eller andra som delats med dig.\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. Välj ett filter i listrutan. Du kan se filter som du eller andra användare har skapat på den här menyn.\
   När du väljer ett filter minskar det automatiskt mängden information som visas i resursplaneraren.

## Redigera ett filter i Resursplanering {#edit-a-filter-in-the-resource-planner}

Du kan redigera ett filter i resursplaneraren på något av följande sätt:

* [Byta namn på ett filter](#rename-a-filter)
* [Redigera informationen i ett filter](#edit-the-information-in-a-filter)
* [Duplicera ett filter](#duplicate-a-filter)

När du redigerar ett filter uppdateras det för alla användare i systemet som har tillgång till resursplaneraren.

### Byta namn på ett filter {#rename-a-filter}

Du kan ändra namnet på ett filter utan att ändra villkoren för det. Vi rekommenderar att du informerar andra användare i systemet om den här ändringen eftersom filter är synliga för andra användare. Den här ändringen påverkar listorna med filter för alla som kan se resursplaneraren.

1. Gå till Resursplanering och expandera **Filter** för att välja ett sparat filter.
1. Expandera **Filter** listruta. Leta reda på filtret som du vill byta namn på och hovra över namnet.
1. Välj **Byt namn på filter** -ikonen bredvid filtrets namn.

   ![](assets/rp-filter-options-edit-350x154.png)

1. Ange ett nytt namn för filtret i **Filternamn** box.
1. Klicka **Spara**.\
   Informationen i filtret är densamma och namnet uppdateras.

### Redigera informationen i ett filter {#edit-the-information-in-a-filter}

Du kan ändra den information som du inkluderar i ett filter utan att ändra dess namn. Vi rekommenderar att du informerar andra användare i systemet om den här ändringen eftersom filter är synliga för dem. Den här ändringen påverkar listorna med filter för alla som kan se resursplaneraren.

1. Gå till Resursplanering och expandera **Filter** listrutan i det övre vänstra hörnet.
1. Markera ett befintligt filter som du vill redigera.
1. Klicka på **Filter** -ikon.\
   ![filter_icon.png](assets/filter-icon.png)

1. Lägg till nya fält i filtret.\
   Mer information om hur du skapar filter finns i [Skapa resursplaneringsfilter](#create-resource-planner-filters).

1. Håll pekaren över de fält som är markerade för filtret och klicka på **Redigera** om du vill markera ett annat fält, eller **Ta bort** -ikonen för att ta bort fältet.\
   ![RP_custom_filter_delete_and_edit_icons.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (Valfritt) Klicka på **Lägg till filterregel** för att lägga till nya fält i filtret.\
   Mer information om hur du definierar filtervillkor finns i [Skapa resursplaneringsfilter](#create-resource-planner-filters).

1. Klicka **Använd** om du vill använda filtret utan att spara det.

   eller

   Klicka **Spara** för att spara filtret.\
   Filtret sparas med samma namn men med nya filtervillkor.

### Duplicera ett filter {#duplicate-a-filter}

Du kan duplicera ett befintligt filter. De ursprungliga filtervillkoren är desamma i det duplicerade filtret och du kan spara det nya filtret med ett nytt namn.

1. Gå till Resursplanering och expandera **Filter** listrutan i det övre vänstra hörnet.
1. Håll pekaren över namnet på ett sparat filter som du vill duplicera.
1. Klicka på **Duplicera** -ikon.

   ![](assets/rp-filter-options---duplicate-350x154.png)\
   Rutan Duplicera filter visas.

1. I **Filternamn** anger du ett nytt namn för det duplicerade filtret.\
   Standardnamnet för det nya filtret är *`<Original Filter Name>`(kopia)*.

1. Klicka **Spara**. Ett nytt filter skapas med samma villkor som det ursprungliga filtret och med ett nytt namn.

   >[!NOTE]
   >
   >Även om du kan ha två filter med samma namn och med identiska villkor rekommenderar vi att du sparar filter med unika filtervillkor och namn i resursplaneraren för att undvika förvirring.

## Ta bort ett filter

Du kan ta bort ett filter när det inte längre behövs. Du kan inte ta bort standardfiltret.

Mer information om standardfiltret finns i [Översikt över standardfiltret i resursplaneraren](#overview-of-the-default-filter-in-the-resource-planner) i den här artikeln.

När du tar bort ett filter tas filtret bort för alla Workfront-användare som har tillgång till resursplaneraren. Innan du tar bort det kontrollerar du att det filter du vill ta bort inte längre används av någon annan som arbetar i resursplaneraren. Ett borttaget filter kan inte återskapas.

Ta bort ett filter:

1. Gå till Resursplaneraren.
1. Expandera **Filter** listruta.
1. Leta reda på filtret som du vill ta bort och hovra över namnet.
1. Välj **Ta bort filter** -ikonen bredvid filtrets namn.

   ![](assets/rp-filter-options---delete-350x154.png)

1. Klicka **Ta bort** i **Ta bort filter** -dialogrutan.

1. Filtret tas bort från resursplaneraren.

## Dela ett filter

Du kan dela ett filter som du har skapat eller som du har åtkomst till att dela med andra användare. Du kan inte dela standardfiltret, men du kan duplicera det och dela kopian.

>[!NOTE]
>
>Alla användare, inklusive Workfront-administratörer, har bara åtkomst till filter som de har skapat eller som har delats med dem. Du kan dela ett filter med specifika användare för att göra ett filter tillgängligt för alla resursplaneringsanvändare.

Mer information om standardfiltret finns i [Översikt över standardfiltret i resursplaneraren](#overview-of-the-default-filter-in-the-resource-planner) i den här artikeln.

Mer information om att duplicera filter finns i [Duplicera ett filter](#duplicate-a-filter) i den här artikeln.

1. Gå till Resursplaneraren.
1. Expandera **Filter** listruta.
1. Leta reda på filtret som du vill dela och hovra över namnet.
1. Välj **Delningsfilter** -ikonen bredvid filtrets namn.

   ![](assets/rp-filter-options---share-350x154.png)

   Dialogrutan Filteråtkomst visas.

1. (Valfritt) Om du vill göra filtret tillgängligt för alla Resursplaneringsanvändare klickar du på **Inställningar** ikon och sedan välja **Gör detta synligt för hela systemet**.

   ![](assets/make-this-visible-system-wide-350x119.png)

1. I **Ge resursplaneringsfilter åtkomst till:** börjar du skriva namnen på de användare, team, roller, grupper eller företag som du vill dela filtret med.
1. Välj bland följande behörighetsnivåer:

   * Visa
   * Hantera

     Information om behörigheter i Workfront finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (Valfritt) Klicka på **Avancerad inställning** Du kan lägga till behörigheter för varje nivå genom att markera dem eller ta bort behörigheter för varje nivå genom att avmarkera dem.

   ![](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. Klicka **Spara**.

   Filtret delas med de enheter som du har valt och det visas i **Delas med mig** område.

   ![](assets/rp-shared-with-me-area.png)

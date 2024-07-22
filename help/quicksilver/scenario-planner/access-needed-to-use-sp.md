---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Åtkomst krävs för att använda scenarioplaneraren
description: Scenarioplaneraren kräver en separat licens från Adobe Workfront och ytterligare åtkomst.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 99711cef67750a04f7a971538a978eff3656ff85
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Åtkomst krävs för att använda [!DNL Scenario Planner]

<!--Audited: 04/2024-->

[!DNL Scenario Planner] har ytterligare licenskrav. Mer information om [!DNL Workfront Scenario Planner] finns i [Översikt [!DNL Scenario Planner] Översikt](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Utan rätt åtkomst eller behörigheter kanske du inte kan visa [!UICONTROL Scenarios]-området för [!DNL  Adobe Workfront] eller hantera planer eller initiativ för din organisation. I hanteringen av planer och initiativ ingår att skapa, redigera och ta bort dem.

## Åtkomst krävs för att visa och använda [!DNL Adobe Workfront Scenario Planner]

Du måste se till att alla följande villkor uppfylls innan du kan komma åt [!DNL Workfront Scenario Planner]:

1. Din organisation måste ha en av Workfront-planerna som beskrivs nedan.

   Beroende på om du använder den nya eller nuvarande Workfront-planen måste din organisation ha något av följande:

   * För de nya planerna måste din organisation ha planen [!UICONTROL Ultimate] [!DNL Workfront]. Scenarioplaneraren ingår bara i planen [!UICONTROL Ultimate].

   * För de aktuella Workfront-planerna måste din organisation ha båda följande:

      * Din organisation måste köpa en [!DNL Workfront] [!UICONTROL Business]-plan eller en senare [!DNL Workfront]-plan. Mer information om [!DNL Workfront]-planerna finns i [Workfront-planer](https://workfront.com/plans).

      * Din organisation måste köpa en [!DNL Workfront Scenario Planner]-licens, förutom en [!DNL Workfront]-licens. Kontakta din [!DNL Workfront]-kontorepresentant om du vill veta mer om [!DNL Workfront Scenario Planner] licenser.

1. Du måste ha en av Workfront-licenserna som beskrivs nedan.

   Beroende på om du använder de nya eller aktuella licenserna måste din [!DNL Workfront]-administratör tilldela dig en licens av någon av följande typer:

   * För de nya licenserna:
      * [!UICONTROL Standard]
      * [!UICONTROL Light]

   * För de aktuella licenserna:

      * [!UICONTROL Plan]
      * [!UICONTROL Work]
      * [!UICONTROL Review]

   >[!NOTE]
   > 
   >* När de nya licenserna används kan användare med en [!UICONTROL Contributor]- eller [!UICONTROL External]-licenstyp inte komma åt [!DNL Scenario Planner].
   >
   >* När de aktuella licenserna används kan användare med en begärande eller extern licenstyp inte komma åt scenarioplaneraren.

1. Din [!DNL Workfront]-administratör måste ge dig [!UICONTROL View] eller [!UICONTROL Edit] åtkomst till [!DNL Scenario Planner] på din åtkomstnivå.

   Mer information om att bevilja åtkomst till [!DNL Workfront Scenario Planner] finns i [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Valfritt och rekommenderas) Om du vill visa eller uppdatera ekonomisk information för dina planer och initiativ måste [!DNL Workfront]-administratören även ge dig åtkomst till [!UICONTROL Financial Data] på din åtkomstnivå. Mer information om att bevilja ekonomiska data på din åtkomstnivå finns i [Bevilja åtkomst till ekonomiska data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Valfritt) Om du behöver komma åt planer som du inte har skapat måste den som skapat planen ge dig rätt behörighet för att komma åt dem. Mer information om vilka behörigheter som krävs för att komma åt planer och initiativ som du inte har skapat finns i avsnittet [Behörigheter som behövs för att komma åt planer och initiativ](#permissions-needed-to-access-plans-and-initiatives) i den här artikeln.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Åtkomst krävs för att visa planer och initiativ

Förutom att ditt företag får rätt licens för [!DNL Workfront Scenario Planner] måste din [!DNL Workfront]-administratör även tilldela dig följande åtkomst och inställningar så att du kan visa [!DNL Workfront Scenario Planner] och informationen i det här området:

* En åtkomstnivå med minst [!UICONTROL View] åtkomst till [!DNL Scenario Planner].

  Mer information om åtkomstnivån till [!DNL Scenario Planner] finns i [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* En åtkomstnivå med minst [!UICONTROL View] åtkomst till [!UICONTROL Financial Data] om du behöver visa ekonomisk information om planen och initiativen. Exempel på ekonomisk information är budgetar, kostnader eller jobbrollstariffer.

  Mer information om åtkomstnivån [!UICONTROL Financial Data] finns i [Bevilja åtkomst till ekonomiska data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] och [!UICONTROL External] användare har inte åtkomst att visa [!DNL Scenario Planner].

* Visa behörigheter för planen. Mer information om vilka behörigheter som krävs för att komma åt planer och initiativ som du inte har skapat finns i avsnittet [Behörigheter som behövs för att komma åt planer och initiativ](#permissions-needed-to-access-plans-and-initiatives) i den här artikeln.

## Tillgång till att hantera planer och initiativ

Din [!DNL Workfront]-administratör måste tilldela dig följande åtkomst så att du kan hantera planer och deras information i [!DNL Scenario Planner]:

* En [!UICONTROL Plan]- eller [!UICONTROL Work]-licenstyp med Redigera-åtkomst till [!DNL Scenario Planner] på din åtkomstnivå.

  Alla andra licenstyper har inte åtkomst till att hantera planer.

  Mer information om att bevilja åtkomst till [!DNL Scenario Planner] från åtkomstnivån finns i [Bevilja åtkomst till  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* En [!UICONTROL Plan]-licenstyp med [!UICONTROL Edit] åtkomst till [!UICONTROL Financial Data] på din åtkomstnivå, om du även behöver uppdatera ekonomisk information om planen.

  Några exempel på ekonomisk information som du kan redigera är [!UICONTROL Budget], [!UICONTROL Planned Benefit] och [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Endast [!UICONTROL Plan] licensinnehavare har [!UICONTROL Edit] åtkomst till [!UICONTROL Financial Data].

  Mer information om åtkomstnivån [!UICONTROL Financial Data] finns i [Bevilja åtkomst till ekonomiska data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Hantera behörigheter till en plan som du inte har skapat. Mer information om vilka behörigheter som krävs för att komma åt planer och initiativ som du inte har skapat finns i avsnittet [Behörigheter som behövs för att komma åt planer och initiativ](#permissions-needed-to-access-plans-and-initiatives) i den här artikeln.

## Behörigheter som krävs för att få tillgång till planer och initiativ

Åtkomstnivåer fungerar tillsammans med behörigheter i [!DNL Workfront] för att ge dig insyn i planer och initiativ som du inte har skapat. Förutom att du måste ha rätt åtkomstnivå för att få åtkomst till [!DNL Scenario Planner] måste du också ha rätt behörighet till planen som du vill visa eller hantera, om du inte är den som har skapat planen.

Alla användare, inklusive systemadministratörer, har endast åtkomst till planer som de har skapat.

Om du vill visa planer som andra användare har skapat måste de dela sina planer med dig på följande sätt:

* Dela planen med dig

  Mer information om delningsplaner finns i [Dela en plan i  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Skicka en länk till en plan som de har skapat

  Om en användare delar en länk till en plan utan att också dela planen, kan du begära behörigheter till planen. Mer information om hur du begär behörigheter till planer finns i [Begär åtkomst till en plan i  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>När en användare inaktiveras har deras planer ingen ägare och går inte att komma åt om de inte tidigare delats med en länk.



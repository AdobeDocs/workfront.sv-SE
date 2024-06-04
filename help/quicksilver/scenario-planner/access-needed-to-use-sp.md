---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Åtkomst krävs för att använda scenarioplaneraren
description: Scenarioplaneraren kräver en separat licens från Adobe Workfront och ytterligare åtkomst.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# Åtkomst krävs för att använda [!DNL Scenario Planner]

The [!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner], se [The [!DNL Scenario Planner] översikt](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Utan rätt åtkomst eller behörigheter kanske du inte kan visa [!UICONTROL Scenarios] område på[!DNL  Adobe Workfront] eller hantera planer eller initiativ för din organisation. I hanteringen av planer och initiativ ingår att skapa, redigera och ta bort dem.

>[!IMPORTANT]
>
>Vid åtkomst [!UICONTROL Scenarios]kan du bara visa och hantera planer som du har skapat. Om du vill att andra användare ska kunna visa eller hantera de planer du har skapat måste du göra följande:
>
>* Skicka en länk till din plan till andra användare
>* Dela planen med andra användare
>
>  Mer information om att dela en plan finns i [Dela en plan i [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>När en användare inaktiveras har deras planer ingen ägare och går inte att komma åt om de inte tidigare delats med en länk.

## Åtkomst som behövs för att visa och använda [!DNL Adobe Workfront Scenario Planner]

Du måste se till att alla följande villkor uppfylls innan du kan komma åt [!DNL Workfront Scenario Planner]:

1. Din organisation måste ha en av Workfront-planerna som beskrivs nedan.

   Beroende på om du använder den nya eller nuvarande Workfront-planen måste din organisation ha något av följande:

   * För de nya planerna måste din organisation ha något av följande:

      * The [!UICONTROL Ultimate] [!DNL Workfront] plan. Scenarioplanen ingår i Ultimate-planen.

        eller

      * The [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] plan, förutom att köpa en separat [!DNL Scenario Planner] licens.

   * För de aktuella Workfront-planerna måste din organisation ha båda följande:

      * Din organisation måste köpa en [!DNL Workfront] [!UICONTROL Business] eller högre [!DNL Workfront] plan. Mer information om [!DNL Workfront] planer, se [Workfront-planer](https://workfront.com/plans).

      * Din organisation måste köpa en [!DNL Workfront Scenario Planner] licens, utöver [!DNL Workfront] licens. Kontakta [!DNL Workfront] Kontorepresentant som kan läsa om [!DNL Workfront Scenario Planner] licenser.

1. Du måste ha en av Workfront-licenserna som beskrivs nedan.

   Beroende på om du använder de nya eller aktuella licenserna kan du [!DNL Workfront] administratören måste tilldela dig en licens av någon av följande typer:

   * För de nya licenserna:
      * [!UICONTROL Standard]
      * [!UICONTROL Light]

   * För de aktuella licenserna:

      * [!UICONTROL Plan]
      * [!UICONTROL Work]
      * [!UICONTROL Review]

   >[!NOTE]
   > 
   >* När de nya licenserna används har användare med [!UICONTROL Contributor] eller [!UICONTROL External] licenstypen kan inte komma åt [!DNL Scenario Planner].
   >
   >* När de aktuella licenserna används kan användare med en begärande eller extern licenstyp inte komma åt scenarioplaneraren.

1. Dina [!DNL Workfront] måste administratören ge dig [!UICONTROL View] eller [!UICONTROL Edit] behörighet till [!DNL Scenario Planner] på din åtkomstnivå.

   Mer information om hur du beviljar åtkomst till [!DNL Workfront Scenario Planner], se [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Valfritt och rekommenderas) Om du vill visa eller uppdatera ekonomisk information för dina planer och initiativ kan du [!DNL Workfront] administratören måste också ge dig åtkomst till [!UICONTROL Financial Data] på din åtkomstnivå. Information om hur du ger ekonomiska data på din åtkomstnivå finns i [Bevilja åtkomst till finansiella uppgifter](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Valfritt) Om du behöver komma åt planer som du inte har skapat måste den som skapat planen ge dig rätt behörighet för att komma åt dem. Information om vilka behörigheter som krävs för att komma åt planer och initiativ som du inte har skapat finns i [Behörigheter som krävs för att få tillgång till planer och initiativ](#permissions-needed-to-access-plans-and-initiatives) i den här artikeln.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Åtkomst krävs för att visa planer och initiativ

Förutom att ditt företag köper rätt licens för [!DNL Workfront Scenario Planner], dina [!DNL Workfront] administratören måste även tilldela dig följande åtkomst och inställningar så att du kan se [!DNL Workfront Scenario Planner] och informationen på detta område:

* En åtkomstnivå med minst [!UICONTROL View] behörighet till [!DNL Scenario Planner].

  Mer information om åtkomstnivån till [!DNL Scenario Planner], se [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* En åtkomstnivå med minst [!UICONTROL View] behörighet till [!UICONTROL Financial Data] om du behöver visa ekonomisk information om planen och initiativen. Exempel på ekonomisk information är budgetar, kostnader eller jobbrollstariffer.

  Mer information om [!UICONTROL Financial Data] åtkomstnivå, se [Bevilja åtkomst till finansiella uppgifter](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] och [!UICONTROL External] Användarna har inte åtkomst att visa [!DNL Scenario Planner].

* Visa behörigheter för planen. Information om vilka behörigheter som krävs för att komma åt planer och initiativ som du inte har skapat finns i [Behörigheter som krävs för att få tillgång till planer och initiativ](#permissions-needed-to-access-plans-and-initiatives) i den här artikeln.

## Tillgång till att hantera planer och initiativ

Dina [!DNL Workfront] administratören måste ge dig följande åtkomst så att du kan hantera planer och deras information i [!DNL Scenario Planner]:

* A [!UICONTROL Plan] eller [!UICONTROL Work] licenstyp med Redigera-åtkomst till [!DNL Scenario Planner] på din åtkomstnivå.

  Alla andra licenstyper har inte åtkomst till att hantera planer.

  Mer information om att bevilja åtkomst till [!DNL Scenario Planner] från åtkomstnivån, se [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] licenstyp med [!UICONTROL Edit] behörighet till [!UICONTROL Financial Data] på din åtkomstnivå, om du även behöver uppdatera ekonomisk information om planen.

  Några exempel på ekonomisk information som du kan redigera är [!UICONTROL Budget], [!UICONTROL Planned Benefit]och [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Endast [!UICONTROL Plan] certifikatinnehavare har [!UICONTROL Edit] behörighet till [!UICONTROL Financial Data].

  Mer information om [!UICONTROL Financial Data] åtkomstnivå, se [Bevilja åtkomst till finansiella uppgifter](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Hantera behörigheter till en plan som du inte har skapat. Information om vilka behörigheter som krävs för att komma åt planer och initiativ som du inte har skapat finns i [Behörigheter som krävs för att få tillgång till planer och initiativ](#permissions-needed-to-access-plans-and-initiatives) i den här artikeln.

## Behörigheter som krävs för att få tillgång till planer och initiativ

Åtkomstnivåer fungerar tillsammans med behörigheter i [!DNL Workfront] för att ge er insyn i planer och initiativ som ni inte har skapat. Förutom att ha rätt åtkomstnivå för att komma åt [!DNL Scenario Planner]måste du också ha rätt behörighet till planen som du vill visa eller hantera, om du inte är den som har skapat planen.

Som standard har du bara tillgång till planer som du har skapat. Om du vill visa planer som andra användare har skapat måste de dela sina planer med dig. Information om delningsplaner finns i [Dela en plan i [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Om en användare delar en länk till en plan utan att också dela planen, kan du begära behörigheter till planen. Information om hur du begär behörigheter till planer finns i [Begär åtkomst till en plan i [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).


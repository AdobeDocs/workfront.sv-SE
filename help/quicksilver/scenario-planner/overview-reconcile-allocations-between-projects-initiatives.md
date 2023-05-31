---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Översikt över avstämning av resursallokeringar mellan projekt och initiativ
description: Översikt över avstämning av resursallokeringar mellan projekt och initiativ
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Översikt över avstämning av resursallokeringar mellan projekt och initiativ

>[!IMPORTANT]
>
>Din organisation måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] så att du kan visa initieringsinformation för ett projekt. Mer information om hur du får [!DNL Workfront Scenario Planner], se [Åtkomst krävs för att använda scenarioplaneraren](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Du kan koppla projekt till initiativ för att säkerställa att dina strategiska planer och det verkliga arbetet är synkroniserade. När du sammanfattar dina strategiska planer och initiativ i [!DNL Scenario Planner] och du planerar det verkliga arbetet i ett projekt kan du se till att resurserna i både projektet och initiativen matchar så att du inte överfördelar eller underutnyttjar dem.

## Förutsättningar

Innan du börjar måste du ha följande:

* En plan i [!DNL Scenario Planner] med ett initiativ som är kopplat till ett projekt.
* Nödvändiga tilldelningar av arbetsroller för initiativet.
* Aktiviteter eller problem i projektet som har planerade timmar och som har tilldelats något av följande:

   * Jobbroller
   * Användare som är associerade med jobbroller

## Koppla samman projekt och initiativ

>[!NOTE]
>
>Du kan skapa initiativ och koppla dem till projekt endast om din organisation har köpt en extra licens för [!DNL Workfront Scenario Planner].

Du kan koppla projekt till initiativ genom att göra något av följande:

* Importera projekt till en plan som nya initiativ

   Mer information finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicera projekt

   Mer information finns i [Uppdatera eller skapa projekt genom att publicera i [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Båda processerna skapar en koppling mellan projekten och deras motsvarande initiativ. När du har anslutit dem kan du hantera deras resursallokeringar genom att jämföra dem och se till att de matchar.

## Överväganden om att sammanföra resurser i länkade projekt och initiativ

>[!NOTE]
>
>Du kan bara visa initiativ, koppla dem till projekt och visa deras resursallokeringar i ett projekt om din organisation har köpt en extra licens för projektet [!DNL Workfront Scenario Planner].

* Du kan tilldela användare, team och jobbroller till arbetsobjekt i ett projekt och du kan tilldela jobbroller till initiativ. Det innebär att du bara kan förena jobbroller mellan projekt och initiativ.

   >[!TIP]
   >
   >Om du vill att användarens tid för ett projekt ska stämma överens med rollallokeringar för initiativen måste du associera användare med jobbroller.

* Du kan visa rollallokering för initialjobb för ett länkat projekt inom följande områden i projektet:

   * [!DNL Scenario Planner] i [!UICONTROL Project Details] område i ett projekt. Mer information finns i följande artiklar:

      * [Uppdatera eller skapa projekt genom att publicera i [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Hantera information i projektet [!UICONTROL Overview] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >Du kan inte se jobbrollsinformation från projektet eller initiativ sida vid sida i [!DNL Scenario Planner] i [!UICONTROL Project Details].

   * The [!UICONTROL Role Allocation] i följande områden:

      * [!UICONTROL Workload Balancer] projektet

         Mer information om hur rollfördelningen mellan initiativet och det länkade projektet i [!UICONTROL Workload Balancer], se [Visa rolltilldelning för projekt och initiativ i [!UICONTROL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Tasks] section

         För information om hur rollfördelningen mellan initiativet och det länkade projektet i [!UICONTROL Tasks] avsnitt, se [Visa rolltilldelning för projekt och initiativ i uppgiftslistan](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Du kan se jobbrollsinformation från projektet och satsningen sida vid sida i [!UICONTROL Role Allocation] -panelen.



* Du kan inte visa jobbrollallokering för ett projekt på ett länkat initiativ. Mer information finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->

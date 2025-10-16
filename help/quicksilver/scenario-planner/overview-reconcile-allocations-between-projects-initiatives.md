---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Översikt över avstämning av resursallokeringar mellan projekt och initiativ
description: Översikt över avstämning av resursallokeringar mellan projekt och initiativ
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Översikt över avstämning av resursallokeringar mellan projekt och initiativ

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Du kan koppla projekt till initiativ för att säkerställa att dina strategiska planer och det verkliga arbetet är synkroniserade. När du utformar dina strategiska planer och initiativ i [!DNL Scenario Planner] och du planerar det verkliga arbetet i ett projekt, kan du se till att dina resurser i både projektet och initiativen matchar, så att du inte överallokerar eller underutnyttjar dem.

## Förutsättningar

Innan du börjar måste du ha följande:

* En plan i [!DNL Scenario Planner] med ett initiativ kopplat till ett projekt.
* Nödvändiga tilldelningar av arbetsroller för initiativet.
* Aktiviteter eller problem i projektet som har planerade timmar och som har tilldelats något av följande:

   * Jobbroller
   * Användare som är associerade med jobbroller

## Koppla samman projekt och initiativ

>[!NOTE]
>
>Du kan bara skapa initiativ och ansluta dem till projekt om din organisation har köpt ytterligare en licens för [!DNL Workfront Scenario Planner].

Du kan koppla projekt till initiativ genom att göra något av följande:

* Importera projekt till en plan som nya initiativ

  Mer information finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicera projekt

  Mer information finns i [Uppdatera eller skapa projekt genom att publicera initiativ i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Båda processerna skapar en koppling mellan projekten och deras motsvarande initiativ. När du har anslutit dem kan du hantera deras resursallokeringar genom att jämföra dem och se till att de matchar.

## Överväganden om att sammanföra resurser i länkade projekt och initiativ

>[!NOTE]
>
>Du kan bara visa initiativ, ansluta dem till projekt och visa deras resursallokeringar för ett projekt om din organisation har köpt ytterligare en licens för [!DNL Workfront Scenario Planner].

* Du kan tilldela användare, team och jobbroller till arbetsobjekt i ett projekt och du kan tilldela jobbroller till initiativ. Det innebär att du bara kan förena jobbroller mellan projekt och initiativ.

  >[!TIP]
  >
  >Om du vill att användarens tid för ett projekt ska stämma överens med rollallokeringar för initiativen måste du associera användare med jobbroller.

* Du kan visa rollallokering för initialjobb för ett länkat projekt inom följande områden i projektet:

   * [!DNL Scenario Planner]-delen av [!UICONTROL Project Details]-området i ett projekt. Mer information finns i följande artiklar:

      * [Uppdatera eller skapa projekt genom att publicera initiativ i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Hantera information i projektområdet [!UICONTROL Overview]](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Du kan inte se jobbrollsinformation från projektet och initiativ sida vid sida i avsnittet [!DNL Scenario Planner] i [!UICONTROL Project Details].

   * Panelen [!UICONTROL Role Allocation] i följande områden:

      * [!UICONTROL Workload Balancer] av projektet

        Mer information om hur du visar och förenar rollallokeringarna mellan initiativet och det länkade projektet i [!UICONTROL Workload Balancer] finns i [Visa rollallokering för projekt och initiativ i [!UICONTROL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Tasks] avsnitt

        Mer information om hur du förenar rollallokeringarna mellan initiativet och det länkade projektet i avsnittet [!UICONTROL Tasks] finns i [Visa rollallokering för projekt och initiativ i uppgiftslistan](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Du kan visa information om jobbroller från projektet och om initiativet sida vid sida på panelen [!UICONTROL Role Allocation].

* Du kan inte visa jobbrollallokering för ett projekt på ett länkat initiativ. Mer information finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->

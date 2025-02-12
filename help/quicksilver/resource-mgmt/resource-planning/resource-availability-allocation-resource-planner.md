---
product-area: resource-management
navigation-topic: resource-planning
title: Granska resurstillgänglighet och allokering med hjälp av Adobe Workfront resursplanerare
description: Du kan visa tillgängligheten för dina resurser och mängden planerat eller budgeterat arbete för dina projekt i resursplaneraren. Dessa värden visas i timmar, FTE (heltidsekvivalent) eller kostnadsbelopp och är ordnade i kolumner.
author: Lisa
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 0%

---

# Granska resurstillgänglighet och allokering med Adobe Workfront Resource Planner

Du kan visa tillgängligheten för dina resurser och mängden planerat eller budgeterat arbete för dina projekt i resursplaneraren. Dessa värden visas i timmar, FTE (heltidsekvivalent) eller kostnadsbelopp och är ordnade i kolumner.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Ljus eller högre</p>
       <p>eller</p>
       <p>Aktuell: Granska eller senare</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomsten till följande:</p> 
    <ul> 
     <li> <p>Resurshantering</p> </li> 
     <li> <p>Finansiella data</p> </li> 
     <li> <p>Användare</p> </li> 
     <li> <p>Projekt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för de projekt som du vill visa i resursplaneraren</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste uppfylla alla krav som krävs för att kunna arbeta med resursplaneraren. Mer information finns i [Översikt över resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Om något av de krav som krävs för att resursplaneraren ska fungera korrekt saknas, kan vissa siffror vara noll, eller så kan budgeterade timmar vara nedtonade.

## Tillgänglighet och resurstilldelning

Kolumnerna som visar tillgängligheten och allokeringen av dina resurser ändras beroende på vilken vy du använder i resursplaneraren. Mer information om hur du visar informationen i resursplaneraren efter projekt, roll eller användare finns i [Navigeringsöversikt för resursplanering](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Tänk på följande när du ändrar vyn till Resursplanering:

* När du använder vyerna **Visa efter projekt** eller **Visa efter roll** kan du se följande kolumner:

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Tillgängliga timmar, heltidsekvivalenter eller kostnad
   * Planerade timmar, heltidsekvivalenter eller kostnad
   * Budgeterade timmar, heltidsekvivalenter eller kostnad
   * Timmar, heltidsekvivalenter eller kostnadsavvikelse
   * Nettotimmar, heltidsekvivalenter eller kostnad

* När du använder vyn **Visa efter användare** kan du se följande kolumner:

   * Tillgängliga timmar eller heltidsekvivalenter
   * Planerade timmar eller heltidsekvivalenter
   * Timme- eller FTE-differens
   * Procentandel för allokering av planerade timmar

>[!TIP]
>
>Informationen är inte tillgänglig som kostnad när vyn **Visa efter användare** används i resursplaneraren.
>
>Mer information om vad varje kolumn visar får du om du för musen över namnet på den kolumn där talet visas.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Mer information om vilka data som visas i varje kolumn finns i följande artiklar:
>
>* [Översikt över timma-, FTE- och kostnadsinformation i projekt- och rollvyerna i resursplaneraren](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när användarvyn används](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## Visa information per timme, heltid eller kostnad

1. Gå till Resursplaneraren.

   Som standard visas informationen som timmar i resursplaneraren.

1. Expandera listrutan.\
   ![Timmar_Efter_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Timmar</td> 
      <td>Visar tillgänglighets- och allokeringsinformation i timmar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>Visar tillgänglighets- och allokeringsinformation i heltidsekvivalenter.</p> <p>Mer information om hur FTE beräknas i resursplaneraren finns i <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kostnad</td> 
      <td> <p>Visar tillgänglighet och allokeringsinformation per kostnad om du visar resursplaneraren i projekt- eller rollvyerna. Informationen visar värden i systemets valuta. Din Workfront-administratör definierar systemvalutan. Mer information om hur du ställer in systemvalutan i Workfront finns i <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Konfigurera valutakurser</a>.</p> <p><b>ANMÄRKNING</b>

   Du måste associera användare och jobbroller med kostnad per timme för att visa kostnadsinformation i resursplaneraren.<br style="font-style: italic;">Mer information om hur du associerar kostnadsnivåer per timme med jobbroller finns i <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.<br style="font-style: italic;">Mer information om hur du associerar kostnadsnivåer per timme med användare finns i <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.<br style="font-style: italic;">Mer information om hur kostnaden beräknas i resursplaneraren finns i <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Beräkna kostnader i resursplaneraren </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Anpassa</td> 
      <td>Skapar en anpassad vy av kolumnerna som visas i resursplaneraren. Välj de alternativ som du vill visa i resursplaneraren enligt anvisningarna i stegen nedan. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du valde **Anpassa** anger du alternativ i rutan **Anpassa visade mätvärden** för att konfigurera din anpassade vy.

   ![Anpassa visningsrutan](assets/planner-customize-view-box-350x114.png)

1. I kolumnen **Vytyp** till vänster väljer du en av följande vyer:

   * Projekt
   * Roll
   * Användare

1. I avsnittet **Visa markerade objekt** väljer du den typ av information som du vill visa i kolumnerna i den markerade vyn. I följande tabell visas vilka alternativ som är tillgängliga i varje vy:

   | **Alternativ** | Användarvy | Projektvy | Rollvy |
   |---|---|---|---|
   | Tillgänglig | ✔ | ✔ | ✔ |
   | Planerad | ✔ | ✔ | ✔ |
   | Budgeterad |   | ✔ | ✔ |
   | Varians |   | ✔ | ✔ |
   | Net |   | ✔ | ✔ |
   | Faktisk | ✔ |   |   |
   | Differens | ✔ |   |   |
   | Procent | ✔ |   |   |

1. Välj **Använd planerade (PLN)-värden i NET-beräkningar** om du vill använda Planerad i stället för Budgeterad information när du beräknar nettovärden i projekt- och rollvyerna.

   När du väljer det här alternativet beräknar Workfront nettovärdena med följande formel:

   `Net = Available - Planned`

   >[!TIP]
   >
   >**Det här alternativet används bara när du väljer minst ett alternativ för att anpassa vyn i avsnittet Visa markerade objekt.**

1. Klicka på **Spara**.

   Den anpassade vy som innehåller de markerade kolumnerna visas.

   Resursplaneraren visar den anpassade vyn som anpassad i listrutan Timmar.

   >[!NOTE]
   >
   >Du kan bara ha en anpassad vy.

   ![Listrutan Planeringstimmar](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Visa användarallokeringsdiagrammet

Du kan visa den planerade fördelningen av användare mot deras tillgänglighet i ett diagram.

Så här visar du allokeringen av användare i ett diagram:

1. Gå till Resursplaneraren.

   Mer information om åtkomst till resursplaneraren finns i avsnittet [Hitta resursplaneraren](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) i artikeln [Översikt över resursplaneraren](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Välj **Visa efter användare**.

   >[!TIP]
   >
   >Du kan bara visa användarallokeringsdiagrammet i användarvyn.

1. Klicka på ikonen **Användarallokeringsdiagram** ![RP_user_allokering_chart.png](assets/rp-user-allocation-chart.png) för att visa följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tillgänglighet % utan överbeläggning för alla användare</td> 
      <td>Detta är den tid som alla användare är tillgängliga för arbete under en tidsperiod, vilket visas som en procentandel av den totala tillgängliga tiden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Överbeläggning % för alla användare </td> 
      <td> <p>Det här är den tid som användare tilldelas för mycket under en tidsperiod, vilket visas som en procentandel av den totala tillgängliga tiden.</p> <p><b>ANMÄRKNING</b>

   En överbeläggning inträffar när antalet planerade timmar är högre än antalet tillgängliga timmar. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Underutnyttjande % för alla användare</td> 
      <td> <p>Det här är den tid som användare har underutnyttjat under en tidsperiod, vilket visas som en procentandel av den totala tillgängliga tiden.</p> <p><b>ANMÄRKNING</b>

   Underutnyttjande inträffar när de planerade timmarna är lägre än de tillgängliga timmarna. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Det finns en överallokering för minst en användare under den här tidsperioden</td> 
      <td>Detta visar att det finns en överallokering för minst en användare i en tidsperiod, även om den totala tiden för alla användare inte är överallokerad för tidsperioden.<br>Du måste bläddra igenom listan över användare och timmarna för den användare som är överallokerad markeras med rött.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP_user_allokering_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Valfritt) Klicka på området **Överbeläggning % för alla användare** i diagrammet.\
   Alla användare som är överallokerade markeras med rött.
1. (Valfritt) Klicka på **Underutnyttjande % för alla användare** i diagrammet.\
   Alla användare som är underutnyttjade markeras med blått.

1. (Valfritt) Klicka på indikatorikonen ![one_user_overallokering_marker.png](assets/one-user-overallocation-marker.png) som visar var du har minst en användare överallokerat.\
   De överallokerade användarna markeras med rött.

1. (Valfritt) Uppdatera sidan om du vill komprimera diagrammet.

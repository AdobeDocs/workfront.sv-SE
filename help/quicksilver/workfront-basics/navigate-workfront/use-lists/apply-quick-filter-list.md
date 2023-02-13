---
navigation-topic: use-lists
title: Använda snabbfiltret på en lista
description: Du kan använda snabbfiltret i en lista med objekt för att bara hitta objekt som är viktiga för dig, så att du snabbt kan granska, uppdatera eller dela dem med andra.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Använda snabbfiltret på en lista

<!--
{{highlighted-preview}}
-->

Du kan använda snabbfiltret i en lista med objekt för att bara hitta objekt som är viktiga för dig, så att du snabbt kan granska, uppdatera eller dela dem med andra.

>[!IMPORTANT]
>
>Du kan söka efter objekt som innehåller ett sökord med hjälp av snabbfilter, oavsett om objektet har visats fysiskt på skärmen eller visas när du har rullat längst ned på sidan. När du använder webbläsarens sökfunktioner kan du bara hitta objekt som visas fysiskt på skärmen. Om listan innehåller flera sidor hittar snabbfiltren inte objekt som finns på sidor som inte visas.

Om du vill spara ett snabbfilter rekommenderar vi att du i stället skapar ett permanent filter för listan.\
Mer information om hur du skapar filter i [!DNL Adobe Workfront], se artikeln [Översikt över filter i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Snabbfiltret är för närvarande tillgängligt i följande områden


Du kan använda tillfälliga snabbfilter i alla listor, förutom följande:

* The [!UICONTROL Reports] area
* Dokumentlistor och rapporter
* Flera [!UICONTROL Setup] områden
   >[!NOTE]
   >
   >Snabbfilter finns i följande inställningsområden: [!UICONTROL Groups], [!UICONTROL Teams], [!UICONTROL Companies], [!UICONTROL Schedules], [!UICONTROL Layout Templates]och [!UICONTROL Custom Forms].


Tänk på följande när du använder snabbfilter på en lista:

* Du kan använda nyckelord för att filtrera efter fält som visas i listvyn. Detta inkluderar anpassade fält eller komplexa fält som [!UICONTROL Predecessors], [!UICONTROL Assignments], [!UICONTROL Assignment] och [!UICONTROL Status], [!UICONTROL Approver] och [!UICONTROL Status], osv.
* Om listan innehåller komprimerade grupperingar utökas de automatiskt när du använder snabbfilter. När du tar bort snabbfiltret komprimeras grupperingarna igen.
* Grupperingar bevarar den sammanställda informationen i den ursprungliga listan oavsett vilka snabbfilter som använts eller ändringar som gjorts på objekten i listan.
* Snabbfilter är tillfälliga. Om du ändrar gruppering, vy, filter eller sortering för listan tas villkoren för snabbfilter bort.
* Du kan inte spara ett snabbfilter. Om du vill spara ett filter och använda det igen bör du skapa ett permanent filter för listan.
* Om du har mer än en gruppering i listan och snabbfiltret hittar objekt i bara en gruppering, visas bara den grupperingen med de hittade objekten. Alla andra grupperingar är dolda.
* I en uppgifts- eller underuppgiftslista tas uppgiftshierarkin bort när resultaten av snabbfiltervisningen visas.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] plan*</b></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licens*</b></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Konfigurationer på åtkomstnivå*</b></td> 
   <td> <p>Visa åtkomst till området som listan finns i</p> <p>Om du till exempel vill använda ett snabbfilter på ett projekt måste du [!UICONTROL View] behörighet till projekt.</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå.<br>För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Objektbehörigheter</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Använda ett snabbfilter på en lista

1. Gå till en lista eller rapport som stöder snabbfilter och klicka sedan på **[!UICONTROL Quick Filter]icon** ![](assets/qs-quick-filter-icon.png) i verktygsfältet.

   eller

   Beroende på operativsystem eller webbläsare och när du använder ett vanligt QWERTY-tangentbord trycker du på följande uppsättning kommandon för att starta snabbfiltret:

   * ALT+F för [!DNL Windows] datorer
   * ALT/Option+F för [!DNL Mac] datorer

      >[!TIP]
      >
      >Om du trycker på CTRL+F eller CMD+F visas ett verktygstips bredvid snabbfiltret för att påminna dig om dessa kommandon. Kommandona visas också i sökrutan för snabbfilter.

1. I **[!UICONTROL Filter page]** anger du nyckelordet som du vill filtrera efter.

   Du kan använda vilket ord som helst som visas i vyn av listan.

   >[!NOTE]
   >
   >Om du använder ett ord som kan visas på en annan sida i listan, kommer snabbfiltret inte att hitta några resultat.

   En lista med objekt som matchar sökvillkoren visas dynamiskt i listan när du skriver och alla andra objekt döljs. Nyckelordet som du använde i sökningen markeras med gult i alla fristående och komplexa fält. Några exempel på komplexa fält är delade kolumner eller något av följande: [!UICONTROL Assignments], [!UICONTROL Assignments] och [!UICONTROL Status], [!UICONTROL Percent Complete], [!UICONTROL Predecessors], [!UICONTROL Approvers and Status], [!UICONTROL Resource Managers], [!UICONTROL Categories], [!UICONTROL Condition], [!UICONTROL Condition Update], osv.

1. (Valfritt) Om du vill redigera objekt som hittas av snabbfiltret satsvis:

   1. Markera alla eller flera av objekten i listan och klicka sedan på **[!UICONTROL Edit]** om du vill redigera objekten gruppvis.
   1. När du är klar klickar du på **[!UICONTROL Save Changes]**.

1. (Valfritt) Om du vill exportera de objekt som hittas av snabbfiltret markerar du alla eller flera av objekten i listan och klickar sedan på **[!UICONTROL Export]**.

   ![select_all_projects_with_highlight_1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Endast de objekt du hittade i snabbfiltersökningen exporteras till den markerade filen. Om du inte markerar några objekt innan du exporterar listan exporteras den fullständiga, ofiltrerade listan.\
   >Mer information finns i [Exportera en lista](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Valfritt) Om du vill rensa de filtrerade resultaten klickar du på **[!UICONTROL Quick Filter]** i fönstrets övre högra hörn.\
   eller\
   Uppdatera sidan.

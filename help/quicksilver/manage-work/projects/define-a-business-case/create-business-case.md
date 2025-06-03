---
navigation-topic: business-case-and-scorecards
title: Skapa ett affärsärende för ett projekt
description: Du kan använda affärsärendet för att begära ett projekt och definiera syfte, budget och den potentiella fördelen för projektet. Portfolio-chefen eller projektsponsorn använder informationen från affärsärendet för att analysera och prioritera projektet innan de godkänner det.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: 9cfb67f627c06a5926e820860d52ba9f1ab58bcf
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Skapa ett affärsärende för ett projekt

Du kan använda affärsärendet för att begära ett projekt och definiera syfte, budget och den potentiella fördelen för projektet. Portfolio-chefen eller projektsponsorn använder informationen från affärsärendet för att analysera och prioritera projektet innan de godkänner det.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> 
   <p>Aktuell: Prime eller senare</p> 
   <p>Äldre: Pro eller senare</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Aktuell: Standard </p> 
   <p>Äldre: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt, finansiella data och resurshantering</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera eller högre behörigheter i projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Tänk på följande när du begär ett projekt via ett affärsärende:

* Adobe Workfront-administratören eller gruppadministratören måste aktivera avsnitten i affärsärendet innan de visas i ditt projekt.\
  Mer information om hur du aktiverar avsnitten i affärsärendet på systemnivå finns i artikeln [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Mer information om områden i affärsärendet finns i artikeln [Översikt över områden i affärsärendet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Du måste fylla i alla delar av affärsärendet utom målområdet om du vill att ditt projekt ska få en poäng i Portfolio Optimizer. Det är valfritt att slutföra målområdet. Projektet får en bakgrundsmusik i Portfolio Optimizer även om detta område inte är färdigt.

  Mer information om hur du arbetar med styrkort och med Portfolio Optimizer finns i artikeln [Använda ett styrkort i ett projekt och generera ett justeringsresultat](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Skapa ett affärsärende

{{step1-to-projects}}

1. Klicka på **Nytt projekt** och välj sedan **Begär projekt** i listrutan som visas. Projektet skapas och statusen **Idea** tilldelas som standard.

   >[!CAUTION]
   >
   >Om Idea-statusen har tagits bort i din Workfront-instans placeras projektet i standardstatus för nya projekt enligt definitionen i området Projektinställningar. Mer information om hur du ställer in projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Ange ett namn i projekttitelfältet.
1. (Valfritt) Klicka på ikonen **Mer** ![Mer](assets/qs-more-icon-on-an-object.png) och sedan på **Koppla mall** för att skapa projektets arbetsgruppsstruktur.

   eller

   Börja lägga till uppgifter i projektet manuellt.

1. (Villkorligt) Om du valde att koppla en mall fortsätter du att koppla mallen till projektet.
1. Klicka på **Affärsärende** i den vänstra panelen.
1. (Valfritt) Om du vill redigera avsnittet **Projektinformation** klickar du på **Redigera projektinformation**. 

   Mer information om hur du redigerar avsnittsfälten **Projektinformation** finns i avsnittet [Projektinformation](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) i artikeln [Översikt över områden i affärsärendet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Valfritt) Om du vill redigera avsnittet **Mål** klickar du på **Redigera mål**.

   Mer information om hur du redigerar avsnittet **Mål** i affärsärendet finns i avsnittet [Mål](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) i artikeln [Översikt över områden i affärsärendet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Valfritt) Om du vill redigera avsnittet **Utgifter** klickar du på **Redigera utgifter**.

   Mer information om hur du redigerar avsnittet **Utgifter** i affärsärendet finns i avsnittet [Utgifter](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) i artikeln [Översikt över områden i affärsärendet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Valfritt) Klicka på **Redigera resursbudgetering** om du vill budgetera dina resurser och hämta den budgeterade arbetskostnaden som är associerad med jobbrollerna i projektet. Mer information finns i [Budgetresurser i affärsärendet](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >Informationen som visas här är densamma som informationen som visas i resursbudgeteringsverktygen på systemnivå.

1. (Valfritt) Klicka på **Redigera risker** om du vill lägga till potentiella risker i projektet. Mer information om hur du lägger till risker i affärsärendet finns i avsnittet [Risker](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) i artikeln [Översikt över områden i affärsärendet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Valfritt) Välj ett **styrkort** i listrutan **Lägg till ett styrkort i det här projektet**.

   Styrkort måste skapas innan de kan kopplas till projekt.

   Mer information om styrkort finns i artikeln [Använda ett styrkort i ett projekt och generera ett justeringsresultat](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Valfritt) Välj ett **anpassat formulär** i listrutan **Egen Forms** .

   Anpassade Forms måste skapas innan de kan kopplas till projekt.

   Mer information om anpassad Forms finns i artikeln [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på **Skicka**. Projektets status ändras till **Begärd** och skickas för att få affärsärendet godkänt.

   Mer information om hur du godkänner ett affärsärende finns i artikeln [Godkänn ett affärsärende](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> När du är klar med affärsärendet kan du exportera en kopia av det till en PDF-fil. Mer information om hur du exporterar affärsärendet till en PDF-fil finns i [Exportera affärsärende för ett projekt](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).



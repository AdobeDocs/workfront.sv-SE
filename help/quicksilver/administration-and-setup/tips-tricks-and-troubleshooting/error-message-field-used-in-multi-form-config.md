---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: Det finns ett litet problem. Det fältet används i en flerformulärskonfiguration'
description: När du ändrar en beräkning i ett beräknat anpassat fält i ett anpassat formulär och ett felmeddelande anger att fältet används i en flerformulärskonfiguration, måste du ersätta fältet med ett nytt fält som innehåller den beräkning som du vill använda.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 0%

---

# Felmeddelande: Det finns ett litet problem. Det fältet används i en flerformulärskonfiguration

## Problem

När du ändrar en beräkning för ett beräknat anpassat fält i ett anpassat formulär, [!DNL Adobe Workfront] kan visa följande varning:

Det finns ett litet problem

[Fältet] används i en konfiguration med flera formulär. Om du vill ändra den här formeln måste du ta bort det här fältet och ersätta det med ett nytt som innehåller den önskade beräkningen.

## Orsak

Minst två anpassade formulär som innehåller det beräknade anpassade fältet som du försöker ändra bifogas till ett enda objekt i [!DNL Workfront] -instans.

**Exempel:** Anpassade formulär A och B är båda kopplade till samma uppgift. Båda formulären innehåller ett beräknat anpassat fält med namnet Vinst. Felet uppstår när du försöker redigera beräkningen i fältet Vinst i det anpassade formuläret A.

Du kan inte ändra beräkningen för det anpassade fältet i något av formulären eftersom det skulle strida mot formeln i samma fält i det andra formuläret.
För att lösa den här konflikten måste du hitta det objekt där flera formulär med samma beräknade anpassade fält är kopplade och sedan göra något av följande:

* Ta bort ett av formulären från objektet.
* Ändra beräkningen efter behov, men gör det i alla anpassade formulär som är kopplade till objektet.
* I alla anpassade formulär som är kopplade till objektet lägger du till ett nytt beräknat anpassat fält som innehåller den beräkning du behöver och markerar det gamla beräknade anpassade fältet som föråldrat.

I den här artikeln beskrivs hur du hittar objektet och sedan löser problemet på något av dessa tre sätt.

## Hitta det objekt som de anpassade formulären är kopplade till {#find-the-object-where-the-custom-forms-are-attached}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Users]** ![](assets/users-icon-in-main-menu.png).

1. Klicka på **[!UICONTROL Custom Forms]** > **[!UICONTROL Fields]**.
1. Använd **[!UICONTROL Field List]** för att hitta det beräkningsfält som du försöker ändra och för att anteckna alla anpassade formulär som det används i (t.ex. formulär 1, formulär 2, formulär 3).
1. Klicka **[!UICONTROL Forms]** och sedan använda **[!UICONTROL Form List]** vy.
1. Klicka på **[!UICONTROL Filter]** nedrullningsbar lista och **[!UICONTROL New Filter]**.

1. Klicka **[!UICONTROL Add a Filter Rule]** börjar du sedan skriva &quot;anpassat formulärnamn&quot; och väljer det här värdet när det visas i listan.
1. Välj **[!UICONTROL Equal]** för filtermodifieraren börjar du skriva namnet på varje formulär som du antecknade i steg 1 och markerar det när det visas.

   **Exempel:** Anpassat formulärnamn är lika med formulär 1, formulär 2, formulär 3.

1. Klicka **[!UICONTROL Save Filter]** och namnge sedan det nya filtret och klicka på **[!UICONTROL Save Filter]**.

1. Observera objekttypen för filtret, till exempel Aktivitet eller Problem, som visas i listan över formulär **[!UICONTROL Type]** kolumn.
1. För varje anpassat formulär som du hittade i steg 1 skapar du ett nytt anpassat kryssrutefält med standardvärdet Ja.

   **Exempel:** Fält 1 i formulär 1 = Ja, fält 2 i formulär 2 = Ja, fält 3 i formulär 3 = Ja. Det betyder&quot;Det beräknade anpassade fältet finns i formulär 1&quot; eller&quot;Det beräknade anpassade fältet finns i formulär 2&quot; och så vidare.

1. I **[!UICONTROL Search icon]** ![](assets/search-icon.png) i skärmens övre högra hörn klickar du på **[!UICONTROL Advanced Search]**.
1. Klicka på objektet i det anpassade formuläret (till exempel Problem) och klicka på **[!UICONTROL Filter your results]** och sedan klicka **[!UICONTROL Add a filter]**.
1. Börja skriva namnet på ett kryssrutefält i dialogrutan **[!UICONTROL Start typing field name]** och markera det när det visas i listan och markera sedan **[!UICONTROL Equal]** och text **[!UICONTROL Yes]** (utan citattecken) i följande ruta.

   **Exempel:** Fält 1 är lika med (skiftlägeskänsligt) Ja.

1. Klicka **[!UICONTROL Add a Filter]** och lägg till alla kryssrutefält i den avancerade sökningen.

   Leta efter alla möjliga kombinationer.

   **Exempel:** Bygg flera filter med de kombinationer du hittar enligt nedan. Du bör söka efter objekt med flera kopplade anpassade formulär som innehåller samma beräkningsfält. Följande scenarier kan finnas:

   * Fält 1= Ja + fält 2 = Ja + fält 3 = Ja (t.ex. inga objekt)
   * Fält 1= Ja + fält 2 = Ja (t.ex. inga objekt)
   * Fält 1= Ja + fält 3 = Ja (t.ex. två objekt)

   Det innebär att beräkningsfältet finns både i formulär 1 och i formulär 3, eftersom motsvarande kryssrutefält (fält 1 och fält 3) finns på dessa objekt.

   Fält 2 = Ja + fält 3 = Ja (t.ex. inga objekt)

1. Fortsätt till ett av följande avsnitt i den här artikeln:

   * [Ta bort ett av de anpassade formulären från objektet och redigera beräkningen där](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Gör identiska ändringar i beräkningen i alla kopplade anpassade formulär](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Lägg till ett nytt beräkningsfält som innehåller den redigerade beräkningen i ett eller alla kopplade anpassade formulär](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Ta bort ett av de anpassade formulären från objektet och redigera beräkningen där {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Hitta det objekt som de anpassade formulären är kopplade till, vilket förklaras i [Hitta det objekt som de anpassade formulären är kopplade till](#find-the-object-where-the-custom-forms-are-attached) öppna objektet i den här artikeln.
1. Ta bort ett av de anpassade formulären från objektet och spara sedan objektet.

   >[!NOTE]
   >
   >Om du vill lägga till fälten från det formulär som du har tagit bort från objektet kan du behöva redigera det anpassade formuläret som fortfarande är kopplat till objektet. På så sätt kan du bevara den anpassade datainformationen för objektet.

1. I det anpassade formuläret som du tog bort redigerar du beräkningen för det anpassade fält som du ursprungligen försökte uppdatera och klickar sedan på **[!UICONTROL Save]**.

   Den här gången [!DNL Workfront] ska inte stöta på en konflikt.

1. (Valfritt) Ta bort kryssrutefälten från anpassade formulär eller ta bort dem från [!DNL Workfront].

## Gör identiska ändringar i beräkningen i alla kopplade anpassade formulär {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Data förloras i de objekt där det anpassade formuläret redan är bifogat när du följer dessa steg. Om beräkningsfältet refererar till statiska fält, inte beräknade fält, kan du använda [!UICONTROL Recalculate Custom Expressions] alternativ på objektet för att återställa förlorade data

1. Hitta det objekt som de anpassade formulären är kopplade till, vilket förklaras i [Hitta det objekt som de anpassade formulären är kopplade till](#find-the-object-where-the-custom-forms-are-attached) i den här artikeln.
1. Ta bort fältet från alla anpassade formulär som är kopplade till objektet och spara sedan formulären.

1. Lägg till det anpassade fältet som innehåller den nya beräkningen i de anpassade formulären.

   >[!IMPORTANT]
   >
   >Beräkningarna måste vara identiska i alla kopplade anpassade formulär.

1. (Valfritt) Ta bort kryssrutefälten från formulären eller ta bort dem från [!DNL Workfront].

## Lägg till ett nytt beräkningsfält som innehåller den redigerade beräkningen i ett eller alla kopplade anpassade formulär {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Så här undviker du att förlora data i det befintliga beräknade anpassade fältet eller om du behöver göra den redigerade beräkningen i endast ett av de anpassade formulären som är kopplade till det objekt du hittade:

1. Hitta det objekt som de anpassade formulären är kopplade till, vilket förklaras i [Hitta det objekt som de anpassade formulären är kopplade till](#find-the-object-where-the-custom-forms-are-attached) i den här artikeln.
1. Lägg till ett nytt beräknat anpassat fält som innehåller beräkningen som du behöver för ett eller alla formulär.
1. Byt namn på det gamla beräknade anpassade fältet **Föråldrad**.

   På alla formulär som bifogats objektet bevarar det här äldre beräknade anpassade formuläret sina historiska data, men användarna slutar använda dem.

   >[!IMPORTANT]
   >
   >Det äldre fältet kan refereras till i andra beräknade anpassade fält, så du måste uppdatera dessa beräkningar efter att ha ändrat dess namn.

1. (Valfritt) Ta bort kryssrutefälten från formulären eller ta bort dem från Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->

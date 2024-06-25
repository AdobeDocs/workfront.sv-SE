---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär med det äldre formulärverktyget
description: Du kan använda samma beräknade anpassade fält i anpassade formulär som tillhör olika objekt. Du kan till exempel använda fältet Resultatberäkning som du skapade för det anpassade projektformuläret i ett anpassat aktivitetsformulär.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär med det äldre formulärverktyget

{{form-designer-default}}

Du kan använda samma beräknade anpassade fält i anpassade formulär som tillhör olika objekt. Du kan till exempel använda fältet Resultatberäkning som du skapade för det anpassade projektformuläret i ett anpassat aktivitetsformulär.

Mer information om hur du lägger till ett beräknat anpassat fält i ett anpassat formulär finns i [Lägga till beräknade data i ett anpassat formulär med äldre formulärverktyg](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

När du använder ett befintligt beräknat anpassat fält överförs inte beräkningen till det nya formuläret. Du måste lägga till beräkningen igen, i samma fält, i det nya anpassade formuläret.

>[!TIP]
>
>Det här är när du använder beräkningen som lagras i **Instruktioner** fält i det anpassade formuläret.

Du kan också ha en annan beräkning för samma fält i det nya formuläret. Om du behåller samma namn för det beräknade anpassade fältet är namnkonventionen konsekvent och konsekvent.

>[!IMPORTANT]
>
>Beräknade anpassade fält kan bli inaktuella över tid. Gör något av följande om du alltid vill se den aktuella beräkningen i dessa fält:
>
>* När du har sparat ett objekt där du har redigerat data i ett kopplat anpassat formulär klickar du på ikonen Mer ![](assets/more-icon.png) på objektets huvudsida och beräkna om anpassade uttryck.
>* Markera alternativet Beräkna om anpassade uttryck när du redigerar flera objekt samtidigt.
>* Välj alternativet Uppdatera tidigare beräkningar när du redigerar ett beräknat anpassat fält i ett anpassat formulär.
>

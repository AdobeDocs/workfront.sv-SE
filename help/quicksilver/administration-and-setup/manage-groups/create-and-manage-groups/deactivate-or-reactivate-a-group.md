---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Inaktivera eller återaktivera en grupp
description: Du kan inaktivera en grupp som du hanterar och som du inte längre använder.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Inaktivera eller återaktivera en grupp

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Du kan inaktivera en grupp som du hanterar och som du inte längre använder.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Inaktivera eller återaktivera en grupp

>[!IMPORTANT]
>
>När du inaktiverar en grupp inaktiveras även undergrupper.
>
>Om du behöver aktivera om någon av dem kan du göra det när du har gjort något av följande:
>
>* Ta bort den från den överordnade gruppen. Mer information finns i avsnittet [Ta bort en undergrupp från den överordnade gruppen och gör den till en grupp på den översta nivån](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) i artikeln [Hantera en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Flytta den under en aktiv grupp. Mer information finns i avsnittet [Skapa, flytta, visa, redigera, kopiera, byta namn på, exportera eller ta bort en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) i artikeln [Hantera en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Välj **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen för att öppna sidan.

1. Klicka på Mer-menyn ![](assets/more-icon.png) bredvid namnet på gruppen och klicka sedan på **Inaktivera** eller **Återaktivera**.

   >[!NOTE]
   >
   >Alternativet Är aktiv (alternativet Återaktivera i förhandsvisning) är inte tillgängligt om gruppen är en undergrupp till en inaktiverad grupp. Innan du kan återaktivera den måste du ta bort den från den överordnade gruppen eller flytta den under en grupp som är aktiv, vilket beskrivs i Viktigt-kommentaren ovan.

1. (Villkorligt) Om du inaktiverar gruppen klickar du på **Inaktivera** i **Inaktivera grupp** som visas.

## Överväganden för inaktiva grupper

Tänk på följande när det gäller en grupp som du inaktiverar genom att inaktivera alternativet Är aktiv som förklaras i avsnittet [Inaktivera eller återaktivera en grupp](#View) i den här artikeln.

* Om du inaktiverar en grupp inaktiveras även alla undergrupper under den. Detta inkluderar undergrupper som du lägger till efter att du har inaktiverat den.

   Information om hur du återaktiverar en undergrupp i den här situationen finns i [Återaktivera en undergrupp under en inaktiv överordnad grupp](#about-reactivating-a-subgroup-below-an-inactive-parent-group) i den här artikeln.

* När du går till området Grupper i Konfigurera kan du bara se aktiva grupper i listan eftersom Aktiv är standardfiltret ![](assets/filter-nwepng.png) för den. Om du vill se alla grupper som du hanterar, inklusive de inaktiva, kan du använda filtret Alla. Eller använd filtret Inaktiv för att endast visa de inaktiva.

   Mer information om filter i listor finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* När du inaktiverar en grupp ändras inte följande:

   * Gruppens associationer till objekt. Associerade objekt fortsätter att fungera som tidigare, utan några ändringar.

      Om ett projekt till exempel är associerat med en grupp som du inaktiverar, fortsätter projektet att använda gruppens inställningar och statusvärden utan att några ändringar görs.

   * Du kan skapa ett nytt objekt, till exempel ett godkännande, ett team eller ett företag, från gruppens sida vid konfigurationen. Som standard är det nya objektet kopplat till den inaktiva gruppen.
   * Som administratör kan du hitta gruppen i filter och rapporter.

      Du kan också söka efter den i grupptypsfält där du kanske vill hantera gruppens inställningar under Konfigurera. Detta omfattar områdena Inställningar, Händelsemeddelanden och Systemlicenser.

      Om du t.ex. går till Inställningar > Projektinställningar > Projekt och rensar textfältet ovanför alternativen där, kan du fortfarande hitta en inaktiv grupp och konfigurera dess projektinställningar.

## Återaktivera en undergrupp under en inaktiv överordnad grupp {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Om du inaktiverar en grupp inaktiveras även alla undergrupper under den. Om du behöver aktivera om en av undergrupperna under en inaktiv grupp kan du göra något av följande:

* Flytta undergruppen under en aktiv grupp. Aktivera sedan alternativet Är aktiv för den flyttade gruppen enligt anvisningarna i avsnittet [Inaktivera eller återaktivera en grupp](#View) i den här artikeln.

   Instruktioner om hur du flyttar en grupp finns i [Flytta en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Ta bort undergruppen från den överordnade gruppen (vilket gör undergruppen till en grupp på den översta nivån). Aktivera sedan alternativet Är aktiv för den flyttade gruppen enligt anvisningarna i avsnittet [Inaktivera eller återaktivera en grupp](#View) i den här artikeln.

   Instruktioner om hur du tar bort en undergrupp från den överordnade gruppen finns i avsnittet [Ta bort en undergrupp från den överordnade gruppen och gör den till en grupp på den översta nivån](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) i artikeln [Hantera en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

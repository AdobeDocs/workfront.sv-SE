---
user-type: administrator
product-area: system-administration;user-management
keywords: hantera,undergrupp,redigera
navigation-topic: create-and-manage-subgroups
title: Hantera en undergrupp
description: Som gruppadministratör för en undergrupp kan du skapa, flytta, visa, redigera, kopiera, byta namn på, exportera och ta bort undergruppen. Du kan också göra en undergrupp till en grupp på den översta nivån genom att ta bort den från den överordnade gruppen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 6c3f5ee43040f81dac734c5e0b4def9021a0d737
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Hantera en undergrupp

Som gruppadministratör för en undergrupp kan du skapa, flytta, visa, redigera, kopiera, byta namn på, exportera och ta bort undergruppen.

Du kan också göra en undergrupp till en grupp på den översta nivån genom att ta bort den från den överordnade gruppen.

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Mer information om undergrupper finns i [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>När du hanterar en grupp som innehåller undergrupper är det praktiskt att kunna identifiera och filtrera data om hela gruppen och alla dess undergrupper. Du kan göra detta genom att använda fältet Överst överordnat ID i en rapport eller lista.
>
>Tänk dig till exempel att du hanterar en stor marknadsföringsavdelning och vill ha en lista över alla projekt som hela avdelningen arbetar med.
>
>I Workfront representeras den här marknadsföringsavdelningen av en grupp som heter Marketing, med tre undergrupper som kallas Field Marketing, Product Marketing och Digital Marketing. Om du vill visa de projekt som tillhör hela marknadsföringsavdelningen (alla fyra grupper) kan du skapa ett filter för projektområdet med följande filterregel:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Du kan också använda fältet Överst överordnat namn för att identifiera data som är kopplade till en grupp på den översta nivån, men bara i vyer, inte i filter eller grupperingar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en undergrupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen där du vill lägga till en undergrupp.
1. Klicka på **Undergrupper** på den vänstra menyn.
1. Klicka på **Lägg till undergrupp** om du vill skapa en ny undergrupp en nivå nedåt från den grupp du visar.

   Om du vill skapa den nya undergruppen under en annan undergrupp i listan, markerar du den undergruppen och klickar sedan på **Lägg till undergrupp**.

   Mer information om de alternativ du kan använda för att konfigurera undergruppen finns i [Skapa en undergrupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

   En grupphierarki får inte överskrida 15 nivåer, men en nivå kan ha ett obegränsat antal parallella grupper.

## Flytta en undergrupp

Du kan flytta befintliga undergrupper under en annan grupp som du administrerar.

En grupphierarki får inte överskrida 15 nivåer, men en nivå kan ha ett obegränsat antal parallella grupper.

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på målgruppen (du anger vilka undergrupper du vill flytta i ett senare steg).
1. Klicka på **Undergrupper** på den vänstra menyn.
1. (Valfritt) Markera en undergrupp för att göra den till målgrupp.

   Om du hoppar över det här steget är den grupp du valde i steg 3 målgruppen.

1. Klicka på **Lägg till undergrupp > Befintlig grupp**.
1. I rutan **Befintlig grupp** som visas börjar du skriva namnet på den undergrupp som du vill flytta.

   Resultatet som visas innehåller inte grupper ovanför målgruppen.

   Du kan kontrollera att du markerar rätt grupp genom att hålla markören över den och klicka på informationsikonen ![informationsikonen](assets/info-icon.png) som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.

1. Markera namnet på den undergrupp som du vill flytta när du hittar den i listan.
1. Upprepa steg 7-8 för alla andra undergrupper som du vill flytta till målgruppen.
1. Klicka på **Spara**.

## Redigera en undergrupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som innehåller den undergrupp som du vill redigera.
1. Klicka på **Undergrupper** på den vänstra menyn.
1. Markera den undergrupp som du vill redigera och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

   Mer information om de alternativ du kan använda för att konfigurera undergruppen finns i [Skapa en undergrupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Kopiera en undergrupp

>[!NOTE]
>
>Endast en systemadministratör kan kopiera en undergrupp.

När du kopierar en undergrupp blir den en överordnad grupp. Alla gruppmedlemmar och undergrupper kopieras med den. Gruppens medlemmar behåller alla uppdrag de hade i den ursprungliga gruppen.

Tänk på följande när du kopierar en undergrupp:

* Om en undergrupp som du kopierar har egna undergrupper, inkluderas de i kopian och deras namn formateras enligt följande:

  `Original subgroup name (Copy)`

* Alla undergrupper som tillhör en offentlig grupp är också publika, så alla användare som har behörighet att redigera användare, i eller utanför gruppen, kan lägga till användare i undergruppen.

Så här kopierar du en undergrupp:

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som innehåller den undergrupp som du vill kopiera.
1. Klicka på **Undergrupper** på den vänstra menyn.
1. Markera en undergrupp och klicka sedan på ikonen **Kopiera** ![Kopiera](assets/copy-icon.png) för att skapa en ny grupp på den översta nivån baserad på den markerade gruppen.
1. Konfigurera den nya gruppens inställningar.

   Hjälp med de här inställningarna finns i [Skapa en grupp på den översta nivån genom att kopiera en befintlig grupp eller undergrupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) i artikeln [Skapa en grupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Klicka på **Skapa grupp**.

## Exportera en undergrupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som innehåller den undergrupp som du vill exportera.
1. Klicka på **Undergrupper** på den vänstra menyn.
1. Markera den eller de undergrupper som du vill exportera.
1. Klicka på ikonen **Exportera** ![Ikonen Exportera](assets/export.png) och välj sedan önskat filformat.

## Ta bort en undergrupp från den överordnade gruppen och gör den till en grupp på den översta nivån

Du kan göra en undergrupp till en grupp på den översta nivån genom att ta bort den från den överordnade gruppen.

>[!TIP]
>
>När du inaktiverar en grupp som innehåller undergrupper blir även dessa undergrupper inaktiva. Om du vill att någon av dem ska vara aktiv kan du använda dessa instruktioner för att ta bort den från den överordnade gruppen och sedan återaktivera den.
>&#x200B;>Instruktioner om hur du inaktiverar och återaktiverar grupper finns i [Inaktivera eller återaktivera en grupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.
1. Markera den överordnade gruppen för den undergrupp som du vill skapa en grupp på den översta nivån och klicka sedan på ikonen **Redigera** ![Redigera ](assets/edit-icon.png) .
1. I rutan **Redigera grupp** som visas börjar du skriva namnet på den undergrupp som du vill skapa en grupp på den översta nivån i fältet **Sök** (under **Gruppmedlemmar och gruppadministratörer**) och klickar sedan på krysset till höger om namnet när det visas.
1. Klicka på **Spara**.

## Ta bort en undergrupp

>[!IMPORTANT]
>
>När du tar bort en grupp eller undergrupp måste du bevara de användare, arbetsobjekt och alla undergrupper som är tilldelade till den. För att du ska kunna vara säker på att objekten bevaras måste du omtilldela gruppens objekt till en annan grupp.

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som innehåller den undergrupp som du vill ta bort.
1. Klicka på **Undergrupper** på den vänstra menyn.
1. Markera undergruppen och klicka sedan på ikonen **Ta bort** ![Ta bort](assets/delete.png) .

   I rutan **Ta bort grupp** som visas börjar du skriva och markerar sedan namnet på gruppen där du vill flytta medlemmarna, arbetsobjekten och undergrupperna i gruppen som du vill ta bort.

1. Klicka på **Ta bort**.

## Visa och hantera undergruppsmedlemmar

När du visar huvudsidan för en grupp som du administrerar kan du visa och hantera alla användare i gruppens undergrupper. Instruktioner finns i [Visa och hantera undergruppsmedlemmar](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).


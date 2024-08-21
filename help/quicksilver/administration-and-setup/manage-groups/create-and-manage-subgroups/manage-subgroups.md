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
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 1%

---

# Hantera en undergrupp

Som gruppadministratör för en undergrupp kan du skapa, flytta, visa, redigera, kopiera, byta namn på, exportera och ta bort undergruppen.

Du kan också göra en undergrupp till en grupp på den översta nivån genom att ta bort den från den överordnade gruppen.

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Mer information om undergrupper finns i [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Skapa, flytta, visa, redigera, kopiera, byta namn på, exportera eller ta bort en undergrupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som innehåller den undergrupp som du vill arbeta med.

   eller

   Om du flyttar en eller flera undergrupper klickar du på namnet på målgruppen (du anger vilka undergrupper du vill flytta i ett senare steg).

1. Klicka på **Undergrupper** på den vänstra menyn.

1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Skapa en ny undergrupp</td> 
      <td> <p>Om du vill skapa den nya undergruppen en nivå ned från den grupp du visar klickar du på <strong>Lägg till undergrupp</strong>.</p> <p>Om du vill skapa den nya undergruppen under en annan undergrupp i listan, markerar du den undergruppen och klickar sedan på <strong>Lägg till som</strong><strong>undergrupp</strong>.</p> <p>Mer information om de alternativ du kan använda för att konfigurera undergruppen finns i tabellen i <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Skapa en undergrupp</a>.</p> <p>En grupphierarki får inte överskrida 15 nivåer, men en nivå kan ha ett obegränsat antal parallella grupper.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flytta en undergrupp </td> 
      <td> <p>Du kan flytta befintliga undergrupper under en annan grupp som du administrerar.</p> <p>En grupphierarki får inte överskrida 15 nivåer, men en nivå kan ha ett obegränsat antal parallella grupper.</p> 
       <ol> 
        <li value="1"> <p>(Valfritt) Markera en undergrupp för att göra den till målgrupp.</p> <p>Om du hoppar över det här steget är den grupp du valde i steg 3 målgruppen.</p> </li> 
        <li value="2">Klicka på <strong>Lägg till undergrupp</strong> &gt; <strong>Befintlig grupp</strong>.</li> 
        <li value="3"> <p>I rutan <strong>Befintlig grupp</strong> som visas börjar du skriva namnet på den undergrupp som du vill flytta.</p> <p>Resultatet som visas innehåller inte grupper ovanför målgruppen.</p> <p>Du kan kontrollera att du markerar rätt grupp genom att hålla markören över den och klicka på informationsikonen <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> </li> 
        <li value="4"> <p>Klicka på namnet på den undergrupp som du vill flytta när den visas i listan.</p> </li> 
        <li value="5"> <p>Upprepa steg c-d för andra undergrupper som du vill flytta till målgruppen</p> </li> 
        <li value="6">Klicka på <strong>Spara</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redigera en undergrupp</td> 
      <td> <p>Markera den undergrupp som du vill redigera och klicka sedan på ikonen Redigera <img src="assets/edit-icon.png">.</p> <p>Mer information om de alternativ du kan använda för att konfigurera undergruppen finns i tabellen i <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Skapa en grupp</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera en eller flera undergrupper</td> 
      <td> 
       <ol> 
        <li value="1">Markera den eller de undergrupper som du vill exportera.</li> 
        <li value="2">Klicka på ikonen Exportera <img src="assets/export.png"> och välj sedan önskat filformat.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiera en undergrupp för att skapa en ny grupp på den översta nivån</td> 
      <td> <p>(Endast tillgängligt för Workfront-administratörer.) När du kopierar en undergrupp blir den en överordnad grupp. Alla gruppmedlemmar och undergrupper kopieras med den. Gruppmedlemmarna behåller de uppdrag de hade i den ursprungliga gruppen.</p> <p>Mer information om hur du kopierar en undergrupp finns i <a href="#about-copying-a-subgroup" class="MCXref xref">Kopiera en undergrupp</a> i den här artikeln.</p> 
       <ol> 
        <li value="1">Markera en undergrupp och klicka sedan på ikonen Kopiera <img src="assets/copy-icon.png"> för att skapa en ny grupp på den översta nivån baserad på den markerade gruppen.</li> 
        <li value="2"> <p>Konfigurera den nya gruppens inställningar.</p> <p>Hjälp med de här inställningarna finns i tabellen i avsnittet <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Skapa en grupp på den översta nivån genom att kopiera en befintlig grupp eller undergrupp</a> i artikeln <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Skapa en grupp på den översta nivån genom att kopiera en befintlig grupp eller undergrupp</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort en undergrupp</td> 
      <td> <p><b>VIKTIGT</b>: När du tar bort en grupp eller undergrupp måste du bevara de användare, arbetsobjekt och undergrupper som för närvarande är tilldelade till den. För att du ska kunna vara säker på att objekten bevaras måste du omtilldela gruppens objekt till en annan grupp i steget nedan.</p> 
       <ol> 
        <li value="1">Markera undergruppen och klicka sedan på ikonen Ta bort <img src="assets/delete.png">.</li> 
        <li value="2">I rutan <strong>Ta bort grupp</strong> som visas börjar du skriva och markerar sedan namnet på gruppen där du vill flytta medlemmarna, arbetsobjekten och undergrupperna i gruppen som du vill ta bort.</li> 
        <li value="3">Klicka på <strong>Ta bort dem</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

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
>Du kan också använda fältet Överst överordnat namn för att identifiera data som är kopplade till en grupp på den översta nivån, men bara i Vyer, inte i Filter eller Grupperingar.

## Ta bort en undergrupp från den överordnade gruppen och gör den till en grupp på den översta nivån

Du kan göra en undergrupp till en grupp på den översta nivån genom att ta bort den från den överordnade gruppen.

>[!TIP]
>
>När du inaktiverar en grupp som innehåller undergrupper blir även dessa undergrupper inaktiva. Om du vill att någon av dem ska vara aktiv kan du använda dessa instruktioner för att ta bort den från den överordnade gruppen och sedan återaktivera den.
>
>Instruktioner om hur du inaktiverar och återaktiverar grupper finns i avsnitten [Visa och hantera information om en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) och [Visa och hantera information om en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) i artikeln [Visa och hantera information om en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Markera den överordnade gruppen för gruppen som du vill skapa en grupp på den översta nivån och klicka sedan på redigeringsikonen ![](assets/edit-icon.png).
1. I rutan **Redigera grupp** som visas, under **Gruppmedlemmar och gruppadministratörer**, börjar du skriva namnet på den undergrupp som du vill skapa en grupp på översta nivån och klickar sedan på krysset till höger om namnet när det visas.
1. Klicka på **Spara**.

## Visa och hantera undergruppsmedlemmar

När du visar huvudsidan för en grupp som du administrerar kan du visa och hantera alla användare i gruppens undergrupper. Instruktioner finns i [Visa och hantera undergruppsmedlemmar](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Kopiera en undergrupp {#about-copying-a-subgroup}

Tänk på följande när du kopierar en undergrupp.

* Om en undergrupp som du kopierar har egna undergrupper, inkluderas de i kopian och deras namn formateras enligt följande:

  `Original subgroup name (Copy)`

* Alla undergrupper som tillhör en offentlig grupp är också publika, så alla användare med redigeringsåtkomst, i eller utanför gruppen, kan lägga till användare i undergruppen.

---
product-area: projects
navigation-topic: use-predecessors
title: Tvinga föregående
description: Föregångare är uppgifter som andra åtgärder är beroende av för att slutföras. Föregående relationer påverkar start- och slutförandedatum för aktiviteterna och påverkar i slutändan tidslinjen för projektet.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Tvinga föregående

<!-- Audited: 11/2025 -->

Föregångare är uppgifter som andra åtgärder är beroende av för att slutföras. Föregående relationer påverkar start- och slutförandedatum för aktiviteterna och påverkar i slutändan tidslinjen för projektet.

Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Genom att ställa in föregående relationer mellan uppgifter definierar du hur början eller slutet av en beroende uppgift beror på början eller slutet av deras föregående aktiviteter. Detta görs genom att använda olika beroendetyper.

Mer information om beroendetyper finns i [Översikt över aktivitetsberoendetyper](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Översikt över framtvingade föregångare

>[!IMPORTANT]
>
>Du måste framtvinga föregående för att kräva att föregående relationer respekteras. Utan att tvinga föregående aktiviteter kan de beroende uppgifterna starta och avslutas oberoende av början och slutet av föregående aktiviteter, oavsett deras beroendetyper.

Du kan använda föregående relation när du anger föregångare för ett projekt.

Om en föregångare används kan efterföljande aktivitet inte starta innan föregångaren har slutförts. Om du till exempel tvingar en relation mellan aktivitet A och Aktivitet B (Slutför/Start) innebär det att aktivitet B inte kan starta (statusen måste förbli Ny och Procent slutfört måste vara 0 %) tills Aktivitet A markeras som slutförd. Tvingande relationer gäller för alla föregående typer.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
      <p>New: Standard</p> 
      <p>OR</p>
      <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Tvinga en föregångare på aktivitetsnivå

1. Gå till den efterföljande uppgift vars föregångare du vill framtvinga.
1. Klicka på **Föregående** i den vänstra panelen och klicka sedan på **Lägg till föregående**.
1. (Villkorligt) Om du vill lägga till en föregångare för flera projekt tar du bort namnet på projektet i fältet **Överordnat projekt** och ersätter det med ett annat projekt.
1. Ange namnet på föregående aktivitet eller aktiviteter i fältet **Uppgifter**.
1. Ange **beroendetyp** mellan dessa två uppgifter.

   Standardberoendetypen **är** **Finish-Start**.

1. Markera fältet **Kräv** om du vill framtvinga föregående.
1. Klicka på **Spara**.

## Tvinga en föregångare i en uppgiftslista

1. Gå till en uppgiftslista i ett projekt.
1. Välj **Standardvy** i listrutan **Visa**.

1. Anteckna antalet uppgifter som du ska ange som föregångare.
1. Hitta den efterföljande uppgift vars föregångare du vill framtvinga.
1. I kolumnen **Föregående** börjar du ange antalet föregående aktiviteter följt av&quot;e&quot;. Skriv till exempel&quot;1e&quot; om du vill lägga till aktivitetsnummer 1 som en föregångare till den valda aktiviteten.
1. Klicka på Retur för att spara föregående information för uppgiften.

   ![Listan över framtvingad föregångare](assets/predecessor-enforced-in-list-350x308.png)

   Informationen om den föregångare som verkställs sparas omedelbart.

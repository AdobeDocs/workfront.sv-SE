---
product-area: projects
navigation-topic: use-predecessors
title: Tvinga föregående
description: Föregångare är uppgifter som andra åtgärder är beroende av för att slutföras. Föregående relationer påverkar start- och slutförandedatum för aktiviteterna och påverkar i slutändan tidslinjen för projektet.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 7a9232f59e4c6f2eac2995be7d7862295b6bab2c
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Tvinga föregående

<!-- Audited: 2/2024 -->

Föregångare är uppgifter som andra åtgärder är beroende av för att slutföras. Föregående relationer påverkar start- och slutförandedatum för aktiviteterna och påverkar i slutändan tidslinjen för projektet.

Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Genom att ställa in föregående relationer mellan uppgifter definierar du hur början eller slutet av en beroende uppgift beror på början eller slutet av deras föregående aktiviteter. Detta görs genom att använda olika beroendetyper.

Mer information om beroendetyper finns i [Översikt över typer av uppgiftsberoenden](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Översikt över framtvingade föregångare

>[!IMPORTANT]
>
>Du måste framtvinga föregående för att kräva att föregående relationer respekteras. Utan att tvinga föregående aktiviteter kan de beroende uppgifterna starta och avslutas oberoende av början och slutet av föregående aktiviteter, oavsett deras beroendetyper.

Du kan använda föregående relation när du anger föregångare för ett projekt.

Om en föregångare används kan efterföljande aktivitet inte starta innan föregångaren har slutförts. Om du till exempel tvingar en relation mellan aktivitet A och Aktivitet B (Slutför/Start) innebär det att aktivitet B inte kan starta (statusen måste förbli Ny och Procent slutfört måste vara 0 %) tills Aktivitet A markeras som slutförd. Tvingande relationer gäller för alla föregående typer.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
      <p>Nytt: Standard</p> 
      <p>ELLER</p>
      <p>Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td><p>Hantera behörigheter för aktiviteterna och projektet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Tvinga en föregångare på aktivitetsnivå

1. Gå till den efterföljande uppgift vars föregångare du vill framtvinga.
1. Klicka **Föregående** i den vänstra panelen och klickar sedan på **Lägg till föregående**. Du kan behöva klicka **Visa fler** sedan **Föregående**.
1. (Villkorligt) Om du vill lägga till en föregångare för flera projekt tar du bort namnet på projektet i **Överordnat projekt** och ersätta det med ett annat projekt.
1. Ange namnet på föregående aktivitet eller uppgifter i dialogrutan **Uppgifter** fält.
1. Ange **Beroendetyp** mellan dessa två uppgifter.

   Standardvärdet **Beroendetyp** är **Slutför-Start**.

1. Välj **Krävs** för att framtvinga föregående.
1. Klicka **Spara**.

## Tvinga en föregångare i en uppgiftslista

1. Gå till en uppgiftslista i ett projekt.
1. Från **Visa** väljer du **Standardvy**.

1. Anteckna antalet uppgifter som du ska ange som föregångare.
1. Hitta den efterföljande uppgift vars föregångare du vill framtvinga.
1. I **Föregående** börjar du ange antalet föregående aktiviteter följt av&quot;e&quot;. Skriv till exempel&quot;1e&quot; om du vill lägga till aktivitetsnummer 1 som en föregångare till den valda aktiviteten.
1. Klicka på Retur för att spara föregående information för uppgiften.

   ![predecessor_enforcement_in_list.png](assets/predecessor-enforced-in-list-350x308.png)

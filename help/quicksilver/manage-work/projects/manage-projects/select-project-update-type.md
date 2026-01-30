---
product-area: projects
navigation-topic: manage-projects
title: Välj typ av projektuppdatering
description: Genom att välja en uppdateringstyp för ett projekt kan du styra hur ofta de ändringar du gör i tidslinjen för projektet sparas för de överordnade uppgifterna eller för projektet.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Välj typ av projektuppdatering

Genom att välja en uppdateringstyp för ett projekt kan du styra hur ofta de ändringar du gör i tidslinjen för projektet sparas för de överordnade uppgifterna eller för projektet.

När projekttidslinjen uppdateras beräknas den om baserat på ändringar som gjorts i projektet, dess uppgifter eller ändringar som gjorts i ett annat projekt som tidslinjen är beroende av.

Följande ändringar av aktiviteterna i projektet utlöser till exempel en uppdatering av tidslinjen i projektet:

* Uppdatera datum för uppgifter
* Ändra föregående relationer för uppgifter
* Ändra överordnade och underordnade relationer genom att lägga till eller ta bort tilldelningar förutom att ändra uppgiftens begränsning eller varaktighet.

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
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uppdatera ett projekts uppdateringstyp

När uppgifterna uppdateras uppdateras deras överordnade objekt (överordnade uppgifter eller projektet) vid den tidpunkt som anges av uppdateringstypen.  Så här anger du en uppdateringstyp för projektet:

1. Gå till det projekt vars uppdateringstyp du vill ange.
1. Klicka på Mer-menyn ![Mer-ikonen](assets/more-icon.png) bredvid namnet på projektet och klicka sedan på **Redigera** .

1. Klicka på **Projekt** **Inställningar**.

   ![Uppdatera typfält i redigeringsrutan för projekt](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. I fältet **Uppdatera typ** väljer du om du vill att Workfront ska beräkna tidslinjen för projektet automatiskt varje dag, när en ändring görs eller om du vill att projektledaren ska beräkna den manuellt.

   Välj bland alternativen i listan nedan.

   >[!IMPORTANT]
   >
   >Om tidslinjen för ett projekt är längre än 15 år beräknas tidslinjen inte automatiskt eller vid ändring i Workfront. Uppdateringstypen för ett projekt som är längre än 15 år är alltid Manuell.

   * **Automatisk och vid ändring:** Det här är standardinställningen. Projektets tidslinje uppdateras varje gång en ändring inträffar i projektet eller i ett annat projekt som tidslinjen är beroende av. Projektets tidslinje uppdateras också varje kväll.\
     Detta är den rekommenderade inställningen eftersom den ser till att projekttidslinjen alltid är uppdaterad.

     När du uppdaterar en uppgift eller ett projekt och utlöser en omberäkning av tidslinjen, visas alla tillgängliga datum omedelbart så att du kan fortsätta arbeta. I projekt med mer än 100 uppgifter är datum som kräver längre beräkningar nedtonade.

     ![Datum nedtonade vid redigering inline](assets/dates-dimmed-when-insline-editing-350x146.png)

     Detta anger att omberäkningen ännu inte är klar och att datumen kan ändras.

   * **Ändra endast:** Projektets tidslinje uppdateras varje gång en ändring inträffar i projektet eller i ett annat projekt som tidslinjen är beroende av. Schemalagda uppdateringar görs inte.\
     Du kan välja det här alternativet om du är oroad över systemprestanda och om det är ovanligt att ändringar görs i projektet eller i andra projekt som tidslinjen är beroende av.

   * **Endast automatiskt:** Projektets tidslinje uppdateras varje natt. Den uppdateras inte omedelbart efter att ändringar har gjorts.\
     Du kanske vill välja det här alternativet om du är oroad över systemprestanda och om många ändringar inträffar varje dag i projektet eller i andra projekt som tidslinjen är beroende av.

     >[!NOTE]
     >
     >Ett projekt beräknas inte automatiskt om varje kväll om det har statusen Planering. Den räknar bara om vid förändring.

   * **Endast manuell:** Projektets tidslinje uppdateras bara när du väljer alternativet **Beräkna om tidslinjer**, vilket beskrivs i avsnittet Manuell omberäkning i artikeln [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
     Du kan välja det här alternativet om du gör många ändringar i projektet samtidigt och du vill att tidslinjen ska räknas om efter att alla ändringar har gjorts (i stället för efter varje enskild ändring).

1. Klicka på **Spara**.

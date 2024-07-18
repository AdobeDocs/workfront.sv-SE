---
product-area: projects
navigation-topic: manage-projects
title: Välj typ av projektuppdatering
description: Genom att välja en uppdateringstyp för ett projekt kan du styra hur ofta de ändringar du gör i tidslinjen för projektet sparas för de överordnade uppgifterna eller för projektet.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Välj typ av projektuppdatering

Genom att välja en uppdateringstyp för ett projekt kan du styra hur ofta de ändringar du gör i tidslinjen för projektet sparas för de överordnade uppgifterna eller för projektet.

När projekttidslinjen uppdateras beräknas den om baserat på ändringar som gjorts i projektet, dess uppgifter eller ändringar som gjorts i ett annat projekt som tidslinjen är beroende av.

Följande ändringar av aktiviteterna i projektet utlöser till exempel en uppdatering av tidslinjen  av projektet:

* Uppdatera datum för uppgifter
* Ändra föregående relationer för uppgifter
* Ändra överordnade och underordnade relationer genom att lägga till eller ta bort tilldelningar förutom att ändra uppgiftens begränsning eller varaktighet.

## Åtkomstkrav

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Uppdatera ett projekts uppdateringstyp

När uppgifterna uppdateras uppdateras deras överordnade objekt (överordnade uppgifter eller projektet) vid den tidpunkt som anges av uppdateringstypen.  Så här anger du en uppdateringstyp för projektet:

1. Gå till det projekt vars uppdateringstyp du vill ange.
1. Klicka på menyn Mer ![](assets/more-icon.png) bredvid namnet på projektet och klicka sedan på **Redigera** .

1. Klicka på **Projekt** **Inställningar**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. I fältet **Uppdatera typ** väljer du om du vill att Workfront ska beräkna tidslinjen för projektet automatiskt varje dag, när en ändring görs eller om du vill att projektledaren ska beräkna den manuellt.

   Välj bland alternativen i listan nedan. 

   >[!IMPORTANT]
   >
   >Om tidslinjen för ett projekt är längre än 15 år beräknas tidslinjen inte automatiskt eller vid ändring i Workfront. Uppdateringstypen för ett projekt som är längre än 15 år är alltid Manuell.

   * **Automatisk och vid ändring:** Det här är standardinställningen. Projektets tidslinje uppdateras varje gång en ändring inträffar i projektet eller i ett annat projekt som tidslinjen är beroende av. Projektets tidslinje uppdateras också varje kväll. \
     Detta är den rekommenderade inställningen eftersom den ser till att projekttidslinjen alltid är uppdaterad.

     När du uppdaterar en uppgift eller ett projekt och utlöser en omberäkning av tidslinjen, visas alla tillgängliga datum omedelbart så att du kan fortsätta arbeta. I projekt med mer än 100 uppgifter är datum som kräver längre beräkningar nedtonade.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

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

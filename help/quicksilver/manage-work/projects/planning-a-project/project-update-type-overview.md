---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över projektuppdateringstyp
description: Uppdateringstypen för ett projekt anger hur Adobe Workfront beräknar tidslinjen för ett projekt. Ändringar i projektplanen kan utlösa ändringar i tidslinjen för projektet. Projektets tidslinje måste beräknas om automatiskt eller manuellt för att vara säker på att den är uppdaterad med dessa ändringar.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Översikt över uppdateringstyp för projekt

Uppdateringstypen för ett projekt anger hur Adobe Workfront beräknar tidslinjen för ett projekt. Ändringar i projektplanen kan utlösa ändringar i tidslinjen för projektet. Projektets tidslinje måste beräknas om automatiskt eller manuellt för att vara säker på att den är uppdaterad med dessa ändringar.

Mer information om hur du beräknar om projekttidslinjen finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Typer av projektuppdateringar

Det finns fyra uppdateringstyper för ett projekt, beroende på när du vill att Workfront ska beräkna om projekttidslinjen. Välj en uppdateringstyp i listan nedan.

Mer information om hur du uppdaterar projektets uppdateringstyp finns i [Välj typ av projektuppdatering](../../../manage-work/projects/manage-projects/select-project-update-type.md).

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

---
title: Ta bort klassiska layoutmallar
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Layoutmallar från den klassiska Workfront-upplevelsen är inte längre tillgängliga i Workfront-gränssnittet, men kan ändå påverka Workfront-data. Detta kan orsaka inkonsekvenser i fält som påverkas av layoutmallar (som Delas med) i rapporter eller instrumentpaneler.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Bevilja administrativ åtkomst för en layoutmall

Layoutmallar från den klassiska Workfront-upplevelsen är inte längre tillgängliga i Workfront-gränssnittet, men kan ändå påverka Workfront-data. Detta kan orsaka inkonsekvenser i fält som påverkas av layoutmallar (som Delas med) i rapporter eller instrumentpaneler.

Du kan lösa dessa inkonsekvenser genom att ta bort de klassiska layoutmallarna. Eftersom de inte är tillgängliga i Workfront-gränssnittet måste du använda Workfront API för att ta bort dem.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Ta bort klassiska layoutmallar med ett API-anrop

Du kan ange API-anrop i webbläsarens URL-fält och trycka på Retur. API-svaret visas i webbläsaren.

>[!NOTE]
>
>Mallar för global layout och systemlayout kan inte tas bort.

1. Logga in på Workfront.
1. Leta reda på layoutmallen som du vill ta bort med följande API-anrop:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Observera ID:t för layoutmallen som du vill ta bort.
1. Hitta ditt sessions-ID med följande API-anrop:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Dela aldrig ditt sessions-ID med någon.

1. Infoga layoutmallens ID och sessions-ID i följande API-anrop:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Klistra in API-anropet från steg 4 i URL-fältet i webbläsaren och tryck på Retur.

   Då tas layoutmallen bort.

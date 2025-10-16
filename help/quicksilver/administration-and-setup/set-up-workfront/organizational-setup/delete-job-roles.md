---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Ta bort jobbroller
description: Du kan ta bort jobbroller som din organisation inte längre använder. Vi rekommenderar att du inte tar bort jobbroller om de tidigare har kopplats till arbetsobjekt. Om du vill behålla all historik om arbetstilldelningar rekommenderar vi att du inaktiverar roller i stället för att ta bort dem när de blir föråldrade. Mer information om hur du inaktiverar roller finns i Inaktivera jobbroller.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Ta bort jobbroller

Du kan ta bort jobbroller som din organisation inte längre använder. Vi rekommenderar att du inte tar bort jobbroller om de tidigare har kopplats till arbetsobjekt.

Om du vill behålla all historik om arbetstilldelningar rekommenderar vi att du inaktiverar roller i stället för att ta bort dem när de blir föråldrade. Mer information om hur du inaktiverar roller finns i [Inaktivera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Åtkomstkrav

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Administrativ åtkomst till jobbroller</td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort en jobbroll

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Job Roles].**
1. Markera den jobbroll som du vill ta bort och klicka sedan på **[!UICONTROL Delete].**
1. Om det finns några objekt (användare, uppgifter, utgåvor) som tilldelats jobbrollen gör du något av följande:

   * **Ersätt jobbrollen med en annan jobbroll:** Välj den nya jobbrollen i listrutan.

     Alla aktuella och tidigare resursallokeringar som är associerade med den borttagna jobbrollen överförs till den jobbroll som du väljer.

     Användare som bara har en tilldelad jobbroll tilldelas om till den jobbroll som du väljer. Användare som har en sekundär jobbroll tilldelad till dem tilldelas inte den jobbroll som du väljer.

   * **Ta bort jobbrollen och dess resursallokering:** Välj **[!UICONTROL None]** i listrutan.

     >[!IMPORTANT]
     >
     >Om du tar bort en jobbroll tas alla aktuella och tidigare resursallokeringar som hör till den jobbrollen bort för alla projekt.

     &#x200B; till exempel om en uppgift eller utleverans endast har tilldelats den jobbrollen, kommer uppgiften eller utleveransen att tas bort efter att jobbrollen har tagits bort.

1. Klicka på **[!UICONTROL Yes, Delete It]**.

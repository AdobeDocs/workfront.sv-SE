---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Ta bort jobbroller
description: Du kan ta bort jobbroller som din organisation inte längre använder. Vi rekommenderar att du inte tar bort jobbroller om de tidigare har kopplats till arbetsobjekt. Om du vill behålla all historik om arbetstilldelningar rekommenderar vi att du inaktiverar roller i stället för att ta bort dem när de blir föråldrade. Mer information om hur du inaktiverar roller finns i Inaktivera jobbroller.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Ta bort jobbroller

Du kan ta bort jobbroller som din organisation inte längre använder. Vi rekommenderar att du inte tar bort jobbroller om de tidigare har kopplats till arbetsobjekt.

Om du vill behålla all historik om arbetstilldelningar rekommenderar vi att du inaktiverar roller i stället för att ta bort dem när de blir föråldrade. Mer information om hur du inaktiverar roller finns i [Inaktivera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till jobbroller</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Ta bort en jobbroll

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Job Roles].**
1. Markera den jobbroll som du vill ta bort och klicka sedan på **[!UICONTROL Delete].**
1. Om det finns några objekt (användare, uppgifter, utgåvor) som tilldelats jobbrollen gör du något av följande:

   * **Ersätt jobbrollen med en annan jobbroll:** Välj den nya jobbrollen i listrutan.

      Alla aktuella och tidigare resursallokeringar som är associerade med den borttagna jobbrollen överförs till den jobbroll som du väljer.

      Användare som bara har en tilldelad jobbroll tilldelas den nya jobbrollen som du väljer; användare som har tilldelats en sekundär jobbroll tilldelas inte om till den jobbroll som du väljer.

   * **Ta bort jobbrollen och dess resursallokering:** Välj **[!UICONTROL None]** i listrutan.

      >[!IMPORTANT]
      >
      >Om du tar bort en jobbroll tas alla aktuella och tidigare resursallokeringar som hör till den jobbrollen bort för alla projekt.

      &#x200B; till exempel om en uppgift eller utleverans endast har tilldelats den jobbrollen, kommer uppgiften eller utleveransen att tas bort efter att jobbrollen har tagits bort.

1. Klicka på  **[!UICONTROL Yes, Delete It]**.

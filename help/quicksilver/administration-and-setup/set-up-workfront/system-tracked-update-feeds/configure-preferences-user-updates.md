---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Konfigurera inställningar för användaruppdateringar
description: Du kan konfigurera inställningar som ger åtkomst till vissa funktioner när användare lägger till kommentarer i ett objekts [!UICONTROL Updates]-område.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 1%

---

# Konfigurera inställningar för användaruppdateringar

<!--Audited: 08/2025-->

Du kan konfigurera inställningar som ger användarna åtkomst till vissa funktioner när de lägger till kommentarer i ett objekts [!UICONTROL Updates]-område.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Systemadministratör, om du vill utföra de här stegen på systemnivå. </p>
   <p>Om du vill utföra de här stegen för en grupp ska du planera, förutom att vara grupphanteraren.</p></td>
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## Tillåt användare att lägga till bilder i uppdateringar

Som standard kan användare inte lägga till bilder i uppdateringar. När du aktiverar den här inställningen kan användare bifoga bilder i uppdateringar. Inställningen gäller för alla uppdateringar i alla områden i [!DNL Workfront]-instansen.

>[!NOTE]
>
>* Bilder som sparas i uppdateringar räknas in i dokumentets lagringsgräns. Mer information finns i [Kontrollera lagringsgränser för dokument](../../../documents/managing-documents/check-document-storage.md).
>* Bilder är tillgängliga via fliken [!UICONTROL Updates] för ett objekt och är även tillgängliga i området [!UICONTROL Documents] under [!UICONTROL Main Menu].
>

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny ](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på ikonen **[!UICONTROL Setup]** ![Nätform ](assets/gear-icon-settings.png) .
1. Välj **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]** i den vänstra panelen.
1. Klicka på fliken **[!UICONTROL Preferences]**.  

   ![Användarinställningar för uppdateringsfeeds](assets/updatefeeds-preferences-350x137.png)

1. Markera kryssrutan **[!UICONTROL Allow users to add images in updates]**.
1. Välj **[!UICONTROL Save]**.

   När den här inställningen är aktiverad kan du inaktivera den när som helst. Bilder som redan har publicerats i uppdateringar finns kvar i [!UICONTROL Updates]-området på objektet.

---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Konfigurera inställningar för användaruppdateringar
description: Du kan konfigurera inställningar som ger åtkomst till vissa funktioner när användare lägger till kommentarer i ett objekts [!UICONTROL Updates] område.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Konfigurera inställningar för användaruppdateringar

Du kan konfigurera inställningar som ger användarna åtkomst till vissa funktioner när de lägger till kommentarer i ett objekts [!UICONTROL Updates] område.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Om du vill utföra de här stegen på systemnivå måste du ha [!UICONTROL System Administrator] åtkomstnivå.</p><p>Om du vill utföra dem för en grupp måste du vara gruppchef.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tillåt användare att lägga till bilder i uppdateringar

Som standard kan användare inte lägga till bilder i uppdateringar. När du aktiverar den här inställningen kan användare bifoga bilder i uppdateringar. Inställningen gäller för alla uppdateringar i alla områden av [!DNL Workfront] -instans.

>[!NOTE]
>
>* Bilder som sparas i uppdateringar räknas in i dokumentets lagringsgräns. Mer information finns i [Kontrollera dokumentlagringsgränser](../../../documents/managing-documents/check-document-storage.md).
>* Bilderna är bara tillgängliga via [!UICONTROL Updates] -fliken på ett objekt och är inte tillgänglig på [!UICONTROL Documents] -fliken.
>




1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Välj **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.
1. Välj **[!UICONTROL Preferences]** -fliken.

   ![Användarinställningar för uppdateringsflöden](assets/updatefeeds-preferences-350x137.png)

1. Välj **[!UICONTROL Allow users to add images in updates]** kryssruta.
1. Välj **[!UICONTROL Save]**.

   När den här inställningen är aktiverad kan du inaktivera den när som helst. Bilder som redan publicerats i uppdateringar finns kvar i [!UICONTROL Updates] på objektet.

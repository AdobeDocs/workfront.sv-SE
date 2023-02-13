---
title: Ställ in metadatamappning
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metadata är beskrivande information som är kopplad till ett dokument. Du kan konfigurera [!DNL Adobe Workfront] för att inkludera metadata i dokument som skickas till [!DNL Workfront] program.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Ställ in metadatamappning

Metadata är beskrivande information som är kopplad till ett dokument. Du kan konfigurera [!DNL Adobe Workfront] för att inkludera metadata i dokument som skickas till [!DNL Workfront] program.

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
   <td> <p>Du måste vara en [!DNL Workfront] administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Om [!DNL Workfront] metadata

Metadata för dokument i [!DNL Workfront] kan innehålla information som projektnamn, aktivitetsbeskrivning eller planerat slutförandedatum. Som [!DNL Workfront] administratör, du kan konfigurera [!DNL Workfront] för att inkludera metadata i dokument som skickas från [!DNL Workfront] till följande [!DNL Workfront] program:

* [!DNL Workfront DAM]

Innan metadata kan skickas med dokument måste du först ange, eller mappa, de metadata som du vill inkludera. Du kan mappa fält som används i [!DNL Workfront]. När du har konfigurerat metadatamappning överförs alla dokument till en [!DNL Workfront] kommer att innehålla mappade metadata.

När en användare skickar ett dokument från [!DNL Workfront] till [!DNL Workfront] program överförs mappade metadata längs dokumentet. Medan versionen av dokumentet i [!DNL Workfront] programmet är länkat till [!DNL Workfront], ändringar av dokumentets metadata i [!DNL Workfront] återspeglas inte i dokumentets metadata i [!DNL Workfront] program. Om ett mappat fält i [!DNL Workfront] ändras måste du skicka en ny version av dokumentet med de uppdaterade metadata till [!DNL Workfront] program.

>[!NOTE]
>
>Du kan bara mappa metadata i en riktning: från [!DNL Workfront] till [!DNL Workfront DAM]. Metadata för dokument som är länkade till [!DNL Workfront] från [!DNL Workfront DAM] kan inte överföras till Workfront.

Du kan mappa samma [!DNL Workfront] fält till olika metadatafält i [!DNL Workfront DAM]men du kan inte använda ett metadatafält i något av dessa program för flera [!DNL Workfront] metadatafält.

Konfigurera flera [!DNL Workfront] fält som ska exporteras till ett metadatafält i ett [!DNL Workfront] program, skapa först ett beräknat anpassat fält i [!DNL Workfront] om du vill visa alla enskilda anpassade fält för ett objekt. Mappa sedan den beräknade [!DNL Workfront] till ett metadatafält i [!DNL Workfront] program. Mer information om beräknade anpassade fält finns i [Lägga till beräknade data i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Innan du kan mappa fält för metadatamappningsprocessen måste du aktivera programmet i [!DNL Workfront]. Mer information finns i [Konfigurera dokumentintegreringar](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Konfigurera [!DNL Workfront] för att skicka metadata

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

   ![](assets/metadata-mapping.png)

1. I **[!UICONTROL Select Source Field for Mapping]** börjar du skriva namnet på det Workfront-fält som du vill mappa till [!DNL Workfront DAM]markerar du den när du ser den i listan.
1. I **[!UICONTROL Select Target Field for Mapping]** markerar du det fält som du vill fylla i med informationen i det markerade [!DNL Workfront] fält.

1. Klicka på **[!UICONTROL Add Mapping]**.

   Det mappade fältet visas i mappade fält längst ned på sidan.

1. Upprepa steg 5 och 6 tills du lägger till alla önskade [!DNL Workfront] fält och deras motsvarande [!DNL Workfront DAM] fält.

## Ta bort mappade fält

1. Logga in på [!DNL Workfront] som administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. I listan med mappade fält markerar du de fält som du vill ta bort från metadatamappningen.
1. Klicka på **[!UICONTROL Delete]**.

   De angivna fälten är inte längre mappade. Nu när en användare skickar ett dokument från [!DNL Workfront] till [!DNL Workfront DAM], överförs inte metadata i de borttagna fälten tillsammans med dokumentet.

   Ett dokument som skickas innan du tar bort de mappade fälten behåller de ursprungliga metadata som skickats med dem, inklusive metadata för de borttagna fälten.

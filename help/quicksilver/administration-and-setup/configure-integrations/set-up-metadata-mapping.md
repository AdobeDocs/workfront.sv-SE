---
title: Konfigurera metadatamappning
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metadata är beskrivande information som är kopplad till ett dokument. Du kan konfigurera  [!DNL Adobe Workfront] så att metadata inkluderas med dokument som skickas till [!DNL Workfront] program.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Ställ in metadatamappning

Metadata är beskrivande information som är kopplad till ett dokument. Du kan konfigurera [!DNL Adobe Workfront] så att den inkluderar metadata med dokument som skickas till [!DNL Workfront]-program.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Om [!DNL Workfront] metadata

Metadata för dokument i [!DNL Workfront] kan innehålla information som det relaterade projektnamnet, aktivitetsbeskrivningen eller det planerade slutförandedatumet. Som [!DNL Workfront]-administratör kan du konfigurera [!DNL Workfront] så att metadata inkluderas med dokument som skickas från [!DNL Workfront] till följande [!DNL Workfront]-program:

* [!DNL Workfront DAM]

Innan metadata kan skickas med dokument måste du först ange, eller mappa, de metadata som du vill inkludera. Du kan mappa alla fält som används i [!DNL Workfront]. När du har konfigurerat metadatamappning kommer alla dokument som överförs till ett [!DNL Workfront]-program att innehålla mappade metadata.

När en användare skickar ett dokument från [!DNL Workfront] till ett [!DNL Workfront]-program överförs mappade metadata längs dokumentet. När versionen av dokumentet i programmet [!DNL Workfront] är länkad till [!DNL Workfront] återspeglas inte ändringar som gjorts i dokumentets metadata i [!DNL Workfront] i dokumentets metadata i programmet [!DNL Workfront]. Om ett mappat fält i [!DNL Workfront] ändras måste du skicka en ny version av dokumentet med de uppdaterade metadata till programmet [!DNL Workfront].

>[!NOTE]
>
>Du kan bara mappa metadata i en riktning: från [!DNL Workfront] till [!DNL Workfront DAM]. Det går inte att överföra metadata för dokument som är länkade till [!DNL Workfront] från [!DNL Workfront DAM] till Workfront.

Du kan mappa samma [!DNL Workfront]-fält till olika metadatafält i [!DNL Workfront DAM], men du kan inte använda ett metadatafält i något av dessa program för flera [!DNL Workfront] metadatafält.

Om du vill konfigurera flera [!DNL Workfront]-fält att exportera till ett metadatafält i ett [!DNL Workfront] -program skapar du först ett beräknat anpassat fält i [!DNL Workfront] så att alla enskilda anpassade fält för ett objekt visas. Mappa sedan det beräknade fältet [!DNL Workfront] till ett metadatafält i programmet [!DNL Workfront]. Mer information om beräknade anpassade fält finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Innan du kan mappa fält för metadatamappningsprocessen måste du aktivera programmet i [!DNL Workfront]. Mer information finns i [Konfigurera dokumentintegreringar](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Konfigurera [!DNL Workfront] för att skicka metadata

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]** i den vänstra panelen.

   ![Metadatamappning](assets/metadata-mapping.png)

1. I rutan **[!UICONTROL Select Source Field for Mapping]** börjar du skriva namnet på det Workfront-fält som du vill mappa till [!DNL Workfront DAM] och markerar det sedan när du ser det i listan.
1. I rutan **[!UICONTROL Select Target Field for Mapping]** markerar du det fält som du vill fylla i med informationen i det markerade [!DNL Workfront]-fältet.

1. Klicka på **[!UICONTROL Add Mapping]**.

   Det mappade fältet visas i mappade fält längst ned på sidan.

1. Upprepa steg 5 och 6 tills du lägger till alla önskade [!DNL Workfront]-fält och deras motsvarande [!DNL Workfront DAM]-fält.

## Ta bort mappade fält

1. Logga in på [!DNL Workfront] som administratör.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]** i den vänstra panelen.

1. I listan med mappade fält markerar du de fält som du vill ta bort från metadatamappningen.
1. Klicka på **[!UICONTROL Delete]**.

   De angivna fälten är inte längre mappade. När en användare skickar ett dokument från [!DNL Workfront] till [!DNL Workfront DAM] överförs inte metadata som finns i de borttagna fälten med dokumentet.

   Ett dokument som skickas innan du tar bort de mappade fälten behåller de ursprungliga metadata som skickats med dem, inklusive metadata för de borttagna fälten.

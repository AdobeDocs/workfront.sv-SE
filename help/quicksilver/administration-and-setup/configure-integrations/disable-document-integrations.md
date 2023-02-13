---
title: Inaktivera dokumentintegreringar
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Som [!DNL anAdobe] [!DNL Workfront] kan du inaktivera anslutningen mellan Workfront och någon tredjepartsleverantör av dokument.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

# Inaktivera dokumentintegreringar

Som en [!DNL Adobe] [!DNL Workfront] kan du inaktivera anslutningen mellan [!DNL Workfront] och någon av dokumentleverantörerna från tredje part.

När du inaktiverar anslutningen mellan [!DNL Workfront] och en dokumentleverantör försvinner länkarna till dokumenten [!DNL Workfront]. Användarna kan inte längre se de länkade dokumenten, de kan inte göra några ändringar i dokumenten via [!DNL Workfront] länkar och de kan inte lägga till fler dokument till den providern.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Inaktivera integreringar med molnleverantörer

Så här inaktiverar du dokumentintegreringar för [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Logga in på [!DNL Workfront] som [!DNL Workfront] administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]**.

1. Avmarkera någon av de molnleverantörer som du vill koppla från [!DNL Workfront].
1. Klicka på **[!UICONTROL Save]**.

   Användarna kan inte ansluta till den specifika molnleverantör du inaktiverade, och de kan inte längre länka dokument från den molnleverantören till Workfront.

## Inaktivera [!DNL SharePoint] integration

1. Logga in på [!DNL Workfront] som [!DNL Workfront] administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Expandera **[!UICONTROL Documents]** och sedan klicka **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Välj [!DNL SharePoint] integrering som du vill inaktivera.
1. Klicka på **[!UICONTROL Disable]**.\
   Användarna kan inte ansluta till [!DNL SharePoint] webbplatsen du inaktiverade och de kan inte längre länka dokument från [!DNL SharePoint] till [!DNL Workfront].

## Inaktivera anpassade integreringar

1. Logga in på [!DNL Workfront] som administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]**.
1. Välj den anpassade integrering som du vill inaktivera.
1. Klicka på **[!UICONTROL Disable]**.

   Användarna kan inte ansluta till den tredjepartsleverantör av dokument som du har inaktiverat, och de kan inte längre länka dokument från den molnleverantören till [!DNL Workfront].

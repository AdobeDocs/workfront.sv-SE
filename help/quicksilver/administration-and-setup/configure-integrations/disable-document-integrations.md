---
title: Inaktivera dokumentintegreringar
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Som  [!DNL anAdobe] [!DNL Workfront]-administratör kan du inaktivera anslutningen mellan Workfront och någon av dokumentleverantörerna från tredje part.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Inaktivera dokumentintegreringar

Som [!DNL Adobe] [!DNL Workfront]-administratör kan du inaktivera anslutningen mellan [!DNL Workfront] och någon av dokumentleverantörerna från tredje part.

När du inaktiverar anslutningen mellan [!DNL Workfront] och en dokumentleverantör försvinner länkarna till dokumenten från [!DNL Workfront]. Användare kan inte längre se de länkade dokumenten, de kan inte göra några ändringar i dokumenten via länkarna [!DNL Workfront] och de kan inte lägga till fler dokument till den providern.

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
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information om [!DNL Workfront] administratörer finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Inaktivera integreringar med molnleverantörer

Så här inaktiverar du dokumentintegreringar för [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Logga in på [!DNL Workfront] som [!DNL Workfront]-administratör.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]**.

1. Avmarkera någon av de molnleverantörer som du vill koppla från [!DNL Workfront].
1. Klicka på **[!UICONTROL Save]**.

   Användarna kan inte ansluta till den specifika molnleverantör du inaktiverade, och de kan inte längre länka dokument från den molnleverantören till Workfront.

## Inaktivera integreringen av [!DNL SharePoint]

1. Logga in på [!DNL Workfront] som [!DNL Workfront]-administratör.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Expandera **[!UICONTROL Documents]** och klicka sedan på **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Välj den [!DNL SharePoint]-integrering som du vill inaktivera.
1. Klicka på **[!UICONTROL Disable]**.\
   Användarna kan inte ansluta till den [!DNL SharePoint]-webbplats som du inaktiverade och de kan inte längre länka dokument från [!DNL SharePoint] till [!DNL Workfront].

## Inaktivera anpassade integreringar

1. Logga in på [!DNL Workfront] som administratör.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]**.
1. Välj den anpassade integrering som du vill inaktivera.
1. Klicka på **[!UICONTROL Disable]**.

   Användarna kan inte ansluta till den tredjepartsleverantör av dokument som du inaktiverade, och de kan inte längre länka dokument från den molnprovidern till [!DNL Workfront].

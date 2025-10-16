---
title: Inaktivera dokumentintegrering
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Som  [!DNL anAdobe] [!DNL Workfront]-administratör kan du inaktivera anslutningen mellan Workfront och någon av dokumentleverantörerna från tredje part.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 1%

---

# Inaktivera dokumentintegreringar

Som [!DNL Adobe] [!DNL Workfront]-administratör kan du inaktivera anslutningen mellan [!DNL Workfront] och någon av dokumentleverantörerna från tredje part.

När du inaktiverar anslutningen mellan [!DNL Workfront] och en dokumentleverantör försvinner länkarna till dokumenten från [!DNL Workfront]. Användare kan inte längre se de länkade dokumenten, de kan inte göra några ändringar i dokumenten via länkarna [!DNL Workfront] och de kan inte lägga till fler dokument till den providern.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table>
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Prime eller Ultimate</p>
    <p>Arbetsflöde Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-licenser
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Inaktivera integreringar med molnleverantörer

Så här inaktiverar du dokumentintegreringar för [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Logga in på [!DNL Workfront] som [!DNL Workfront]-administratör.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]**.

1. Avmarkera någon av de molnleverantörer som du vill koppla från [!DNL Workfront].
1. Klicka på **[!UICONTROL Save]**.

   Användarna kan inte ansluta till den specifika molnleverantör du inaktiverade, och de kan inte längre länka dokument från den molnleverantören till Workfront.

## Inaktivera integreringen av [!DNL SharePoint]

1. Logga in på [!DNL Workfront] som [!DNL Workfront]-administratör.

{{step-1-to-setup}}

1. Expandera **[!UICONTROL Documents]** och klicka sedan på **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Välj den [!DNL SharePoint]-integrering som du vill inaktivera.
1. Klicka på **[!UICONTROL Disable]**.\
   Användarna kan inte ansluta till den [!DNL SharePoint]-webbplats som du inaktiverade och de kan inte längre länka dokument från [!DNL SharePoint] till [!DNL Workfront].

## Inaktivera anpassade integreringar

1. Logga in på [!DNL Workfront] som administratör.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]**.
1. Välj den anpassade integrering som du vill inaktivera.
1. Klicka på **[!UICONTROL Disable]**.

   Användarna kan inte ansluta till den tredjepartsleverantör av dokument som du inaktiverade, och de kan inte längre länka dokument från den molnprovidern till [!DNL Workfront].

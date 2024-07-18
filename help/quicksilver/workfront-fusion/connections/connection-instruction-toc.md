---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: connections-annd-webhooks
title: Skapa anslutningar i  [!DNL Adobe Workfront Fusion]
description: En anslutning måste uppfylla de krav som anges i API:t för det program eller den webbtjänst den ansluter till. Instruktionerna för hur du konfigurerar en anslutning varierar därför beroende på programmet eller webbtjänsten. Den här artikeln kan hjälpa dig att identifiera och hitta instruktionerna för att ansluta [!DNL Adobe Workfront Fusion] till den app eller webbtjänst du valt.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Skapa anslutningar i [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

En anslutning måste uppfylla de krav som anges i API:t för det program eller den webbtjänst den ansluter till. Instruktionerna för hur du konfigurerar en anslutning varierar därför beroende på programmet eller webbtjänsten. Den här artikeln kan hjälpa dig att identifiera och hitta instruktionerna för att ansluta [!DNL Adobe Workfront Fusion] till den app eller webbtjänst du valt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Alla</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licens</td>  
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Work] eller högre</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td>  
   <td> 
   <p>Aktuell: Inga [!DNL Workfront Fusion]-licenskrav.</p> 
   <p>eller</p> 
   <p>Äldre: Alla </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Planen [!DNL Workfront Fusion] ingår.</li></ul> 
   <p>eller</p> 
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Anslut till ett program eller en webbtjänst som inte kräver konfiguration

I de flesta fall kan du använda modulen för att skapa en anslutning med liten eller ingen extra information. [!DNL Workfront Fusion] hanterar autentiseringen automatiskt.

Instruktioner om hur du skapar en anslutning utan att göra några speciella justeringar finns i [Skapa en anslutning till  [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Anslut till ett [!DNL Microsoft]-program eller en webbtjänst

I de flesta av [!DNL Microsoft]-apparna i [!DNL Workfront Fusion] kan du skapa en anslutning utan extra information.

Följande omständigheter kräver extra steg när du skapar en anslutning:

* Använder [!DNL Microsoft Dynamics 365] moduler.

  Instruktioner finns i [[!DNL Microsoft Dynamics 365] moduler](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Ansluta till [!DNL Microsoft Graph API] med en [!UICONTROL HTTP]-modul

  Instruktioner finns i [Anropa  [!DNL MS Graph REST API] via  [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md) .

## Anslut till ett [!DNL Google]-program eller en webbtjänst

Hur du ansluter till [!DNL Google]-appar kan variera beroende på vilken typ av [!DNL Google]-konto du använder. Dessutom kan [!DNL Google]-säkerhetsåtgärder kräva extra konfiguration när du ansluter till [!DNL Workfront Fusion].

Mer information finns i:

* [Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med uppdaterade säkerhetsåtgärder](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Andra program som kräver ytterligare konfiguration

Följande program följer inte den grundläggande konfigurationen för [!DNL Workfront Fusion] anslutningar. Du hittar instruktioner om hur du ansluter de här apparna i artikeln för den appen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>App-/webbtjänst</th> 
   <th>Ytterligare information om anslutningar</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Anslut [!DNL Adobe Workfront] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Anslut [!DNL Anaplan] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] moduler </a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] moduler</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Anslut [!DNL CloudConvert] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] moduler </a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Anslut [!DNL Datadog] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>E-post</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Anslut din e-post till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email] moduler</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Anslut [!DNL Gmail] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Anslut [!DNL Jira Cloud] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Anslut [!DNL Jira Server] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Anslut [!DNL MariaDB] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Anslut [!DNL Marketo] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Anslut [!DNL Microsoft Dynamics 365] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Ansluter [!DNL Qualtrics] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Anslut [!DNL ServiceNow] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Anslut SFTP till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP] moduler</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Anslut [!DNL SharePoint] till [!DNL Workfront Fusion]</a> i <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] moduler </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Anslut [!DNL Split.io] till [!DNL Workfront Fusion] </a> i <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] moduler</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Widen</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] moduler</a></td> 
  </tr> 
 </tbody> 
</table>

---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filterknappar visas inte i sidhuvuden
description: Läs den här artikeln om du vill felsöka filterknappar som inte visas i sidhuvuden.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---

# Filterknappar visas inte i sidhuvuden

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

## Problem

Följande filterknappar visas inte i sina respektive områden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Filterknappar</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects I'm On]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Lösning

Filterknapparna i området [!UICONTROL Projects and Timesheets] visas inte eftersom motsvarande filter inte ingår i den layoutmall som används för användaren. Administratören [!DNL Workfront] måste tilldela en layoutmall som innehåller filtren.

>[!NOTE]
>
>Ibland tas filtren bort från området [!UICONTROL List Controls] i [!UICONTROL Setup]. Administratören [!DNL Workfront] måste inkludera dem i listorna i det här området för att de ska vara tillgängliga i layoutmallarna.

1. Kontrollera att layoutmallen innehåller följande filter:

   * [!UICONTROL Projects I'm On] och [!UICONTROL Projects I Own] i området [!UICONTROL Projects]
   * [!UICONTROL My Timesheet Approvals] och [!UICONTROL My Timesheets] i området [!UICONTROL Timesheet]

   Så här gör du:

   1. Öppna layoutmallen.
   1. Välj **[!UICONTROL Lists]** under **[!UICONTROL Customize what users see]**.
   1. Välj **[!UICONTROL Projects]** eller **[!UICONTROL Timesheets]** under **[!UICONTROL Select a list to customize]**.
   1. I avsnittet **[!UICONTROL Filter]** kontrollerar du att **[!UICONTROL Projects I'm On]**, **[!UICONTROL Projects I Own]** (för projekt) och **[!UICONTROL My Timesheet Approvals]** och **[!UICONTROL My Timesheets]** (för tidrapporter) är markerade.
   1. Klicka på **[!UICONTROL Save]**.

   Mer information finns i [Anpassa filter, vyer och grupperingar med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Tilldela layoutmallen till rätt användare, jobbroller, team eller grupper. Mer information finns i [Tilldela användare till en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

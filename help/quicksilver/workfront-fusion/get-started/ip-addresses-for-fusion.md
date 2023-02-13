---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP-adresser för åtkomst till Adobe Workfront Fusion
description: Adobe Workfront Fusion kräver en Adobe Workfront Fusion-licens förutom en Adobe Workfront-licens.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# IP-adresser för åtkomst [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver [!DNL Adobe Workfront Fusion] utöver en [!DNL Adobe Workfront license].

Om brandväggen eller e-postservern är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista för att tillåta öppen kommunikation mellan din miljö och [!DNL Adobe Workfront Fusion].

Lägg till följande IP-adresser i tillåtelselista för att aktivera [!DNL Workfront Fusion] för att komma åt ditt system.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Om din organisation använder utgående nätverksfiltrering lägger du till följande domän i tillåtelselista för att ge ditt system tillgång till Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Utgående nätverksfiltrering är ovanlig. Fråga nätverksadministratören om du behöver uppdatera tillåtelselista för att få plats.

Mer information om hur du ställer in tillåtelselista i din organisation finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

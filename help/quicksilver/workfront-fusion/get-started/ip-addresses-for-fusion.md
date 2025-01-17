---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP-adresser för åtkomst till Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# IP-adresser för åtkomst till [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Konfigurera IP-adresser för Fusion i din organisations tillåtelselista](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-up-ip-addresses-for-fusion.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver en [!DNL Adobe Workfront Fusion]-licens utöver en [!DNL Adobe Workfront license].

Om brandväggen eller e-postservern är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista för att tillåta öppen kommunikation mellan din miljö och [!DNL Adobe Workfront Fusion].

Du kan lägga till alla Fusion-IP-adresser och domäner på tillåtelselista, eller så kan du hitta ditt Fusion-kluster och bara lägga till IP-adresser och domäner för det klustret.

## Lägg till alla Fusion-IP-adresser och domäner

Lägg till följande IP-adresser i tillåtelselista:

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

Om din organisation använder utgående nätverksfiltrering lägger du till följande domän i tillåtelselista för att ge ditt system tillgång till Workfront Fusion. De här används för webbhooks.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Lägg endast till Fusion-IP-adresser och domäner för ditt kluster

### Identifiera ditt datacenter

IP-adresserna varierar beroende på var data lagras.

Om du kommer åt Fusion via en URL kan du leta rätt på ditt datacenter genom att undersöka URL:en.

| URL | Datacenter |
| --- | --- |
| `https://app.workfrontfusion.com/` | Amerikanskt datacenter |
| `https://app-eu.workfrontfusion.com/` | EU datacenter |
| `https://app-az.workfrontfusion.com/` | Azure datacenter |

Om du öppnar Fusion via experience.adobe.com kan du kontrollera nätverksfliken i webbläsaren för att identifiera datacentret.

| URL | Datacenter |
| --- | --- |
| Anrop till `https://fusion.adobe.com` | Amerikanskt datacenter |
| Anrop till `https://eu.fusion.adobe.com` | EU datacenter |
| Anrop till `https://az.fusion.adobe.com` | Azure datacenter |

### Lägg till IP-adresser och domäner för ditt datacenter

Lägg till följande IP-adresser i tillåtelselista för att [!DNL Workfront Fusion] ska kunna komma åt ditt system.

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
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Amerikanskt datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li>
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] på Microsoft Azure-klustret</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
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
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Amerikanskt datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] på Microsoft Azure-klustret</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Utgående nätverksfiltrering är ovanlig. Fråga nätverksadministratören om du behöver uppdatera tillåtelselista för att få plats.

Mer information om hur du konfigurerar tillåtelselista i din organisation finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

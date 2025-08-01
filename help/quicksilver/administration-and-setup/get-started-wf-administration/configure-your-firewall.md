---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurera brandväggens Tillåtelselista
description: Om brandväggen eller e-postservern är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista. Detta öppnar kommunikationen mellan din miljö och Adobe Workfront-servrarna och gör att dina användare kan skicka meddelanden från Workfront och använda enkel inloggning med Active Directory eller LDAP.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: d890d467dfdade676a5c93f061a5cbeda53556b6
workflow-type: tm+mt
source-wordcount: '1609'
ht-degree: 0%

---

# Konfigurera brandväggens tillåtelselista

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
>
>Mer information om hur du konfigurerar din tillåtelselista om din organisation har anslutit till Adobe Admin Console finns i [Domäner som tillåts för Adobe appar och tjänster](https://helpx.adobe.com/se/enterprise/kb/network-endpoints.html).
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Organisationens sätt att konfigurera tillåtelselista är unikt för varje organisation. Samarbeta med IT-avdelningen för att identifiera organisationens rutiner och implementera dessa tillägg.

Om brandväggen eller e-postservern är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista. Detta öppnar kommunikationen mellan din miljö och Adobe Workfront-servrarna och tillåter följande processer:

* Skicka meddelanden från Workfront-programmet

  >[!NOTE]
  >
  >Detta är inte tillgängligt om din organisations Workfront-instans har aktiverats med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

* Använda dokumentwebhooks när du konfigurerar anpassade dokumentintegreringar
* Använda Workfront Event-prenumerationer

  Mer information finns i [API för händelseprenumeration](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Du måste även öppna vissa portar för att e-postmeddelanden ska kunna krypteras när de levereras.

## Workfront tillåtslista som du kan använda

Om din organisation har Enterprise-planen kan du även konfigurera två Workfront-tillåtelselista:

* **E-post tillåtelselista**: Här kan du styra var användare kan skicka e-postdata som lagras i Workfront. Mer information finns i [Konfigurera e-posttillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP-tillåtelselista**: Begränsar åtkomst till Workfront till 75 IP-adresser eller IP-adressintervall som du anger, vilket ger ytterligare ett säkerhetslager för Workfront-programmet. Mer information finns i [Begränsa åtkomst till Adobe Workfront via IP-adress](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Hitta ditt Workfront-kluster

IP-adresserna som du måste lägga till i tillåtelselista på brandväggen beror på vilket kluster som produktionsmiljön körs i.

Så här hittar du din organisations kluster:

{{step-1-to-setup}}

1. Klicka på **System** i den vänstra navigeringen och välj sedan **Kundinformation**.
1. Leta reda på fältet **Klusterinställning** längst upp till höger på sidan. Organisationens kluster listas här.

   CL01 refererar till Cluster 1, CL02 är Cluster 2 osv.

Mer information finns i avsnittet [Visa din organisations kluster och Workfront-plan](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) i artikeln [Översikt över brandväggen](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## IP-adresser som ska läggas till i tillåtelselista

>[!IMPORTANT]
>
>Vissa Workfront-integreringar fungerar inte när tillåtelselista är aktiverat eftersom de inte kan konfigureras med en statisk IP-adress. Om du vill använda följande integreringar måste du inaktivera tillåtelselista.
>
>* Workfront för Outlook

* [IP-adresser som tillåter kluster 1, 2, 3, 5, 7, 8 och 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [IP-adresser som tillåter kluster 4](#ip-addresses-to-allow-for-cluster-4)
* [IP-adresser som tillåter kluster 6](#ip-addresses-to-allow-for-cluster-6)
* [IP-adresser som tillåter kluster 10](#ip-addresses-to-allow-for-cluster-10)
* [IP-adresser som tillåter en testenhet](#IP%20Addre2)
* [IP-adresser som ska tillåtas vid implementering av händelseprenumerationer](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [IP-adresser att lägga till för åtkomst till Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [IP-adresser att lägga till för att använda Workfront för Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL:er att lägga till för alla kluster med Workfront](#urls-to-add-for-all-clusters-workfront)

### IP-adresser som tillåter Kluster 1, 2, 3, 5, 7, 8 och 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Om produktionsmiljön finns i kluster 1, 2, 3, 5, 7, 8 eller 9 måste du tillåta följande IP-adresser.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">För enkel inloggning, dokumentwebhooks eller andra funktioner</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Så här tar du emot e-post från Workfront-programmet</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>Mer information om följande IP-adresser finns i <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Nya IP-adresser för Adobe Workfront-e-post med version 21.1</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-adresser som tillåter kluster 4 {#ip-addresses-to-allow-for-cluster-4}

Om produktionsmiljön finns i kluster 4 lägger du till följande IP-adresser för enkel inloggning, dokumentwebbhotell och för att få e-post från Workfront-programmet:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230,232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

Mer information om följande IP-adresser finns i [Nya IP-adresser för Adobe Workfront-e-post med version 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23.251.239.98
* 23.251.239.99

### IP-adresser som tillåter kluster 6 {#ip-addresses-to-allow-for-cluster-6}

Om produktionsmiljön finns i kluster 6 lägger du till följande IP-adresser.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Så här tar du emot e-post från Workfront-programmet</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Så här använder du e-posttjänsten</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Så här använder du e-posttjänsten Mailgun</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-adresser som tillåter kluster 10

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

### IP-adresser som tillåter en testenhet

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Så här tar du emot e-post från Workfront-programmet när du använder en testenhet</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">För SSO- och dokumentwebbkrokintegreringar när du använder en testenhet</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Den här adressen måste också läggas till i tillåtelselista för att dina användare ska kunna ta emot e-postmeddelanden från Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-adresser som ska tillåtas vid implementering av händelseprenumerationer  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

För alla miljöer lägger du till följande IP-adresser för att ta emot nyttolaster från Workfront-händelseprenumerationer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> För kunder i Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">För kunder på andra platser än Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-adresser att lägga till för åtkomst till Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Lägg till följande IP-adresser i tillåtelselista för att Workfront Fusion ska kunna komma åt ditt system.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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

Om din organisation använder utgående nätverksfiltrering lägger du till följande domän i tillåtelselista för att ge ditt system tillgång till Workfront Fusion. Dessa URL:er används för webhooks i Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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

### IP-adresser att lägga till för att använda Workfront för Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Lägg till följande IP-adresser i tillåtelselista för att använda Workfront för Jira-integrering.

jira.workfront.com måste också vara åtkomlig från företagets servrar. Den här domänen krävs eftersom den fungerar som mellanvara mellan Workfront och Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> För kunder i Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">För kunder på andra platser än Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domäner att lägga till för åtkomst till Workfront

Om din organisation använder utgående nätverksfiltrering lägger du till följande domäner på tillåtelselista så att ditt system kan komma åt Workfront.

>[!NOTE]
>
>Utgående nätverksfiltrering är ovanlig. Fråga nätverksadministratören om du behöver uppdatera tillåtelselista för att få plats.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* snippet.maze.co
* *.aptrinsic.com
* *.static.workfront.com


  Det här är en statisk domän som expanderar alla följande domäner. Du kan lägga till de enskilda domänerna om du vill:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

Om din organisation använder Adobe Unified Experience används följande domäner. Dessa domäner täcks av `*.adobe.com`, men kan läggas till om så önskas.

* &lt;your domain>.my.workfront.adobe.com
* &lt;your domain>.preview.workfront.adobe.com
* &lt;your domain>.sb01.workfront.adobe.com
* &lt;your domain>.sb02.workfront.adobe.com


För Workfront Fusion lägger du till följande domäner:

* För företag som inte är med i Adobe Unified Experience:
   * app.workfrontfusion.com (US AWS)
   * app-eu.workfrontfusion.com (EU AWS)
   * app-az.workfrontfusion.com (US Azure)

* För företag som använder Adobe Unified Experience
(De här domänerna täcks av `*.adobe.com`, men kan läggas till om så önskas.)

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## URL:er att lägga till för alla kluster med Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Så här kan hjälpinnehåll visas i din Workfront-miljö</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Om du vill att Workfront Proof ska få åtkomst till Workfront i alla kluster lägger du till dessa i alla miljöer</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Krävs för att visa korrektur i Workfront</li> 
     <li>*.proofhq.com - Krävs för att visa korrektur i Workfront Proof</li> 
     <li>*.proofhq.eu - krävs för att visa korrektur i Workfront Proof</li> 
    </ul> <p><b>OBS</b>:  <p>Vi stöder inte tillägg av IP-adresser till din tillåtelselista för Workfront Proof. De har varit dynamiska sedan Workfront flyttat till AWS. Vi rekommenderar att du bara tillåter Workfront Proof-domäner.</p> <p>Om du har problem med att lägga till de här domänerna på tillåtelselista och du behöver en IP-adress i stället kontaktar du Workfront kundsupport.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## IP-adresser och URL:er att lägga till för åtkomst till Workfront Proof

Du måste lägga till följande IP-adresser i tillåtelselista för att kunna använda olika funktioner.

* [För återanrop och korrektur för webbhämtning](#for-callbacks-and-webcapture-proofs)
* [För utgående e-post](#for-outgoing-email)

### För återanrop och webbinspelningskorrektur {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (kluster 1, 2, 3, 5 och 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54 184 151 122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (kluster 4)</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>Obs!</b> DNS-serveralternativ stöds inte längre.</p> </td> 
  </tr> 
 </tbody> 
</table>

### För utgående e-post {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (kluster 1, 2, 3, 5 och 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (kluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Portar att öppna för bästa Workfront Proof-prestanda

Öppna följande portar om du har problem med att läsa in korrektur eller inte fungerar i Workfront Proof:

* 5671
* 5672
* 15671

## Portar att öppna för krypterad e-post

E-postmeddelanden från Workfront-programmet skickas krypterade med portarna 465 och 587. Om e-postservern inte stöder krypterad e-post levereras e-postmeddelanden okrypterade med port 25.

## E-postmeddelanden från Workfront Support

Om du inte får e-post från Workfront Support måste du lägga till de Salesforce IP-adresser och domäner du behöver. Mer information finns i Salesforce hjälpartiklar om Salesforce IP-adresser och domäner som ska tillåtas.

---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Översikt över brandväggen
description: Eftersom Adobe Workfront kommunicerar med din organisations nätverk måste organisationens brandvägg vara konfigurerad för att tillåta sådan kommunikation. Brandväggar är mycket effektiva säkerhetsåtgärder som fungerar genom att en organisations nätverk skiljs från internet. De ser till att endast utvalda data- och nätverkstrafik kan flyttas in i eller ut ur organisationens nätverk. Brandväggen tillåter eller blockerar data baserat på den webbplats som skickar eller tar emot data. Som Adobe Workfront-administratör måste du se till att data som skickas till eller från Workfront kan passera företagets brandvägg.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Översikt över brandväggen

Eftersom Adobe Workfront kommunicerar med din organisations nätverk måste organisationens brandvägg vara konfigurerad för att tillåta sådan kommunikation. Brandväggar är mycket effektiva säkerhetsåtgärder som fungerar genom att en organisations nätverk skiljs från internet. De ser till att endast utvalda data- och nätverkstrafik kan flyttas in i eller ut ur organisationens nätverk. Brandväggen tillåter eller blockerar data baserat på den webbplats som skickar eller tar emot data. Som Adobe Workfront-administratör måste du se till att data som skickas till eller från Workfront kan passera företagets brandvägg.

Detta uppnås genom en tillåtelselista, som i huvudsak är en lista över webbplatser som&quot;tillåts&quot; att skicka eller ta emot data via brandväggen. Platserna kan identifieras på ett av två sätt:

* **IP-adress**: en serie siffror som 52.31.132.175
* **Domän**: del av en URL, t.ex.&quot;den här domänen&quot; i www.thisdomain.com

Workfront använder specifika IP-adresser och domäner för webbkommunikation. Dessa måste läggas till i din organisations tillåtelselista innan du kan använda Workfront i din organisation.

I allmänhet konfigureras en tillåtelselista av en nätverksadministratör. Samarbeta med organisationens nätverksadministratör för att säkerställa att brandväggen tillåter dessa IP-adresser. Om du inte vet vem din nätverksadministratör är kan din organisations IT-avdelning peka dig i rätt riktning.

>[!IMPORTANT]
>
>Som Workfront-administratör måste du se till att dessa IP-adresser och domäner läggs till i din organisations tillåtelselista. Detta gäller även om du inte själv lägger till dem. Workfront kan inte konfigurera din organisations tillåtelselista.

## Samla in information för att konfigurera brandväggen

Om du vill konfigurera brandväggen för Workfront måste nätverksadministratören veta vilka IP-adresser och domäner som ska läggas till. En del av den här informationen är bara tillgänglig för en Workfront-administratör. Som Workfront-administratör måste du leta reda på informationen och skicka den till nätverksadministratören.

>[!NOTE]
>
>Det bästa sättet att skydda är att lägga till enbart IP-adresser och domäner som är anslutna till funktioner som din organisation aktivt använder. Genom att ange den här informationen kan du se till att den bästa metoden följs.

Ge nätverksadministratören följande information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Specifika IP-adresser och domäner som ska tillåtas</td> 
   <td> <p>Artikeln <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Konfigurera brandväggens tillåtelselista</a> innehåller en lista över IP-adresser och domäner som din organisation måste lägga till i tillåtelselista. </p> <p>Nätverksadministratören kanske inte har tillgång till artikeln Konfigurera tillåtelselista i brandväggen. I så fall måste du ge dem det. Vi rekommenderar inte att du skriver ut en papperskopia. Med en digital kopia kan nätverksadministratören kopiera och klistra in adresserna, vilket är snabbare och exaktare än att skriva in från en kopia.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ditt kluster</td> 
   <td>Information om hur du hittar din organisations kluster finns i <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visa din organisations kluster och Workfront-plan</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Din Workfront-plan</td> 
   <td> <p>Information om hur du hittar din organisations plan finns i <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visa din organisations kluster och Workfront-plan.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Din domän</td> 
   <td> <p>Om du vill hitta din domän tittar du på den webbadress som du använder för att ansluta till Workfront.</p> <p>Exempel: i webbadressen <code>greatcompany.my.workfront.com</code> är domänen"storföretag"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andra Adobe Workfront-produkter</td> 
   <td> <p>Informera nätverksadministratören om du har licenser för något av följande:</p> 
    <ul> 
     <li> <p>Adobe Workfront Proof</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-integreringar</td> 
   <td>Informera nätverksadministratören om du använder något av följande:
    <ul>
     <li><p>Workfront för Jira</p></li>
     <li><p>Workfront för Google Workspace</p></li>
     <li><p>Workfront för Microsoft Teams</p></li>
     <li><p>Workfront för Outlook</p></li>
     <li><p>Workfront för Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare funktioner</td> 
   <td> <p>Informera nätverksadministratören om du använder följande:</p> 
    <ul> 
     <li> <p>En Workfront-testenhet</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Om du lägger till någon av dessa produkter, integreringar eller funktioner vid ett senare tillfälle måste du kontakta nätverksadministratören så att de kan justera tillåtelselista.

### Visa din organisations kluster och Workfront-plan {#view-your-organization-s-cluster-and-workfront-plan}

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).

1. Klicka på **System** i den vänstra panelen
1. Välj **Kundinformation** om du vill visa klustret.

   Klustret visas uppe till höger i avsnittet **Grundläggande information**.

   ![](assets/locate-cluster.png)

1. Om du vill visa din Workfront-plan väljer du **licenser**.

   Din plan visas längst ned på sidan.

   ![](assets/locate-plan.png)

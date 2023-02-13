---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurera din e-postadress tillåtelselista
description: Om din organisation använder WorkfrontEnterprise-planen kan du skapa en Workfront-tillåtelselista för att styra vilka e-postdomäner som tillåts ta emot e-post från Workfront och vilka e-postdomäner som kan finnas i den e-postadress som användarna anger i sina användarprofiler. Detta är användbart om organisationens säkerhetspolicy begränsar användare från att skicka data som lagras i Workfront till externa e-postadresser. Du kan bara inkludera dina interna företagsdomäner i tillåtelselista för att se till att den här policyn följs.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Konfigurera din e-postadress tillåtelselista

Om din organisation använder WorkfrontEnterprise-planen kan du skapa en Workfront-tillåtelselista för att styra:

* Vilka e-postdomäner får ta emot e-postmeddelanden från Workfront.
* Vilka e-postdomäner kan finnas i den e-postadress som användarna anger i sina användarprofiler.

Detta är användbart om organisationens säkerhetspolicy begränsar användare från att skicka data som lagras i Workfront till externa e-postadresser. Du kan bara inkludera dina interna företagsdomäner i tillåtelselista för att se till att policyn följs.

>[!IMPORTANT]
>
>IT-teamet bör se till att inkommande e-post från `notifications@my.workfront.com` är inte blockerad i din organisations system.
>
>Alla e-postmeddelanden från Workfront skickas från den adressen för att öka e-postleveransen och för att eliminera förfalskning av e-postmeddelanden. Detta innefattar både automatiska varningar och kommunikation mellan användare.
>
>Från-raden i ett Workfront-e-postmeddelande som du får från en användare som heter Joan Harris skulle till exempel se ut så här:
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Information om hur du konfigurerar brandväggen för din organisation för att öppna kommunikationen mellan din miljö och Adobe Workfront-servrarna finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Andra tillåtelselista

Om din organisation har Enterprise-planen kan du konfigurera en Adobe Workfront IP-tillåtelselista som begränsar åtkomsten till Workfront till 45 IP-adresser eller IP-adressintervall som du anger. Detta ger ytterligare ett säkerhetslager för Workfront. Mer information finns i [Begränsa åtkomst till Adobe Workfront via IP-adress](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Om din brandvägg eller e-postserver är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista. Detta öppnar för kommunikation mellan din miljö och Adobe Workfront-servrarna. Mer information om detta finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurera din e-postadress tillåtelselista

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System** > **Kundinformation**.

1. I **E-post Tillåtelselista** avsnitt, markera **Aktivera Tillåtelselista för domän** och sedan klicka **Lägg till domän**.
1. I rutan som visas skriver du en domän som du vill tillåta, till exempel `ourcompany.com`och sedan klicka **Lägg till domän**.

1. Upprepa föregående steg om du vill lägga till andra domäner som du vill tillåta.
1. När du är klar klickar du på **Spara**.

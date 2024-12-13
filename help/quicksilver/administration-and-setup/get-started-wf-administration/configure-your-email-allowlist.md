---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurera e-postTillåtelselista
description: Om din organisation använder WorkfrontEnterprise-planen kan du skapa en Workfront-tillåtelselista för att styra vilka e-postdomäner som tillåts ta emot e-post från Workfront och vilka e-postdomäner som kan finnas i den e-postadress som användarna anger i sina användarprofiler. Detta är användbart om organisationens säkerhetspolicy begränsar användare från att skicka data som lagras i Workfront till externa e-postadresser. Du kan bara inkludera dina interna företagsdomäner i tillåtelselista för att se till att den här policyn följs.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Konfigurera din e-postadress tillåtelselista

Om din organisation använder Workfront Enterprise-planen kan du skapa en e-posttillåtelselista från Workfront för att styra:

* Vilka e-postdomäner får ta emot e-postmeddelanden från Workfront.
* Vilka e-postdomäner kan finnas i den e-postadress som användarna anger i sina användarprofiler.

Detta är användbart om organisationens säkerhetspolicy begränsar användare från att skicka data som lagras i Workfront till externa e-postadresser. Du kan bara inkludera dina interna företagsdomäner i tillåtelselista för att se till att policyn följs.

>[!IMPORTANT]
>
>IT-teamet bör se till att inkommande e-post från `notifications@my.workfront.com` inte blockeras i din organisations system.
>
>Alla e-postmeddelanden från Workfront skickas från den adressen för att öka e-postleveransen och för att eliminera förfalskning av e-postmeddelanden. Detta innefattar både automatiska varningar och kommunikation mellan användare.
>
>Från-raden i ett Workfront-e-postmeddelande som du får från en användare som heter Joan Harris skulle till exempel se ut så här:
>`Joan Harris <notifications@my.workfront.com>`

Information om hur du konfigurerar brandväggen för din organisation för att öppna kommunikationen mellan din miljö och Adobe Workfront-servrarna finns i [Konfigurera tillåtelselista för din brandvägg](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Du måste vara Workfront-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Andra tillåtelselista

Om din organisation har Enterprise-planen kan du konfigurera en Adobe Workfront IP-tillåtelselista som begränsar åtkomsten till Workfront till 75 IP-adresser eller IP-adressintervall som du anger. Detta ger ytterligare ett säkerhetslager för Workfront-programmet. Mer information finns i [Begränsa åtkomst till Adobe Workfront via IP-adress](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Om din brandvägg eller e-postserver är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista. Detta öppnar för kommunikation mellan din miljö och Adobe Workfront-servrarna. Mer information om detta finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurera din e-postadress tillåtelselista

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation**.
1. I avsnittet **E-post Tillåtelselista** väljer du **Aktivera domän Tillåtelselista** och klickar sedan på **Lägg till domän**.
1. I rutan som visas skriver du in en domän som du vill tillåta, till exempel `ourcompany.com`, och klickar sedan på **Lägg till domän**.
1. Upprepa föregående steg om du vill lägga till andra domäner som du vill tillåta.
1. När du är klar klickar du på **Spara**.

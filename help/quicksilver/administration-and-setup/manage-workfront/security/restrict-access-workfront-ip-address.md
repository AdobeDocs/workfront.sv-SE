---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Begränsa åtkomst till Adobe Workfront via IP-adress
description: Du kan konfigurera en Adobe Workfront IP tillåtelselista som begränsar åtkomsten till Workfront till 75 IP-adresser eller IP-adressintervall som du anger. Detta ger ytterligare ett säkerhetslager för Workfront-programmet.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Begränsa åtkomst till Adobe Workfront via IP-adress

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release. -->

Du kan konfigurera en Adobe Workfront IP tillåtelselista som begränsar åtkomsten till Workfront till 75 IP-adresser eller IP-adressintervall som du anger. Detta ger ytterligare ett säkerhetslager för Workfront-programmet.

Dessa IP-adresser eller IP-adressintervall ska anges av nätverksadministratören.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Andra tillåtelselista

Om brandväggen eller e-postservern är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa IP-adresser i tillåtelselista. Detta öppnar för kommunikation mellan din miljö och Adobe Workfront-servrarna. Mer information om detta finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Om din organisation använder Enterprise-planen kan du konfigurera Workfront e-postadress tillåtelselista för att styra vilka e-postdomäner som tillåts ta emot e-post från Workfront och vilka e-postdomäner som kan finnas i den e-postadress som användarna anger i Workfront-användarprofilen. Mer information finns i [Konfigurera e-posttillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Lägga till IP-adresser i tillåtelselista

När du har lagt till IP-adresser i Workfront tillåtslista kan bara de IP-adresserna användas för åtkomst till Workfront. Användare som försöker få åtkomst till Workfront från en annan IP-adress får ett felmeddelande om att deras IP-adress är blockerad.

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation.**

1. I avsnittet **IP-tillåtelselista** väljer du **Aktivera IP-tillåtelselista.**

   Det här alternativet är inaktiverat som standard.

1. Ange den IP-adress som du använder för att komma åt Workfront-systemet.

   eller

   Ange ett intervall med IP-adresser som innehåller den du använder för att få åtkomst till Workfront-systemet.

   IP-adressen som du använder för att få åtkomst till Workfront måste läggas till i tillåtelselista innan tillåtelselista aktiveras.

1. Klicka på **Lägg till IP-intervall** och ange IP-adressen eller det intervall med IP-adresser som du vill ska kunna komma åt Workfront.
1. (Valfritt) Upprepa föregående steg om du vill lägga till ytterligare IP-adresser eller IP-adressintervall.

   Du kan lägga till upp till 75 adresser eller intervall.

1. Klicka på **Spara.**

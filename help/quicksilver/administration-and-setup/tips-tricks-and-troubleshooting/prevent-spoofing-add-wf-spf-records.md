---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Förhindra att objekt fläckas och lägg till  [!DNL Adobe Workfront] SPF-poster
description: Om användarna inte får  [!DNL Adobe Workfront] e-postmeddelanden måste du lägga till  [!DNL Workfront] SPF-poster i brandväggen. Du måste samarbeta med IT-avdelningen för att lägga till SPF-poster.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Förhindra förfalskning och lägg till [!DNL Adobe Workfront] SPF-poster

## Problem

Om användarna inte får [!DNL Adobe Workfront] e-postmeddelanden måste du lägga till [!DNL Workfront] SPF-poster i brandväggen. Du måste samarbeta med IT-avdelningen för att lägga till SPF-poster.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara en [!DNL Workfront]-administratör. </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösning

Om du redan har lagt till IP-adresserna i tillåtelselista för din produktionsmiljö enligt beskrivningen i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) och användare fortfarande inte får några e-postmeddelanden:

1. Lägg till följande SPF-post i brandväggen:

   *spf.workfront.com*

   Detta lägger automatiskt till alla [!DNL Workfront] IP-adresser i tillåtelselista på brandväggen och tillåter att alla skräppostfilter (som använder SPF-poster) validerar [!DNL Workfront]-servrar som giltiga avsändare för din domän.

   >[!NOTE]
   >
   > En SPF-post är en TXT-post som är en del av en DNS-zonfil. Det går inte att ändra DNS-zonfilen.

1. Du måste ange vilken typ av SPF-post som behöver konfigureras. Det här är de giltiga typerna av SPF-poster:

   * alla (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * finns (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Exempel: &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Om du inte kan lägga till SPF-poster i din brandvägg på grund av en företagspolicy, kontaktar du [!DNL Workfront] supportrepresentant.

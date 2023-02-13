---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Förhindra fläckning och lägg till [!DNL Adobe Workfront] SPF-poster
description: Om användarna inte får [!DNL Adobe Workfront] e-postmeddelanden, du måste lägga till [!DNL Workfront] SPF-poster till brandväggen. Du måste samarbeta med IT-avdelningen för att lägga till SPF-poster.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Förhindra fläckning och lägg till [!DNL Adobe Workfront] SPF-poster

## Problem

Om användarna inte får [!DNL Adobe Workfront] e-postmeddelanden, du måste lägga till [!DNL Workfront] SPF-poster till brandväggen. Du måste samarbeta med IT-avdelningen för att lägga till SPF-poster.

## Åtkomstkrav

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösning

Om du redan har lagt till IP-adresserna i tillåtelselista för produktionsmiljön enligt beskrivningen i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) och användarna får fortfarande inga e-postmeddelanden:

1. Lägg till följande SPF-post i brandväggen:

   *spf.workfront.com*

   Detta lägger automatiskt till alla [!DNL Workfront] IP-adresser till tillåtelselista på brandväggen och tillåter att alla skräppostfilter (som använder SPF-poster) validerar [!DNL Workfront] servrar som giltiga avsändare för din domän.

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

   Exempel: &quot;v=spf1 a mx inkluderar: [spf.workfront.com](http://spf.workfront.com/) -all&quot;

Om du inte kan lägga till SPF-poster i brandväggen på grund av en företagspolicy bör du arbeta med [!DNL Workfront] Supportrepresentant.

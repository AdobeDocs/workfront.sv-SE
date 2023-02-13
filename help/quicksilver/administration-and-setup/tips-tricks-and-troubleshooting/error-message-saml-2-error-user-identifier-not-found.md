---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: SAML 2.0-fel: Användaridentifieraren hittades inte'
description: Du kan inte upprätta en anslutning till ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Felmeddelande: SAML 2.0-fel: Användaridentifieraren hittades inte

## Problem

Du kan inte upprätta en anslutning till ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Om du upprättar en lyckad testanslutning och fortfarande har problem, kan du ha felaktiga attributmappningar eller problem med federations-ID:n. Kontakta kundsupporten med frågor.

## Orsak:

Anspråk på ADFS-servern är felaktiga

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

Kontrollera att det finns ett anspråk för namn-ID på ADFS-servern:

1. I Windows klickar du på **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Dialogrutan ADFS 2.0-hantering visas.

1. Välj **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** i den vänstra rutan.

1. Högerklicka på förlitande part-förtroendet för Adobe Workfront och välj **[!UICONTROL Edit Claim Rules]**.
1. Verifiera att anspråket har en **[!UICONTROL Outgoing Claim Type]** av **[!UICONTROL Name ID]**.

![1.png](assets/1-350x287.png)

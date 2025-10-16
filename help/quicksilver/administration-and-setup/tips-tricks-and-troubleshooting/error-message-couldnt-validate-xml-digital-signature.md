---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: Det gick inte att verifiera den digitala XML-signaturen'
description: Du kan inte upprätta en anslutning till ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 2%

---

# Felmeddelande: Det gick inte att verifiera den digitala XML-signaturen

## Problem

Du kan inte upprätta en anslutning till ADFS.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Om du upprättar en lyckad testanslutning och fortfarande har problem, kan du ha felaktiga attributmappningar eller problem med federations-ID:n. Kontakta kundsupporten med frågor.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Orsak 1: Certifikatet är felaktigt

### Lösning

Hämta signeringscertifikatet manuellt från ADFS-servern:

1. I [!DNL Windows] klickar du på **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Dialogrutan ADFS 2.0-hantering visas.

1. Välj **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** i den vänstra rutan.

1. Högerklicka på **[!UICONTROL Relying Party Trust]** och välj **[!UICONTROL Properties]**.

1. Klicka på fliken **[!UICONTROL Signature]**.
1. Klicka på signeringscertifikatets namn och klicka på **[!UICONTROL View]**.
1. Klicka på Kopiera till **[!UICONTROL File]**.. och välj **[!UICONTROL Next]**.

1. Välj **[!UICONTROL Base-64 encoded x.509 (CER)]** och klicka på **[!UICONTROL Next]**.

1. Ange filnamnet och klicka på **[!UICONTROL Next]**.
1. Klicka på **[!UICONTROL Finish]**.
1. I [!DNL Adobe Workfront] går du till **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** och överför signeringscertifikatet manuellt.

## Orsak 2: Certifikatet har signerats med DSA när [!DNL Workfront] förväntar en RSA-signatur

### Lösning

Återskapa certifikatet och använd RSA-signaturen i stället för DSA.

## Orsak 3: XML-data är felaktiga

### Lösning

Exportera och importera XML-metadata igen från ADFS-hanteringssystemet.

## Orsak 4: Begäran kunde inte utföras på grund av ett fel på SAML-sidan

### Lösning

Kontakta din SAML-leverantör.

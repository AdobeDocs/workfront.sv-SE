---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: SAML 2.0-fel: Primär statuskod'
description: Du kan inte upprätta en anslutning till ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 1%

---

# Felmeddelande: SAML 2.0-fel: Primär statuskod

## Problem

Du kan inte upprätta en anslutning till ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

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

## Orsak 1: Den säkra hash-algoritmen är inställd på SHA-256

### Lösning

1. I Windows klickar du på **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Dialogrutan ADFS 2.0-hantering visas.

1. Välj **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** i den vänstra rutan.

1. Högerklicka på förlitande part-förtroendet som är relaterat till [!DNL Adobe Workfront] och välj sedan **[!UICONTROL Properties]**.
1. Klicka på fliken **[!UICONTROL Advanced]** och välj sedan **[!UICONTROL SHA-1]** i listrutan **[!UICONTROL Secure hash algorithm]**.
   ![SHA-1](assets/1-350x287.png)

## Orsak 2: ADFS-signeringscertifikatet upphör snart att gälla och har ersatts med ett nytt certifikat med överlappande datum

### Lösning

På inställningssidan för enkel inloggning ( [!DNL Workfront]) visas certifikatets förfallodatum. Om certifikatet snart upphör att gälla måste du hämta det nya signeringscertifikatet manuellt från ADFS-servern:

1. I Windows klickar du på **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Dialogrutan ADFS 2.0-hantering visas.

1. Välj **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** i den vänstra rutan.

1. Högerklicka på förlitande part-förtroendet som är relaterat till [!DNL Workfront] och välj **[!UICONTROL Properties]**.
1. Klicka på fliken **[!UICONTROL Signature]**.
1. Klicka på signeringscertifikatets namn och klicka på **[!UICONTROL View]**.
1. Klicka på Kopiera till **[!UICONTROL File]**.. och välj **[!UICONTROL Next]**.

1. Välj **[!UICONTROL Base-64 encoded x.509 (CER)]** och klicka på **[!UICONTROL Next]**.

1. Ange filnamnet och klicka på **[!UICONTROL Next]**.
1. Klicka på **[!UICONTROL Finish]**.
1. I [!DNL Workfront] går du till **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** och överför signeringscertifikatet manuellt.

## Orsak 3: Certifikatåterkallningskontrollen misslyckades

Lösningen för detta beror på vilken version av [!DNL Microsoft] ADFS du använder. Läs dokumentationen för [!DNL Microsoft] om hur du får tillgång till lämpliga kommandon för din version.

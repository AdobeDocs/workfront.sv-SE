---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Felmeddelande: SAML 2.0-fel: Primär statuskod'
description: Du kan inte upprätta en anslutning till ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Felmeddelande: SAML 2.0-fel: Primär statuskod

## Problem

Du kan inte upprätta en anslutning till ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Om du upprättar en lyckad testanslutning och fortfarande har problem, kan du ha felaktiga attributmappningar eller problem med federations-ID:n. Kontakta kundsupporten med frågor.

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

## Orsak 1: Den säkra hash-algoritmen är inställd på SHA-256

### Lösning

1. I Windows klickar du på **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Dialogrutan ADFS 2.0-hantering visas.

1. Välj **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** i den vänstra rutan.

1. Högerklicka på förlitande part-förtroendet för [!DNL Adobe Workfront]väljer **[!UICONTROL Properties]**.
1. Klicka på **[!UICONTROL Advanced]** tabbtangenten och sedan **[!UICONTROL SHA-1]** från **[!UICONTROL Secure hash algorithm]** nedrullningsbar meny.\
   ![](assets/1-350x287.png)

## Orsak 2: ADFS-signeringscertifikatet upphör snart att gälla och har ersatts med ett nytt certifikat med överlappande datum

### Lösning

The [!DNL Workfront] SSO-inställningssidan visar certifikatets förfallodatum. Om certifikatet snart upphör att gälla måste du hämta det nya signeringscertifikatet manuellt från ADFS-servern:

1. I Windows klickar du på **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   Dialogrutan ADFS 2.0-hantering visas.

1. Välj **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** i den vänstra rutan.

1. Högerklicka på förlitande part-förtroendet för [!DNL Workfront]och markera **[!UICONTROL Properties]**.
1. Klicka på **[!UICONTROL Signature]** -fliken.
1. Klicka på signeringscertifikatets namn och klicka på **[!UICONTROL View]**.
1. Klicka på Kopiera till **[!UICONTROL File]**... och välj **[!UICONTROL Next]**.

1. Välj **[!UICONTROL Base-64 encoded x.509 (CER)]** och klicka **[!UICONTROL Next]**.

1. Ange filnamnet och klicka på **[!UICONTROL Next]**.
1. Klicka på **[!UICONTROL Finish]**.
1. I [!DNL Workfront], navigera till **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** och överför signeringscertifikatet manuellt.

## Orsak 3: Certifikatåterkallningskontrollen misslyckades

Lösningen för detta beror på vilken version av [!DNL Microsoft] ADFS som du använder. Konsult [!DNL Microsoft]Dokumentation för att få rätt kommandon för din version.

---
title: 2.2 Integration enhancements
description: 2.2 Integration enhancements
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 2.2 Integration enhancements

Den här sidan beskriver alla integreringsförbättringar som gjorts i version 2.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

den 4 april 2022.

En lista över alla ändringar som är tillgängliga i version 2.2 finns i [2.2 versionsöversikt](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Integrering med Adobe Workfront med Anaplan är nu tillgängligt

Workfront kan nu integreras med ditt Anaplan-konto för att ge dig större flexibilitet och insikt i de ekonomiska aspekterna av dina Workfront-projekt. Genom att länka Workfront-objekt till Anaplan-objekt kan du uppdatera information mellan de båda kontona automatiskt, så att informationen i båda är aktuell och identisk. Du kan också aktivera automatiserade processer i Anaplan baserat på åtgärder i Workfront (eller vice versa).

Du kan till exempel skapa en kampanj i Anaplan och sedan skapa ett Workfront-projekt eller -program som är länkat till kampanjen. Alla kostnader som spåras i Workfront kan sedan överföras tillbaka till Anaplan för att granska kampanjens resultat.

Andra arbetsflöden du kan överväga att använda Workfront till Anaplan-integrering för är bland annat:

* Skapa Anaplan-budgetbegäranden från nya Workfront-projekt
* Skapa Workfront-projekt från nya listobjekt i Anaplan
* Initiera förfrågningar från Anaplan-leverantörer från Workfront-projekt

Mer information finns i [Adobe Workfront med Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront för Experience Manager förbättrade anslutningsfunktioner

Workfront för Experience Manager förbättrade anslutningsprogram innehåller nu följande uppdateringar:

* Nu kan du skapa länkade mappar mellan Adobe Workfront och Adobe Experience Manager Assets as a Cloud Service även om det finns flera projektlänkade mappkonfigurationer.
* Stöd för sidnumrering av händelseabonnemang har lagts till
* Stöd för AEM 6.4.x har lagts till
* Stöd för proxymiljöer har lagts till
* Flera felkorrigeringar baseras på feedback från partner och kunder

Mer information finns i [Översikt över den förbättrade anslutningen för Workfront för Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Driftsättning och konfiguration av den här kopplingen kräver en certifierad partner. Mer information finns i [Installera Workfront for Experience Manager Enhanced Connector](https://experienceleague.adobe.com/sv/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install).

## Adobe Creative Cloud integreringar använder nu OAuth2

För större säkerhet och för att skapa en mer enhetlig upplevelse i alla integreringar har vi uppdaterat Adobe Creative Cloud-integreringarna så att de använder OAuth2-autentisering, ett branschstandardsätt att autentisera användare. När användarna loggar in kan de nu se de specifika åtgärder och områden som integreringarna har tillgång till och tillåta åtkomst till. Därefter behöver de inte logga in så ofta.

Mer information finns i [Använda Workfront-tillägget för Illustrator och InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Se information om klienthemlighet för anpassade OAuth2- eller JWT-integreringar

För att skapa transparens i användningen av era anpassade OAuth2- och JWT-integreringar har vi gjort det möjligt för er att se information om de kundhemligheter som era integreringar använder. Nu kan du se de datum då klienthemligheten skapades och senast användes. Du kan också lägga till och visa dina egna anteckningar om klienthemligheten.

Tidigare var dessa uppgifter inte tillgängliga.

Mer information om klienthemligheter i anpassade OAuth2- eller JWT-integreringar finns i [Skapa OAuth2-program för Workfront-integreringar](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Se typ av autentisering i listan över anpassade OAuth2-program

När du nu visar listan över anpassade OAuth2-program i din organisation kan du se om respektive program använder användarautentisering eller serverautentisering.

Tidigare kunde du bara se den här informationen genom att gå till redigeringsalternativen för varje program.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Ange förfallodatum för uppdateringstoken i dina anpassade OAuth2-integreringar

För att få bättre kontroll över åtkomst och säkerhet för dina anpassade OAuth2-integreringar kan du nu anpassa uppdateringstokenernas livslängd. När en användares uppdateringstoken har upphört att gälla, måste användaren logga in på integreringen igen.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Använd publika och privata nycklar i dina anpassade OAuth2-integreringar för server-till-server-appar

Nu kan du konfigurera OAuth2-program server-till-server i dina anpassade integreringar. Genom att ställa in offentliga och privata nycklar kan du tillåta att Workfront kommunicerar med ett annat program utan att använda inloggningsuppgifter.

Tidigare användes användarens inloggningsuppgifter för all autentisering i dina anpassade OAuth2-program.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Integreringen med Google Google Workspace använder nu OAuth2

För större säkerhet och för att skapa en mer enhetlig upplevelse i alla integreringar har vi uppdaterat integreringen med Google Google Workspace så att OAuth2-autentisering används, ett branschstandardsätt att autentisera användare. När användarna loggar in kan de nu se de specifika åtgärder och områden som integreringarna har tillgång till och tillåta åtkomst till. Därefter behöver de inte logga in så ofta.

Mer information finns i [Logga in och ut från Adobe Workfront för Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).

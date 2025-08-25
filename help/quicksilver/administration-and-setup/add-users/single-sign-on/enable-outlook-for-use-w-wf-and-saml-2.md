---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Aktivera Outlook för användning med Workfront och SAML 2.0
description: Om du aktiverar SAML 2.0-autentisering och du vill att dina användare ska kunna logga in på Workfront från Microsoft Outlook med sina SAML 2.0-inloggningsuppgifter, måste du aktivera SAML 2.0 för autentisering i Office-tillägg.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 9fa4f85c914121adddcba4189af1398021544776
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Aktivera Outlook för Workfront och SAML 2.0

>[!IMPORTANT]
>
>[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.
>
>* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**
>
>Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**

<!--DELETE ME MARCH 2026-->

Om du aktiverar SAML 2.0-autentisering och du vill att dina användare ska kunna logga in på Workfront från Microsoft Outlook med sina SAML 2.0-inloggningsuppgifter, måste du aktivera SAML 2.0 för autentisering i Office-tillägg.

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations Workfront-instans använder en anpassad SSO-portal.
>&#x200B;>Kontakta nätverks- eller IT-administratören om du behöver mer information.
<!--
or is enabled with Adobe IMS-->

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Aktivera Outlook för Workfront och SAML 2.0

{{step-1-to-setup}}

1. Klicka på **System** > **Inställningar**.

1. Kontrollera att **Tillåt SAML 2.0-autentisering i Office 365-tillägg** är aktiverat i avsnittet **Säkerhet**.

   Med det här alternativet aktiveras inbäddning av Workfront i en Iframe endast för Office 365-tillägg. Detta öppnar inte en klickbar kapsel eftersom det inte finns något klickbart innehåll.

   Det här alternativet är aktiverat som standard.

   >[!NOTE]
   >
   >Om du aktiverar alternativet **Tillåt inbäddning av Workfront i en iframe** inaktiveras alternativet **Tillåt SAML 2.0-autentisering i Office 365-tillägg** och aktiveras.
   >
   >![Tillåt inbäddningsalternativ](assets/if-you-enable.png)
   >

1. Klicka på **Spara**.

   De ändringar du har sparat här påverkar upplevelsen för alla användare i Workfront.

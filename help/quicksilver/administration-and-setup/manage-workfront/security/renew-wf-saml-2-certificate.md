---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,säkerhet,certifikat,administratör,undantag,konfigurera,metadata
navigation-topic: security
title: Förnya Adobe Workfront SAML 2.0-metadatacertifikatet
description: Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Förnya Adobe Workfront SAML 2.0-metadatacertifikatet

>[!IMPORTANT]
>
>Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om ni har anslutit er till Adobe Admin Console behöver ni inte vidta några åtgärder.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront-servrarna använder SAML 2.0-protokollet för autentisering och auktorisering. När det nya certifikatet har uppdaterats är det giltigt i ett år. När det är dags för dig att förnya certifikatet på din identitetsleverantör får du en varning i Workfront om att den här ändringen måste utföras. Som Workfront-administratör kan du hantera den här ändringen på systemnivå.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations Workfront-instans har aktiverats med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

## Åtkomstkrav

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera SAML 2.0 i Workfront

Så här granskar du varningsmeddelandet och bekräftar uppdateringen av SAML 2.0-metadata hos din identitetsleverantör:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System** > **Enkel inloggning**.

1. I **Typ** nedrullningsbar meny, välja **SAML 2.0**.

1. Klicka **Ladda ned SAML 2.0-metadata**.

   Detta hämtar det förnyade Workfront-certifikatet för SAML 2.0, som innehåller rätt metadata för servern.

   >[!CAUTION]
   >
   >Innan du överför Workfront-metadata till din Single Sign-On-leverantör (SSO) i steg 5 kopierar du din aktuella ACS-URL (Assertion Consumer Service) till en säker plats. Denna URL, som också kallas svars-URL, finns på SSO-leverantörens Workfront-konfigurationssida.
   >
   >
   >Om ACS-URL:en ändras efter att du har överfört Workfront-metadata, innebär det att metadata kan innehålla en felaktig ACS-URL. Du måste ändra tillbaka den till den du kopierade för att undvika att bryta din Single Sign-On-anslutning. Det uppdaterade certifikatet kommer fortfarande att vara korrekt när du har gjort det.

1. Gå till din identitetsleverantörsserver och uppdatera det nya certifikatet som du hämtade.
1. I Workfront på **SSO-sida (Single Sign-on)** kontrollerar du att det här alternativet är markerat: **Det nya Workfront-certifikatet har redan överförts till identitetsleverantören**.

   När det här fältet är markerat kan Workfront-administratörer logga in på Workfront med sina inloggningsuppgifter för enkel inloggning eller Workfront-uppgifter.

1. Klicka **Spara**.

   Varningsmeddelandet visas inte längre eftersom du har bekräftat att SAML 2.0-certifikatet har förnyats på identitetsleverantörens server.

1. Klicka **Testanslutning** för att testa konfigurationen.

   Ett meddelande som bekräftar att anslutningen lyckades visas.

Om du vill ha mer information eller behöver hjälp med att konfigurera metadata manuellt kontaktar du vårt supportteam, vilket förklaras i [Kontakta kundsupport](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

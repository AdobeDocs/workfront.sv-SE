---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,säkerhet,certifikat,administratör,undantag,konfigurera,metadata
navigation-topic: security
title: Förnya Adobe Workfront SAML 2.0 Metadata Certificate
description: Adobe Workfront-servrarna använder SAML 2.0-protokollet för autentisering och auktorisering. När det nya certifikatet har uppdaterats är det giltigt i ett år. När det är dags för dig att förnya certifikatet på din identitetsleverantör får du en varning i Workfront om att den här ändringen måste utföras. Som Workfront-administratör kan du hantera den här ändringen på systemnivå.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Förnya Adobe Workfront SAML 2.0-metadatacertifikatet

>[!IMPORTANT]
>
>Den procedur som beskrivs på den här sidan har tagits bort eftersom den endast gäller för organisationer som ännu inte har anslutit sig till Adobe Admin Console. Denna procedur är inte nödvändig för företag i Adobe Admin Console.
>
>Eftersom alla Workfront-organisationer nu har anslutit sig till Adobe Admin Console kommer den här artikeln att tas bort inom en nära framtid.

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om ni har anslutit er till Adobe Admin Console behöver ni inte vidta några åtgärder.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront-servrarna använder SAML 2.0-protokollet för autentisering och auktorisering. När det nya certifikatet har uppdaterats är det giltigt i ett år. När det är dags för dig att förnya certifikatet på din identitetsleverantör får du en varning i Workfront om att den här ändringen måste utföras. Som Workfront-administratör kan du hantera den här ändringen på systemnivå.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations Workfront-instans har aktiverats med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

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
  <td> <p>Nytt: Standard </p>
 <p>eller</p> 
<p>Aktuell: Planera </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera SAML 2.0 i Workfront

Så här granskar du varningsmeddelandet och bekräftar uppdateringen av SAML 2.0-metadata hos din identitetsleverantör:

{{step-1-to-setup}}

1. Klicka på **System** > **Enkel inloggning**.

1. I listrutan **Typ** väljer du **SAML 2.0**.

1. Klicka på **Hämta SAML 2.0-metadata**.

   Detta hämtar det förnyade Workfront-certifikatet för SAML 2.0, som innehåller rätt metadata för servern.

1. I identitetsleverantören kopierar du den aktuella ACS-URL (Assertion Consumer Service) (kallas även svars-URL) till en säker plats.

   >[!CAUTION]
   >
   >Innan du överför Workfront-metadata till din Single Sign-On-leverantör (SSO) i steg 6 kopierar du din aktuella ACS-URL (Assertion Consumer Service) till en säker plats. Denna URL, som också kallas svars-URL, finns på SSO-leverantörens Workfront-konfigurationssida.
   >
   >
   >Om ACS-URL:en ändras efter att du har överfört Workfront-metadata, innebär det att metadata kan innehålla en felaktig ACS-URL. Du måste ändra tillbaka den till den du kopierade för att undvika att bryta din Single Sign-On-anslutning. Det uppdaterade certifikatet kommer fortfarande att vara korrekt när du har gjort det.

1. Uppdatera det nya certifikatet som du hämtade på din identitetsleverantörsserver.
1. (Villkorligt) Om URL:en för ACS (Assertion Consumer Service) eller URL:en för svar har ändrats hos din identitetsleverantör, ändrar du tillbaka den till den URL du kopierade i steg 5.
1. Kontrollera att det här alternativet är markerat på sidan **enkel inloggning (SSO)** i Workfront: **Det nya Workfront-certifikatet har redan överförts till identitetsleverantören**.

   >[!NOTE]
   >
   >* Det här alternativet är bara synligt om följande gäller:
   >   * Din organisation har redan konfigurerats för SAML 2.0
   >   * Det aktuella certifikatet är klart att upphöra att gälla
   >   * Det nya certifikatet är tillgängligt
   >* När det här fältet är markerat kan Workfront-administratörer logga in på Workfront med sina inloggningsuppgifter för enkel inloggning eller Workfront-uppgifter.

1. Klicka på **Spara**.

   Varningsmeddelandet visas inte längre eftersom du har bekräftat att SAML 2.0-certifikatet har förnyats på identitetsleverantörens server.

1. Klicka på **Testa anslutningen** för att testa konfigurationen.

   Ett meddelande som bekräftar att anslutningen lyckades visas.

Om du vill ha mer information eller behöver hjälp med att konfigurera metadata manuellt kontaktar du vårt supportteam, vilket förklaras i [Kontakta kundsupport](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: The [!DNL Adobe Workfront] Anpassad miljö för uppdatering av sandlådan
description: Sandlådan för anpassad uppdatering är en miljö där du kan testa och arbeta med data från din produktionsmiljö. Det är också idealiskt för att köra kurser och fastställa installationsfunktioner.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 8ceb370df6ff6f3a7a4376d6086fbabe99609e29
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 0%

---

# The [!DNL Adobe Workfront] Anpassad miljö för uppdatering av sandlådan

Sandlådan för anpassad uppdatering är en miljö där du kan testa och arbeta med data från din produktionsmiljö. Det är också idealiskt för att köra kurser och fastställa installationsfunktioner.

>[!NOTE]
>
>Detta skiljer sig från förhandsvisningssandlådan, som också är en testmiljö som replikerar din [!DNL Workfront] produktionsmiljö.
>
>* Nya funktioner introduceras i förhandsvisningssandlådan innan de blir tillgängliga i produktionen.
>* Nya funktioner införs inte i sandlådan för anpassad uppdatering innan de blir tillgängliga i produktionen.
>
>  Det finns också en extra kostnad för att hämta den anpassade uppdateringssandlådan som inte behövs för förhandsvisningssandlådan.
>
>  Mer information om förhandsvisningssandlådan finns i [The [!DNL Adobe Workfront] Förhandsgranska sandlådemiljö](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licens</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Supportpaket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred], eller [!UICONTROL Enterprise]</p> <p>Standardsupportpaketet har inte tillgång till den anpassade uppdateringssandlådan, men det har tillgång till förhandsvisningens sandlåda.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Uppdatera den anpassade uppdateringssandlådan

Sandlådan för anpassad uppdatering innehåller dina faktiska produktionsdata, och den uppdateras inte förrän du schemalägger den att göra det. Du kan schemalägga en uppdatering när som helst, så ofta som en gång i veckan.

>[!NOTE]
>
>* Du kan inte schemalägga en uppdatering för den aktuella dagen. Om idag till exempel är 1 juni är den tidigaste dagen då du kan schemalägga en uppdatering 2 juni.
>* Den schemalagda uppdateringen sker någon gång under natten, baserat på användarens kluster (amerikanska kluster uppdateras under natten i USA). Den angivna tiden är oförutsägbar på grund av andra kunder i kön och hur mycket data som uppdateras. Om kön har många stora kunder kan det hända att uppdateringen inte körs förrän den dagen eller nästa dag.
>* Din anpassade uppdateringssandlåda har alltid samma produktfunktioner som din produktionsmiljö. När du uppdaterar din anpassade uppdateringssandlåda bevaras dock endast varumärket för inloggningsskärmens bakgrundsfärg. Inloggningsskärmen och navigeringsfältets logotyper återställs till [!DNL Workfront] standardvärden, och eventuella varumärkesbilder som du har ändrat före uppdateringen visas inte.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Få åtkomst till sandlådan för anpassad uppdatering från produktionsmiljön {#access-the-custom-refresh-sandbox-from-your-production-environment}

Som en [!DNL Workfront] -administratör kan du komma åt din anpassade uppdateringssandlåda från din produktionsmiljö.

>[!NOTE]
>
>Om ditt konto finns i kluster 4 (EMEA-kluster) kan du inte komma åt din anpassade uppdateringssandlåda från produktionsmiljön. Mer information om hur du får åtkomst till din anpassade uppdateringssandlåda när du har ett konto i kluster 4 finns i [Få åtkomst till sandlådan för anpassad uppdatering för konton i kluster 4 (EMEA-konton)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Få åtkomst till sandlådan för anpassad uppdatering för konton i kluster 4 (EMEA-konton)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Så här kommer du åt din anpassade uppdateringssandlåda:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka **[!UICONTROL System]** >**[!UICONTROL Preferences]**.

1. I **[!UICONTROL Test Environment]** avsnitt, klicka **[!UICONTROL Sandbox 1]** eller **[!UICONTROL Sandbox 2]**.

   Supportpaketet anger om du har tillgång till en eller två anpassade uppdateringssandlådor.

1. Logga in med dina egna autentiseringsuppgifter för uppdateringssandlådan.

   Dina autentiseringsuppgifter för anpassade uppdateringssandlådor är desamma som dina produktionsuppgifter, såvida du inte har ändrat dina produktionsuppgifter sedan du senast uppdaterade din anpassade uppdateringssandlåda. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.

   I sandlådan för anpassad uppdatering visas både version och senaste uppdateringsdatum i banderollen högst upp på skärmen. All information från produktionen finns tillgänglig och kan användas när uppdateringen är klar.

## Öppna den anpassade uppdateringssandlådan med en URL {#access-the-custom-refresh-sandbox-using-a-url}

Alla användare kan komma åt den anpassade uppdateringssandlådan via en URL.

* [Få åtkomst till sandlådan för anpassad uppdatering för konton i kluster 1,2,3 och 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Få åtkomst till sandlådan för anpassad uppdatering för konton i kluster 4 (EMEA-konton)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Få åtkomst till sandlådan för anpassad uppdatering för konton i kluster 1,2,3 och 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Beroende på ditt supportpaket bör du ha tillgång till en eller två anpassade uppdateringssandlådor.

Så här kommer du åt din anpassade uppdateringssandlåda via en URL:

1. Navigera till den här URL:en om du bara har en anpassad uppdateringssandlåda:

   https://companyname.sb01.workfront.com (gammal URL:https://cr1.attasksandbox.com/.)

   Eller om du har två anpassade uppdateringssandlådor, utöver URL:erna ovan, kan du även gå till följande URL för att komma åt din andra anpassade uppdateringssandlåda:

   https://companyname.sb02.workfront.com (gammal URL:https://cr2.attasksandbox.com/)

1. På inloggningsskärmen loggar du in med dina anpassade autentiseringsuppgifter för uppdateringssandlådan.
1. Dina autentiseringsuppgifter för anpassade uppdateringssandlådor är desamma som dina produktionsuppgifter, såvida du inte har ändrat dina produktionsuppgifter sedan din anpassade uppdateringssandlåda senast uppdaterades. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.

### Få åtkomst till sandlådan för anpassad uppdatering för konton i kluster 4 (EMEA-konton) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Om [!DNL Workfront] kontot finns i kluster 4 (EMEA-kluster). Du har bara åtkomst till din anpassade uppdateringssandlåda via en URL. Kontakta vårt kundsupportteam för att ta reda på vilket kluster ditt konto är i.

Beroende på ditt supportpaket bör du ha tillgång till en eller två anpassade uppdateringssandlådor.

Så här kommer du åt din anpassade uppdateringssandlåda via en URL:

1. Navigera till den här URL:en om du bara har en anpassad uppdateringssandlåda:

   https://companyname.sb01.workfront.com (gammal URL:https://cr3.attasksandbox.com)

   eller

   Gå till någon av dessa URL:er om du har två anpassade uppdateringssandlådor:

   https://companyname.sb01.workfront.com (gammal URL:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (gammal URL:https://cr4.attasksandbox.com)

1. På inloggningsskärmen loggar du in med dina anpassade autentiseringsuppgifter för uppdateringssandlådan.

   Dina autentiseringsuppgifter för anpassade uppdateringssandlådor är desamma som dina produktionsuppgifter, såvida du inte har ändrat dina produktionsuppgifter sedan din anpassade uppdateringssandlåda senast uppdaterades. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.

## Schemalägg en uppdatering av din anpassade uppdateringssandlåda

>[!IMPORTANT]
>
>Uppdateringens varaktighet beror på storleken på de data som uppdateras. Under uppdateringsprocessen är det viktigt att din anpassade uppdateringssandlådemiljö inte används på något sätt (inklusive API-anrop och integreringar) eftersom det förhindrar att uppdateringen av sandlådan slutförs. [!DNL Workfront] inaktiverar den anpassade uppdateringssandlådemiljön innan den börjar, men du måste avsluta alla aktiva sessioner för att se till att uppdateringen av sandlådan lyckas.

När du har schemalagt en uppdatering av din anpassade uppdateringssandlåda kan du avbryta den genom att klicka på [!UICONTROL Cancel] överst på sidan. Du kan också schemalägga om den senare.

>[!NOTE]
>
>Du kan inte schemalägga automatiska uppdateringar av sandlådan.

Så här schemalägger du en uppdatering av din kunduppdateringssandlåda:

1. Logga in på din anpassade uppdateringssandlåda.
1. Klicka **[!UICONTROL Schedule]** i bannern högst upp på skärmen och välj ett datum i kalendern.
1. Välj ett datum för när du vill att uppdateringen ska ske och klicka sedan på **[!UICONTROL Schedule Refresh]**.

## Växla till produktion från den anpassade uppdateringssandlådan

1. Logga in på din anpassade uppdateringssandlåda.

   Mer information om hur du använder din anpassade uppdateringssandlåda finns i [Få åtkomst till sandlådan för anpassad uppdatering från produktionsmiljön](#access-the-custom-refresh-sandbox-from-your-production-environment) eller [Öppna den anpassade uppdateringssandlådan med en URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Klicka **[!UICONTROL Go To Production]** i banderollen högst upp på skärmen.

   Kom ihåg att arbete som utförs i sandlådan inte visas i [!UICONTROL production] -miljö, allt eftersom överföringen av data är enkel, från produktion till din anpassade uppdateringssandlåda, och inte i omvänd ordning.

## Ta emot e-postmeddelanden från sandlådan för anpassad uppdatering

[!DNL Workfront] inaktiverar all e-postkommunikation från sandlådemiljön för anpassad uppdatering. Om du vill få e-postmeddelanden från sandlådemiljön för anpassad uppdatering måste du aktivera den här funktionen i dina användarinställningar. Mer information om hur du aktiverar e-postmeddelanden i sandlådemiljön för anpassad uppdatering finns i [Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Rapportleverans och push-meddelanden på mobilappen är alltid inaktiverade för sandlådemiljön för anpassad uppdatering. Varken du eller [!DNL Workfront] administratören kan aktivera rapportleverans eller push-meddelanden för mobilappen när du öppnar sandlådemiljön för anpassad uppdatering.\
>Mer information om rapportleveranser för produktionsmiljön finns i [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Mer information om push-meddelanden i mobilappen för produktionsmiljön finns i avsnittet i .

## Konfigurera enkel inloggning i sandlådan Anpassad uppdatering

Om du vill konfigurera din anpassade uppdateringssandlåda så att den fungerar med en enkel inloggningslösning kan du göra det genom att konfigurera den separat från produktionsmiljön. SSO-konfigurationen i sandlådan för anpassad uppdatering är oberoende av SSO-konfigurationen i produktionsmiljön.\
När du uppdaterar din anpassade uppdateringssandlåda kopieras inte SSO-informationen från produktionsmiljön för att skriva över konfigurationen för den anpassade uppdateringssandlådan.

Stegen för att konfigurera enkel inloggning i sandlådan för anpassad uppdatering liknar de som används för att konfigurera den i produktionsmiljön.\
Mer information om konfiguration [!DNL Workfront] med SSO, se [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations [!DNL Workfront] -instansen aktiveras med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

## Avsedd användning och tillgänglighet

* [!DNL Workfront] Anpassade sandlådemiljöer för uppdatering är inte avsedda för prestanda- eller inläsningstestning. Använd i stället dessa miljöer för att validera funktionaliteten med organisationens befintliga arbetsflöden.

* [!DNL Workfront] Anpassade sandlådemiljöer för uppdatering är alltid tillgängliga. Alla avbrott i Workfront anpassade uppdateringssandlådemiljö under normal kontorstid är den första prioriteten omedelbart efter att eventuella produktionsproblem har åtgärdats. Alla avbrott i Workfront anpassade uppdateringssandlådemiljö på helger (lördagar och söndagar) åtgärdas så att miljön körs under kontorstid på måndag.

* Korrektur är inte tillgängligt i anpassade sandlådemiljöer för uppdatering.

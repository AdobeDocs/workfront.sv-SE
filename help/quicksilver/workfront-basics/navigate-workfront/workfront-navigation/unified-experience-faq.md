---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Vanliga frågor om Adobe Unified Experience
description: Vissa funktioner skiljer sig åt mellan  [!DNL Workfront]  och Adobe Experience Cloud, och du kan ha frågor när din [!DNL Workfront] instans migreras till den enhetliga upplevelsen.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: ff8866b2b48ead3b7b2e035a394fa038036fbfc0
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Vanliga frågor om [!DNL Adobe Unified Experience]

Med [!DNL Adobe Unified Experience] för [!DNL Workfront] kan du hantera alla dina [!DNL Adobe]-program på ett och samma ställe med en enda inloggning. Navigeringsområdet [!DNL Adobe] är integrerat med [!DNL Workfront]. Några funktioner är annorlunda och du kan ha frågor när din [!DNL Workfront]-instans migreras till den enhetliga upplevelsen.

Mer information om hur du loggar in på [!DNL Adobe Unified Experience] finns i [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Jämförelse av upplevelsen [!DNL Adobe Unified Experience] och [!DNL Workfront only]

Endast kunder som använder [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] har åtkomst till [!DNL Adobe Unified Experience]. Kunder som ännu inte har migrerat kommer att se [!DNL Workfront only]-upplevelsen, utan möjlighet att växla mellan [!DNL Adobe]-program.

I tabellen beskrivs några funktioner som skiljer sig åt mellan de båda upplevelserna.

| [!DNL Adobe Unified Experience] | Endast [!DNL Workfront]-upplevelse |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Main Menu] finns till vänster ![Huvudmeny](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Main Menu] är till höger ![Huvudmeny](assets/main-menu-icon.png) |
| En enda inloggnings-URL är tillgänglig för alla [!DNL Adobe Experience Cloud]-program | Logga in på [!DNL Workfront] med en anpassad [!DNL Workfront]-URL |
| Med en&quot;organisationsväljare&quot; kan du växla mellan [!DNL Workfront] organisationer och miljöer | &quot;Organisationsväxlaren&quot; är inte tillgänglig |
| Navigeringen innehåller ett navigeringsområde på den översta nivån för [!DNL Adobe] produkter, [!DNL Adobe] meddelanden, hjälp och din användarprofil, förutom navigeringsfältet [!DNL Workfront] | Navigeringen innehåller endast navigeringsfältet [!DNL Workfront] |
| Hjälpen är tillgänglig via [!UICONTROL Main Menu] och det övre navigeringsområdet | Hjälpen är tillgänglig via navigeringsfältet [!UICONTROL Main Menu] och [!DNL Workfront] |
| Språkvisningsprogrammet öppnas på en ny flik | Språkvisningsprogrammet öppnas i Workfront |
| Den URL som används för att komma åt Workfront är `experience.adobe.com` | Den URL som används för att komma åt Workfront är `(CompanyName).my.workfront.adobe.com` |
| Datumformatet (t.ex. MM/DD/ÅÅÅÅ) baseras på språkinställningarna för enhetlig upplevelse. Om användaren inte har uppdaterat sina språkinställningar används `en-US`-inställningarna. | Datumformatet (t.ex. MM/DD/ÅÅÅ) baseras på webbläsarens inställningar |

{style="table-layout:auto"}

## Frågor och svar

### Hur avgör jag om jag använder Adobe Unified Experience eller Adobe Workfront?

Om du vill ta reda på om din organisation använder Adobe Unified Experience kontrollerar du den URL som du använder för att få tillgång till Workfront.

| URL | Adobe Experience |
|------------|------------|
| (CompanyName).my.workfront.com | Workfront |
| experience.adobe.com | Adobe Unified Experience |

### Hur kan jag lära mig mer om [!DNL Adobe Admin Console]?

Mer information om [!DNL Admin Console] finns i följande artiklar:

* [Förbered för  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] översikt](https://helpx.adobe.com/se/enterprise/using/admin-console.html)

### Vad behöver jag som kund för att underlätta migreringen?

Befintliga kunder kontaktas för att schemalägga migreringar. De supportteam som arbetar med migrering kommer att hjälpa kunderna genom processen, ge råd om konfigurationen av [!DNL Admin Console] och tillhandahålla länkar till dokumentation som behövs för att göra flytten så enkel och krångelfri som möjligt. Mer information finns i [[!DNL Adobe Business Platform] och [!DNL Admin Console] Vanliga frågor](https://experienceleague.adobe.com/sv/docs/support-resources/adobe-support-tools-guide/workfront/faq).

### Hur hanterar du [!DNL Adobe Admin Console] för företag som redan har detta aktiverat för Federated ID:n på ett annat sätt än [!DNL Workfront] enkel inloggning har konfigurerats?

[!DNL Adobe Admin Console] kan inkludera [!DNL Workfront] och ersätta enkel inloggning med Adobe Identity Management System (IMS). All användaretablering sker i [!DNL Admin Console], och användarna ser inloggningsskärmen [!DNL Adobe] för att komma till [!DNL Experience Cloud] där de ser [!DNL Workfront] som ett alternativ (om de beviljas åtkomst till den).

### Hur påverkar detta kunder som redan har AEM administratörspanel för [!DNL Adobe Assets] - men enkel inloggning är konfigurerad på ett annat sätt än [!DNL Workfront?]

När [!DNL Workfront] har lagts till som ett [!DNL Admin Console]-program behöver du inte göra något annat för [!DNL Workfront] för att utnyttja den befintliga SSO-konfigurationen som du har för [!DNL Adobe Assets].

### Hur påverkar detta de som har konfigurerats med enkel inloggning?

enkel inloggning har konfigurerats i [!DNL Admin Console] och ärvs av programmet [!DNL Workfront].

### Kommer enkel inloggning med vår interna [!DNL Active Directory] fortfarande att vara ett alternativ med Adobe Identity Management System (IMS)?

IMS ersätter enkel inloggning och fungerar i huvudsak på samma sätt. Alla användarbehörigheter beviljas och etableras i [!DNL Adobe Admin Console], och användaren ser inloggningsskärmen [!DNL Adobe] där han/hon kan välja [!UICONTROL Personal Account] eller [!UICONTROL Company Account] för att logga in (om du har [!DNL Active Directory] loggar de flesta in med ett företagskonto).

### För de som inte använder enkel inloggning, ändras inloggnings-URL:en för [!DNL Workfront]?

Inloggnings-URL:en ändras, men den gamla URL:en omdirigeras till den nya inloggnings-URL:en, så du bör omdirigera dina användare dit de ska gå.

### Kommer alias som vi har konfigurerat fortfarande att fungera, eller ändras [!DNL Workfront]-länkarna med den här migreringen?

[!DNL Workfront] omdirigeringar/alias är tillgängliga för att komma till hemsidan.

### Kommer omdirigeringar att inaktiveras någon gång? Eller kan vi alltid skriva i my.company.workfront.com?

Du kan alltid använda anpassade URL:er. När du har klickat på någon av länkarna dirigeras du till [!DNL Workfront] och en annan URL visas. Det är dock bättre för [!DNL experience] att logga in på experience.adobe.com och bokmärkeslänkar inifrån [!DNL Experience Cloud]. Mindre omdirigering är lika med mindre fördröjning/inläsningstid.

### Kommer direkta länkar till begärandeköer att brytas?

Alla direkta länkar ska omdirigeras till de nya URL-mönstren. Om du har distribuerat länkar till personer bör du dock skicka en uppdatering som utnyttjar direktlänken och förhindrar att det tar för lång tid att komma till den förväntade sidan.

### Migrerar vi till [!DNL Experience Cloud] globalt eller kan vi välja för vissa användare (inte alla våra användare använder ens andra Adobe-produkter)?

Hela [!DNL Workfront]-kundkontot migreras. Det kan inte göras per användare.

### Måste alla [!DNL Workfront]-användare logga in via [!DNL Experience Cloud]? Eller bara administratörer?

Ja, alla användare loggar in via [!DNL Experience Cloud]. Inloggningen för Adobe Identity Management System (IMS) ersätter enkel inloggning. Det är en väldigt likartad upplevelse, bara en annan inloggningsskärm.

### Måste användare länka sina [!DNL Adobe]-konton till sina [!DNL Workfront]-konton om de redan har båda?

Ja, det finns en process för detta och mer information kommer att ges när det är dags för din organisation att gå över till IMS.

### Vad händer med de [!DNL Workfront]-användare som inte har något [!DNL Adobe]-konto?

Användare som inte har beviljats åtkomst i [!DNL Adobe Admin Console] för att komma in i [!DNL Workfront] måste skapa ett [!UICONTROL personal account]- eller ett [!DNL Adobe] ID-konto för att kunna logga in. Detta skickar ett e-postmeddelande till administratören för att godkänna eller avvisa deras begäran, och det gör även att administratören kan konfigurera vilken typ av åtkomst användaren har. När de loggar in går de till experience.adobe.com, anger sin e-postadress och väljer [!UICONTROL Personal Account]. Därifrån kan de komma åt [!DNL Workfront].

### Vad händer om vi inte har några andra [!DNL Adobe]-produkter än [!DNL Workfront?]

Vi rekommenderar fortfarande att din organisation migrerar till [!DNL Adobe Unified Experience]. Du får ett [!DNL Adobe]-ID tillsammans med förmånerna som anges ovan.

### Externa användare ingår i vår [!DNL Workfront]-instans. Vi vill inte att de ska ha tillgång till några andra produkter som ingår i [!DNL Adobe]. Hur begränsar vi deras åtkomst inom konsolen?

[!DNL Admin Console] ger administratörer stor kontroll över vad användare kan och inte kan komma åt. När en extern användare vill ha åtkomst måste de skapa ett [!DNL Adobe]-ID, som skickar ett e-postmeddelande till administratören. Administratören kan sedan godkänna eller avslå åtkomsten till en produkt och definiera vad han/hon kan eller inte får åtkomst till för produkter som ägs av den organisationen. Sedan kan systemadministratören för [!DNL Workfront] gå in i [!UICONTROL Users]-området för [!DNL Workfront] och göra mer detaljerade behörigheter för den externa användaren.

### Gruppadministratörer används för att skapa personer i [!DNL Workfront]. Med flytten till [!DNL Experience Cloud], kommer gruppadministratörer fortfarande att kunna skapa personer?

Ja, det går fortfarande att skapa användare via [!DNL Workfront]. Dessa användare kan läggas till i [!DNL Experience Cloud] automatiskt. Du kan också konfigurera dina gruppadministratörer som produktägare i [!DNL Admin Console] så att de kan tilldela [!DNL Workfront] till användare.

### Vad är tidsgränsen för att växla till [!DNL Experience Cloud]?

Det finns ingen tidsgräns att flytta till [!DNL Adobe Experience Cloud]. Vi arbetar med kunderna för att låta dem välja när de är redo att ta steget.

### Kommer vårt supportteam att behöva göra något för denna förändring?

Om supportteamet ansvarar för att skapa nya användare måste de bekanta sig med de [!DNL Admin Console]-gränssnitt som används för att skapa användare och tilldela ett berättigande till Workfront. I annat fall är det sannolikt att det interna supportteamet inte kommer att förändras nämnvärt.

### Hur påverkar detta integreringar vi har via API-funktionen?

Den befintliga URL-sökvägen är fortfarande tillgänglig för API-trafik. Du ska inte behöva göra något för att uppdatera slutpunkterna i dina integreringar. Direktinloggning via användarnamn och lösenord stöds dock inte. Du måste använda en API-nyckel, med undantaget [!DNL Workfront Fusion]-anslutningar.

### Vad gäller för [!DNL Creative Cloud] användare? Hur påverkar migreringen dem? Finns det några fördelar för dem?

Det påverkar inte [!DNL Creative Cloud]-användare när de migrerar till [!DNL Adobe Unified Experience].

### Kommer inloggningarna att ändras för [!DNL Workfront] mobila användare?

[!DNL Workfront] mobila användare bör inte påverkas av migreringen till [!DNL Adobe Unified Experience].

### JumpSeat fungerar inte med [!DNL Adobe Unified Experience]. Hur kan jag lösa det här?

JumpSeat fungerar med [!DNL Adobe Unified Experience], men kräver en konfigurationsuppdatering. Ändra program-URL:en från `workfront.com` till slut med `.workfront.adobe.com` med hjälp av JumpSeat-administratörspanelen.

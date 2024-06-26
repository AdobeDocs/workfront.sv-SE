---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe - frågor och svar om enhetliga upplevelser
description: Vissa funktioner skiljer sig åt [!DNL Workfront] och Adobe Experience Cloud, och du kan ha frågor som [!DNL Workfront] -instansen migreras till den enhetliga upplevelsen.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 019a1b61cd97d5d61f9a4fbf3f98eccab50809a8
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Vanliga frågor

The [!DNL Adobe Unified Experience] for [!DNL Workfront] kan du hantera alla [!DNL Adobe] program på ett och samma ställe med en enda inloggning. The [!DNL Adobe] navigeringsområdet är integrerat med [!DNL Workfront]. Vissa funktioner är annorlunda och du kan ha frågor om [!DNL Workfront] -instansen migreras till den enhetliga upplevelsen.

Mer information om hur du loggar in på [!DNL Adobe Unified Experience], se [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Jämförelse av [!DNL Adobe Unified Experience] och [!DNL Workfront only] upplevelse

Endast kunder som använder [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] kan komma åt [!DNL Adobe Unified Experience]. Kunder som ännu inte har migrerat kan se [!DNL Workfront only] utan möjlighet att växla mellan [!DNL Adobe] program.

I tabellen beskrivs några funktioner som skiljer sig åt mellan de båda upplevelserna.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] endast upplevelsen |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Main Menu] finns till vänster ![Huvudmeny](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Main Menu] är till höger ![Huvudmeny](assets/main-menu-icon.png) |
| En enda inloggnings-URL är tillgänglig för alla [!DNL Adobe Experience Cloud] program | Logga in på [!DNL Workfront] med en egen [!DNL Workfront] URL |
| Med en&quot;företagsväljare&quot; kan du gå mellan [!DNL Workfront] organisationer och miljöer | &quot;Organisationsväxlaren&quot; är inte tillgänglig |
| Navigeringen innehåller ett navigeringsområde på översta nivån för [!DNL Adobe] produkter, [!DNL Adobe] meddelanden, hjälp och din användarprofil, förutom [!DNL Workfront] navigeringsfält | Navigeringen innehåller [!DNL Workfront] endast navigeringsfältet |
| Hjälpen är tillgänglig via [!UICONTROL Main Menu] och övre navigeringsområde | Hjälpen är tillgänglig via [!UICONTROL Main Menu] och [!DNL Workfront] navigeringsfält |

{style="table-layout:auto"}

## Frågor och svar

### Hur avgör jag om jag använder Adobe Unified Experience eller Adobe Workfront?

Om du vill ta reda på om din organisation använder Adobe Unified Experience, kontrollerar du den URL som du använder för att få tillgång till Workfront.

| URL | Adobe Experience |
|------------|------------|
| (CompanyName).my.workfront.com | Workfront |
| experience.adobe.com | Adobe enhetliga upplevelse |

### Hur kan jag lära mig mer om [!DNL Adobe Admin Console]?

Mer information om [!DNL Admin Console]granskar du dessa artiklar:

* [Förbered dig för [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] översikt](https://helpx.adobe.com/se/enterprise/using/admin-console.html)

### Vad behöver jag som kund för att underlätta migreringen?

Befintliga kunder kontaktas för att schemalägga migreringar. De supportteam som arbetar med migrering kommer att hjälpa kunderna genom processen och ge råd om [!DNL Admin Console] konfigurera och tillhandahålla länkar till dokumentation som behövs för att göra flyttningen så enkel och krångelfri som möjligt.

* [[!DNL Adobe Workfront] Supportöversikt](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] information](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] och [!DNL Admin Console] Vanliga frågor](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Hur hanterar du [!DNL Adobe Admin Console] för företag som redan har detta aktiverat för Federated ID på ett annat sätt än [!DNL Workfront] Har enkel inloggning konfigurerats?

[!DNL Adobe Admin Console] har möjlighet att inkludera [!DNL Workfront], ersätter enkel inloggning med IMS. All användaretablering sker i [!DNL Admin Console]och användarna ser [!DNL Adobe] inloggningsskärm för att komma till [!DNL Experience Cloud] där de ser [!DNL Workfront] som ett alternativ (om de har beviljats tillgång till det).

### Hur påverkar detta kunder som redan har AEM administratörspanel för [!DNL Adobe Assets] - men enkel inloggning har konfigurerats annorlunda än [!DNL Workfront?]

En gång [!DNL Workfront] läggs till som [!DNL Admin Console] ska du inte behöva göra något annat för [!DNL Workfront] för att utnyttja befintlig enkel inloggning [!DNL Adobe Assets].

### Hur påverkar detta de som har konfigurerats med enkel inloggning?

enkel inloggning har konfigurerats i [!DNL Admin Console] och ärvs av [!DNL Workfront] program.

### Är enkel inloggning med vår interna [!DNL Active Directory] Kommer du fortfarande att vara ett alternativ med IMS?

IMS ersätter enkel inloggning och fungerar i huvudsak på samma sätt. Alla användarbehörigheter beviljas och tilldelas i [!DNL Adobe Admin Console]och användaren ser [!DNL Adobe] inloggningsskärm där de kan välja &quot;[!UICONTROL Personal Account]&quot; eller &quot;[!UICONTROL Company Account]&quot; för att logga in (om du har [!DNL Active Directory]loggar de flesta in med ett företagskonto).

### För dem som inte använder enkel inloggning gör [!DNL Workfront] ändra inloggnings-URL?

Inloggnings-URL:en ändras, men den gamla URL:en omdirigeras till den nya inloggnings-URL:en, så du bör omdirigera dina användare dit de ska gå.

### Kommer alias som vi har konfigurerat fortfarande att fungera, eller är [!DNL Workfront] länkar som ändras med den här migreringen?

[!DNL Workfront] omdirigeringar/alias finns tillgängliga för att komma till hemsidan.

### Kommer omdirigeringar att inaktiveras någon gång? Eller kan vi alltid skriva i my.company.workfront.com?

Du kan alltid använda anpassade URL:er. När du har klickat på någon av länkarna dirigeras du till [!DNL Workfront] och visa en annan URL. Men det är bättre [!DNL experience] för att logga in på experience.adobe.com och bokmärkeslänkar inifrån [!DNL Experience Cloud]. Mindre omdirigering är lika med mindre fördröjning/inläsningstid.

### Kommer direkta länkar till begärandeköer att brytas?

Alla direkta länkar ska omdirigeras till de nya URL-mönstren. Om du har distribuerat länkar till personer bör du dock skicka en uppdatering som utnyttjar direktlänken och förhindrar att det tar för lång tid att komma till den förväntade sidan.

### Ska vi migrera till [!DNL Experience Cloud] globalt eller kan vi välja för vissa användare (inte alla våra användare ens använder andra Adobe-produkter)?

Hela [!DNL Workfront] kundkontot migreras. Det kan inte göras per användare.

### Kommer alla [!DNL Workfront] användare måste logga in via [!DNL Experience Cloud]? Eller bara administratörer?

Ja, alla användare loggar in via [!DNL Experience Cloud]. IMS-inloggningen ersätter enkel inloggning. Det är en väldigt likartad upplevelse, bara en annan inloggningsskärm.

### Kommer användarna att behöva länka sina [!DNL Adobe] konton hos [!DNL Workfront] konton om de redan har båda?

Ja, det finns en process för detta och mer information kommer att ges när det är dags för din organisation att gå över till IMS.

### Vad händer med [!DNL Workfront] användare som inte har [!DNL Adobe] konto?

Användare som inte har beviljats åtkomst i [!DNL Adobe Admin Console] för att komma igång [!DNL Workfront] måste skapa en[!UICONTROL personal account]&quot; eller [!DNL Adobe] ID-konto som ska kunna logga in. Detta skickar ett e-postmeddelande till administratören för att godkänna eller avvisa deras begäran, och det gör även att administratören kan konfigurera vilken typ av åtkomst användaren har. När de loggar in går de till experience.adobe.com, anger sin e-postadress och väljer [!UICONTROL Personal Account]. Därifrån kan de komma åt [!DNL Workfront].

### Tänk om vi inte har några [!DNL Adobe] andra produkter än [!DNL Workfront?]

Vi rekommenderar fortfarande att din organisation migrerar till [!DNL Adobe Unified Experience]. Du får en [!DNL Adobe] ID tillsammans med de förmåner som anges ovan.

### Vi har externa användare inräknade i våra [!DNL Workfront] -instans. Vi vill inte att de ska ha tillgång till andra produkter som ingår i [!DNL Adobe]. Hur begränsar vi deras åtkomst inom konsolen?

[!DNL Admin Console] ger administratörer stor kontroll över vad användare kan och inte kan komma åt. När en extern användare vill ha åtkomst måste de skapa en [!DNL Adobe] ID, som skickar ett e-postmeddelande till administratören. Administratören kan sedan godkänna eller avslå åtkomsten till en produkt och definiera vad han/hon kan eller inte får åtkomst till för produkter som ägs av den organisationen. Sedan [!DNL Workfront] Systemadministratören kan gå till [!UICONTROL Users] område på [!DNL Workfront] för att ge mer detaljerad behörighet till den externa användaren.

### Gruppadministratörer används för att skapa personer i [!DNL Workfront]. I och med övergången till [!DNL Experience Cloud], kommer gruppadministratörer fortfarande att kunna skapa personer?

Ja, det går fortfarande att skapa användare via [!DNL Workfront]. Dessa användare kan läggas till i [!DNL Experience Cloud] automatiskt. Du kan också konfigurera gruppadministratörer som produktägare i [!DNL Admin Console] så att de kan tilldela [!DNL Workfront] till användare.

### Vad är tidsgränsen för att byta till? [!DNL Experience Cloud]?

Det finns ingen tidsgräns att gå till [!DNL Adobe Experience Cloud]. Vi arbetar med kunderna för att låta dem välja när de är redo att ta steget.

### Kommer vårt supportteam att behöva göra något för denna förändring?

Om supportteamet ansvarar för att skapa nya användare måste de bekanta sig med [!DNL Admin Console] gränssnitt som används för att skapa användare och tilldela ett berättigande till Workfront. I annat fall är det sannolikt att det interna supportteamet inte kommer att förändras nämnvärt.

### Hur påverkar detta integreringar vi har via API-funktionen?

Den befintliga URL-sökvägen är fortfarande tillgänglig för API-trafik. Du ska inte behöva göra något för att uppdatera slutpunkterna i dina integreringar. Direktinloggning via användarnamn och lösenord stöds dock inte - du måste använda en API-nyckel, med undantaget att [!DNL Workfront Fusion] kontakter.

### Vad händer med [!DNL Creative Cloud] användare? Hur påverkar migreringen dem? Finns det några fördelar för dem?

Det påverkar inte [!DNL Creative Cloud] användare med migrering till [!DNL Adobe Unified Experience].

### Kommer inloggningar att ändras för [!DNL Workfront] mobilanvändare?

[!DNL Workfront] mobilanvändare bör inte påverkas av migreringen till [!DNL Adobe Unified Experience].

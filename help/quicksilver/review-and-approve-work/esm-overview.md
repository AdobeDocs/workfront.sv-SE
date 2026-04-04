---
product-area: documents
navigation-topic: approvals
title: Adobe Enterprise Storage - översikt
description: Adobe Enterprise Storage - översikt
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Adobe Enterprise Storage - översikt

Adobe Enterprise-lagring är en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter. Integreringen av Workfront och Frame.io bygger på Adobe Enterprise-lagring, vilket möjliggör smidigt samarbete och filhantering mellan dessa plattformar.

Det här lagringsalternativet banar också väg för framtida integrering av resurshantering med andra Adobe-produkter, som Adobe Creative Cloud.

## Viktiga funktioner

* **Enhetligt lagringslager**: Adobe Enterprise-lagring fungerar som en delad lagringsserver för Workfront, Frame.io, Document Cloud och Creative Cloud. Detta möjliggör smidigt samarbete och filhantering på dessa plattformar.

* **Aktivera supply chain-innehåll**: Adobe Enterprise-lagring är en grundläggande komponent för Adobe Content Supply chain-vision, vilket gör att team kan hantera resurser som är under arbete utan att behöva hämta eller ladda upp manuellt i olika Adobe-program.

* **Centraliserad behörighet och åtkomst**: Adobe Enterprise-lagring har stöd för åtkomstkontroller på företagsnivå, integrering med Adobe IMS (Identity Management System) för säkra och skalbara användarbehörigheter.

* **Komplett synlighet för resurser**: Assets som lagras i Adobe Enterprise-lagring kan nås och hanteras direkt i Workfront-, Frame.io- och Creative Cloud-appar, vilket ger enhetlig metadata, versionshantering och verifieringskedja.

* **Integrering med arbetsflöden för granskning och godkännande**: Adobe Enterprise-lagring möjliggör kreativa arbetsflöden för granskning och godkännande genom att fungera som en källa för sanning för alla resurser, vilket säkerställer att feedback och godkännanden spåras centralt.

* **Skalbar lagring och kvothantering**: Adobe Enterprise-lagring erbjuder skalbara lagringsalternativ och enhetlig kvotspårning för alla Adobe-produkter.

## Integrering med arbetsflöden för granskning och godkännande

Integreringen av Workfront och Frame.io utnyttjar Adobe Enterprise-lagring för att ge en enhetlig gransknings- och godkännandeupplevelse. Tack vare den här integreringen kan projektsamordnare hantera projekt och planera arbetet i Workfront, medan kreatörer, marknadsförare och intressenter kan granska och godkänna resurser i Frame.io. Detta garanterar att alla intressenter har tillgång till de senaste versionerna av mediefilerna och att feedback samlas på ett och samma ställe.

Mer information om integrationen mellan Workfront och Frame.io finns i [Översikt över enhetlig granskning och godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Skillnader mellan Adobe Enterprise-lagring och Workfront-lagring

Befintliga Workfront-miljöer har en kombination av Adobe Enterprise-lagring och äldre Workfront-lagring. Objekt som skapats innan Adobe Enterprise-lagring släpptes använder äldre Workfront-lagring.

När du har aktiverat Adobe Enterprise-lagring i din miljö kan du skapa både Adobe Enterprise-lagring och äldre Workfront-lagringsprojekt.

>[!NOTE]
>
>Nya Net-miljöer har Adobe Enterprise-lagring aktiverad som standard och har inte möjlighet att använda äldre Workfront-lagring.


### Dokument

#### Nytt dokumentområde

Det nya dokumentområdet är ett enhetligt dokumentområde som har gjorts om för Adobe Enterprise-lagring.

Det uppdaterade gränssnittet förenklar navigeringen, ger större tydlighet och gör det enklare för team att hantera granskningar och godkännanden i en enhetlig miljö. Mer information finns i [Översikt över dokumentområdet](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Ny behörighetsmodell för dokument

>[!IMPORTANT]
>
>I Adobe Enterprise-lagring fungerar dokumentbehörigheter annorlunda än i äldre Workfront-lagring. Dokument ärver behörigheter från det projekt, den uppgift eller det problem de är länkade till.

Dokument kan inte delas individuellt. I stället genererar systemet automatiskt en mapp för varje uppgift eller problem och ärver behörigheter från uppgiften eller utgåvan. Alla dokument som överförs till uppgiften eller utgåvan lagras i den genererade mappen.

Mer information om den nya dokumentbehörighetsmodellen finns i [Översikt över objektbehörigheter och åtkomstnivå för Adobe Enterprise-lagringsmodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Länkade objekt i mappar

På projektnivå visar systemgenererade mappar ett länkat objekt. Mappen får automatiskt samma namn som den uppgift eller utgåva den tillhör. Länkade mappar är hur systemet vet vilken åtgärd eller vilket problem mappen ska visas på.

Mer information finns i [Så här fungerar dokumentbehörigheter](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Workfront-objekt

I tabellen nedan jämförs funktionerna för Adobe Enterprise-lagring och äldre Workfront-lagring för Workfront-objekt.

Workfront-objekt omfattar portföljer, program, projekt, mallar, uppgifter och ärenden.

| Adobe Enterprise-lagring | Äldre Workfront-lagring |
|---|---|
| <ul><li>Använder Adobe Enterprise-lagring</li><li>Integrerat med Frame.io</li><li>Använder den nya dokumentupplevelsen</li><li>Tillämpar strikta namnkonventioner</li><li>Direktdokumentdelning är inte tillgängligt</li><li>Dokument finns i andra Adobe-produkter som Frame.io och Creative Cloud</li></ul> | <ul><li>Använder Workfront-lagring</li><li>Använder korrekturläsaren</li><li>Stöder delning av enskilda dokument</li></ul> |

### Flytta, kopiera och konvertera objekt

Du kan flytta, kopiera och konvertera Workfront-objekt mellan olika lagringsmodeller. Du kan till exempel flytta en uppgift från ett Adobe Enterprise-lagringsprojekt till ett annat Adobe Enterprise-lagringsprojekt. Du kan inte flytta en uppgift från ett Adobe Enterprise-lagringsprojekt till ett äldre Workfront-lagringsprojekt.

Dessa åtgärder är tillgängliga på menyn Mer om en uppgift eller ett problem. Varje åtgärd respekterar dokumentens integritet, behörighetsarv och Adobe Enterprise-lagringsregler.

## Aktivera Adobe Enterprise-lagring

Befintliga kunder kan aktivera Adobe Enterprise-lagring i sin miljö när avtalet förnyas. Mer information om hur du aktiverar Adobe Enterprise-lagring finns i [Aktivera Adobe Enterprise-lagring för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Nya kunder har Adobe Enterprise-lagring aktiverad som standard och har inte möjlighet att använda Workfront-lagring.



## Överväganden

* Workfront kan bli osynkroniserat med Frame.io eller Creative Cloud, t.ex. en resurs som tas bort i Workfront men fortfarande visas i Frame.io, kontakta Workfront support för att få din miljö omsynkroniserad.



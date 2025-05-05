---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: '2020.2 Resurshanteringsförbättringar: Arbetsbelastningsutjämnaren'
description: Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts med 2020.2-versionen till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# 2020.2 Resurshanteringsförbättringar: Arbetsbelastningsutjämnaren

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts med 2020.2-versionen till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.

En lista över alla ändringar som är tillgängliga i version 2020.2 finns i [2020.2 versionsöversikt](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

Personer är en Tier 1-resurs. Med belastningsutjämnaren kan du skydda dem från utbränning och ge dem möjlighet att göra sitt bästa, samtidigt som de anpassas till viktiga företagsstrategier. Vi presenterar en omdesignad schemaläggningsfunktion som gör att du kan visualisera och hantera människors arbetsbelastning och efterfrågan i samma vy. Användargränssnittet ger tydlig visuell mappning av över- och underanvändning och är transparent för alla intressenter. Personhanterare kan använda den informationen som indata och från samma skärm balansera arbetet genom tidslinjen, som sedan återspeglas i resten av Workfront-plattformen.

>[!NOTE]
>
>Utjämningen av arbetsbelastning började lanseras som en betaversion i version 2019.4. Alla förbättringar av belastningsutjämnaren är i allmänhet tillgängliga i version 2020.2. De förbättringar som beskrivs på den här sidan lades till i version 2020.2. En översikt över arbetsbelastningsutjämnaren finns i [Översikt över arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Justera daglig och veckovis allokering i Utjämning av arbetsbelastning

För att undvika att resurser belastas kan du nu justera användarnas dagliga och veckovisa allokering så att de fungerar med hjälp av Utjämning av arbetsbelastning.

Före den här förbättringen var detta bara möjligt med verktygen för resursplanering.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Utjämningsfilter för arbetsbelastning

Om du vill göra informationen i Utjämning av arbetsbelastning relevant för dig kan du nu skapa filter för både Ej tilldelat arbete och Tilldelade arbetsområden i Utjämning av arbetsbelastning och spara dem för framtida bruk. Du kan sedan redigera den sparade versionen för att göra små ändringar i den i stället för att börja från början med ett nytt filter.

Mer information om filtrering i arbetsbelastningsutjämnaren finns i [Hantera filter i arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Visa återstående timmar i Utjämning av arbetsbelastning

För att du ska kunna fatta rätt beslut om tilldelning kan du nu med en ny inställning visa skillnaden mellan antalet timmar mellan de timmar som en användare är tillgänglig att arbeta enligt sitt schema och de timmar som han/hon redan har tilldelats till arbetet (återstående timmar). Den nya inställningen är nu tillgänglig i Utjämning av arbetsbelastning.

Mer information om hur du visar information i arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (eller om du använder Adobe Workfront Classic, se [Navigera i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Nya Adobe Workfront

## Visa dagliga planerade timmar för aktiviteter och projekt i Ej tilldelat arbetsområde i Utjämning av arbetsbelastning

För att du lättare ska förstå hur uppgifter påverkar arbetsbelastningen för dina användare innan du tilldelar dem hanterar inställningen Visa tilldelningar nu vilken information som visas i området Ej tilldelat arbete i Utjämning av arbetsbelastning. När den här inställningen är aktiverad visas Planerade timmar för både uppgifter och projekt i området Ej tilldelat arbete i Utjämning av arbetsbelastning.

Före den här ändringen uppdaterades endast information i området Tilldelad arbetsyta i Utjämnaren.

Mer information om hur du navigerar i arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (eller om du använder Adobe Workfront Classic, se [Navigera i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/home).)

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Den nya Adobe Workfront-upplevelsen (tidigare endast för uppgifter)

## Ny inställningsruta för belastningsutjämnaren

För att effektivisera din upplevelse finns nu en inställningsruta som visar ytterligare verktyg för att uppdatera vyn i belastningsutjämnaren. Den här rutan innehåller följande inställningar:

* Gruppera efter projekt
* Visa antingen Allokerade timmar eller Återstående timmar för dina aktiviteter och projekt.

Mer information om hur du visar information i arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (eller om du använder Adobe Workfront Classic, se [Navigera i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/home).)

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Dela arbetsbelastningsutjämnaren med en länk

Nu kan du dela personalens arbetsbörda med chefer så att de kan få en kontext om personalens behov. För detta kan du nu dela arbetsbelastningsutjämnaren genom att dela en unik URL till arbetsbelastningsutjämnaren med någon annan.

Mer information om hur du navigerar i arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (eller om du använder Adobe Workfront Classic, se [Navigera i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Ändra datumintervallet i Utjämning av arbetsbelastning

För att ytterligare hjälpa dig att anpassa tidslinjens varaktighet för belastningsutjämnaren så att den passar dina behov kan du nu välja en anpassad period på 2, 4 eller 6 veckor att visa samtidigt.

Före den här förbättringen visas alltid information om arbetsbelastningsutjämnaren med början i den aktuella veckan.

Mer information om hur du navigerar i arbetsbelastningsutjämnaren finns i [Navigera i arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (eller om du använder Adobe Workfront Classic, se [Navigera i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Den nya Adobe Workfront-upplevelsen (tidigare)

## När du flyttar och kopierar uppgifter till ett annat projekt behålls uppgiftsbegränsningen när uppgifterna får plats inom projektets tidslinje

Vi har förbättrat sättet som Workfront hanterar den datumspecifika uppgiftsbegränsningen för en uppgift när du kopierar uppgiften eller flyttar den till ett annat projekt. Exempel på datumspecifika aktivitetsbegränsningar är Måste starta, Måste sluta på, Fasta datum, Starta inte senare än och så vidare.

Om du till exempel flyttar eller kopierar en uppgift med en must Start On-begränsning till ett annat projekt vars planerade startdatum är före startdatumet för aktiviteten, behåller aktiviteten villkoret när den har kopierats eller flyttats. När du flyttar eller kopierar en uppgift med en must Start On-begränsning till ett projekt vars planerade startdatum är efter startdatumet för aktiviteten, ändras aktivitetsbegränsningen till Så snart som möjligt.

Före den här ändringen ändras alltid aktivitetsbegränsningen till Så snart som möjligt.

Mer information om hur du flyttar uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md) (eller om du använder Adobe Workfront Classic, se [Flytta uppgifter](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

Information om hur du kopierar uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (eller om du använder Adobe Workfront Classic, se [Kopiera och duplicera uppgifter](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

En översikt över alla aktivitetsbegränsningar finns i [Översikt över aktivitetsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (eller om du använder Adobe Workfront Classic, se [Översikt över aktivitetsbegränsning](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Förhindra dataförlust vid ändringar på fliken Detaljer eller i en uppgiftslista

För att förhindra dataförlust när du uppdaterar information på detaljsidan för ett objekt eller uppgifter i en uppgiftslista på projektnivå när du sparar ändringar manuellt, visas ett varningsmeddelande som meddelar dig om att du har osparade ändringar innan du försöker redigera information i rubriken. De enda åtgärder som är tillåtna innan du sparar ändringarna är att prenumerera eller lägga till objektet i dina favoriter.

Mer information om hur du redigerar uppgifter i en lista finns i [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Tillgängligt i dessa miljöer:**

* Nya Adobe Workfront

## Skapa godkännandeprocesser för grupper med anpassade statusvärden

För att göra det enklare för grupper att hantera sina egna unika arbetsflöden kan du nu använda gruppspecifika anpassade statusvärden i godkännandeprocesser.

Tidigare kunde en grupp inte använda sina egna anpassade statusvärden med sina gruppspecifika godkännandeprocesser. Det fanns bara systemomfattande statusar tillgängliga och dessa passade inte alltid in i gruppens godkännandeprocesser.

Anpassade statusvärden kan nu användas både i enstaka och i systemomfattande godkännandeprocesser:

* Skapa en godkännandeprocess för ett objekt (projekt, uppgift eller utgåva) och basera den på statusvärden som är kopplade till gruppen som arbetar med objektet. Detta inkluderar alla anpassade statusvärden som är associerade med gruppen.
* Skapa en global godkännandeprocess och gör den tillgänglig endast för gruppen eller för alla i systemet.

För användare med administrativ åtkomst till godkännandeprocesser finns information om hur du konfigurerar godkännandeprocesser i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (eller om du använder Adobe Workfront Classic, se [Skapa godkännandeprocesser](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

Information om hur du associerar godkännandeprocesser med arbetsobjekt finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (eller om du använder Adobe Workfront Classic, se [Associera en ny eller befintlig godkännandeprocess med arbete](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Ett bekvämare sätt att uppdatera allokeringar i arbetsbelastningsutjämnaren

För att göra det enklare att hantera en användares tilldelningar till en arbetsuppgift i Utjämning av arbetsbelastning kan du nu dubbelklicka på arbetsposten. Du kan även använda menyalternativet Redigera allokeringar. Dessutom behöver du inte längre aktivera displaying-allokeringar för att kunna uppdatera dem.

Mer information om hur du hanterar allokeringar i belastningsutjämnaren finns i [Hantera användarallokeringar i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Uppdatera aktivitetsplanerade timmar i arbetsbelastningsutjämnaren

>[!NOTE]
>
>Den här förbättringen kommer att vara tillgänglig i produktionen strax efter version 2020.2.

Ett nytt alternativ i området Resurshantering på åtkomstnivån ger nu användare med den här åtkomsten möjlighet att redigera Planerade timmar från belastningsutjämnaren. När du justerar allokeringar i belastningsutjämnaren behöver den totala dagliga allokeringen inte matcha antalet planerade timmar för aktiviteterna. När du har sparat dina allokeringar blir det totala antalet allokeringstimmar antalet planerade timmar för uppgiften. Detta är bara möjligt för aktiviteter som har en enkel varaktighetstyp.

Mer information om hur du hanterar allokeringar i belastningsutjämnaren finns i [Hantera användarallokeringar i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Mer information om hur du beviljar åtkomst till resurshantering finns i [Bevilja åtkomst till resurshantering](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Ta bort betaetiketten från arbetsbelastningsutjämnaren

I version 2020.2 är arbetsbelastningsutjämnaren inte längre i betaversion och du kan använda resursutjämnaren för att granska och hantera resurstilldelningar och allokeringar. Betaetiketten har tagits bort i förhandsvisningsmiljön. Samma ändring kommer att göras i 20.2-utgåvan. Mer information om arbetsbelastningsutjämnaren finns i [Översikt över arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

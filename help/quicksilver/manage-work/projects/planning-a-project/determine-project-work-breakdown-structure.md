---
product-area: projects
navigation-topic: plan-a-project
title: Bestämma struktur för arbetsfördelning i ett projekt
description: Att definiera en struktur för arbetsfördelning (WBS) för ett projekt är en uppsättning aktiviteter som i slutänden anger projektplanen. Strukturen delar upp projektresultatet i hanterbara arbetselement som kan användas för att definiera milstolpar och organisera arbetsuppgifterna.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 0%

---

# Bestämma struktur för arbetsfördelning i ett projekt

Att definiera en struktur för arbetsfördelning (WBS) för ett projekt är en uppsättning aktiviteter som i slutänden anger projektplanen. Strukturen delar upp projektresultatet i hanterbara arbetselement som kan användas för att definiera milstolpar och organisera arbetsuppgifterna.

Du måste ha en planlicens med Redigera-åtkomst till projekt för att kunna skapa arbetsfördelningsstrukturen för ett projekt. Ytterligare åtkomst till andra delar av Adobe Workfront kan behövas, beroende på hur många aktiviteter du utför när du skapar strukturen.

Vi rekommenderar att du håller projektet i planeringsstatus samtidigt som du ändrar arbetsgruppsstrukturen, så att du inte får meddelanden om att utlösa för användare i projektgruppen.

## Definiera projektslutprodukterna

Syftet med ett projekt är att ge konkreta resultat till interna och externa intressenter. Resultatet av ett projekt är de resultat du vill uppnå genom att slutföra projektet. Resultatet är nästan alltid kopplat till minst en slutprodukt, och alla slutprodukter ska kopplas till ett projekt.

Projektleveranser kan vara konsumentvaror, intellektuella utdata (t.ex. rapporter) eller tjänster. Om ditt projekt till exempel ska bygga ett hus kan vissa av slutprodukterna omfatta:

* skapa arkitektoniska planer
* slutföra rörmokeri
* elarbete
* genom att sudda ut grunden
* ramverk
* att stänga försäljningen av hemmet.

Beroende på projektets storlek och omfattning kan det bestå av flera produkter.

När du har identifierat dina produkter kan du börja dela upp dem i olika uppgifter. Uppgifter är de utdata som du uppnår för att leverera det övergripande resultatet för projektet. När du definierar dina uppgifter ska du ta hänsyn till följande parametrar:

* Tidsåtgång för slutförande.
* Budget som krävs för att slutföra arbetet.
* Nödvändiga resurser krävs för att slutföra arbetet.
* Schemaläggning av resurser baserat på aktiviteternas logiska tidslinje.

När du definierar uppgifter ska du se till att du inte planerar för mycket arbete för en enskild uppgift. Om det arbete som krävs för en uppgift är längre än 40 timmar (en vanlig arbetsvecka) kan du behöva dela upp mängden arbete i underaktiviteter. Alla underaktiviteter slutförs sedan i huvuduppgiften.

Om du vill definiera strukturresultat och slutprodukter i Workfront rekommenderar vi att du utför följande aktiviteter för att skapa en hierarkisk vy över projektuppgifter:

* Om du inte redan har gjort det skapar du ett nytt projekt.\
  Mer information om hur du skapar ett projekt finns i artikeln [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

* Skapa uppgifter för alla åtgärdsobjekt som krävs för att slutföra varje resultat och slutprodukt.\
  Mer information om hur du skapar uppgifter finns i artikeln [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* Identifiera vilka som är de viktigaste resultaten av de uppgifter du just har skapat och koppla dem till milstolparna.\
  Mer information om hur du skapar milstolpeuppgifter finns i artiklarna [Skapa en milstolpe-bana](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) och [Koppla milstolpar till uppgifter](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Dela upp uppgifter med för stort omfång i underaktiviteter. Koppla dem till den överordnade som definierar din slutprodukt.\
  Mer information om hur du skapar underaktiviteter finns i artikeln [Skapa underaktiviteter](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identifiera beroendeförhållanden mellan underaktiviteter och mellan milstolpar.\
  I en beroenderelation är starten av en uppgift beroende av att en annan uppgift eller grupp av uppgifter har slutförts.\
  Mer information om uppgiftsberoenden finns i artiklarna [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) och [Skapa en föregående relation i uppgiftslistan](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Fastställ om det behövs godkännanden och granskningar under projektets livstid. Skapa godkännandeprocesser som tillgodoser detta behov.\
  Mer information om godkännanden finns i artikeln [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Beräkna arbetsscheman och schemaläggningsbegränsningar

När du har skapat den grundläggande milstolpen och uppgiftsstrukturen för projektet kan du beräkna hur lång tid det tar att slutföra det övergripande projektet genom att definiera begränsningar och varaktigheter för aktiviteten.

Tänk på följande:

* Uppgiftsbegränsningar definierar när arbete med en uppgift måste påbörjas eller avslutas.

  Mer information om hur du definierar uppgiftsbegränsningar finns i artikeln [Översikt över uppgiftsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* En uppgifts varaktighet är den tidsram som är tillgänglig för att slutföra en uppgift. När du beräknar Varaktighet kanske du vill ange ett värde som tar hänsyn till möjligheten till en fördröjning. Om liknande projekt har slutförts tidigare kan det vara bra att ange det här värdet.

  Eftersom varaktighet är en uppskattning bör du se till att fastställa optimistiska tidsvärden för att ta hänsyn till faktorer som kan påverka uppgiften, t.ex. väder, strömavbrott, leverantörssvårigheter eller andra oförutsedda händelser. Se även till att du tar hänsyn till om det finns några associerade föregående- eller beroendeuppgifter och hur de kan placera begränsningar i arbetet och påverka slutförandet av uppgifter.

  Beroende på aktivitetens varaktighetstyp kan du ändra varaktigheten för en aktivitet under ett projekts livstid, men detta påverkar även tidslinjen för projektet. Mer information om varaktigheten för en uppgift finns i artikeln [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Tilldela uppgifter

När du har definierat varaktigheten och begränsningarna för varje uppgift kan du bestämma vem som har tid och kompetens att utföra arbetet. Du kan tilldela uppgifter till följande enheter i Workfront:

* Användare\
  Endast användare med en planerings- eller arbetaråtkomstnivå kan tilldelas aktiviteter. Även om du kan tilldela uppgifter till beställare och granskare kan de inte slutföra dem. Därför rekommenderar vi inte att du tilldelar dem uppgifter.

  Mer information om åtkomstnivåer och hur de definierar vad användare kan göra med Workfront-objekt finns i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Jobbroller
* Team

Mer information om hur du tilldelar uppgifter finns i artiklarna i [Tilldela uppgifter](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) -avsnitt.

## Hantera resurser

Med Resurshantering i Workfront kan du avgöra om det finns tillräckligt med personal för att slutföra projektet. När användare läggs till i ett projekt visar Workfront hur varje användare används. Resurshanterare kan se det totala antalet timmar som personen tilldelas till andra projekt under projektets tidsram.

>[!NOTE]
>
>Så länge projektet har statusen Planering visas inte uppgifter som tilldelats användare i deras uppgiftslistor.

I början av ett räkenskapsår eller ett kvartal kanske du vill hantera dina resurser på en högre nivå, i flera projekt, utan att du behöver känna till någon särskild arbetsfördelningsstruktur.\
Mer information om hur du planerar att använda dina resurser på en högre nivå finns i artikeln [Kom igång med resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

När du hanterar dina resurser i samband med att du skapar arbetsfördelningsstrukturen för ett projekt och ser till att varje uppgift tilldelas rätt resurs, är du redo att schemalägga dina resurser för det arbete som behöver utföras.\
Mer information om hur du schemalägger resurser finns i artiklarna i [Utjämning av arbetsbelastning: artikelindex](../../../resource-mgmt/workload-balancer/workload-balancer.md) -avsnitt.

## Uppskatta projektekonomi

Workfront beräknar de planerade kostnaderna för varje uppgift och de totala kostnaderna för ett projekt. Planerade kostnader för en aktivitet inkluderar alla utgifter för aktiviteten plus kostnaden för medarbetaren eller rollen som tilldelats uppgiften. Timtaxor för uppgiften, rollen och medarbetaren tilldelas när uppgiften, rollen och användaren skapas.

Mer information om projektets ekonomi finns i avsnittet [Projektekonomi: artikelindex](../../../manage-work/projects/project-finances/project-finances-overview.md).

## Fastställa godkännandepunkter för projektet

Genom att skapa godkännandeprocesser i Workfront kan du skapa granskningspunkter för projektet för att övervaka förloppet och eventuella problemområden. Genom godkännandeprocessen kan projektägarna identifiera vilka uppgifter som är sena och tidiga, visa granskningsspår med en lista över vilka som ändrat en aktivitetsstatus och se historik över problem, inklusive hur problem löstes och när de stängdes. När du granskar ett projekt kan projektägaren avgöra vilka steg som ska vidtas och uppdatera projektplanen, om det behövs.

Mer information om godkännanden finns i artikeln [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Visa din struktur

Om du vill veta mer om strukturen för ett projekt vill du visa följande uppgiftselement:

* Aktivitetssekvens och tidslinje (Planerade start- och slutförandedatum och aktivitetsvaraktighet)
* Föregående beroenden
* Underordnad och överordnad relation
* Uppdrag

När du är klar med strukturlistan kan du visa den i en uppgiftslista på projektnivå eller i en rapport.

* [Visa strukturlistan i en uppgiftslista](#view-the-wbs-in-a-task-list)
* [Visa strukturlistan i en uppgiftsrapport](#view-the-wbs-in-a-task-report)

### Visa strukturlistan i en uppgiftslista {#view-the-wbs-in-a-task-list}

Du kan visa uppgiftslistan på projektnivå.

1. Gå till det projekt som du vill visa strukturen för arbetsfördelning för.
1. Välj **Uppgifter** -fliken.
1. (Valfritt) Välj **Ingenting** i **Gruppering** listruta.

   Arbetsfördelningsstrukturen visar inte indraget för uppgifterna i strukturen.

1. Från **Visa** och väljer **Arbetsfördelning** vy.

   Arbetsfördelningsstrukturen visas i den andra kolumnen i den valda vyn.

   ![Arbetsgruppsstruktur i en uppgiftslista](assets/work-breakdown-structure.png)

### Visa strukturlistan i en uppgiftsrapport {#view-the-wbs-in-a-task-report}

Du kan skapa en uppgiftsrapport och visa strukturlistan för uppgifterna genom att göra något av följande:

* Använd den befintliga vyn Arbetsfördelningsstruktur på rapporten.
* Lägg till kolumnen Arbetsgruppsstruktur till en anpassad rapport.

>[!TIP]
>
>Vi rekommenderar att du lägger till en projektgruppering för att förtydliga vilka projekt som aktiviteterna tillhör. Indraget för aktiviteterna visas inte i en aktivitetsrapport.

Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Spara strukturen för ett projekt som en mall

Om du arbetar med andra projekt som följer arbetsscheman som liknar den struktur du just skapade, kanske du vill spara projektet som en mall. En mall sparar tid och arbete när du skapar framtida relaterade projekt.

Om din organisation har liten omsättning kan du vänta tills användartilldelningar har gjorts för att spara mallen. Oavsett när ett projekt sparas som en mall kan användartilldelningar eller specifika uppgifter tas bort när mallen bifogas till ett nytt projekt.

Följande element i en arbetsgruppsstruktur kan sparas i en mall för framtida bruk med ett annat projekt:

* Föregående beroenden
* Uppdrag (inklusive projektägare, sponsor och resurshanterare)
* Godkännandeprocesser
* Aktivitetsbegränsningar
* Dokument
* Utgifter och annan ekonomisk information
* Mål
* Timtyper
* Begäranköstruktur
* Påminnelsemeddelanden
* Risker
* Faktureringstaxor
* Dela information
* Anpassad Forms

Mer information om hur du sparar projekt som mallar finns i artikeln [Skapa mall från projekt](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .

---
product-area: projects
navigation-topic: plan-a-project
title: Planera ett projekt - översikt
description: Ett projekt är en stor arbetsuppgift i Adobe Workfront. Du kan dela upp ett projekt i uppgifter som är mindre arbetsobjekt. Uppgifter kan tilldelas användare eller team som ansvarar för att de slutförs. När alla användare har slutfört sina uppgifter blir projektet också färdigt.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: 23372e16-3933-445d-977c-901f52299cb2
source-git-commit: aa3645e2ed8c36a3b07caad72083a43467889fce
workflow-type: tm+mt
source-wordcount: '1672'
ht-degree: 0%

---

# Planera en projektöversikt

<!--Audited: 12/2025-->

<!--
< see if you need to add something about approval settings, issue for ad-hoc happenings and how to work with documents??-->

<!--this article is linked to the ESM area in the UI; the ESM team on the Adobe side linked to this article for their -->

Ett projekt är en stor arbetsuppgift i Adobe Workfront. Du kan dela upp ett projekt i uppgifter som är mindre arbetsobjekt. Uppgifter kan tilldelas användare eller team som ansvarar för att de slutförs. När alla användare har slutfört sina uppgifter blir projektet också färdigt.

Förutom att planera dina uppgifter i ett projekt, finns det många andra detaljer att tänka på. Det finns många projektdelar som behöver uppmärksammas, från att fastställa de ekonomiska effekterna till att överväga resurstillgänglighet.

## Skapa ett projektomfång

Projektplanering innebär att exakt fastställa vilka huvudmål du måste uppnå för att slutföra projektet.

I de inledande faserna av ett projekt har du kanske inte bestämt om du ska genomföra projektet än. Det kanske inte är kostnadseffektivt eller så har du inte resurserna. I det här skedet av planeringen kan du skapa ett projekt i Workfront utan att lägga till några uppgifter och ange planeringens status.

Du kan också skicka in en projektförfrågan och fråga Portfolio Manager om det går att skapa projektet över huvud taget. På så sätt kan du skicka in ett affärsärende för projektet där du kan uppskatta vad som behövs för att slutföra projektet. Detta skapar ett projekt med statusen Begärt.

Mer information om hur du skapar ett projekt finns i artikeln [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

Mer information om hur du skapar en projektförfrågan finns i [Begär ett projekt](/help/quicksilver/manage-work/projects/create-projects/request-project.md).

Tänk på följande innan du planerar ett projekt:

* Vilka mål är obligatoriska och vilka är frivilliga?
* Har ni tillräckligt med tid för att uppnå alla eller endast de centrala målen?
* Har ni tillräckligt med budget för att uppnå alla mål nu?

Med Business Case för ett projekt kan du definiera dina mål och se till att projektet är i linje med organisationens strategi.

Mer information om hur du definierar ett affärsärende för ett projekt finns i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

När du har definierat projektets övergripande omfattning kan du sedan bestämma om du vill genomföra projektet överhuvudtaget och börja planera det.

## Preliminär projektplanering

* [Definiera projektets start- och slutförandedatum](#define-the-start-and-completion-date-of-the-project)
* [Definiera projektschemat](#define-the-project-schedule)
* [Hantera ytterligare information som behövs för att planera projektet](#manage-additional-information-needed-for-planning-the-project)

### Definiera start- och slutdatum för projektet {#define-the-start-and-completion-date-of-the-project}

När du planerar ett projekt är det första du måste bestämma tidslinjen: bestämma när projektet kan starta och efter vilken tid det måste slutföras.

Bestäm om det finns en fast tidsgräns för när projektet måste vara färdigt eller om du ska ange en startpunkt och arbeta därifrån.

Du kan schemalägga ett projekt från ett startdatum, eller så kan du schemalägga det från datumet för slutförandet. Du kan ange det här attributet när du skapar projektet och du kan när som helst ändra det genom att redigera projektet.

Mer information finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

### Definiera projektschemat {#define-the-project-schedule}

Du måste bestämma ett schema och associera det med projektet samt med de användare som ansvarar för att slutföra uppgifterna i projektet.

Ett schema anger vilken tid användarna har tid att arbeta med projektet.

Överväg att definiera följande i ett schema:

* Helgdagar
* Ledig tid
* Antal tillgängliga timmar för arbete under en dag eller vecka

Det är viktigt att veta när användare är tillgängliga att arbeta när du vill förstå hur dina uppgifter fortskrider i projektet.

Du kan skapa flera scheman i din Workfront-instans och använda ett standardschema som ska användas för alla projekt. Du kan också skapa ytterligare anpassade scheman för att associera dem med olika personer.

Mer information om scheman finns i artikeln [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Bygg projekttidslinjen

När du har fastställt de viktigaste målen för ett projekt och du har beslutat att projektet är värt att eftersträva, bör du beräkna tidslinjen för varje mål. Varje mål kan bli en av dina uppgifter i projektet.

Detta hjälper dig att prioritera dina mål och planera arbetsfördelningsstrukturen utifrån detta. Arbetsfördelningsstrukturen definierar tidslinjen för projektet.\
Mer information om hur du skapar aktiviteter i ett projekt finns i avsnittet [Definiera uppgifter](#define-tasks) i den här artikeln.

Tänk på följande när du skapar tidslinjen för projektet:

* Dela upp större mål i underordnade uppgifter och definiera deras Start- och slutdatum.
* Tilldela uppgifter till enskilda personer eller team så att ni vet vem som ansvarar för att de slutförs. Du kan tilldela uppgifter till jobbroller, men bara för den inledande planeringsfasen av projektet, när du inte är helt säker på vem som kan tilldelas till aktiviteterna. När du har startat projektet är det bättre att ersätta jobbrollerna med användar- eller teamtilldelningar.
* Bestäm om dina mål är beroende av andra mål.

  Du kan ställa in dessa beroenden som föregångare.

  Du kan till exempel ha ett projekt för att bygga en lägenhetsbyggnad. Ett av era mål är rörmokningen och ett annat är att lägga grunden. En av dina rörmokningsuppgifter är att koppla upp dig till vattenlinjen i huvudstaden, och detta måste göras innan du lägger grunden. De flesta av dina andra rörmokningsuppgifter kan dock inte utföras förrän efter att grunden lagts. I det här fallet bör du överväga att använda föregångare för att förstå när ett mål kan börja efter att dess förutsättning är klar.

  När du använder överordnade uppgifter för att ordna mål kan du skapa en uppgift för varje viktigt mål och lägga till underuppgifter när du kommer till steget att dela upp viktiga mål i enskilda uppgifter. Detta håller de uppgifter som är en del av målet organiserade i projektet.

  Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Tänk på de viktigaste målen för projektet och flagga dem som milstolpar.

  Vi rekommenderar att du använder överordnade uppgifter som milstolpar.

  Mer information om hur du använder milstolpeuppgifter finns i [Skapa en milstolpebana](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Definiera en tidslinje för varje mål. Om du arbetar med överordnade uppgifter måste varje underordnad uppgift ha ett definierat Start- och Slutförandedatum. Tiden mellan det tidigaste startdatumet för en aktivitet och det senaste slutförandedatumet för en aktivitet i samma projekt resulterar i projekttidslinjen.

## Definiera uppgifter {#define-tasks}

När du definierar målen för projektet och de uppgifter som är kopplade till dem skapar du tidslinjen för projektet.

Du kan skapa uppgifter i ett projekt på följande sätt:

* Lägg till uppgifter i ett projekt manuellt när du infogar en uppgiftslista i projektet.
* Använd en mall med definierade malluppgifter och lägg till den i projektet.

  Malluppgifterna blir projektets uppgifter.

  Mer information om hur du skapar uppgifter finns i artikeln [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Tänk på följande när du definierar uppgifter:

* Definiera tidslinjen för varje uppgift. Detta hämtas i fältet Varaktighet för varje uppgift.

  Mer information om aktivitetens varaktighet finns i artikeln [Översikt över aktivitetens varaktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Definiera relationen mellan de överordnade och underordnade aktiviteterna.
* Definiera föregående relation mellan aktiviteterna.
* Koppla en milstolpe-sökväg till projektet och associera en milstolpe med dess respektive uppgift.

  Mer information om hur du använder milstolpeuppgifter finns i artikeln [Skapa en milstolpebana](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Definiera mängden arbete som behövs för att slutföra varje uppgift. Detta visas i fältet Planerade timmar för varje uppgift.

  Mer information om planerade timmar finns i artikeln [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

* Tilldela varje uppgift till en användare eller ett team som ansvarar för att slutföra den.
* Kontrollera tillgängligheten för de användare som du tilldelar uppgifterna. Se till att de är lediga och inte överallokerade så att de kan slutföra sina tilldelade uppgifter. Om användarna är överallokerade eller om de har tid över i sina scheman, bör du tänka på något av följande:

   * Minska antalet planerade timmar för varje uppgift.
   * Lägg till fler användare i en uppgift för att se till att den kan slutföras under den tilldelade tiden.
   * Tilldela om uppgifterna till användare som inte har några andra begränsningar.\
     Mer information om planering av projektresurser finns i artikeln [Resursplanering: artikelindex](../../../resource-mgmt/resource-planning/resource-planning-overview.md).\
     Mer information om hur du schemalägger resurser för att utföra arbetet i ett projekt finns i [Översikt över belastningsutjämning](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Hantera ytterligare information som behövs för att planera projektet {#manage-additional-information-needed-for-planning-the-project}

När du planerar ett projekt finns det ytterligare information som måste ställas in innan du kan börja arbeta med projektet.

Du kan ställa följande frågor:

* Finns det någon förordning som föreskriver att ni ska registrera händelser och processer? Om så är fallet, vad behöver du spåra?

  Med Workfront kan du registrera ändringar, omfångsändringar, statusändringar och åtgärder så att du kan följa branschspecifika regler.\
  Mer information om hur du definierar vilka uppdateringar som ska spåras i Workfront finns i artikeln [Systemspårade uppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* Är det någon information som du måste spåra som inte har något fält i Workfront att lagra det i?

  Om ja, skapar du Anpassad Forms för projekt eller uppgifter där du kan lagra den här informationen.

  Mer information om hur du skapar anpassade formulär finns i artikeln [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Måste du dokumentera processer och arbeta med resurser som antingen är en del av det dagliga arbetet eller avgöra vilken lösning projektet har? Om ja, skapa ett system för lagring av dokument.

  Mer information finns i [Dokument: artikelindex](/help/quicksilver/documents/documents-overview.md).

* Finns det några kontrollpunkter för godkännande som måste beviljas innan arbetet med ett projekt kan fortsätta? Om ja, skapar du godkännandeprocesser för projekt eller uppgifter som du kan använda när du skapar ditt projekt och inventerar vilka dokument eller korrektur som måste godkännas innan arbetet kan fortsätta.

  Mer information om godkännanden finns i följande artiklar:

   * [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Granska och godkänn arbetet](/help/quicksilver/review-and-approve-work/review-and-approve-work.md)
   * [Tillgängliga funktioner för dokumentgodkännanden](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)

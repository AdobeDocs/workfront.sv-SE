---
title: 22.2&nbsp;Projektförbättringar
description: 22.2&nbsp;Projektförbättringar
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# 2.2 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 2.2 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

den 4 april 2022. En lista över alla ändringar som är tillgängliga i version 2.2 finns i [22.2 Versionsöversikt](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront Boards finns nu att köpa!

Styrelserna är flexibla verktyg som ger teamsamarbete genom att ge åtkomst till en delad anslagstavla som innehåller kolumner och kort.

Med anslagstavlor kan du:

* Konfigurera snabbt en arbetsyta med flera kolumner
* Konfigurera kolumner för att visa status eller kategori
* Lägg till andra användare på styrelsen och tilldela dem till kort
* Lägg snabbt till öppna färdiga kort och checklistor

Observera att korten på ritytan inte är kopplade till objekt och arbetsobjekt i Adobe Workfront.

En systemadministratör måste aktivera anslagstavlor i layoutmallar för att göra alternativet tillgängligt för alla användare på huvudmenyn.

Mer information finns i [Översikt över styrelser](../../../agile/boards-overview.md).

## Ytterligare förbättringar i Workfront Boards

Följande ytterligare förbättringar är nu tillgängliga för Workfront Boards:

* Tagga kort på anslagstavlor

   Nu kan du kategorisera kort på din anslagstavla med färgkodade taggar. Med taggar kan du snabbt identifiera kort. Du kan till och med sortera din anslagstavla baserat på märkord.

* Hantera kort på anslagstavlor

   Vi har lagt till följande funktioner som hjälper dig att hantera kort på din bräda:

   * Kopiera ett kort: Skapa en kopia av ett befintligt kort på din bräda.
   * Flytta ett kort: Flytta snabbt kort till antingen överkanten eller nederkanten av en rityta med de nya alternativen i överkanten av kolumnen och underkanten av kolumnmenyn.

* Sök på anslagstavlor

   Vi har lagt till ett sökfält som hjälper dig att söka efter alla kort på din anslagstavla.

* Ange ett förfallodatum för ett kort på en anslagstavla

   Du kan nu ange ett förfallodatum för enskilda kort på din bräda.

Mer information finns i [Kom igång med anslagstavlor i Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Ångra-alternativ för Uppdatera inlägg

Det är nu enklare att fånga upp misstag när en uppdatering publiceras. När du slutför en kommentar på objektets uppdateringsflik skapas nu ett popup-fönster i 7 sekunder som gör att du kan avbryta inlägget och återgå till redigering - innan systemet tidsstämplar det eller skickar e-postmeddelanden och meddelanden i programmet. Om du stänger popup-fönstret, lämnar sidan eller väntar i 7 sekunder på att fönstret ska timeout, kommer inlägget att göras normalt.

Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Uppdaterad upplevelse vid kopiering och flyttning av problem

För att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen har vi omdesignat gränssnittet för att kopiera och flytta problem. Detta är för närvarande tillgängligt när du kopierar eller flyttar ett enstaka problem eller när du kopierar eller flyttar flera utgåvor samtidigt från en lista eller rapport.

Några av förbättringarna i det nya gränssnittet:

* All information som du måste uppdatera innan flytten visas på en kontinuerlig sida.
* Workfront kontrollerar om du har åtkomst till målprojektet direkt efter att du har valt projektet. Före den här förbättringen varnade Workfront dig för att du inte har rätt åtkomst efter att du har bekräftat flytten som resulterade i extra steg och flytten inte tillåts.
* Möjlighet att begära åtkomst till ett projekt där du vill flytta problemen utan att lämna rutan Flytta uppgift.
* Möjlighet att ta bort objekt (uppdrag, förlopp, dokument, behörigheter, uppdateringar) från ett problem när du flyttar det till en annan plats. Den här funktionen var tidigare endast tillgänglig för kopieringsproblem.
* Möjlighet att välja en måluppgift utöver att välja ett målprojekt när du kopierar ett problem.

Mer information om hur du flyttar eller kopierar problem finns i följande artiklar:

* [Kopiera problem](../../../manage-work/issues/manage-issues/copy-issues.md)
* [Flytta problem](../../../manage-work/issues/manage-issues/move-issues.md)

## Ny upplevelse när du kopierar ett projekt

För att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen har vi omdesignat gränssnittet för att kopiera projekt. Detta är för närvarande tillgängligt när du kopierar ett projekt från projektsidan eller när du kopierar ett projekt från en lista eller rapport. Före den här uppdateringen kunde du bara kopiera ett projekt från projektsidan.

Mer information finns i [Kopiera ett projekt](../../../manage-work/projects/manage-projects/copy-project.md).

## Möjlighet att hantera projekt från listor och rapporter via en ny Mer-meny

Vi har lagt till en ny Mer-meny i projektlistor och rapporter så att du kan utföra följande åtgärder från dessa områden:

* För flera projekt i taget:
* Beräkna om tidslinje
* Beräkna om ekonomi
* Beräkna om anpassade uttryck
* För ett enskilt projekt:
* Bifoga mall
* Exportera till MS-projekt
* Prenumerera

Mer information finns i följande artiklar:

* [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [Beräkna om projektekonomi](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [Redigera information i anpassade formulärfält](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [Bifoga en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Exportera ett projekt till Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Prenumerera på objekt i Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Håll användarna på kontrollpanelen, i listan eller i rapporten efter att ha konverterat ett problem till ett projekt

För att öka effektiviteten och eliminera antalet klick har vi släppt en förbättring när vi konverterar problem till projekt från en lista, rapport eller kontrollpanel.

Användarna finns kvar på listan, rapporten eller kontrollpanelen efter att ha konverterat ett problem till ett projekt i stället för att omdirigeras till projektets sida. Ett meddelande om att projektet lyckades med länken till projektet visas när konverteringen är klar, så att du enkelt kan navigera till projektet, om det behövs.

Mer information finns i [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Allokeringstider tas inte längre bort när du ändrar tilldelningar

>[!NOTE]
>
>Den här funktionen var ursprungligen planerad att lanseras med version 22.2. Den släpps till produktion den 21 april 2022.

För att dina data ska bli korrekta har vi gjort en ändring som bevarar tilldelningstimmar och behåller planerad tid för aktiviteten oförändrad när du ändrar tilldelningar för aktiviteten.

Följande ändringar har gjorts för aktiviteter med en enkel varaktighetstyp:

* Planerade timmar bevaras när alla tilldelningar tas bort.
* Enskilda tilldelningar bevaras när användare och roller ersätts.
* Enskilda tilldelningar bevaras för rollen när användaren tas bort. (Borttagen från release. Planerade timmar anges till 0 när alla tilldelningar har tagits bort.)

Mer information om planerade timmar finns i [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

## Dela mappar endast på de fem översta nivåerna i en mapphierarki

>[!NOTE]
>
>Den här funktionen är inte tillgänglig för tillfället. Vi uppdaterar den här versionsinformationen när funktionen är tillgänglig i produktionen.

För att säkerställa bästa prestanda för användare som delar mappar begränsar vi för närvarande delningen till de fem högsta nivåerna i en mapphierarki på ett objekt.

Varje mapp på sjätte nivån eller tidigare ärver sina delningskonfigurationer från mappen direkt ovanför den.

Mer information om att dela mappar finns i [Dela en dokumentmapp](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).


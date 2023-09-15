---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 1 och 2
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön med versionerna R1.1 och R1.2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 19 januari 2017.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# R1 Preview 1 och 2

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön med versionerna R1.1 och R1.2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 19 januari 2017.

En lista över alla ändringar som gjorts i R1 finns i [Aktivitetsöversikt för R1-release](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Återställ projekt, uppgifter och problem från papperskorgen 

Workfront-administratörer kan nu återställa projekt, uppgifter och ärenden som har tagits bort under de senaste 30 dagarna. All information som är kopplad till projektet, uppgiften eller problemet återställs, inklusive dokument och anpassade data.

Det finns även nya alternativ för att konfigurera vad som händer med timmar som är loggade mot ett projekt, en uppgift eller ett problem som tas bort. Mer information finns i [Konfigurera påverkan på timmar när ett objekt tas bort och återställs](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Mer information om hur du återställer objekt i Workfront finns i [Återställ borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Mer information om hur du visar projekt, uppgifter och problem som nyligen har återställts finns i [Visa återställt objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Godkännandediagram visar visuell representation av föregående, nuvarande och framtida godkännandesteg

Nu när ett godkännande av ett projekt, en uppgift eller ett problem väntar visas ett diagram. Godkännandediagrammet visar det aktuella steget i godkännandeprocessen (som väntar) och gör det även möjligt att snabbt visa föregående och framtida godkännandesteg utan att navigera till fliken Godkännanden.

Före den här ändringen var information om godkännandesteg bara tillgänglig på fliken Godkännanden i projektet, aktiviteten eller utgåvan, och den visades bara i en listvy i stället för i en diagramvy. (Informationen är fortfarande tillgänglig och oförändrad på fliken Godkännanden.)

I projekt visas godkännandeinformationen i huvudet bredvid projekttiteln. För uppgifter och ärenden visas godkännandeinformationen på den högra panelen.

Mer information finns i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Konfigurera objekt som ska uppdateras och som väntar på godkännande

När ett projekt, en uppgift eller ett problem väntar på godkännande kan du nu konfigurera om användarna ska kunna:

* Redigera det anpassade formuläret för ett projekt, en uppgift eller ett problem som väntar på godkännande.\
  Mer information om hur du konfigurerar projekt, uppgifter och utgåvor som ska redigeras när du väntar på godkännande finns i [Konfigurera globala inställningar för godkännande](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Lägg till ärenden i ett projekt som väntar på godkännande.\
  Mer information om hur du konfigurerar projekt så att användare kan lägga till problem när projektet väntar på godkännande finns i [Konfigurera systemomfattande projektinställningar](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Redigera uppgifter och ärenden i ett projekt som väntar på godkännande.\
  Mer information om hur du konfigurerar projekt så att användare kan redigera uppgifter och problem när projektet väntar på godkännande finns i [Konfigurera systemomfattande projektinställningar](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Före den här ändringen gick det inte att redigera projekt, uppgifter och utgåvor som inte hade godkänts. Det gick inte heller att lägga till problem i projekt som väntar på godkännande, och aktiviteter och ärenden kunde inte redigeras i projekt som inte hade godkänts.

## Tilldela layoutmallar till grupper

Nu kan du tilldela layoutmallar till grupper.

Före den här ändringen kan du tilldela layoutmallar till användare, team och jobbroller. Om du tilldelar en layoutmall till grupper får du den lägsta prioriteten i tilldelningsprioriteten för layoutmallar. 

Mer information finns i&quot;Skapa och hantera layoutmallar&quot;.

## Ändringar av användarmeddelanden för gruppredigering

Funktionen har ändrats kring redigering av e-postaviseringsinställningar för användare i grupp. När du väljer att flera användare ska redigera sina e-postinställningar för meddelanden ändras bara de specifika meddelanden som du uppdaterar för alla markerade användare. Alla oförändrade inställningar för e-postmeddelanden förblir desamma för alla användare som har markerats, även om de inte är samma användare som användare. 

Före den här ändringen sparades de inställningar för e-postmeddelanden som du valde och alla övriga inställningar för oförändrade meddelanden avmarkerades när du sparade ändringarna. 

Mer information finns i&quot;Ändra inställningar för användarmeddelanden gruppvis&quot; i [Ändra dina egna e-postmeddelanden](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Uppdaterat utseende och känsla för flera e-postmeddelanden

Utseendet och känslan i följande e-postmeddelanden har uppdaterats med ett nytt användargränssnitt:

* Ärendetilldelning
* Genomför datumändringar
* Ett projekt som jag håller på att bli aktivt
* Godkännandebeslut för berörda parter
* En föregående uppgiftsslutförande till aktivitetsberoende
* Väntande godkännande (projekt, uppgift, utgåvor)
* Statusändring för projekt, uppgifter, problem

Kom ihåg att uppdatera e-postadressen som är kopplad till ditt konto för att kunna testa den här funktionen, eftersom e-postadresserna för alla användare rensas i sandlådan Förhandsgranska.    Mer information om e-postmeddelanden finns i [Adobe Workfront-meddelanden](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nya alternativ för e-postsammandrag för flera meddelandeområden

I följande meddelandeområden har alternativet &quot;Daglig sammanfattning&quot; lagts till:

* Information om projekt som jag är på
* Information om projekt i sponsor
* Godkännandeinformation
* Information om arbete som tilldelats mig
* Kommunikation

Mer information finns i [Adobe Workfront-meddelanden](../../../../workfront-basics/using-notifications/wf-notifications.md).  Kom ihåg att uppdatera e-postadressen som är kopplad till ditt konto för att kunna testa den här funktionen, eftersom e-postadresserna för alla användare rensas i sandlådan Förhandsgranska. 

## Gör en grupp offentlig

När du gör en grupp offentlig kan du nu lägga till den gruppen till användare utan att vara gruppägare. Du måste ha administratörsbehörighet för att kunna redigera användare.

Mer information om hur du gör en grupp offentlig finns i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) avsnitt i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Dela URL:en för ett objekt i mobilappen 

Nu kan du dela URL-adressen för följande objekt i Workfront mobilapp:

* Projekt
* Uppgifter
* Problem
* Tidrapporter
* Dokument

Du kan dela en URL för ett objekt i följande program:

* Textmeddelande
* E-post
* Lagringsenhet (till exempel iCloud-enhet)
* Ett annat installerat program (till exempel Notes, Facebook)
* Du kan kopiera en länk till objektet till Urklipp och klistra in det senare i ett annat program. 

## Sammanhangsberoende hjälp i installationsprogrammet

Alla områden på menyn Inställningar har uppdaterats med en hjälpikon i det övre högra hörnet av området. Med den här ikonen får du en länk till en artikel om hjälpwebbplatsen om det området. Vissa avsnitt i inställningsområdena har också uppdaterats med hjälpikonen. 

## Lägg till exaktare utgiftsnivåer

Nu kan du lägga till mer exakta utgiftstariffer när du skapar utgiftstyper. Utgiftsfrekvenser kan innehålla upp till 4 tecken efter decimaltecknet (till exempel 1,0375). Det innebär att alla fält som använder den här hastigheten kan vara mer exakta.

Före den här ändringen kan kostnadstarifferna endast innehålla upp till 2 tecken efter decimaltalet (till exempel 1,03).

Mer information om hur du skapar utgiftssatser finns i [Skapa anpassade utgiftstyper](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1 Preview 1 and 2 Release Webinar Recording

Det här webbinariet presenterades av Workfront Release Readiness Team den 19 januari 2017. Det här webbinariet fokuserade på releaseändringarna 2017 och innehöll nya funktioner som är tillgängliga att testa i förhandsgranskningen.

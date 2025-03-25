---
title: Vanliga frågor om projekt
description: Vanliga frågor om projekt
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Vanliga frågor om projekt

Här följer vanliga frågor om projekt.

## Varför saknas Infoga aktivitet ovan/ nedan när jag högerklickar på en uppgift i uppgiftslistan?

### Svar

Om du vill använda infogningsalternativen måste uppgiftslistan sorteras efter nummer. Om du vill sortera kolumnen efter nummer klickar du på **#** i kolumnrubriken till vänster om **Aktivitetsnamn** för att sortera om uppgiften efter nummer.

## Vad är det faktiska slutförandedatumet?

### Svar

Faktiskt slutförandedatum representerar datum och tid då arbetet är slutfört. Mer information finns i [Översikt över projektets faktiska slutförandedatum](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Varför saknas knappen Indrag/Minska indrag?

### Svar

Om du vill använda knappen Indrag/Minska indrag måste du se till att aktiviteterna sorteras efter aktivitetsnumret och att inga grupperingar används.

## Varför kan jag inte ändra projektstatus till Fullständig?

Jag får följande felmeddelande när jag försöker markera mitt projekt som färdigt:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Svar

Du kan inte ändra status för ett projekt till slutfört om du har något av följande i projektet:

* Ofullständiga uppgifter eller problem
* Aktivitet eller problem som väntar på godkännandestatus

## Varför kan jag inte ändra projektstatus från Fullständig till Aktuell?

### Svar

Om slutförandeläget är inställt på Automatiskt för projektet, när alla uppgifter och ärenden är slutförda, ändras projektets status automatiskt till Fullständigt och du kan inte ändra den till någon annan status. Slutförandeläget för projektet måste anges till Manuellt för att ett fullständigt projekt ska kunna ändras till Aktuell. Mer information finns i [Projektstatus ändras inte från Fullständigt till Aktuellt](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## Varför kan jag inte lägga till ett projekt i en Portfolio, även om jag har rätt behörighet att göra det?

Även om jag har rätt behörigheter saknas knappen Lägg till projekt på fliken Projekt i Portfolio.

### Svar

Detta beror på att Portfolio-statusen är inaktiv. Så här ändrar du status för Portfolio:

1. Klicka på **Portfolio Details > Overview**.
1. Ändra **status** till **Aktiv.**

1. Klicka på **Spara**.\
   Knappen **Lägg till projekt** bör nu visas på fliken **Projekt**.

## Vilken åtkomst får en resurshanterare när den läggs till i ett projekt?

### Svar

Resurshanterare får automatiskt Hantera åtkomst till projekt. Om användaren tas bort från resurshanterarrollen tas inte användarens hanteringsdelningsåtkomst bort.

## Varför ändras projektets status när jag lägger till en grupp?

### Svar

Projektets status ändras på grund av gruppens standardstatus. När du lägger till en grupp i ett projekt ändras statuslistan till standardstatusvärdena som angetts för gruppen.

Mer information finns i artikeln [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Vad är budgetstatus?

### Svar

Budgetstatus visar om projektet för närvarande har lagts till i kapacitetsplaneraren och om budgetberäkningen har slutförts.

Följande är budgetstatus:

* Ingår inte - projektet läggs inte till i kapacitetsplaneraren.
* Ingår, men inte beräknat - Projektet läggs till i kapacitetsplaneraren men tas inte med i budgetberäkningen.
* Inkluderad och beräknad - Projektet läggs till i kapacitetsplaneraren och inkluderas i budgetberäkningen.

## Varför kan jag inte dela ett projekt som jag är ägare till och där jag har behörigheten Hantera med ett team? Jag kan helt enkelt inte hitta teamet i delningsdialogrutan för projektet.

### Svar

Adobe Workfront-administratören har begränsat dig till att endast visa företag, grupper och team som du tillhör på din åtkomstnivå för . Teamet du letar efter är inte ett av de team du tillhör.

![Visa endast team, grupper och företag som de tillhör](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Mer information om hur du gör det möjligt för en användare att visa alla team i systemet finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

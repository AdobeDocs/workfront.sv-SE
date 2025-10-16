---
title: Översikt över granskningsloggar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du spåra användarändringar som utlösts i systemet under de senaste 90 dagarna med hjälp av granskningsloggar.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Översikt över granskningsloggar

<!--Audited: 08/2025-->

Som Adobe Workfront-administratör kan du spåra användarändringar som utlösts i systemet under de senaste 90 dagarna med hjälp av granskningsloggarna som beskrivs nedan.

Instruktioner om hur du visar och filtrerar det du vill se i dessa granskningsloggar finns i [Visa och exportera granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Information som finns i en granskningslogg

Följande fält registreras i alla poster i granskningsloggen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datum och tid</td> 
   <td>När åtgärden utfördes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Loggtyp</td> 
   <td>Typ av granskningslogg, till exempel åtkomstnivå eller anpassat formulär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Användarnamn</td> 
   <td> <p>Namnet på den användare som utförde åtgärden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärd</td> 
   <td> Åtgärder som utförs av användaren, till exempel Ändra, Skapa och Ta bort. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objekt</td> 
   <td> Namnet på det objekt som påverkas som ett resultat av åtgärden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Information</td> 
   <td>Mer information om åtgärden. För musen över texten för att läsa hela meddelandet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP-adress</td> 
   <td> <p>IP-adress till den användare som utförde åtgärden vid tidpunkten för åtgärden.</p> <p>IP-adressen är inte tillgänglig för vissa systemåtgärder.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Granskningsloggtyper och de åtgärder som utlöser dem

* [Åtkomstnivå](#access-level)
* [Affärsregler](#business-rules)
* [Företag](#company)
* [Villkor](#condition)
* [Anpassat fält](#custom-field)
* [Anpassat formulär](#custom-forms)
* [Anpassat avsnitt](#custom-section)
* [Växelkurs](#exchange-rate)
* [Grupp](#group)
* [Jobbroll](#job-role)
* [Prioritet](#priority)
* [Projektinställningar](#project-preference)
* [Allvarlighetsgrad](#severity)
* [Status](#status)
* [Inställningar för aktiviteter och ärenden](#tasks-issues-preferences)
* [Användare](#user)
<!--* [Login Attempt](#login-attempt) -->

### Åtkomstnivå {#access-level}

Systemet genererar en loggpost på åtkomstnivå när en användare utför någon av följande åtgärder:

* Skapar en åtkomstnivå
* Tar bort en åtkomstnivå
* Ändrar en åtkomstnivå:

   * Ändrar licenstypen
   * Ändrar behörigheter till projekt, uppgifter, ärenden, portfolior, program, rapporter, dokument, användare eller mallar

     >[!NOTE]
     >
     >Systemet registrerar inte några behörighetsändringar i finansiella data eller inom följande åtkomsttyper: Visa och redigera.
     >
     >Om en användare t.ex. ändrar åtkomsttypen Planering från Visa till Redigera, visas inte information i den nedrullningsbara menyn Finjustera inställningarna.

### Affärsregler

Affärsreglerna är endast tillgängliga för kunder som har köpt en Ultimate Workfront-plan. Mer information finns i [Skapa och redigera affärsregler](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Systemet genererar en loggpost för affärsregelgranskning när en användare gör något av följande:

* Skapar en affärsregel
* Redigerar en affärsregel:

   * Byter namn på den
   * Lägger till eller tar bort uttryck
   * Ändrar en utlösare

* Tar bort en affärsregel

### Företag {#company}

Systemet genererar en loggpost för företagsgranskning när en användare gör något av följande:

* Skapar ett företag
* Ändrar ett företag:

   * Byter namn på den
   * Lägger till eller tar bort medlemmar
   * Lägger till, redigerar eller tar bort värdet i fältet Grupp
   * Lägger till eller redigerar en företagsfaktureringssats för en jobbroll
   * Tar bort en företagsfaktureringsfrekvens för en jobbroll
   * Anger det som primärt företag för organisationen
   * Bifogar eller tar bort ett anpassat formulär

* Tar bort ett företag

Mer information om status finns i [Statusöversikt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Villkor {#condition}

Systemet genererar en loggpost för villkorsgranskning när en användare utför någon av följande åtgärder:

* Skapar ett villkor
* Ändrar ett villkor:

   * Ändrar namnet
   * Ändrar färgen
   * Anger det som standard
   * Ändrar eller tar bort beskrivningen av villkoret
   * Döljer eller visar villkoret

* Tar bort ett villkor

Mer information om hur du konfigurerar jobbroller finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Anpassat fält {#custom-field}

Systemet genererar en loggpost för anpassad fältgranskning när en användare utför någon av följande åtgärder:

* Skapar ett anpassat fält
* Ändrar ett anpassat fält:

   * Ändrar namn, etikett, instruktioner eller format
   * Ändrar visningstypen

     Detta är endast tillgängligt om fältet är en av följande typer: en rad, ett stycke, nedrullningsbar lista, kryssruta, alternativknapp

   * Ändrar fältstorleken

     Detta är endast tillgängligt om fältet är en av följande typer: en rad, ett stycke, text med formatering

   * Lägger till, tar bort eller döljer ett fältval
   * Redigerar en etikett eller ett värde för fältval
   * Konfigurerar fältvalet som ska markeras eller inte markeras som standard
   * Konfigurerar ett nedrullningsbart fält för att tillåta flera markeringar eller en enda markering
   * Konfigurerar ett datumfält så att det visas eller inte visas tid på dagen
   * Redigerar hyperlänken eller ändrar värdet i ett beskrivande textfält

* Tar bort ett anpassat fält
* Delar ett anpassat fält

### Eget formulär {#custom-form}

Systemet genererar en anpassad Forms-granskningsloggpost när en användare utför någon av följande åtgärder:

* Skapar ett anpassat formulär
* Ändrar ett anpassat formulär:

   * Ändrar namn eller beskrivning
   * Aktiverar eller inaktiverar Är aktiv
   * Lägger till eller tar bort ett fält eller avsnitt
   * För ett anpassat avsnitt ändrar en inställning under Ytterligare inställningar
   * Ändrar ett fält till obligatoriskt eller inte obligatoriskt
   * Ändrar en beräkning i ett anpassat fält
   * Döljer eller visar formeln som är associerad med ett beräkningsfält i hovringstexten för instruktioner
   * Aktiverar eller inaktiverar Uppdatera tidigare beräkningar
   * Lägger till eller ändrar hopplogik eller visningslogik

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Tar bort ett anpassat formulär
* Delar ett eget formulär

### Anpassat avsnitt {#custom-section}

Systemet genererar en loggpost för anpassad avsnittsgranskning när en användare gör någon av följande åtgärder i ett anpassat format:

* Skapar ett eget avsnitt
* Ändrar namnet eller beskrivningen för ett anpassat avsnitt
* Tar bort ett anpassat avsnitt

Mer information om anpassade avsnitt i anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Växelkurs {#exchange-rate}

Systemet genererar en loggpost för granskning av valutakurs när en användare utför någon av följande åtgärder:

* Skapar en valutakurs
* Ändrar en växelkurs:

   * Lägger till en valuta
   * Ändrar kursen för valutan
   * Anger valutan som basvaluta (standard) för alla projekt och rapporter i hela systemet

* Tar bort en valutakurs

Mer information om hur du konfigurerar valutakurser finns i [Konfigurera valutakurser](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Grupp {#group}

Systemet genererar en loggpost för gruppgranskning när en användare utför någon av följande åtgärder:

* Skapar en grupp
* Tar bort en grupp
* Ändrar en grupp:

   * Lägger till eller tar bort användare
   * Lägger till eller tar bort undergrupper

### s {#job-role}

Systemet genererar en loggpost för jobbrollsgranskning när en användare utför någon av följande åtgärder:

* Skapar en jobbroll
* Ändrar en jobbroll:

   * Ändrar namnet
   * Lägger till, ändrar eller tar bort beskrivningen
   * Lägger till, ändrar eller tar bort kostnaden per timme (kostnad/tim)
   * Lägger till, ändrar eller tar bort faktureringssatsen (Faktura/tim.)

* Tar bort en jobbroll

Mer information om hur du konfigurerar jobbroller finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Inloggningsförsök {#login-attempt}

Systemet genererar en inloggningsförsöksloggpost när en användare utför någon av följande åtgärder:

* Loggar in, loggar ut eller misslyckas med ett inloggningsförsök i Workfront (i en webbläsare och i mobilappen)
* Loggar in, loggar ut eller misslyckas med ett inloggningsförsök i någon Workfront-integrering (t.ex. Workfront för Slack)
* Loggar in eller loggar ut från Workfront API

Inloggningsförsöksloggar registreras inte när en Workfront-administratör använder funktionen Logga in som.

>[!NOTE]
>
>Detta är inte tillgängligt om din organisation har anslutit sig till Adobe Admin Console. Kontakta nätverks- eller IT-administratören om du behöver mer information.

### Prioritet {#priority}

Systemet genererar en post i prioritetsgranskningsloggen när en användare utför någon av följande åtgärder:

* Skapar en prioritet
* Ändrar en prioritet:

   * Ändrar namnet
   * Ändrar färgen
   * Anger det som standard
   * Lägger till, ändrar eller tar bort beskrivningen av prioriteten
   * Döljer eller visar prioriteten

* Tar bort en prioritet

Mer information om hur du konfigurerar prioriteringar finns i [Skapa och anpassa prioriteringar](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Projektinställningar {#project-preference}

Systemet genererar en granskningsloggpost för projektinställningar när en användare utför någon av följande åtgärder:

* Skapar ett eget kvartal
* Ändrar en projektinställning:

   * Låser eller låser upp den
   * Ändrar en av dess inställningar
   * Aktiverar, inaktiverar eller redigerar den
   * Redigerar en tidslinjeberäkning

* Tar bort ett anpassat kvartal

Mer information om projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Allvarlighetsgrad {#severity}

Systemet genererar en loggpost för allvarlighetsgrad när en användare utför någon av följande åtgärder:

* Skapar en allvarlighetsgrad för ett problem
* Ändrar allvarlighetsgrad för ett problem:

   * Ändrar namnet
   * Ändrar färgen
   * Anger det som standard
   * Ändrar eller tar bort beskrivningen av allvarlighetsgraden
   * Döljer eller visar allvarlighetsgraden

* Tar bort en allvarlighetsgrad för ett problem

Mer information om hur du konfigurerar jobbroller finns i [Skapa eller anpassa utgåvans svårighetsgrad](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Status {#status}

Systemet genererar en loggpost för statusgranskning när en användare utför någon av följande åtgärder:

* Skapar en status på system- eller gruppnivå
* Ändrar en status på system- eller gruppnivå:

   * Byter namn på den
   * Gör den till standardstatus
   * Låser eller låser upp den
   * Döljer eller döljer den
   * Ändrar färg eller beskrivning

* Tar bort en status på system- eller gruppnivå

Mer information om status finns i [Statusöversikt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Inställningar för uppgifter och ärenden {#tasks-issues-preferences}

Systemet genererar en post i granskningsloggen i Inställningar för uppgifter och problem när en användare ändrar en inställning för uppgifter och problem på något av följande sätt:

* Låser eller låser upp en inställning
* Ändrar inställningen för en inställning
* Ändrar en åtkomstinställning för uppgifter, ärenden eller förfrågningar

Mer information om inställningar för aktiviteter och problem finns i [Konfigurera inställningar för aktiviteter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Användare {#user}

Systemet genererar en loggpost för användargranskning när en användare utför någon av följande åtgärder:

* Skapar en användare

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Detta är inte tillgängligt om din organisation har anslutit sig till Adobe Admin Console. Kontakta nätverks- eller IT-administratören om du behöver mer information.

* Tar bort en användare
* Ändrar en användares åtkomstnivå, företag, team eller grupp
* Aktivera en användare
* Inaktiverar en användare

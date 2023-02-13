---
navigation-topic: financials
title: Skapa faktureringsposter
description: Förutom att ställa in intäkter och spåra utgifter kan du skapa faktureringsposter för ett projekt för information som behöver faktureras.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 0%

---

# Skapa faktureringsposter

Förutom att ställa in intäkter och spåra utgifter kan du skapa faktureringsposter för ett projekt för information som behöver faktureras.

Du kan inte skapa faktureringsposter för uppgifter. Du kan bara skapa faktureringsposter för projekt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Översikt över faktureringsposter

Faktureringsposter skapas som bilagor till ett projekt och innehåller ekonomiska data från projektet samt viss finansiell information för aktiviteterna i ett projekt.

Tänk på följande när du planerar att använda faktureringsposter:

* Du skapar en faktureringspost när du vill fakturera ett belopp som är relaterat till projektet till en extern leverantör eller partner. Förutom att fakturera ett fast belopp till en extern källa, finns det tillfällen då du måste fakturera ut mängden arbete i projektet (från loggade timmar) till en extern leverantör, liksom utgifter eller beloppet för fasta intäkter. Du kan inkludera all den här informationen i samma faktureringspost.
* När en faktureringspost har angetts till Fakturerad går det inte att redigera den.

   >[!IMPORTANT]
   >
   >Detta är viktigt när priset varierar och du vill låsa intäkt- och utgiftsinformationen för projektet. Om du lägger till den i en faktureringspost och markerar den som Fakturerad uppdateras den inte när tarifferna uppdateras i ditt system.

* Ett projekt med faktureringsposter som har markerats som Fakturerade kan inte tas bort.

## Skapa en faktureringspost

1. Navigera till ett projekt.
1. Klicka **Faktureringsposter** i den vänstra panelen.

   Det här avsnittet kan finnas under **Visa fler**.

1. Med **Faktureringspostdetaljer** till vänster klickar du på **Ny faktureringspost**.
1. I **Ny faktureringspost** anger du följande information i rutan som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Detta är ett obligatoriskt fält. Ange en beskrivning för faktureringsposten, för att återspegla syftet eller avsikten med posten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktureringsstatus</td> 
      <td> <p>Välj <strong>Ej fakturerad</strong>, om posten inte har fakturerats än.</p> <p>Välj <strong>Fakturerad</strong> när faktureringsposten faktureras.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktureringsdatum</td> 
      <td>Välj det datum då den här faktureringsposten ska faktureras genom att klicka på kalenderikonen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">PO-nummer</td> 
      <td>Om det finns ett inköpsordernummer som är associerat med den här faktureringsposten anger du den här informationen i det här fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktura-ID</td> 
      <td>Om det finns en faktura som är associerad med den här faktureringsposten anger du den här informationen i det här fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ytterligare belopp</td> 
      <td>Ange det fasta beloppet för din faktureringspost. Detta är det belopp som du avser att debitera en extern kund, leverantör eller partner för det här projektet. Det här beloppet kan inte ändras efter att status för faktureringsposten har ändrats till Fakturerad.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Under **Anpassad Forms** väljer du ett anpassat formulär för faktureringsposter som du vill lägga till i faktureringsposten.

   Du (eller en annan användare med tillgång till anpassade formulär) måste skapa ett anpassat formulär för faktureringsposter innan du kan markera det här. Endast aktiva anpassade formulär visas i listan. Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   Du kan upprepa det här steget om du vill lägga till andra anpassade formulär som du behöver för faktureringsposten.

1. Klicka **Spara.**

   Faktureringsposten skapas. Om du vill inkludera fakturerbara timmar, utgifter och fasta intäkter i faktureringsposten följer du stegen som beskrivs i följande underavsnitt.

## Inkludera fakturerbara timmar, utgifter och fasta intäkter i en faktureringspost

* [Inkludera fakturerbara timmar i en faktureringspost](#include-billable-hours-in-a-billing-record)
* [Inkludera fakturerbara utgifter i en faktureringspost](#include-billable-expenses-in-a-billing-record)
* [Inkludera fasta intäkter i en faktureringspost](#include-fixed-revenues-in-a-billing-record)

### Inkludera fakturerbara timmar i en faktureringspost {#include-billable-hours-in-a-billing-record}

Du kan inkludera timmar som har loggats in på uppgifter, utleveranser eller projektet i dina faktureringsposter.\
Om den användare som loggar timmarna eller deras primära roll är associerad med en faktureringstid per timme, läggs intäkterna från dessa timmar till i faktureringsposten.

* [Vilka timmar som kan läggas till i en faktureringspost](#what-hours-can-be-added-to-a-billing-record)
* [Lägg till timmar i en faktureringspost](#add-hours-to-a-billing-record)

#### Vilka timmar som kan läggas till i en faktureringspost {#what-hours-can-be-added-to-a-billing-record}

Du kan lägga till timmar i en faktureringspost när följande villkor är uppfyllda:

* Uppgifter, ärenden eller projektet har loggats i timmar.
* Timtypen för de timmar som loggas markeras som Antal som Intäkter.

   Mer information om timtyper finns i artikeln [Hantera timtyper](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Alla timmar som loggats för utleveranser eller för projektet kan läggas till i en faktureringspost om användaren som loggar tiden har en faktureringstid per timme som är associerad med dem eller deras primära roll.
* Om timmarna är inloggade på en uppgift måste uppgiften ha följande intäktstyp:

   * Intäktstypen kan inte anges till Inte fakturerbar.
   * Om intäktstypen är inställd på Användare per timme måste användaren som loggar tiden ha en faktureringstakt per timme angiven i sin profil.
   * Om intäktstypen är inställd på Roll-timme måste den primära rollen för användaren som loggar tiden ha en faktureringstid per timme.

      >[!NOTE]
      >
      >Du kan åsidosätta faktureringstariffer för jobbroller på projektnivå.\
      >Mer information om hur du åsidosätter faktureringstariffer för jobbroller finns i avsnittet Åsidosätta faktureringstariffer för jobbroller på projektnivå i artikeln [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* If **Kräv tid för godkännande av det här projektet** är markerat under Projektinställningar måste projektägaren godkänna de loggade timmarna.\
   Mer information om hur du kräver godkännande under projekttimmar finns i artikeln [Kräv tid för godkännande av ett projekt](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Lägg till timmar i en faktureringspost {#add-hours-to-a-billing-record}

Så här lägger du till fakturerbara timmar i en faktureringspost:

1. Gå till projektet med faktureringsposterna.
1. Klicka **Faktureringsposter** i den vänstra panelen.

   Det här avsnittet kan finnas under **Visa fler**.

1. Klicka på **Beskrivning** av en faktureringspost för att öppna **Faktureringspostdetaljer** -fliken.

1. Klicka **Fakturerbara timmar** i den vänstra panelen.
1. Om det finns timmar som kan inkluderas i en faktureringspost klickar du på **Lägg till timmar**.\
   The **Lägg till fakturerbara timmar** öppnas.

   >[!NOTE]
   >
   >Om inga timmar är loggade eller om de loggade timmarna inte uppfyller villkoren som måste läggas till i en faktureringspost, **Lägg till timmar** knappen visas inte. Mer information om vilka timmar som kan loggas i en faktureringspost finns i avsnittet [Vilka timmar som kan läggas till i en faktureringspost](#what-hours-can-be-added-to-a-billing-record) i den här artikeln.

1. Markera timposterna som du vill inkludera i faktureringsposten och klicka på **Lägg till timmar**.\
   Den faktiska kostnaden för timmarna läggs till som **Fakturerbara timmar** belopp till **Faktureringspost totalt**.

1. (Valfritt) Klicka på **Information om faktureringsposter** för att granska **Fakturerbara timmar** och **Faktureringspost totalt** belopp. Du kan även se summan för faktureringsposten i huvudet på faktureringsposten.

### Inkludera fakturerbara utgifter i en faktureringspost {#include-billable-expenses-in-a-billing-record}

Om du lägger till Fakturerbara utgifter i faktureringsposten kontrollerar du att utgifterna för aktiviteterna och projektet är markerade som Fakturerbara. Utgifter som inte är markerade som fakturerbara är inte tillgängliga att lägga till i en faktureringspost. Mer information om hur du lägger till utgifter finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Så här lägger du till fakturerbara utgifter i en faktureringspost:

1. Gå till projektet med faktureringsposterna.
1. Klicka **Faktureringsposter** i den vänstra panelen.

   Du kanske måste klicka **Visa fler** sedan **Faktureringsposter**.

1. Klicka på **Beskrivning** av en faktureringspost för att öppna **Faktureringspostdetaljer** -fliken.

1. Klicka **Fakturerbara utgifter** i den vänstra panelen.
1. (Villkorligt) Om du har lagt till utgifter för dina aktiviteter eller projektet och har markerat dem som fakturerbara klickar du på **Lägg till utgifter**.

   >[!NOTE]
   >
   >Om du har utgifter men de inte är markerade som fakturerbara visas **Lägg till utgifter** knappen visas inte. Endast fakturerbara utgifter med ett faktiskt belopp som är större än noll kan inkluderas i en faktureringspost.

1. Välj de fakturerbara utgifter som är tillgängliga att läggas till i faktureringsposten och klicka sedan på **Lägg till utgifter**.\
   Det faktiska beloppet för utgifterna läggs till som **Fakturerbara utgifter** belopp till **Faktureringspost totalt**.

1. (Valfritt) Klicka på **Information om faktureringsposter** för att granska **Fakturerbara utgifter** och **Faktureringspost totalt** belopp. Du kan även se summan för faktureringsposten i huvudet på faktureringsposten.

### Inkludera fasta intäkter i en faktureringspost {#include-fixed-revenues-in-a-billing-record}

Du kan lägga till fasta intäkter i dina faktureringsposter om du har uppgifter som har Fast intäkt tillgänglig. Det finns inga andra typer av aktiviteter eller projektintäkter att lägga till i en faktureringspost. Mer information om intäktstyper finns i [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) avsnitt i [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Så här lägger du till fasta intäkter i en faktureringspost:

1. Gå till projektet med faktureringsposterna.
1. Klicka **Faktureringsposter** i den vänstra panelen.

   Du kanske måste klicka **Visa fler** sedan **Faktureringsposter**.

1. Klicka på **Beskrivning** av en faktureringspost för att öppna **Faktureringspostdetaljer** -fliken.

1. Välj **Fasta intäkter** -fliken.
1. Om du har lagt till fasta intäkter i dina uppgifter klickar du på **Lägg till fasta intäkter**.

   >[!NOTE]
   >
   >Om du har intäktsbelopp för aktiviteter men inte har markerats som Fast, visas **Lägg till fast intäkt** knappen visas inte.

1. Välj de uppgifter vars fasta inkomster du vill inkludera i faktureringsposten och klicka sedan på **Lägg till aktiviteter**.\
   The **Fast intäkt** mängden uppgifter läggs till som **Fakturerbara intäkter** belopp till **Faktureringspost totalt**.

1. (Valfritt) Klicka på **Information om faktureringsposter** för att granska **Fakturerbara intäkter** och **Faktureringspost totalt** belopp. Du kan även se summan för faktureringsposten i huvudet på faktureringsposten.

## Redigera en faktureringspost

När du har skapat en faktureringspost och inkluderat timmar, utgifter och intäkter i faktureringsposten kan du redigera viss information i den befintliga posten innan den markeras som Fakturerad.

1. Gå till faktureringsposten.
1. Med **Faktureringspostdetaljer** i den vänstra panelen redigerar du information i alla tillgängliga fält

   eller

   Klicka på **Ikonen Redigera** ![](assets/edit-icon.png) i det övre högra hörnet och redigera sedan information i alla tillgängliga fält.

   Uppdatera följande:

   * **Beskrivning**
   * **Faktureringsstatus**

      >[!TIP]
      >
      >Om du väljer **Fakturerad** Faktureringsstatus: Faktureringsposten kan inte redigeras när du har sparat ändringarna.

   * **Faktureringsdatum**
   * **PO-nummer**
   * **Faktura-ID**
   * **Ytterligare belopp**

   Följande fält är inte tillgängliga för redigering:

   * **Fakturerbara timmar:** Summan av faktisk intäkt för de timmar som ingår i faktureringsposten. Mer information om hur du inkluderar timmar i en faktureringspost finns i avsnittet [Inkludera fakturerbara timmar i en faktureringspost](#include-billable-hours-in-a-billing-record) i den här artikeln.

   * **Fakturerbara utgifter**: Det totala faktiska beloppet för fakturerbara utgifter som ingår i faktureringsposten. Mer information om hur du inkluderar fakturerbara utgifter i en faktureringspost finns i avsnittet [Inkludera fakturerbara utgifter i en faktureringspost](#include-billable-expenses-in-a-billing-record) i den här artikeln.

   * **Fakturerbara intäkter**: Summan av fasta intäkter för de uppgifter som ingår i faktureringsposten. Mer information om hur du inkluderar fasta intäkter i en faktureringspost finns i avsnittet [Inkludera fasta intäkter i en faktureringspost](#include-fixed-revenues-in-a-billing-record) i den här artikeln.

   * **Faktureringspost totalt**: Summan av alla fakturerbara belopp. Detta beräknas med följande formel:

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. Klicka **Spara****Ändringar**.

---
navigation-topic: financials
title: Skapa faktureringsposter
description: Förutom att ställa in intäkter och spåra utgifter kan du skapa faktureringsposter för ett projekt för information som behöver faktureras.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1931'
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
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
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
* När en faktureringspost är inställd på Fakturerad går det inte att redigera den.

  >[!IMPORTANT]
  >
  >Detta är viktigt när priset varierar och du vill låsa intäkt- och utgiftsinformationen för projektet. Om du lägger till den i en faktureringspost och markerar den som Fakturerad, uppdateras den inte när tarifferna uppdateras i ditt system.

* Ett projekt med faktureringsposter som har markerats som Fakturerade kan inte tas bort.

## Skapa en faktureringspost

1. Navigera till ett projekt.
1. Klicka på **Faktureringsposter** i den vänstra panelen.

   Det här avsnittet kan finnas under **Visa mer**.

1. Välj **Information om faktureringspost** i den vänstra panelen och klicka på **Ny faktureringspost**.
1. Ange följande information i rutan **Ny faktureringspost** som visas:

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
      <td> <p>Välj <strong>Inte fakturerad</strong>, om posten inte har fakturerats än.</p> <p>Välj <strong>Fakturerad</strong> när faktureringsposten faktureras.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktureringsdatum</td> 
      <td>Välj det datum då den här faktureringsposten ska faktureras genom att klicka på kalenderikonen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">IO-nummer</td> 
      <td>Om det finns ett inköpsordernummer som är associerat med den här faktureringsposten anger du den här informationen i det här fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktura-ID</td> 
      <td>Om det finns en faktura associerad med den här faktureringsposten anger du den här informationen i det här fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ytterligare belopp</td> 
      <td>Ange det fasta beloppet för din faktureringspost. Detta är det belopp som du avser att debitera en extern kund, leverantör eller partner för det här projektet. Det här beloppet kan inte ändras efter att status för faktureringsposten har ändrats till Fakturerad.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Under **Anpassad Forms** väljer du ett anpassat formulär för faktureringsposter som du vill lägga till i faktureringsposten.

   Du (eller en annan användare med tillgång till anpassade formulär) måste skapa ett anpassat formulär för faktureringsposter innan du kan markera det här. Endast aktiva anpassade formulär visas i listan. Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Du kan upprepa det här steget om du vill lägga till andra anpassade formulär som du behöver för faktureringsposten.

1. Klicka på **Spara.**

   Faktureringsposten skapas. Om du vill inkludera fakturerbara timmar, utgifter och fasta intäkter i faktureringsposten följer du stegen som beskrivs i följande underavsnitt.

## Inkludera fakturerbara timmar, utgifter och fasta intäkter i en faktureringspost

* [Inkludera fakturerbara timmar i en faktureringspost](#include-billable-hours-in-a-billing-record)
* [Inkludera fakturerbara utgifter i en faktureringspost](#include-billable-expenses-in-a-billing-record)
* [Inkludera fasta intäkter i en faktureringspost](#include-fixed-revenues-in-a-billing-record)

### Inkludera fakturerbara timmar i en faktureringspost {#include-billable-hours-in-a-billing-record}

Du kan inkludera timmar som har loggats in på uppgifter, utleveranser eller projektet i dina faktureringsposter.\
Om den användare som loggar timmarna eller deras primära roll är associerad med en faktureringstid per timme, läggs intäkterna från dessa timmar till i faktureringsposten.

* [Vilka timmar kan läggas till i en faktureringspost](#what-hours-can-be-added-to-a-billing-record)
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
     >Mer information om hur du åsidosätter faktureringstariffer för jobbroller finns i avsnittet Åsidosätta faktureringstariffer för jobbroller på projektnivå i artikeln [Översikt över faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Om **Kräv tid för godkännande av det här projektet** är markerat under Projektinställningar, måste projektägaren godkänna de timmar som loggas.\
  Mer information om att kräva godkännande under projekttimmar finns i artikeln [Kräv tid för att godkännas för ett projekt](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Lägg till timmar i en faktureringspost {#add-hours-to-a-billing-record}

Så här lägger du till fakturerbara timmar i en faktureringspost:

1. Gå till projektet med faktureringsposterna.
1. Klicka på **Faktureringsposter** i den vänstra panelen.

   Det här avsnittet kan finnas under **Visa mer**.

1. Klicka på **Beskrivning** för en faktureringspost för att öppna fliken **Information om faktureringspost**.

1. Klicka på **Fakturerbara timmar** i den vänstra panelen.
1. Om det finns timmar som kan inkluderas i en faktureringspost klickar du på **Lägg till timmar**.\
   Rutan **Lägg till fakturerbara timmar** öppnas.

   >[!NOTE]
   >
   >Om det inte finns några timmar loggade eller om de timmar som loggas inte uppfyller villkoren som måste läggas till i en faktureringspost visas inte knappen **Lägg till timmar**. Mer information om vilka timmar som kan loggas i en faktureringspost finns i avsnittet [Vilka timmar som kan läggas till i en faktureringspost](#what-hours-can-be-added-to-a-billing-record) i den här artikeln.

1. Markera timposterna som du vill ta med i faktureringsposten och klicka på **Lägg till timmar**.\
   Den faktiska kostnaden för timmarna läggs till som beloppet **Fakturerbara timmar** till totalt **Faktureringspost**.

1. (Valfritt) Klicka på **Information om faktureringsposter** om du vill granska summorna för **fakturerbara timmar** och **faktureringspost**. Du kan även se summan för faktureringsposten i huvudet på faktureringsposten.

### Inkludera fakturerbara utgifter i en faktureringspost {#include-billable-expenses-in-a-billing-record}

Om du lägger till Fakturerbara utgifter i faktureringsposten kontrollerar du att utgifterna för aktiviteterna och projektet är markerade som Fakturerbara. Utgifter som inte är markerade som fakturerbara är inte tillgängliga att lägga till i en faktureringspost. Mer information om hur du lägger till utgifter finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Så här lägger du till fakturerbara utgifter i en faktureringspost:

1. Gå till projektet med faktureringsposterna.
1. Klicka på **Faktureringsposter** i den vänstra panelen.

   Du kan behöva klicka på **Visa fler** och sedan på **Faktureringsposter**.

1. Klicka på **Beskrivning** för en faktureringspost för att öppna fliken **Information om faktureringspost**.

1. Klicka på **Fakturerbara utgifter** i den vänstra panelen.
1. (Villkorligt) Om du har lagt till utgifter för dina aktiviteter eller projektet och har markerat dem som fakturerbara klickar du på **Lägg till utgifter**.

   >[!NOTE]
   >
   >Om du har utgifter men de inte är markerade som fakturerbara visas inte knappen **Lägg till utgifter** . Endast fakturerbara utgifter med ett faktiskt belopp som är större än noll kan inkluderas i en faktureringspost.

1. Välj de fakturerbara utgifter som är tillgängliga att läggas till i faktureringsposten och klicka sedan på **Lägg till utgifter**.\
   Det faktiska beloppet för utgifterna läggs till som beloppet **Fakturerbara utgifter** till totalt **Faktureringspost**.

1. (Valfritt) Klicka på **Information om faktureringsposter** om du vill granska summorna för **fakturerbara utgifter** och **faktureringspost**. Du kan även se summan för faktureringsposten i huvudet på faktureringsposten.

### Inkludera fasta intäkter i en faktureringspost {#include-fixed-revenues-in-a-billing-record}

Du kan lägga till fasta intäkter i dina faktureringsposter om du har uppgifter som har Fast intäkt tillgänglig. Det finns inga andra typer av aktiviteter eller projektintäkter att lägga till i en faktureringspost. Mer information om intäktstyper finns i avsnittet [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) i [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Så här lägger du till fasta intäkter i en faktureringspost:

1. Gå till projektet med faktureringsposterna.
1. Klicka på **Faktureringsposter** i den vänstra panelen.

   Du kan behöva klicka på **Visa fler** och sedan på **Faktureringsposter**.

1. Klicka på **Beskrivning** för en faktureringspost för att öppna fliken **Information om faktureringspost**.

1. Välj fliken **Fasta intäkter**.
1. Om du har lagt till fasta intäkter i dina aktiviteter klickar du på **Lägg till fasta intäkter**.

   >[!NOTE]
   >
   >Om du har intäktsbelopp för aktiviteter, men de inte är markerade som fasta, visas inte knappen **Lägg till fast intäkt** .

1. Välj de uppgifter vars fasta inkomster du vill inkludera i faktureringsposten och klicka sedan på **Lägg till uppgifter**.\
   Beloppet **Fast intäkt** för aktiviteterna läggs till som beloppet **Fakturerbara intäkter** till totalt **Faktureringspost**.

1. (Valfritt) Klicka på **Information om faktureringsposter** om du vill granska summorna för **fakturerbara intäkter** och **faktureringspost**. Du kan även se summan för faktureringsposten i huvudet på faktureringsposten.

## Redigera en faktureringspost

När du har skapat en faktureringspost och inkluderat timmar, utgifter och intäkter i faktureringsposten kan du redigera viss information i den befintliga posten innan den markeras som Fakturerad.

1. Gå till faktureringsposten.
1. Om **Information om faktureringspost** är markerad på den vänstra panelen redigerar du information i alla tillgängliga fält

   eller

   Klicka på ikonen **Redigera** ![](assets/edit-icon.png) i det övre högra hörnet och redigera sedan information i alla tillgängliga fält.

   Uppdatera följande:

   * **Beskrivning**
   * **Faktureringsstatus**

     >[!TIP]
     >
     >Om du väljer **Fakturerad** som faktureringsstatus kan faktureringsposten inte redigeras efter att du har sparat ändringarna.

   * **Faktureringsdatum**
   * **IO-nummer**
   * **Faktura-ID**
   * **Ytterligare belopp**

   Följande fält är inte tillgängliga för redigering:

   * **Fakturerbara timmar:** Summan av faktisk intäkt för de timmar som ingår i faktureringsposten. Mer information om hur du inkluderar timmar i en faktureringspost finns i avsnittet [Inkludera fakturerbara timmar i en faktureringspost](#include-billable-hours-in-a-billing-record) i den här artikeln.

   * **Fakturerbara utgifter**: Summan av det faktiska beloppet för fakturerbara utgifter som ingår i faktureringsposten. Mer information om hur du inkluderar fakturerbara utgifter i en faktureringspost finns i avsnittet [Inkludera fakturerbara utgifter i en faktureringspost](#include-billable-expenses-in-a-billing-record) i den här artikeln.

   * **Fakturerbara intäkter**: Summan av den fasta intäkten för aktiviteterna som ingår i faktureringsposten. Mer information om hur du inkluderar fasta intäkter i en faktureringspost finns i avsnittet [Inkludera fasta intäkter i en faktureringspost](#include-fixed-revenues-in-a-billing-record) i den här artikeln.

   * **Totalt antal faktureringsposter**: Summan av alla fakturerbara belopp. Detta beräknas med följande formel:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Klicka på **Spara***Ändringar**.

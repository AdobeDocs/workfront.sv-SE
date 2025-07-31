---
navigation-topic: financials
title: Skapa faktureringsposter
description: Förutom att ställa in intäkter och spåra utgifter kan du skapa faktureringsposter för ett projekt för information som behöver faktureras.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: ec6ddb50d6b9137837c8031b22f213cd6ada70ff
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 0%

---

# Skapa faktureringsposter

<!-- Audited: 6/2025 -->

Förutom att ställa in intäkter och spåra utgifter kan du skapa faktureringsposter för ett projekt för information som behöver faktureras.

Du kan inte skapa faktureringsposter för uppgifter. Du kan bara skapa faktureringsposter för projekt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera behörigheter till projektet med behörigheter för att hantera ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över faktureringsposter

Faktureringsposter skapas som bilagor till ett projekt och innehåller ekonomiska data från projektet samt projektaktiviteternas ekonomiska information.

Tänk på följande när du planerar att använda faktureringsposter:

* Du skapar en faktureringspost när du vill fakturera ett belopp som är relaterat till projektet till en extern leverantör eller partner. Förutom att fakturera ett fast belopp till en extern källa, finns det tillfällen då du måste fakturera ut mängden arbete i projektet (från loggade timmar) till en extern leverantör, liksom utgifter eller beloppet för fasta intäkter. Du kan inkludera all den här informationen i samma faktureringspost.
* När en faktureringspost har angetts till Fakturerad kan den inte redigeras.

  >[!IMPORTANT]
  >
  >Detta är viktigt när priset varierar och du vill låsa intäkt- och utgiftsinformationen för projektet. Om du lägger till den i en faktureringspost och markerar den som Fakturerad, uppdateras den inte när tarifferna uppdateras i ditt system.

* Ett projekt med faktureringsposter som har markerats som Fakturerade kan inte tas bort.

## Skapa en faktureringspost

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på **Faktureringsposter** i den vänstra panelen.
1. Klicka på **Ny faktureringspost**.
1. Ange följande information i rutan **Ny faktureringspost** som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>(Obligatoriskt) Ange en beskrivning för faktureringsposten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktureringsstatus</td> 
      <td> <p>Välj <strong>Inte fakturerad</strong> om den här posten inte har fakturerats än.</p> <p>Välj <strong>Fakturerad</strong> om faktureringsposten har fakturerats.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktureringsdatum</td> 
      <td>Välj det datum då faktureringsposten fakturerades genom att klicka på kalenderikonen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">IO-nummer</td> 
      <td>Ange det inköpsordernummer som är associerat med den här faktureringsposten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktura-ID</td> 
      <td>Ange fakturan som är associerad med den här faktureringsposten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ytterligare belopp</td> 
      <td>Ange det fasta beloppet för din faktureringspost. Detta är det belopp som du avser att debitera en extern kund, leverantör eller partner för det här projektet. Det här beloppet kan inte ändras efter att status för faktureringsposten har ändrats till Fakturerad.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Välj ett anpassat formulär som du vill lägga till i posten under **Anpassad Forms**.

   Ett anpassat formulär för faktureringsposter måste skapas innan du kan välja det här. Endast aktiva anpassade formulär visas i listan. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på **Spara.** Faktureringsposten skapas.

## Inkludera fakturerbara timmar, utgifter och fasta intäkter i en faktureringspost

### Inkludera fakturerbara timmar i en faktureringspost {#include-billable-hours-in-a-billing-record}

Du kan inkludera timmar som har loggats in på uppgifter, utleveranser eller projektet i dina faktureringsposter.

Om användaren som loggar timmarna eller deras primära jobbroll är associerad med en faktureringstid per timhastighet, läggs intäkterna från dessa timmar till i faktureringsposten.

* [Vilka timmar kan läggas till i en faktureringspost](#what-hours-can-be-added-to-a-billing-record)
* [Lägg till timmar i en faktureringspost](#add-hours-to-a-billing-record)

#### Vilka timmar som kan läggas till i en faktureringspost {#what-hours-can-be-added-to-a-billing-record}

Du kan lägga till timmar i en faktureringspost när följande villkor är uppfyllda:

* Timmar har loggats för uppgifter, utgåvor eller projekt.
* Timtypen för de timmar som loggas markeras som Antal som Intäkter.

  Mer information finns i artikeln [Hantera timtyper](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Alla timmar som loggats för utleveranser eller projektet kan läggas till i en faktureringspost om användaren som loggar tiden har en faktureringstakt per timme som är associerad med dem eller deras primära jobbroll.
* Om timmarna är inloggade på en uppgift måste uppgiften ha följande intäktstyp:

   * Det går inte att ange intäktstypen till Inte fakturerbar.
   * Om intäktstypen är inställd på Användare per timme måste användaren som loggar tiden ha en faktureringstakt per timme angiven i sin profil.
   * Om intäktstypen är inställd på Roll-timme måste den primära rollen för användaren som loggar tiden ha en faktureringstakt per timme.

     >[!NOTE]
     >
     >Du kan åsidosätta faktureringstariffer för jobbroller på projektnivå.\
     >Mer information finns i avsnittet Åsidosätta faktureringssatser för jobbroller på projektnivå i artikeln [Översikt över åsidosättande av faktureringssatser för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Om alternativet Kräv tid att godkänna för det här projektet har valts under Projektinställningar måste projektägaren godkänna de loggade timmarna.\
  Mer information finns i [Kräv tid för att godkännas för ett projekt](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Lägg till timmar i en faktureringspost {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på **Faktureringsposter** i den vänstra panelen.
1. Klicka på faktureringsposten **Beskrivning** för att öppna fliken **Information om faktureringspost**.
1. Klicka på **Fakturerbara timmar** i den vänstra panelen.
1. Om det finns timmar som kan inkluderas i en faktureringspost klickar du på **Lägg till timmar**. Rutan **Lägg till fakturerbara timmar** öppnas.

   >[!NOTE]
   >
   >Om det inte finns några timmar loggade eller om de timmar som loggas inte uppfyller villkoren som måste läggas till i en faktureringspost visas inte knappen **Lägg till timmar**. Mer information finns i följande avsnitt i den här artikeln: [Vilka timmar kan läggas till i en faktureringspost](#what-hours-can-be-added-to-a-billing-record).

1. Markera timposterna som du vill inkludera i faktureringsposten och klicka sedan på **Lägg till timmar**. Den faktiska kostnaden för timmarna läggs till som beloppet **Fakturerbara timmar** till totalt **Faktureringspost**.

1. (Valfritt) Klicka på **Information om faktureringsposter** om du vill granska summorna för **fakturerbara timmar** och **faktureringspost** och faktureringsposten totalt i faktureringsposthuvudet.

### Inkludera fakturerbara utgifter i en faktureringspost {#include-billable-expenses-in-a-billing-record}

Om du lägger till fakturerbara utgifter i faktureringsposten kontrollerar du att utgifterna för aktiviteterna och projektet är markerade som fakturerbara. Utgifter som inte är markerade som fakturerbara är inte tillgängliga att lägga till i en faktureringspost. Mer information om hur du lägger till utgifter finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Så här lägger du till fakturerbara utgifter i en faktureringspost:

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på **Faktureringsposter** i den vänstra panelen.
1. Klicka på faktureringsposten **Beskrivning** för att öppna fliken **Information om faktureringspost**.
1. Klicka på **Fakturerbara utgifter** i den vänstra panelen.
1. (Villkorligt) Om du har lagt till utgifter för dina aktiviteter eller projektet och markerat dem som fakturerbara klickar du på **Lägg till utgifter**.

   >[!NOTE]
   >
   >Om du har utgifter men de inte har markerats som fakturerbara visas inte knappen **Lägg till utgifter**. Endast fakturerbara utgifter med ett faktiskt belopp som är större än noll kan inkluderas i en faktureringspost.

1. Välj de fakturerbara utgifter som är tillgängliga att läggas till i faktureringsposten och klicka sedan på **Lägg till utgifter**.  Det faktiska beloppet för utgifterna läggs till som beloppet **Fakturerbara utgifter** till totalt **Faktureringspost**.

1. (Valfritt) Klicka på **Information om faktureringsposter** om du vill granska summorna för **fakturerbara utgifter** och **faktureringspost** och faktureringsposten totalt i faktureringsposthuvudet.

### Inkludera fasta intäkter i en faktureringspost {#include-fixed-revenues-in-a-billing-record}

Du kan lägga till fasta intäkter i dina faktureringsposter om du har uppgifter som har fasta intäkter tillgängliga. Det finns ingen annan typ av aktivitet eller projektintäkter att lägga till i en faktureringspost. Mer information om intäktstyper finns i avsnittet Översikt över fakturering och intäkt i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på **Faktureringsposter** i den vänstra panelen.
1. Klicka på faktureringspostens **beskrivning** för att öppna fliken **Information om faktureringsposten**.
1. Välj fliken **Fasta intäkter**.
1. Om du har lagt till fasta intäkter till dina aktiviteter klickar du på **Lägg till fasta intäkter**.

   >[!NOTE]
   >
   >Om du har intäktsbelopp för aktiviteter, men de inte är markerade som fasta, visas inte knappen **Lägg till fasta intäkter** .

1. Välj de uppgifter vars fasta inkomster du vill inkludera i faktureringsposten och klicka sedan på **Lägg till aktiviteter**.  Beloppet **Fast intäkt** för aktiviteterna läggs till som beloppet **Fakturerbara intäkter** till totalt **Faktureringspost**.

1. (Valfritt) Klicka på **Information om faktureringsposter** om du vill granska summorna för **fakturerbara intäkter** och **faktureringspost** och faktureringsposten totalt i faktureringsposthuvudet.

## Redigera en faktureringspost

När du har skapat en faktureringspost och lagt till timmar, utgifter och intäkter kan du redigera viss information på den befintliga posten innan den markeras som Fakturerad.

1. Navigera till faktureringsposten.
1. Välj **Information om faktureringspost** i den vänstra panelen.
1. Redigera information i alla tillgängliga fält.

   eller

   Klicka på ikonen **Redigera** ![Redigera](assets/edit-icon.png) i det övre högra hörnet och redigera sedan information i alla tillgängliga fält.

   Uppdatera följande:

   * **Beskrivning**
   * **Faktureringsdatum**
   * **Faktureringsstatus**

     >[!TIP]
     >
     >Om du väljer **Fakturerad** som faktureringsstatus kan faktureringsposten inte redigeras när du har sparat ändringarna.

   * **Faktura-ID**
   * **IO-nummer**
   * **Ytterligare belopp**

   Följande fält är inte tillgängliga för redigering:

   * **Fakturerbara timmar:** Summan av faktisk intäkt för de timmar som ingår i faktureringsposten. Mer information finns i följande avsnitt i den här artikeln: [Inkludera fakturerbara timmar i en faktureringspost](#include-billable-hours-in-a-billing-record).

   * **Fakturerbara utgifter**: Summan av det faktiska beloppet för fakturerbara utgifter som ingår i faktureringsposten. Mer information finns i följande avsnitt i den här artikeln: [Inkludera fakturerbara utgifter i en faktureringspost](#include-billable-expenses-in-a-billing-record).

   * **Fakturerbara intäkter**: Summan av den fasta intäkten för aktiviteterna som ingår i faktureringsposten. Mer information finns i följande avsnitt i den här artikeln: [Inkludera fasta intäkter i en faktureringspost](#include-fixed-revenues-in-a-billing-record).

   * **Totalt antal faktureringsposter**: Summan av alla fakturerbara belopp. Detta beräknas med följande formel:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Klicka på **Spara ändringar**.

---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Skapa och hantera jobbroller
description: Som  [!DNL Adobe Workfront] administratör eller en användare med administrativ åtkomst till jobbroller kan du skapa jobbroller som kan tilldelas användare och ta bort standardjobbroller som inte är relevanta för din organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: df1d844346d7ed26dcb004ba1a10ec9e8d07422a
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# Skapa och hantera jobbroller

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>I version 25.11 har åsidosättningsvalutan för jobbroller tagits bort i produktionen. (Borttagningen ägde rum den 30 oktober i förhandsvisningsmiljön.) I stället för att ha en basvaluta och åsidosätta valutor finns nu en valuta tillgänglig för jobbroller, och kostnads- och faktureringstarifferna definieras med den valutan.

Som administratör för [!DNL Adobe Workfront] eller standardanvändare med Redigera-åtkomst till jobbroller kan du skapa jobbroller som kan tilldelas användare och ta bort standardjobbroller som inte är relevanta för din organisation. Mer information om administrativ åtkomst i [!DNL Workfront] finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>Jobbroller är en viktig del i hanteringen av resurser. Om du vill använda verktygen för resursplanering behöver jobbrollerna en kostnad och faktureringsfrekvens som är kopplad till dem. Mer information finns i [Kom igång med resurshantering](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Så här skapar eller redigerar du en jobbroll: Alla Workfront- eller arbetsflödespaket</p>
   <p>Så här använder du tariffattribut och lägger till anpassade formulär i jobbrollen: Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Administrativ åtkomst till jobbroller</td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en jobbroll

Så här skapar du en jobbroll:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Job Roles]** i den vänstra panelen.
1. Klicka på **[!UICONTROL New Job Role]> Skapa ny jobbroll**.
1. Ange information i följande fält:

   * **Namn**: Ange ett namn för jobbrollen. Det här namnet visas överallt i Workfront där fältet Jobbroll visas.

     >[!TIP]
     >
     >Namnet på en jobbroll kan innehålla upp till 255 tecken. Längre namn kan dock förkortas i vissa delar av Workfront.

   * **Beskrivning**: Ange en beskrivning för rollen som anger vad som är unikt med den.
   * **Är aktiv**: Välj **Ja** om du vill att rollen ska vara aktiv och tillgänglig överallt i Workfront för att associeras med användare, arbetsobjekt osv. Välj **Nej** om du vill att rollen ska inaktiveras och inte vara tillgänglig för tilldelning till användare, arbetsobjekt osv.

     Mer information om hur du inaktiverar jobbroller finns i [Inaktivera jobbroller](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

1. Klicka på **[!UICONTROL Create Job Role]**. Jobbrollen är nu tillgänglig för att tilldelas aktiviteter, utgåvor, godkännanden eller så kan du dela layoutmallar eller andra objekt med den. Mer information om all användning av jobbroller i [!DNL Workfront] finns i [Översikt över jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Mer information om hur du tar bort en jobbroll finns i [Ta bort jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

## Lägg till satser och attribut i en jobbroll

Fakturering och kostnadstariffer för en jobbroll används i finansiella beräkningar.

Graderingsattribut stöds i områden i Workfront där det finns priser, t.ex. jobbroller och användare. När attribut tillämpas på en jobbroll, tolkas deras tilldelningar automatiskt till rätt frekvenser.

Mer information finns i [Definiera tariffattribut](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Job Roles]** i den vänstra panelen.
1. Klicka på namnet på en befintlig jobbroll för att redigera den.
1. Klicka på **Information** i den vänstra panelen om du vill uppdatera jobbrollsinformationen.
1. (Valfritt) Om du vill bifoga ett anpassat formulär till jobbrollen klickar du på fältet **Lägg till anpassat formulär** i det övre högra hörnet på detaljsidan och väljer ett anpassat formulär i listan som visas.

   Mer information om hur du bifogar ett anpassat formulär finns i [Lägga till ett anpassat formulär till ett objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicka på [!UICONTROL **Kurser**] i den vänstra panelen.
1. Klicka på [!UICONTROL **Fakturering**] eller [!UICONTROL **Kostnad**] för att välja tarifftyp.
1. Klicka på [!UICONTROL **Lägg till priser**] om du vill lägga till en ny tariff.

   eller

   Välj en befintlig frekvens och klicka på ikonen **Redigera** ![Redigera](assets/edit-icon.png) för att uppdatera den.

   >[!NOTE]
   >
   >Eftersom varje frekvens är associerad med kombinationen av rollen och attribut för att skapa en unik frekvens, kan attributen inte ändras när du redigerar en frekvens.

1. I rutan **Ny hastighet** väljer du attribut för den hastighet som t.ex. byrå, plats eller kostnadsställe.

   >[!NOTE]
   >
   >Dessa attribut definieras separat och kan påverka intäkter och kostnadsberäkningar. Mer information finns i [Definiera tariffattribut](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Välj **Valuta** för tariffen. Workfront-administratören lägger till basvalutan under Konfigurera. Du kan ändra valet till en annan tillgänglig valuta och du kan ändra valutan i gällande datumintervall.

   >[!TIP]
   >
   >I det här fältet är endast valutor tillgängliga i området Valutakurser i ditt system. Om du bara har ställt in en valuta är endast den valutan tillgänglig.

   Mer information om hur du ställer in basvalutan i Workfront finns i [Konfigurera valutakurser](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Mer information om hur du ändrar valuta för ett projekt finns i [Ändra projektvalutan](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Villkorligt) Ange **Faktureringshastighet** för den här jobbrollen för en faktureringsfrekvens.

   Det här är faktureringen per timma för jobbrollen. Detta värde beräknar de planerade och faktiska intäkterna för uppgifter och ärenden som är kopplade till rollen och slutligen projektens planerade och faktiska intäkter. Ange kursen med den valda valutan.

   Om du använder attribut kombineras attributen och jobbrollen för att definiera en unik frekvens. En Designer-roll i New York för byrå A kan till exempel ha en separat avgift jämfört med en Designer-roll i Paris för byrå B.

   Klicka på **Lägg till ränta** om du vill se gällande faktureringspriser för datum. Ange värdet för fakturering/timme för tidsperioden och tilldela startdatum och slutdatum efter behov. Den första faktureringstakten har inget startdatum och den sista faktureringstakten har inget slutdatum.

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   I Workfront kan du lämna tomrum mellan datumintervall, men du får en varning som bekräftar att detta är avsiktligt.

   Mer information om hur Workfront beräknar intäkter finns i [Översikt över fakturering och intäkter](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >När du redigerar en befintlig jobbroll kan du sortera listan så att du ser det senaste startdatumet högst upp i hastighetslistan.

1. (Villkorligt) Ange **kostnadstariff** för den här jobbrollen för en kostnadstariff.

   Detta är kostnaden per timme för jobbrollen. Detta värde beräknar de planerade och faktiska kostnaderna för aktiviteter och ärenden som är kopplade till rollen samt slutligen de planerade och faktiska kostnaderna för projekten. Ange kursen med den valda valutan.

   Om du använder attribut kombineras attributen och jobbrollen för att definiera en unik frekvens. En Designer-roll i New York för byrå A kan till exempel ha en separat avgift jämfört med en Designer-roll i Paris för byrå B.

   Klicka på **Lägg till kurs** om du vill se datumfaktiska kostnadstariffer. Ange värdet för kostnad/timme för tidsperioden och tilldela ett startdatum och ett slutdatum efter behov. Den första kostnadstariffen har inget startdatum och den sista kostnadstariffen har inget slutdatum.

   Vissa datum läggs till automatiskt. Om till exempel den första kostnadstariffen inte har ett slutdatum och du lägger till en andra kostnadstariff med startdatumet 1 maj, läggs slutdatumet 30 april till den första kostnadstariffen så att inga luckor uppstår.

   Mer information om hur Workfront beräknar kostnader finns i [Spåra kostnader](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >När du redigerar en befintlig jobbroll kan du sortera listan så att du ser det senaste startdatumet högst upp i hastighetslistan.

1. Klicka på [!UICONTROL **Spara**].

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->




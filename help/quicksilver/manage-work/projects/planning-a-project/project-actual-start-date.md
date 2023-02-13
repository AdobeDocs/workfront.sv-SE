---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över projektets faktiska startdatum
description: Projekt, uppgifter och ärenden har ett faktiskt startdatum i Adobe Workfront. För uppgifter och ärenden är detta det datum då de har markerats som Pågår. För projekt är detta det datum då den första aktiviteten i projektet markeras som Pågår eller har slutförts.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Översikt över projektets faktiska startdatum

Projekt, uppgifter och ärenden har ett faktiskt startdatum i Adobe Workfront. För uppgifter och ärenden är detta det datum då de har markerats som Pågår. För projekt är detta det datum då den första aktiviteten i projektet markeras som Pågår eller har slutförts.

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
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när det gäller faktiska startdatum i Workfront

* Det faktiska startdatumet finns i avsnittet Detaljer för projekt, uppgifter och ärenden. 
* Det faktiska startdatumet för ett projekt, en uppgift eller en utgåva fylls inte i när objekten skapas.
* Det faktiska startdatumet fylls i när arbetet faktiskt börjar med projektet, aktiviteten eller utgåvan.
* Faktiskt startdatum visas inte på fliken Projektinformation om projektet inte har startats ännu.

   Faktiskt startdatum visas tomt på flikarna Aktivitets- och Utfärdandeinformation om arbetet inte har startats ännu.

* Du kan ändra det faktiska startdatumet för en uppgift eller ett problem manuellt, men du kan inte ändra det faktiska startdatumet för ett projekt.

## Överväganden om faktiska startdatum för projekt

* Workfront ställer automatiskt in faktiskt datum för ett projekt när något av följande inträffar:

   * En uppgiftstilldelad ändrar status för en uppgift från *Nytt* till en annan status som inte motsvarar *Nytt*.

   * En tilldelad uppgift ändrar Procent färdigt för en uppgift.

      >[!IMPORTANT]
      >
      >Projektets faktiska startdatum fylls inte i när projektet har markerats som Aktuellt. Faktiskt arbete måste starta på aktiviteterna i projektet innan projektets faktiska startdatum fylls i.

      I dessa fall anges projektets faktiska startdatum till det datum och den tidpunkt då dessa åtgärder utfördes för den tidigaste aktiviteten i projektet. Detta anger att projektet faktiskt startades på detta datum och denna tid.

## Hitta det faktiska startdatumet för ett projekt

Du kan hitta det faktiska startdatumet för ett projekt i följande områden:

* I avsnittet Detaljer för ett projekt.
* När du lägger till det faktiska startdatumet för objektet Projekt i rapporten i en projektrapport eller projektvy.

   Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Så här hittar du det faktiska startdatumet i avsnittet Detaljer i projektet:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Projekt**.
1. Klicka på det projekt som du vill visa det faktiska startdatumet för.
1. Klicka **Projektinformation** i den vänstra panelen och sedan gå till **Översikt** -avsnitt.

   Det faktiska startdatumet visas tillsammans med andra projektdatum.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 

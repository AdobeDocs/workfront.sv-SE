---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över projektets faktiska startdatum
description: Projekt, uppgifter och ärenden har ett faktiskt startdatum i Adobe Workfront. För uppgifter och ärenden är detta det datum då de har markerats som Pågår. För projekt är detta det datum då den första aktiviteten i projektet markeras som Pågår eller har slutförts.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Översikt över projektets faktiska startdatum

Projekt, uppgifter och ärenden har ett faktiskt startdatum i Adobe Workfront. För uppgifter och ärenden är detta det datum då de har markerats som Pågår. För projekt är detta det datum då den första aktiviteten i projektet markeras som Pågår eller har slutförts.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Ljus eller högre</p> 
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på när det gäller faktiska startdatum i Workfront

* Det faktiska startdatumet finns i avsnittet Detaljer för projekt, uppgifter och ärenden.
* Det faktiska startdatumet för ett projekt, en uppgift eller en utgåva fylls inte i när objekten skapas.
* Det faktiska startdatumet fylls i när arbetet faktiskt börjar med projektet, aktiviteten eller utgåvan.
* Faktiskt startdatum visas inte på fliken Projektinformation om projektet inte har startats ännu.

  Faktiskt startdatum visas tomt på flikarna Aktivitets- och Utfärdandeinformation om arbetet inte har startats ännu.

* Du kan ändra det faktiska startdatumet för en uppgift eller ett problem manuellt, men du kan inte ändra det faktiska startdatumet för ett projekt.

## Överväganden om faktiska startdatum för projekt

* Workfront ställer automatiskt in faktiskt datum för ett projekt när något av följande inträffar:

   * En tilldelad aktivitet ändrar status för en aktivitet från *Nytt* till en annan status som inte motsvarar *Nytt*.

   * En tilldelad uppgift ändrar Procent färdigt för en uppgift.

     >[!IMPORTANT]
     >
     >Projektets faktiska startdatum fylls inte i när projektet har markerats som Aktuellt. Faktiskt arbete måste starta på aktiviteterna i projektet innan projektets faktiska startdatum fylls i.

     I dessa fall anges projektets faktiska startdatum till det datum och den tidpunkt då dessa åtgärder utfördes för den tidigaste aktiviteten i projektet. Detta anger att projektet faktiskt startades på detta datum och denna tid.

## Hitta det faktiska startdatumet för ett projekt

Du kan hitta det faktiska startdatumet för ett projekt i följande områden:

* I avsnittet Detaljer för ett projekt.
* När du lägger till **Faktiskt startdatum** för projektobjektet i rapporten i en projektrapport eller projektvy.

  Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Så här hittar du det faktiska startdatumet i avsnittet Detaljer i projektet:

{{step1-to-projects}}

1. Klicka på det projekt som du vill visa det faktiska startdatumet för.
1. Klicka på **Projektinformation** i den vänstra panelen och gå sedan till avsnittet **Översikt**.

   ![Projektets faktiska startdatum är markerat](assets/nwe-project-actual-start-date--highlighted-350x367.png)

   **Faktiskt startdatum** visas tillsammans med andra projektdatum.



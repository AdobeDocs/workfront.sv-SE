---
title: Inaktivera eller återaktivera en användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Workfront-administratör kan du inaktivera eller återaktivera en användare.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 0%

---

# Inaktivera eller återaktivera en användare

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Om en användare lämnar organisationen kan du behöva ta bort dem från Adobe Workfront. De bör inte vara aktiva i systemet eftersom detta skulle skapa förvirring för andra användare när de lägger till dem i uppdateringar eller tilldelar dem arbete. När du inaktiverar en användare ser andra användare inte längre sitt namn när de söker efter personer i systemet.

Administratörer kan se inaktiva användare under Konfigurera.

Du kan återaktivera en användare när som helst.

>[!IMPORTANT]
>
>Vi rekommenderar att du inaktiverar användare som har lämnat organisationen i stället för att ta bort dem. Om en användare tas bort går all historik i Workfront som är kopplad till den användaren förlorad. Detta inkluderar deras arbetsuppgifter, deras koppling till anteckningar, timmar, dokument och alla andra objekt som de en gång har skapat.
>
>När du inaktiverar en användare i Workfront tas användarens licenser bort både för Workfront och för digitalt korrektur. Dessutom kan användaren inte längre tilldelas arbete. När en användare inaktiveras blir användarens Workfront-licens och språklicens tillgängliga och kan användas av en annan användare. All annan information i den inaktiverade användarens profil ändras inte.
>
>Mer information om hur borttagning och inaktivering av användare påverkas finns i [Ta bort användare](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: Standard</p><p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om användaren <b>Admin (gruppanvändare)</b> är aktiverad måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du inaktiverar en Workfront-administratör, Standard eller Plan-licens måste du koppla deras objekt och aktiviteter till en annan användare.

Mer information finns i [Inaktivera Workfront-administratörer och Planera licensanvändare](#about-deactivating-workfront-administrators-and-plan-license-users) i den här artikeln.

## Inaktivera en användare

Tänk på följande när du inaktiverar en användare:

* Användaren kommer inte att kunna komma åt systemet.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Alla data som är kopplade till användaren behålls.
* Du kan tilldela en inaktiverad användarlicens till en annan användare.

Så här inaktiverar du en användare:

{{step-1-to-users}}

1. Markera en användare, klicka på ikonen **Mer** ![](assets/more-icon.png) och klicka sedan på **Inaktivera**.

1. Klicka på **Inaktivera** i rutan som visas.

## Schemalägg användare för inaktivering

Som chef kanske du vill markera användare för inaktivering innan de faktiskt lämnar organisationen. Om du till exempel arbetar med en användare som är bunden enligt avtal finns de i ditt system under en begränsad tidsperiod och du vet när de upphör. Du kan schemalägga att de ska inaktiveras det datumet.

Workfront-administratörer och användare av Planera licenser kan se avaktiveringsdatumet i sin användarprofil.

Så här schemalägger du en användare för inaktivering:

{{step-1-to-users}}

1. Välj användarens namn.

   eller

   (Valfritt) Välj flera användare för att schemalägga att de ska inaktiveras gruppvis.

1. Klicka på ikonen Redigera ![](assets/edit-icon.png).
1. I rutan Redigera användare som visas klickar du på **Resursplanering** för att gå till det området.
1. Aktivera alternativet **Schemalägg inaktivering**.

1. I kalendern som visas anger du datum och tid för **schemalagt inaktiveringsdatum**.

   >[!NOTE]
   >
   >* I tidsrutan kan du bara välja hela timsteg, inte minuter.
   >* Om du väljer en tid för den aktuella dagen som har gått schemalägger Workfront avaktiveringen för följande dag kl. 12:00. Den valda tiden matchar datorns tidszon för användaren som schemalägger inaktiveringen.

1. Klicka på **Spara ändringar**.

   Användaren inaktiveras den valda dagen någon gång efter den valda tiden. Om du har valt att inaktivera flera användare samtidigt inaktiveras alla markerade användare den valda dagen någon gång efter den valda tiden.

Vi rekommenderar att du skapar en rapport för användare som du har schemalagt för inaktivering, så att du håller dig informerad om vilka användare som kommer att inaktiveras. Det finns ingen bekräftelse på att inaktiveringen skedde efter att användarna inaktiverades.

## Återaktivera en användare

{{step-1-to-users}}

1. Markera en användare, klicka på ikonen Mer ![](assets/more-icon.png) och sedan på **Aktivera**.

1. Tilldela en ny **åtkomstnivå** i listrutan och klicka sedan på **Återaktivera**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Korrekturera påverkan när du återaktiverar en användare

Inaktiverade användare förlorar sin tilldelade standardkorrekturroll och sin korrekturlicens (om du har en äldre Workfront Premium-plan). Om du väljer att återaktivera användaren måste du:

* Tilldela om licensen (om du har en äldre Workfront Premium-plan). Mer information om Workfront korrekturplaner finns i [Åtkomst till korrekturfunktioner i Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Kontrollera att de har rätt korrekturroll. Återaktiverade korrekturanvändare tilldelas det som har angetts som standardkorrekturroll för nya användare. Mer information finns i [Konfigurera standardspråkroller](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md).

## Inaktivera Workfront-administratörer och Standard- eller Plan-licensanvändare

Innan du inaktiverar en Workfront-administratör eller en användare med en Planera-licens är det viktigt att kontrollera om det finns Workfront-objekt och -aktiviteter som berör den personen och sedan associera dem med en annan Workfront-administratör eller planera licensanvändare efter behov.

Objekten och aktiviteterna kan omfatta följande:

* Uppgifter eller ärenden som tilldelats användaren
* Projekt som ägs av användaren
* Rapporter som har konfigurerats för att köras med användarens åtkomsträttigheter
* Mallar som ägs av användaren
* Projekt och mallar som användaren har angetts för som resurshanterare
* Begär köhanteringsregler som Workfront-administratören eller planlicensanvändaren är standardtilldelad för
* Godkännandeprocesser som har ett stadium som inkluderar användaren (särskilt om de var den enda godkännaren på scenen)
* Tidrapporter som listar användaren som godkännare
* Tidrapportprofiler som listar användaren som godkännare
* Korrektur på automatiserade arbetsflöden som innehåller användaren

## Resursplaneringseffekt när du schemalägger en användare för inaktivering

När du schemalägger en användare för inaktivering visas de inte längre som tillgängliga för budgetering i resursplaneraren. Om de fortfarande är en del av resurspoolerna visas de i resursplaneraren, men deras tillgänglighet anges till noll timmar med början det datum då de schemalagts för inaktivering.

Resursplaneraren tar hänsyn till användarnas alla roller och aktiviteternas planerade slutförandedatum och beräknar resurser utifrån detta.

Mer information om resursplaneraren finns i [Översikt över resursplaneraren](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

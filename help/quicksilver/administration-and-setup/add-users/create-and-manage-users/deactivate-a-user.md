---
title: Inaktivera eller återaktivera en användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Workfront-administratör kan du inaktivera eller återaktivera en användare.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Inaktivera eller återaktivera en användare

>[!IMPORTANT]
>
>Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
>
>Instruktioner om hur du inaktiverar en användare i Adobe Admin Console finns i avsnittet Ta bort användare i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) eller kontakta din Adobe Admin Console-administratör.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Dina användare kan lämna organisationen och du kan behöva ta bort dem från Adobe Workfront. De bör inte vara aktiva i systemet eftersom detta skulle skapa förvirring för andra användare när de lägger till dem i uppdateringar eller tilldelar dem arbete. När du inaktiverar en användare ser andra användare inte längre sitt namn när de söker efter personer i systemet.

Administratörer kan se inaktiva användare under Konfigurera.

Du kan återaktivera en användare när som helst.

>[!IMPORTANT]
>
>Vi rekommenderar att du inaktiverar användare som har lämnat organisationen i stället för att ta bort dem. Om en användare tas bort går all historik i Workfront som är kopplad till den användaren förlorad. Detta inkluderar deras arbetsuppgifter, deras koppling till anteckningar, timmar, dokument och alla andra objekt som de en gång har skapat.
>
>När du inaktiverar en användare i Workfront tas användarens licenser bort både för Workfront och för digitalt korrektur. Dessutom kan användaren inte längre tilldelas arbete. När en användare inaktiveras blir användarens Workfront-licens och korrekturlicens tillgängliga och kan användas av en annan användare. all annan information i den inaktiverade användarens profil förblir oförändrad.
>
>Mer information om hur borttagning och inaktivering av användare påverkar finns i [Ta bort användare](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Åtkomstkrav

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
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> ange din åtkomstnivå som <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst en av de två <b>Användaradministratör</b> alternativ aktiverade under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om användaren <b>Administratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om <b>Användare</b> ange en åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Inaktivera en användare

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).

1. Markera en användare och klicka på ikonen Mer ![](assets/more-icon.png)och sedan klicka **Inaktivera**.

1. Klicka **Inaktivera** i rutan som visas.

## Schemalägg användare för inaktivering

Som chef kan du markera användare för inaktivering innan de faktiskt lämnar organisationen. Om du till exempel arbetar med en användare som är bunden enligt avtal finns de i ditt system under en begränsad tidsperiod och du vet när de upphör. Du kan schemalägga att de ska inaktiveras det datumet.

Workfront-administratörer och användare av Planera licenser kan se avaktiveringsdatumet i sin användarprofil.

Så här schemalägger du en användare för inaktivering:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).

1. Välj användarens namn.

   eller

   (Valfritt) Välj flera användare för att schemalägga att de ska inaktiveras gruppvis.

1. Klicka på ikonen Redigera ![](assets/edit-icon.png).
1. I rutan Redigera användare som visas klickar du på **Resursplanering** att åka till det området.
1. Aktivera **Schemalägg inaktivering** alternativ.

1. I kalendern som visas anger du datum och tid för **Schemalagt inaktiveringsdatum**.

   >[!NOTE]
   >
   >* I tidsrutan kan du bara välja hela timsteg, inte minuter.
   >* Om du väljer en tid för den aktuella dagen som har gått schemalägger Workfront avaktiveringen för följande dag kl. 12:00. Den valda tiden matchar datorns tidszon för användaren som schemalägger inaktiveringen.


1. Klicka **Spara ändringar**.

   Användaren inaktiveras den valda dagen ibland efter den valda tiden. Om du har valt att inaktivera flera användare samtidigt inaktiveras alla markerade användare den valda dagen ibland efter den valda tiden.

Vi rekommenderar att du skapar en rapport för användare som du har schemalagt för inaktivering, så att du håller dig informerad om vilka användare som kommer att inaktiveras. Det finns ingen bekräftelse på att inaktiveringen skedde när användarna inaktiverades.

## Återaktivera en användare

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).

1. Markera en användare och klicka på ikonen Mer ![](assets/more-icon.png)och sedan klicka **Aktivera**.

1. Tilldela en ny **Åtkomstnivå** i listrutan.

### Korrekturera påverkan när du återaktiverar en användare

Inaktiverade användare förlorar sin tilldelade standardkorrekturroll och sin korrekturlicens (om du har en äldre Workfront Premium-plan). Om du väljer att återaktivera användaren måste du:

* Tilldela om licensen (om du har en äldre Workfront Premium-plan). Mer information om Workfront korrekturplaner finns i [Tillgång till korrekturfunktioner i Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Kontrollera att de har rätt korrekturroll. Återaktiverade korrekturanvändare tilldelas det som anges som standardkorrekturroll för nya användare. Se [Konfigurera standardspråkroller](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) för mer information.

## Inaktivera Workfront-administratörer och avtalslicensanvändare

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

Mer information om resursplaneraren finns i [Översikt över resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

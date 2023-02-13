---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Dela en rapport i Adobe Workfront
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera rapporter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till problem finns i Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Dela en rapport i Adobe Workfront

Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera rapporter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till problem finns i [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera specifika rapporter som du har åtkomst till att dela. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

## Åtkomstkrav

Du måste ha följande för att kunna dela objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller högre till rapporter, instrumentpaneler, kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för rapporten</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när det gäller att dela rapporter

Förutom övervägandena nedan, se även [Dela rapporter, kontrollpaneler och kalendrar](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Du kan dela rapporter som du skapar med andra personer, team, grupper, jobbroller eller företag. Du kan också dela rapporter som andra har skapat och som delats med dig.
* Du kan också dela dem med hela organisationen eller göra dem offentliga. När du gör en rapport offentlig genereras en URL som kan delas med andra.
* Du kan dela en enskild rapport eller dela flera rapporter från en lista med rapporter.

## Olika sätt att dela rapporter

Du kan dela rapporter i Workfront på följande sätt:

* Manuellt, enligt beskrivningen i [Dela en rapport](#share-a-report) nedan.
* Genom att automatiskt ärva behörigheten Visa från en kontrollpanel som innehåller den delade rapporten. Mer information om hur du visar ärvda behörigheter för objekt finns i [Visa ärvda behörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Dela en rapport {#share-a-report}

Att dela en eller flera rapporter från en lista är identiskt.

1. Gå till en lista med rapporter och välj en eller flera rapporter. Klicka sedan på **Dela**.

   eller

   Klicka på namnet på en rapport och klicka sedan på **Rapportåtgärder >****Delning**.

   ![](assets/qs-report-actions-sharing.png)

1. I rutan som visas i **Lägg till personer, team, roller, grupper eller företag ...** börja skriva namnet på användaren, teamet, jobbrollen, gruppen eller företaget som du vill dela rapporten med och tryck sedan på **Retur** när namnet visas.

1. Om du vill justera åtkomstnivån för ett namn som du har lagt till klickar du på den nedrullningsbara menyn till höger om namnet och väljer sedan ett av alternativen nedan.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Se det</td> 
      <td> <p>Gör att mottagaren kan visa rapporten i <strong>Rapporter</strong> <img src="assets/reports-in-main-menu.png"> och kör.</p> <p>Du kan klicka <strong>Avancerade inställningar</strong> för att ange om du vill att användaren eller användarna ska kunna <strong>Dela</strong> med alla i systemet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hantera det</td> 
      <td> <p>Ger mottagaren fullständig redigeringsåtkomst till rapporten.</p> <p>Du kan klicka <strong>Avancerade inställningar</strong> för att ange om du vill att användaren eller användarna ska kunna <strong>Ta bort</strong> rapporten från systemet, och <strong>Dela</strong> med alla i systemet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa de två föregående stegen för att lägga till andra namn i listan och konfigurera deras alternativ.
1. (Valfritt) Klicka på **Kugghjul** icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) i det övre högra hörnet av delningsrutan väljer du något av följande alternativ:

   * **Gör detta offentligt för externa användare:** Välj det här alternativet om du vill generera en URL som kan delas med andra. Alla som har URL-adressen kan komma åt rapporten utan att ha någon Adobe Workfront-licens.

      >[!CAUTION]
      >
      >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

      >[!NOTE]
      >
      >Om rapporten har en fråga och du delar den offentligt, måste de användare som kör rapporten vara inloggade på Workfront för att kunna köra rapporten med hjälp av uppmaningen. Om de inte kan logga in på Workfront ser de rapporten utan uppmaningen. Mer information om begränsningar för att dela rapporter med uppmaningar finns i avsnittet [Begränsningar för delning av obligatoriska rapporter](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) i artikeln [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Gör detta synligt för hela systemet:** Välj det här alternativet så att alla i Workfront som har åtkomst till rapporter kan se rapporten.

1. Klicka **Spara**.

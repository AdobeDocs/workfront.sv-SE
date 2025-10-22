---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Dela en rapport i Adobe Workfront
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera rapporter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till problem finns i Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Dela en rapport i Adobe Workfront

<!-- Audited: 11/2024 -->

Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera rapporter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till problem finns i [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera specifika rapporter som du har åtkomst till att dela. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

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
   <td> 
      <p>Ljus</p>
      <p>Granska</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller högre till rapporter, instrumentpaneler, kalendrar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre till rapporten</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller att dela rapporter

Förutom övervägandena nedan finns även [Dela rapporter, instrumentpaneler och kalendrar](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Du kan dela rapporter som du skapar med andra personer, team, grupper, jobbroller eller företag. Du kan också dela rapporter som andra har skapat och som delats med dig.
* Du kan dela rapporter med hela organisationen eller göra dem offentliga. När du gör en rapport offentlig genereras en URL som kan delas med andra.
* Du kan dela en enskild rapport eller dela flera rapporter från en lista med rapporter.

## Olika sätt att dela rapporter

Du kan dela rapporter i Workfront på följande sätt:

* Manuellt, enligt beskrivningen i avsnittet [Dela en rapport](#share-a-report) nedan.
* Automatiskt genom att ärva behörigheten Visa från en kontrollpanel som innehåller den delade rapporten. Mer information om hur du visar ärvda behörigheter för objekt finns i [Visa ärvda behörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Dela en rapport {#share-a-report}

Att dela en eller flera rapporter från en lista är identiskt.

1. Gå till en lista med rapporter och välj en eller flera rapporter. Klicka sedan på ikonen **Dela** ![Dela](assets/share-icon.png) .

   eller

   Klicka på namnet på en rapport och klicka sedan på **Rapportåtgärder** > **Delning**. Rutan **Dela [RAPPORTNAMN]** öppnas.

   ![Delningsalternativ](assets/unshimmed-report-actions-sharing.png)

1. I fältet **Bevilja rapportåtkomst till** börjar du skriva namnet på den användare, det team, den jobbroll, den grupp eller det företag som du vill dela rapporten med och väljer det sedan när den visas.

1. Om du vill justera åtkomstnivån för ett namn som du har lagt till klickar du på den nedrullningsbara menyn till höger om namnet och väljer sedan ett av alternativen nedan.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visa</td> 
      <td> <p>Gör att mottagaren kan visa rapporten i området <strong>Rapporter</strong> och köra den.</p> <p>Du kan klicka på ikonen <strong>Avancerade inställningar</strong> till höger för att ange om du vill att användaren eller användarna ska kunna <strong>dela</strong> den med någon i systemet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hantera</td> 
      <td> <p>Ger mottagaren fullständig redigeringsåtkomst till rapporten.</p> <p>Du kan klicka på ikonen <strong>Avancerade inställningar</strong> till höger för att ange om du vill att användaren eller användarna ska kunna <strong>ta bort</strong> rapporten från systemet och <strong>dela</strong> den med någon i systemet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa de två föregående stegen för att lägga till andra namn i listan och konfigurera deras alternativ.
1. (Valfritt) Klicka på listrutan **Endast inbjudna personer har åtkomst** i delningsrutan och välj sedan mellan följande alternativ:

   * **Endast inbjudna personer har åtkomst till**: Välj det här alternativet så att endast användare som har beviljats åtkomst till rapporten kan visa den.

   * **Alla i systemet kan visa**: Välj det här alternativet så att alla i Workfront som har åtkomst till rapporter kan visa rapporten.

1. (Valfritt) Klicka på ikonen **Kugghjulet** ![Inställningar för kugghjulsikonen](assets/gear-icon-settings-with-dn-arrow.jpg) i det övre högra hörnet av delningsrutan och välj sedan eventuellt följande alternativ:

   * **Gör detta offentligt för externa användare**: Välj det här alternativet om du vill generera en URL som kan delas med andra. Alla som har URL-adressen kan komma åt rapporten utan att ha någon Adobe Workfront-licens.

     >[!CAUTION]
     >
     >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

     >[!NOTE]
     >
     >Om rapporten har en fråga och du delar den offentligt, kommer de användare som kör rapporten via länken för offentlig delning inte att kunna köra rapporten via uppmaningen. De kommer att se rapporten utan att tillfrågas om de inte loggar in på Workfront och öppnar rapporten utan att använda länken för offentlig delning. Mer information om begränsningar för att dela rapporter med uppmaningar finns i avsnittet [Begränsningar för delning av promptrapporter](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) i artikeln [Lägga till en uppmaning i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicka på **Spara**.

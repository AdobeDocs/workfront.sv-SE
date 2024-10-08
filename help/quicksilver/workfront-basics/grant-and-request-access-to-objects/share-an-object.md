---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Dela ett objekt
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera objekt när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till objekt finns i Skapa eller ändra anpassade åtkomstnivåer.
author: Alina, Nolan
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 73f339b54985b725f265d582992a43b9f80dbd7c
workflow-type: tm+mt
source-wordcount: '1971'
ht-degree: 0%

---

# Dela ett objekt

<!--Audited: 01/2024-->

Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera objekt när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till objekt finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller redigera specifika objekt som du har skapat eller har åtkomst till att dela. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

Mer information om att dela behörigheter för objekt finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

I den här artikeln beskrivs hur du delar följande objekt:

* Projekt, uppgifter, problem
* Portfolio, program
* Dokument

Mer information om hur du delar alla andra objekt i Workfront finns i följande artiklar:

* Mer information om mallar finns i [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Korrektur finns i [Dela ett korrektur i Workfront Proof](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).
* Rapporter, kontrollpaneler och kalendrar finns i följande artiklar:

   * [Dela en rapport i Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Dela en kontrollpanel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Dela en kalenderrapport](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

  Se även [Dela rapporter, instrumentpaneler och kalendrar](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) för allmän information om delning av rapporter, instrumentpaneler och kalendrar.

* Information om filter, vyer och grupperingar finns i [Dela ett filter, en vy eller en gruppering](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Mer information om dokumentmappar finns i [Dela en dokumentmapp](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).
* Information om planer finns i [Dela en plan i scenarioplanen](../../scenario-planner/share-a-plan.md).

  Workfront Scenario Planner kan kräva ytterligare licens.

* Se [Dela ett mål i Workfront-mål](../../workfront-goals/workfront-goals-settings/share-a-goal.md) för mer information.

  Workfront Goals kan kräva ytterligare licens.

* Information om Workfront Planning-objekt finns i följande artiklar:

   * [Visa](/help/quicksilver/planning/access/share-views.md)
   * [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)

  Workfront Planning kräver ytterligare licens.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna dela objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Ny licens: Standard</p> 
   eller
   <p>Aktuell licens: Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela ett projekt, en uppgift eller ett ärende från sidan

1. Gå till sidan för projektet, aktiviteten eller problemet som du vill dela.

   Mer information om vilka objekt som kan delas finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicka på knappen **Dela** bredvid objektnamnet.

   ![](assets/new-share-button.png)

1. I rutan **Bevilja &lt; objektnamn > åtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela objektet med och klickar sedan på namnet när det visas i listrutan.

   ![](assets/new-share-button-add-people.png){width="350"}

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

   >[!TIP]
   >
   >Om du har flera entiteter med liknande namn visas alla under deras typ. Namnen på enheterna visas i alfabetisk ordning. Den ordning i vilken enhetstyperna visas är dock slumpmässig.
   >

1. (Valfritt) Upprepa steg 3 för varje användare, team, roll eller grupp som du vill ge åtkomst till objektet.

1. Ange behörigheter för varje användare, team, roll, grupp eller företag som du har lagt till i steg 3 genom att klicka på listrutan till höger om namnet och sedan välja den behörighetsnivå som du vill bevilja.

   ![](assets/new-share-permissions-dropdown.png)

   Information om hur du tar bort behörigheter från ett objekt finns i [Ta bort behörigheter från objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   Följande alternativ är tillgängliga:

   * **Visa:** Användare kan granska och dela objektet.
   * **Contribute**: Användare kan göra uppdateringar, logga information, göra mindre ändringar och dela, plus alla visningsbehörigheter.
   * **Hantera:** Användare har fullständig åtkomst till objektet utan administratörsbehörighet (som ges på åtkomstnivå). Dessutom har de alla behörigheterna Visa och Contribute.

     >[!NOTE]
     >
     >Workfront-administratören eller objektskaparen kan ta bort behörigheter från dessa entiteter.

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för objektet.

   ![](assets/new-share-advanced-permissions-dropdown.png)

   Visa, Hantera och Contribute har olika avancerade alternativ beroende på vilket objekt som är markerat.

   Mer information om behörighetsnivåer finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Om du vill göra det här objektet tillgängligt för alla användare i systemet klickar du på listrutan under **Vem har åtkomst** och sedan på **Alla i systemet kan visa** i listrutan.

   ![](assets/new-share-everyone-access.png)

   Alla användare kan se objektet baserat på de behörigheter som du anger.

1. (Valfritt och villkorligt) När du delar ett projekt klickar du på ikonen **Kugga** ![](assets/gear-icon-settings.png) och markerar sedan kryssrutan bredvid **Ange som mall för projektåtkomst** för att ange behörigheterna som en mall.

   När du har definierat behörigheter för ett projekt tillämpas dessa behörigheter automatiskt nästa gång du skapar ett projekt från början.

   >[!NOTE]
   >
   >Projektets åtkomstmall åsidosätter delningsstandardinställningarna som du har fått av Workfront-administratören på din åtkomstnivå.\
   >Mer information om hur du anger delningsstandardvärden för projekt på åtkomstnivå finns i [Bevilja åtkomst till projekt](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->

   Du kan ange behörigheter för de projekt som ska skapas från en mall när du delar mallen. Mer information finns i [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (Villkorligt) Om du vill dela objektet med externa användare klickar du på **Kopiera länk** och distribuerar sedan länken till externa användare.

   Alla användare med länken kan visa objektet.

   >[!CAUTION]
   >
   >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

1. Klicka på **Spara**.

## Dela ett dokument, en portfölj eller ett program från sidan

1. Gå till dokumentets, portföljens eller programmets sida som du vill dela.

   Mer information om vilka objekt som kan delas finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. För portföljer och program:

   Klicka på knappen **Dela** bredvid objektnamnet.

   ![](assets/new-share-button-on-portfolio.png)

   eller

   För dokument:

   Klicka på ikonen **Mer** ![](assets/more-icon.png) bredvid objektnamnet och klicka sedan på **Dela**.

   ![](assets/share-a-document-350x160.png)

1. I fältet **Ge &lt; Objektnamn > åtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela objektet med och klickar sedan på namnet när det visas i listrutan.

   ![](assets/portfolio-access-box.png)

   >[!TIP]
   >
   >* Om du har flera entiteter med liknande namn visas alla under deras typ. Namnen på enheterna visas i alfabetisk ordning. Den ordning i vilken enhetstyperna visas är dock slumpmässig.
   >
   >* Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. (Valfritt) Upprepa steg 3 för varje användare, team, roll eller grupp som du vill ge åtkomst till objektet.

1. Ange behörigheter för varje användare, team, roll, grupp eller företag som du har lagt till i steg 3 genom att klicka på listrutan och sedan välja den behörighetsnivå som du vill bevilja.

   Information om hur du tar bort behörigheter från ett objekt finns i [Ta bort behörigheter från objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   Följande alternativ är tillgängliga:

   * **Visa:** Användare kan granska och dela objektet.
   * **Hantera:** Användare har fullständig åtkomst till objektet utan administratörsbehörighet (som ges på åtkomstnivå). Dessutom har de alla behörigheterna Visa och Contribute.

     >[!NOTE]
     >
     >Workfront-administratören eller objektskaparen kan ta bort behörigheter från dessa entiteter.

     ![](assets/view-manage-sharing-options-for-portfolio-or-document.png)

1. (Valfritt) Klicka på **Avancerade inställningar** om du vill konfigurera specifika behörigheter för objektet.

   Behörigheterna Visa och Hantera har olika avancerade alternativ beroende på det markerade objektet.\
   Mer information om behörighetsnivåer finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Om du vill göra det här objektet tillgängligt för alla användare i systemet klickar du på ikonen **Kugga** ![](assets/gear-icon-settings-with-dn-arrow.jpg) och sedan på **Gör det synligt i hela systemet** i listrutan.

   Alla användare kan se objektet baserat på de behörigheter som du anger.

1. (Valfritt) Om du vill göra objektet offentligt klickar du på **Gör det offentligt för externa användare**.

   >[!TIP]
   >
   >Det här alternativet är inte tillgängligt för alla objekt.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png){width="350"}

1. (Villkorligt) Om du har gjort objektet offentligt för externa användare klickar du på **kopiera länken** och distribuerar sedan länken till externa användare.

   Alla användare med länken kan visa objektet.

   >[!CAUTION]
   >
   >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

1. Klicka på **Spara**.

## Dela enstaka objekt eller gruppobjekt från en lista

1. Gå till listan som innehåller de objekt som du vill dela.

   Mer information om vilka objekt som kan delas finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicka i kryssrutan bredvid de objekt som du vill dela och klicka sedan på ikonen **Dela** ![](assets/share-icon.png) överst på sidan.

   Rutan **&lt; Objekt > Åtkomst** öppnas.

   ![](assets/list-share-object-select.png){width="350"}

1. I rutan **Redigera &lt; Objektnamn > åtkomst för** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela objekten med och klickar sedan på namnet när det visas i listrutan.

   ![](assets/list-share-add-people.png){width="350"}

   >[!TIP]
   >
   >* Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.
   >
   >
   >* Om du har flera entiteter med liknande namn visas alla under deras typ. Namnen på enheterna visas i alfabetisk ordning. Den ordning i vilken enhetstyperna visas är dock slumpmässig.
   >

1. (Valfritt) Upprepa steg 3 för varje användare, team, roll eller grupp som du vill ge åtkomst till objekten.

1. Ange behörigheter för varje användare, team, roll, grupp eller företag som du har lagt till i steg 3 genom att klicka på listrutan till höger om namnet och sedan välja den behörighetsnivå som du vill bevilja.

   Information om hur du tar bort behörigheter från ett objekt finns i [Ta bort behörigheter från objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

   Följande alternativ är tillgängliga:

   * **Visa:** Användare kan granska och dela objektet.
   * **Contribute**: Användare kan göra uppdateringar, logga information, göra mindre ändringar och dela, plus alla visningsbehörigheter.

     >[!TIP]
     >
     >Du kan bara ge Contribute behörigheter till följande objekt:
     >
     >* Projekt
     >* Uppgifter
     >* Problem
     >

   * **Hantera:** Användare har fullständig åtkomst till objektet utan administratörsbehörighet (som ges på åtkomstnivå). Dessutom har de alla behörigheterna Visa och Contribute.

     >[!NOTE]
     >
     >Workfront-administratören eller objektskaparen kan ta bort behörigheter från dessa entiteter.

1. (Valfritt) Klicka på **Avancerade inställningar** om du vill konfigurera specifika behörigheter för objektet.

   Visa, Hantera och Contribute har olika avancerade alternativ beroende på vilket objekt som är markerat.\
   Mer information om behörighetsnivåer finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. (Valfritt) Om du vill göra det här objektet tillgängligt för alla användare i systemet klickar du på ikonen **Kugga** ![](assets/gear-icon-settings-with-dn-arrow.jpg) och sedan på **Gör det synligt i hela systemet** i listrutan.

   Alla användare kan se objekten baserat på de behörigheter som du anger.

1. (Valfritt och villkorligt) När du delar ett projekt klickar du på ikonen **Kugga** ![](assets/gear-icon-settings-with-dn-arrow.jpg) och sedan på **Ange som mall för projektåtkomst** i listrutan för att ange behörigheterna som en mall.

   När du har definierat behörigheter för ett projekt tillämpas dessa behörigheter automatiskt nästa gång du skapar ett projekt från början.

   >[!NOTE]
   >
   >Projektets åtkomstmall åsidosätter delningsstandardinställningarna som du har fått av Workfront-administratören på din åtkomstnivå.\
   >Mer information om hur du anger delningsstandardvärden för projekt på åtkomstnivå finns i [Bevilja åtkomst till projekt](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->

   Du kan ange behörigheter för de projekt som ska skapas från en mall när du delar mallen. Mer information finns i [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (Valfritt) Klicka på **Gör detta offentligt för externa användare** om du vill göra objektet/objekten offentliga.

   >[!TIP]
   >
   >Det här alternativet är inte tillgängligt för alla objekt.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png){width="350"}

1. (Villkorligt) Om du har gjort objektet/objekten offentliga för externa användare klickar du på **kopiera länken** och distribuerar sedan länken till externa användare.

   Alla användare med länken kan visa objektet.

   >[!CAUTION]
   >
   >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

1. Klicka på **Spara**.

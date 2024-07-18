---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera implementeringsdatum för aktiviteter och ärenden
description: Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i Genomför-datumöversikt.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# Uppdatera implementeringsdatum för aktiviteter och ärenden

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön för alla kunder, eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Mer information om den aktuella versionen finns i [Översikt över utgåvan för tredje kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Åtkomstkrav

<!--Audited: 01/2024-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
   För de nya licenserna:
   <ul>
   <li><p>Standard för uppgifter</p> </li>
   <li><p>Medarbetare eller högre för problem</p></li>
   </ul>
   För aktuella licenser:
<ul>
   <li><p>Arbeta eller högre för uppgifter</p></li> 
   <li><p>Begär eller högre för problem</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och ärenden</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteten eller problemet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Innan du kan redigera implementeringsdatumet för en uppgift eller utgåva måste du tilldelas den uppgift eller utgåva vars implementeringsdatum du måste uppdatera.

## Uppdatera implementeringsdatum för aktiviteter och ärenden


Du kan uppdatera implementeringsdatumet för en uppgift eller ett problem i följande områden i Workfront:

* Avsnittet Information om en uppgift eller ett problem
* <span class="preview">Aktivitets- eller problemhuvudet</span>

  <span class="preview">Din Workfront- eller gruppadministratör måste lägga till implementeringsdatumet i huvud för aktiviteten eller utgåvan av din layoutmall för att kunna visa det från aktivitets- eller utgivningssidan.
Mer information finns i [Anpassa objektrubriker med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

Uppdateringen av implementeringsdatumet är identisk för uppgifter och utgåvor.

>[!NOTE]
>
>Du kan be din system- eller gruppadministratör att lägga till fältet Genomför datum på panelen Sammanfattning för att göra det enklare att uppdatera det i olika områden av Workfront.
>
>Mer information finns i följande artiklar:
>
>* [Sammanfattningsöversikt](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Anpassa hem och sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Gå till en aktivitet eller ett problem som du har tilldelats som **ägare**.

   Mer information om hur du tar reda på vem som är aktivitetsägare för ett problem eller en uppgift finns i avsnittet [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">(Villkorligt och valfritt) Om Workfront- eller gruppadministratören har lagt till implementeringsdatumet i huvud för aktiviteten eller utgåvan klickar du på fältet **Bekräftelsedatum** i huvudet och väljer sedan ett datum i kalendern. Om implementeringsdatumet inte finns i huvudet fortsätter du med följande steg. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

1. Klicka på **Uppgiftsinformation** eller **Ärendeinformation** i den vänstra panelen.
1. Klicka på **Översikt** för att expandera den.
1. Uppdatera fältet **Verkställ datum**.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicka på **Spara ändringar**.

   När du har gjort den här ändringen händer följande:

   * Bekräftelsedatumet och det planerade slutförandedatumet för aktiviteten eller utgåvan är inte längre desamma.

     Istället ändras datumet för implementering och det beräknade slutförandedatumet för aktiviteten eller utgåvan.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Projektägaren meddelas i ett meddelande från Workfront i appen om att du har föreslagit ett nytt implementeringsdatum för uppgiften eller utgåvan.
   * Projektägaren meddelas i uppdateringsavsnittet att du har föreslagit ett nytt implementeringsdatum och de kan för närvarande uppdatera det planerade slutförandedatumet för aktiviteten eller utgåvan så att det matchar det implementeringsdatum du föreslog.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Mer information om de meddelanden och uppdateringar som utlöses av den här ändringen finns i avsnittet&quot;Meddelanden och uppdateringar som utlöses av ändring av implementeringsdatumet&quot; i artikeln [Bekräfta datumöversikt](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
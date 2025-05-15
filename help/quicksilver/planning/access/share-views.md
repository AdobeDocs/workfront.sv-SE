---
title: Dela vyer
description: Du kan dela en vy med andra för att säkerställa samarbete när du använder Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: eb3db3b056cea359f77e56f77d6e9520954e2abb
workflow-type: tm+mt
source-wordcount: '1657'
ht-degree: 0%

---


# Visa

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan dela en vy med andra för att säkerställa samarbete när du arbetar med poster i Adobe Workfront Planning.

>[!IMPORTANT]
>
>* Om du ger behörighet till en arbetsyta ger det inte andra användare behörighet till vyerna på posttypssidorna. Du måste tilldela behörigheter till enskilda vyer på en posttypsida för att kunna dela dem med andra användare.
>
>* Att bevilja behörigheter till en vy påverkar inte behörigheterna att visa posterna. Registreringsbehörigheter beviljas genom att arbetsytor för delning delas.
>
>* När du delar en vy ger du andra behörighet att komma åt alla element i vyn. Om du till exempel ger dem behörigheten Hantera för en vy kan de ändra grupperingen, filtret, sorteringen eller utseendet på fält.


Du kan dela en vy med följande enheter:

* Internt, med Workfront användare, grupper, team, företag och arbetsroller
* Offentligt, med användare utanför Workfront

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Din organisation måste vara registrerad på Adobe Unified Experience för att användare ska kunna begära och bevilja behörigheter för en vy från en behörighetsbegäran. </p>
<p>Användare måste läggas till i Adobe Admin Console för att få behörighet till Workfront Planning-vyer.</p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  <p>Hantera behörigheter till en vy</p>  
   <p>Endast användare med behörigheten Hantera på en arbetsyta kan dela en vy offentligt.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller planeringsområdena.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer planeringsområdet aktiverat som standard.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på vid vydelning

* Allmän information om delning av objekt i Workfront Planning finns även i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Du kan ge interna Workfront-användare behörigheten Visa eller Hantera för en vy.

* Användare med behörigheten Hantera kan ändra visningsinställningarna, dela, duplicera eller ta bort dem.

* Du kan dela vyer med personer utanför organisationen via en offentlig länk.

* När du delar en vy offentligt är länken tillgänglig för alla utanför företaget under en begränsad tid, vilket anges med utgångsdatumet. Det krävs ingen inloggning för att visa den delade vyn.

* Personer utanför organisationen som har åtkomst till en vy kan inte skapa andra vyer, redigera den delade vyn eller lägga till, ta bort eller redigera postinformation i vyn.

## Dela behörigheter till en vy internt

Du kan dela vyer som du har skapat eller vyer som du har behörigheten Hantera med användare, grupper, team, företag och jobbroller i Workfront Planning.

>[!NOTE]
>
>Systemadministratörer kan inte visa eller dela vyer som de inte själva skapat. De kan bara komma åt eller dela vyer som delas med dem.
>
>Systemadministratörer kan bara ha behörigheten Hantera för en vy.

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill dela och klicka sedan på ett posttypskort.

   Då öppnas posttypssidan.

1. <span class="preview">Håll markören över den vy du vill dela på fliken Visa och klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om vynamnet. Klicka sedan på **Dela**. </span>

   <span class="preview">![Mer meny för en vy](assets/more-menu-for-views-expanded-with-share-option.png) </span>

   Fliken **Intern delning** bör vara markerad som standard.

1. (Valfritt) Välj bland följande alternativ i området **Vem har åtkomst**:

   * **Endast inbjudna personer har åtkomst till**: Du måste ange användare, grupper, team, företag eller jobbroll som du vill dela vyn med. Det här är standardalternativet.

     >[!NOTE]
     >
     >   Förutom team, grupper, företag och jobbroller kan du bara dela med användare som har lagts till i Adobe Admin Console.


   * **Alla på arbetsytan kan visa**: Alla användare som har behörighet att visa eller högre på arbetsytor kan komma åt vyn.

1. I fältet **Bevilja åtkomst till den här vyn** börjar du skriva namnet på en användare, en grupp, ett team, företag eller en jobbroll och klickar sedan på den när den visas i listan.

   ![Dela en vy med grupper](assets/sharing-a-view-ui-with-groups.png)

1. Välj någon av följande behörighetsnivåer i listrutan:
   * Visa
   * Hantera

     Mer information om behörighetsnivåer och vilka åtgärder användare kan utföra för varje nivå finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratörer får alltid behörigheten Hantera för vyer som delas med dem.

1. Klicka på **Kopiera länk** för att kopiera en länk till vyn till Urklipp.
1. Klicka på **Spara**.

   Vyn uppdateras med en personikon ![Vyn som delas med andra ikoner](assets/view-shared-with-others-people-icon.png) för att ange att vyn nu delas med andra användare.

   >[!TIP]
   >
   >Vyer utan personer eller globala ikoner är vyer som du har skapat och som inte delas med andra. Vyer som inte delas visas bara för dig.

1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt posttypssidan och visa den i den valda vyn.

## Dela behörigheter till en vy offentligt

Du kan dela vyer som du har skapat eller vyer som du har behörigheten Hantera med personer som inte har någon Workfront-licens och som kan vara externa för din organisation.

>[!IMPORTANT]
>
>Endast användare med behörigheten Hantera på en arbetsyta kan dela arbetsytans vyer offentligt.


Så här delar du en vy offentligt i Workfront Planning:

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill dela och klicka sedan på ett posttypskort.

   Då öppnas posttypssidan.

1. Håll markören över den vy du vill dela på fliken Visa och klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om vynamnet. Klicka sedan på **Dela**.

   ![Fler menyer för vyer utökade med delningsalternativ](assets/more-menu-for-views-expanded-with-share-option.png)

1. Klicka på **Offentlig delning**.

   ![Fliken Dela offentligt för vyer](assets/public-sharing-tab-for-views.png)

1. Aktivera inställningen **Skapa offentlig länk**.

   En länk blir tillgänglig. Det här är en offentlig länk. När de delas kan alla som har länken, även personer utanför organisationen, få åtkomst till posttypssidan och visa poster och fält på sidan.

1. Klicka på ikonen **Kopiera länk** ![Kopiera länkvy](assets/copy-link-view.png) för att kopiera länken till Urklipp.

1. Ange ett datum manuellt eller använd kalendern i fältet **Länkens förfallodatum** för att välja ett förfallodatum för den offentliga länken. Postsidvyn är inte tillgänglig efter det valda datumet.

1. Klicka på **Spara**.

   Vyn uppdateras med den globala ikonen ![Offentlig delad vy markerad](assets/public-shared-view-icon-highlighted.png) för att visa att vyn delas offentligt.

   >[!TIP]
   >
   >Vyer utan personer eller globala ikoner är vyer som du har skapat och som inte delas med andra. Vyer som inte delas visas bara för dig.


1. (Valfritt) Klistra in länken som du kopierade till ett e-postmeddelande, chattmeddelande, dokument eller i en Workfront-kommentar för att dela den med andra.

## Bevilja behörigheter för en vy från en behörighetsbegäran

Användare som har åtkomst till en länk till en vy som de inte har behörighet till kan begära behörighet till vyn. Alla användare med behörigheten Hantera för vyn får behörighetsbegäran och kan bevilja eller neka behörigheter.

1. (Villkorligt) Om du är vyhanterare kan du få en begäran från en annan användare om att få åtkomst till vyn i följande områden:

   * Ett meddelande i appen

     ![Meddelande i appen om åtkomstbegäran för vyn](assets/in-app-notification-for-access-request-for-view.png)
   * Ett e-postmeddelande

     ![Meddelande i appen om åtkomstbegäran för vyn](assets/in-app-notification-for-access-request-for-view.png)
1. (Villkorligt) Klicka på meddelandet i appen i meddelandefältet i Workfront
eller
Klicka på **Visa alla meddelanden** i e-postmeddelandet och klicka sedan på meddelandet i listan.

   Rutan **Väntande åtkomstbegäranden** visas.

   ![Godkännanderuta för meddelandelista](assets/notifications-list-approval-box.png)
1. (Valfritt) För den användare vars behörigheter du vill godkänna väljer du något av följande alternativ på den nedrullningsbara menyn till höger om användarens namn:
   * **Visa**
   * **Hantera**
1. Markera den användare som du vill godkänna eller neka behörighet för och klicka sedan på **Godkänn alla** eller **Neka alla**.
1. Klicka på vänsterpilen till vänster om **Väntande åtkomstbegäranden** och klicka sedan på **Spara**.

   Om du godkände begäran läggs användarna till i delningsrutan för vyn. Användaren som begär behörighet får en e-postbekräftelse på att deras begäran har godkänts. <!--will they also get an in-app notification??-->

## Ta bort behörigheter till en vy

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill sluta dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.
1. Håll muspekaren över fliknamnet för den vy du vill ta bort delning från och klicka på menyn **Mer** ![Mer](assets/more-menu.png) och sedan på **Dela**.
1. Så här tar du bort den interna delningen av en vy:

   1. Kontrollera att fliken **Intern delning** är markerad.
   1. Hitta den användare, grupp, team, företag eller jobbroll du vill ta bort, utöka listrutan Behörigheter till höger om namnet på den enhet du delar vyn med och klicka sedan på **Ta bort**.

1. Så här tar du bort den offentliga delningen av en vy:

   1. Klicka på fliken **Offentlig delning**.
   1. Avmarkera alternativet **Skapa offentlig länk**.

1. Klicka på **Spara**.

   Personer har inte längre åtkomst till vyn. Användarna som har tagits bort från vyn får inget meddelande om att de inte längre har åtkomst till den.

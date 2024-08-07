---
title: Visa
description: Du kan dela en vy med andra för att säkerställa samarbete när du använder Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Visa

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

* Internt, med Workfront användare och grupper
* Offentligt, med användare utanför Workfront

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en vy</p>  
   <p>Endast användare med behörigheten Hantera på en arbetsyta kan dela en vy offentligt.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på vid vydelning

* Du kan ge interna Workfront-användare behörigheten Visa eller Hantera för en vy.

* Användare med behörigheten Hantera kan ändra visningsinställningarna, dela, duplicera eller ta bort dem.

* Du kan dela vyer med personer utanför organisationen via en offentlig länk.

* När du delar en vy offentligt är länken tillgänglig för alla utanför företaget under en begränsad tid, vilket anges med utgångsdatumet. Det krävs ingen inloggning för att visa den delade vyn.

* Personer utanför organisationen som har åtkomst till en vy kan inte skapa andra vyer, redigera den delade vyn eller lägga till, ta bort eller redigera postinformation i vyn.

## Dela behörigheter till en vy internt

Du kan dela vyer som du har skapat eller vyer som du har behörigheten Hantera med användare eller grupper i Workfront.

>[!NOTE]
>
>Systemadministratörer kan inte visa eller dela vyer som de inte själva skapat. De kan bara komma åt eller dela vyer som delas med dem.
>
>Systemadministratörer kan bara ha behörigheten Hantera för en vy.

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill dela och klicka sedan på ett posttypskort.

   Då öppnas posttypssidan.

1. Håll markören över den vy du vill dela på fliken Visa och klicka på menyn **Mer** ![](assets/more-menu.png) till höger om vynamnet. Klicka sedan på **Dela**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   Fliken **Intern delning** bör vara markerad som standard.

1. (Valfritt) Välj bland följande alternativ i området **Vem har åtkomst**:

   * **Endast inbjudna personer har åtkomst till**: Du måste ange användare eller grupper som du vill dela vyn med. Det här är standardalternativet.
   * **Alla på arbetsytan kan visa**: Alla användare som har behörighet att visa eller högre på arbetsytor kan komma åt vyn.

1. I fältet **Bevilja åtkomst till** kan du börja skriva namnet på en användare eller grupp och sedan klicka på den när den visas i listan.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Välj någon av följande behörighetsnivåer i listrutan:
   * Visa
   * Hantera

     Mer information om behörighetsnivåer och vilka åtgärder användare kan utföra för varje nivå finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratörer får alltid behörigheten Hantera för vyer som delas med dem.

1. Klicka på **Kopiera länk** för att kopiera en länk till vyn till Urklipp.
1. Klicka på **Spara**.

   Vyn uppdateras med en personikon ![](assets/view-shared-with-others-people-icon.png) som anger att vyn nu delas med andra användare.

   >>
   >[!TIP]
   >>
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

1. Håll markören över den vy du vill dela på fliken Visa och klicka på menyn **Mer** ![](assets/more-menu.png) till höger om vynamnet. Klicka sedan på **Dela**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Klicka på **Offentlig delning**.

   ![](assets/public-sharing-tab-for-views.png)

1. Aktivera inställningen **Skapa offentlig länk**.

   En länk blir tillgänglig. Det här är en offentlig länk. När de delas kan alla som har länken, även personer utanför organisationen, få åtkomst till posttypssidan och visa poster och fält på sidan.

1. Klicka på ikonen **Kopiera länk** ![](assets/copy-link-view.png) för att kopiera länken till Urklipp.

1. Ange ett datum manuellt eller använd kalendern i fältet **Länkens förfallodatum** för att välja ett förfallodatum för den offentliga länken. Postsidvyn är inte tillgänglig efter det valda datumet.

1. Klicka på **Spara**.

   Vyn uppdateras med den globala ikonen ![](assets/public-shared-view-icon-highlighted.png) som anger att vyn delas offentligt.

   >>
   >[!TIP]
   >
   >Vyer utan personer eller globala ikoner är vyer som du har skapat och som inte delas med andra. Vyer som inte delas visas bara för dig.


1. (Valfritt) Klistra in länken som du kopierade till ett e-postmeddelande, chattmeddelande, dokument eller i en Workfront-kommentar för att dela den med andra.

## Ta bort behörigheter till en vy

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill sluta dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.
1. Håll muspekaren över fliknamnet för den vy du vill ta bort delning från och klicka på menyn **Mer** ![](assets/more-menu.png) och sedan på **Dela**.
1. Så här tar du bort den interna delningen av en vy:

   1. Kontrollera att fliken **Intern delning** är markerad.
   1. Hitta användaren eller gruppen du vill ta bort, utöka listrutan med behörigheter till höger om användarens eller gruppens namn och klicka sedan på **Ta bort**.

1. Så här tar du bort den offentliga delningen av en vy:

   1. Klicka på fliken **Offentlig delning**.
   1. Avmarkera alternativet **Skapa offentlig länk**.

1. Klicka på **Spara**.

   Personer har inte längre åtkomst till vyn. Användarna som har tagits bort från vyn får inget meddelande om att de inte längre har åtkomst till den.
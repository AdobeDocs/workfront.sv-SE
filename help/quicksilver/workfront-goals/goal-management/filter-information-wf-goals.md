---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrera information i Adobe Workfront mål
description: Du kan visa mål som du eller någon annan har lagt till i Adobe Workfront-mål. Mer information om hur du skapar mål finns i Skapa mål i Adobe Workfront-mål. När du tittar på dina mål kan du filtrera information i Workfront-mål så att du bara ser de mål som är viktiga för dig.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# Filtrera information i Adobe Workfront-mål

<!--Audited for P&P only: 4/2025-->

Du kan visa mål som du eller någon annan har lagt till i Adobe Workfront-mål. Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md). När du tittar på dina mål kan du filtrera information i Workfront-mål så att du bara ser de mål som är viktiga för dig.

## Åtkomstkrav

>[!NOTE]
>
>Ditt företag kan välja att fortsätta använda Adobe Workfront-mål om de tidigare har köpt det här paketet. Du måste prata med din kontorepresentant för mer information.
>
>Adobe Workfront-mål går inte längre att köpa.

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront package</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens</td>
 <td>
 <p>Medarbetare eller högre</p>
<p>Begäran eller senare</p></td>
 </tr>
  <tr>
 <td role="rowheader">Åtkomstnivåkonfiguration</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målen för att visa dem</p>
  <p>Hantera behörigheter till målen för att redigera dem</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive systemadministratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
  <p>Or</p>
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Översikt över filter i Workfront-mål

>[!NOTE]
>
>För att effektivt hitta rätt mål rekommenderar vi att du använder filter i Workfront-mål. På så sätt kan du visa rätt information innan du börjar hantera mål som är viktiga för dig. Som standard visar Workfront-mål alla mål i systemet.

Du kan hitta och filtrera efter mål i följande avsnitt av målområdet i Workfront:

* Mållista
* Diagram
* Måljustering

Mer information om avsnitten i målområdet finns i [Översikt över avsnitten om Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Du kan konfigurera filter för ett avsnitt och de förblir beständiga när du flyttar till ett annat avsnitt av Workfront-målen.

Tänk på följande när du arbetar med filter i Workfront-mål:

* Du kan skapa och använda ett filter utan att spara det, eller så kan du spara ett filter och återanvända det senare.

  Följande scenarier finns:

   * När du sparar ett filter blir det standardfiltret för dig varje gång du loggar in på Workfront-mål.
   * När du tillämpar ett filter utan att spara det kan du återgå till de ursprungliga listorna genom att uppdatera sidan.

* Du kan bara visa och använda filter som du har skapat. Filter som skapas av andra användare visas endast för dessa användare.
* Du kan inte dela filter som du har skapat med andra användare.

## Använda ett snabbfilter i Workfront-mål

Du kan använda ett snabbfilter i en lista med mål om du bara vill hitta objekt som är viktiga för dig. Du kan inte spara snabbfilter och de är inte beständiga. Workfront rensar resultatet av ett snabbfilter när du uppdaterar sidan.

Mer information finns i [Använda snabbfiltret i en lista](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Skapa och använda ett filter i Workfront-mål

Processen för att skapa filter är densamma för alla avsnitt av Workfront-mål.

Du kan skapa ett filter från grunden eller redigera något av de inbyggda filtren.

1. Gå till Workfront mål.

   Mer information om åtkomst till Workfront-mål finns i [Åtkomst och öppna mål i Adobe Workfront-mål](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   Som standard visas avsnittet Mållista.

1. Klicka på **Filter** i det övre högra hörnet av listan.

   ![Filterikon](assets/filter-icon-and-label.png)

   Som standard använder Workfront filtret **Alla** som visar alla mål i systemet.

   >[!TIP]
   >
   >Du kan inte redigera eller ta bort filtret Alla.

1. Gör något av följande:

   * Klicka på något av följande fördefinierade filter om du bara vill visa mål för följande ägare:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Alla</td> 
        <td> <p>Alla mål i systemet, oavsett vem som skapade dem, vilken tidsperiod de har eller vem ägaren är. Det här är standardfiltret som du inte kan redigera. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Personligt</td> 
        <td>De mål som du är ägare till.</td> 
       </tr> 
       <tr> 
        <td>Mina team</td> 
        <td> <p>De mål som något av dina team har valts som ägare för. </p> <p><b>TIPS</b>

     Inga mål visas när du inte har tilldelats några team. </p> </td>
     </tr> 
       <tr> 
        <td>Mina grupper</td> 
        <td>De mål som någon av dina grupper har valts som ägare för. </td> 
       </tr> 
       <tr> 
        <td>Företag</td> 
        <td> <p>De mål som är kopplade till din organisation. </p> <p><b>TIPS</b>
        <p>I Adobe Workfront Goals visar filtret Company de mål som din organisation har valts som ägare för. </p> <p>Du kan inte söka efter företag som använder det här fältet. Som standard är det bara den organisation som äger din Workfront-instans som är vald. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Håll muspekaren över namnet på ett filter och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) bredvid namnet för att anpassa den och lägga till specifika namn på användare, team, grupper eller namnet på din organisation. Markera sedan den när de visas i listan.

   * Klicka på **Nytt filter** för att skapa ett nytt filter och välj sedan bland följande alternativ för att anpassa det nya filtret:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Period</td> 
        <td>Välj en tidsperiod i listrutan. Du kan välja flera tidsperioder. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Status</td> 
        <td> <p>Välj en status på den nedrullningsbara menyn bland följande alternativ:</p> 
         <ul> 
          <li> <p>Aktiv</p> </li> 
          <li> <p>Utkast</p> </li> 
          <li> <p>Inaktiv</p> </li> 
          <li> <p>Stängd</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Förlopp</td> 
        <td> <p>Välj ett förlopp i listrutan bland följande alternativ: </p> 
         <ul> 
          <li> <p>I problem</p> </li> 
          <li> <p>Risk</p> </li> 
          <li> <p>På mål</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Ägare</td> 
        <td> <p>Börja skriva namnet på en ägare och markera den när den visas i listan. </p> <p>Du kan skriva namnen på användare, team, grupper eller namnet på din organisation eller välja bland fördefinierade alternativ. </p> <p>Följande fördefinierade filteralternativ avser alltid den användare som är inloggad: </p> 
         <ul> 
          <li> <p><strong>Me</strong>: Visar mål där du är ägare.</p> </li> 
          <li> <p><strong>Mitt hemteam</strong> och <strong>Alla mina team</strong>: Visar mål där antingen ditt hemteam eller något av dina team har utsetts till ägare. </p> <p>Tips! Inga mål visas när du inte är tilldelad några team. </p> </li> 
          <li> <p><strong>Min hemgrupp</strong> och <strong>Alla mina grupper</strong>: Visar mål där din hemgrupp eller någon av dina grupper har angetts som ägare.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Valfritt) Klicka på **Återställ** i det nedre högra hörnet av filterrutan om du vill ta bort alla fält som du har markerat och börja skapa filtret från grunden.
1. (Valfritt) Klicka på **Använd** om du vill använda filtret utan att spara.

   Filtret visas i området **Osparat** i filterverktyget som **Nytt filter**.

   Du kan inte byta namn på ett osparat filter.

   Osparade filter tas bort från målområdet nästa gång du loggar ut från Workfront och loggar in igen.

   >[!TIP]
   >
   >Du kan bara ha ett osparat nytt filter åt gången.

1. Klicka på **Spara** om du vill spara filtret och använda det senare, lägg till ett namn för filtret i fältet **Lägg till filternamn** och klicka på **Klar**.

   Detta sparar filtret i avsnittet **Sparat** i filterverktyget. Du kan använda detta filter i framtiden.

   Det senast sparade och tillämpade filtret visas som standard nästa gång du loggar in på Workfront igen

1. (Valfritt) Klicka på den **vänsterriktade pilen** bredvid **Nytt filter** för att avsluta filterverktyget och återgå till filterlistan.
1. (Valfritt) Håll pekaren över namnet på ett anpassat filter, klicka på menyn **Mer**, klicka på **Ta bort** och sedan på **Ta bort**. Filtret tas bort och du kan inte återställa det.

   >[!TIP]
   >
   >Du kan inte ta bort något av de fördefinierade filtren.

1. Klicka på ikonen **X** i det övre högra hörnet av filterverktyget för att stänga filterverktyget.

   Namnet på det filter som används visas till höger om filterikonen i det övre högra hörnet av mållistan.

   Listan med mål filtreras efter filtervillkoren.

1. (Valfritt och villkorligt) När du visar mål i avsnittet Måljustering klickar du på **Visa dem** om du vill visa de filtrerade målen.

   ![Visa länkar för filtrerade objekt](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   Filternamnet visas med en gul kontur som anger att det ignoreras.

   ![Filtrera gula konturer](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Valfritt och villkorligt) Klicka på **Använd om filter** om du vill använda filtret och utesluta objekt som du visade i föregående steg.



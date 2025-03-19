---
title: Dela posttyper
description: Du kan dela en posttyp med andra för att säkerställa samarbete när du använder Adobe Workfront Planning.
hide: true
hidefromtoc: true
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 08c9eb508861d585d8f76de5bb523132f3be371f
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 0%

---

<!-- add these to metadata on release:

author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog-->

# Dela posttyper

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan dela en posttyp med andra för att säkerställa samarbete när du arbetar med poster i Adobe Workfront Planning.

>[!IMPORTANT]
>
>* Om du ger behörigheter till en arbetsyta får användarna som standard samma behörigheter som posttyperna på arbetsytan.
>* Dessutom kan du justera behörigheter för enskilda posttyper.
>* Du kan dock inte ge användare högre behörigheter för en posttyp än de behörigheter som de har för arbetsytan.
>* Personer med behörigheten Hantera på arbetsytan behåller alltid behörigheten Hantera för alla posttyper på arbetsytan. Deras behörigheter kan inte sänkas för posttyper, även när ärvda behörigheter är inaktiverade.
> 
> Mer information finns i avsnittet [Att tänka på när du delar posttyper](#considerations-when-sharing-record-types) i den här artikeln.

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
   <td>  <p>Hantera behörigheter till en posttyp</p>  
   <p>Endast användare med behörigheten Hantera på en arbetsyta kan dela behörigheten Hantera till en posttyp</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på vid delning av posttyper

* Allmän information om delning av objekt i Workfront Planning finns även i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

* För närvarande kan du uppnå följande när du delar posttyper:
   * Ge personer behörigheten Visa till en arbetsyta när du delar en posttyp med dem för första gången och de inte har några behörigheter till arbetsytan.

     Detta ger dem även behörigheten Visa för alla posttyper på arbetsytan.

     När du ger dem behörighet till posttypen finns det en indikation i delningsrutan om att de också läggs till på arbetsytan.
   * Gör posttypsvisningen till en enda vy för alla på arbetsytan (förutom för arbetsytehanterare) när du inaktiverar Ärvda behörigheter.

     Personer med behörigheten Hantera på arbetsytan har alltid behörigheten Hantera för posttyperna, även när du inaktiverar Ärvda behörigheter för posttypen.
  <!-- checking with Lilit - this doesn't make much sense: * Add people with Contribute permission to the workspace, who will retain Contribute permission to the record type. This way, only the selected people can manage records in the record type, while others can only view them. -->
   * Lägre behörighet för en posttyp. Du kan inte öka någons behörighet till en posttyp från vad de har på arbetsytan.

     Om någon till exempel har Contribute-behörighet till arbetsytan kan du ändra deras behörighet till en viss posttyp till Visa. Om de har behörigheten Visa på arbetsytan kan du inte ge dem Contribute-behörighet till någon posttyp.

* Det går inte att ta bort åtkomst till en posttyp för personer på arbetsytan. Alla har alltid minst behörigheten Visa.

* Du kan dela en posttyp internt med följande enheter:

   * Workfront användare, grupper, team, företag och jobbroller
* Du kan inte dela posttyper externt, med användare utanför Workfront.
* Om du vill ge en användare som inte har en arbetsytebehörighet som är högre än behörigheten Visa till en posttyp, måste du först dela arbetsytan med honom/henne med en högre behörighet än Visa.

## Dela behörigheter till en posttyp

Du kan justera behörigheter till enskilda posttyper på en arbetsyta om du har behörigheten Hantera på arbetsytan.

{{step1-to-planning}}

1. Öppna arbetsytan vars posttyper du vill dela och klicka sedan på ett posttypskort.

   Då öppnas posttypssidan.

1. Klicka på **Dela** i det övre högra hörnet av posttypen på fliken i valfri vy.

   Rutan **Dela** öppnas.

   ![Behörigheter för posttyper med ärvda behörigheter ](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Valfritt) Välj bland följande alternativ i området **Vem har åtkomst**: <!--the Only invited people is supposed to be removed - rewrite this - according to Vahan-->

   * **Endast inbjudna personer har åtkomst till**: Du måste ange användare, grupper, team, företag eller jobbroller som du vill dela vyn med.
   * **Alla på arbetsytan kan visa**: Alla användare som har behörighet att visa eller högre på arbetsytan kan komma åt vyn. Det här är standardalternativet. <!--rewrite this based on what Lilit says in the proof: At this point, once the inherited permissions are disabled, everyone in the workspace except workspace managers will have View permission to the record type because the "Everyone in the workspace can view"  setting cannot be changed. -->

1. (Valfritt) Expandera alternativet **Ärvda behörigheter** om du vill visa användare, team, grupper, företag eller jobbroller som ärver behörigheter från arbetsytan.

   >[!TIP]
   >
   >Du kan inte ta bort enskilda entiteter från listan Ärvda behörigheter.


1. (Valfritt och villkorligt) Om du vill dela posttypen med specifika entiteter och ge dem en annan åtkomst till posttypen än de redan har för arbetsytan gör du följande:

1. **Inaktivera** ärvda behörigheter.

   >[!TIP]
   >
   >Workspace-hanterare har fortfarande behörighet att hantera posttypen.

   1. I fältet **Bevilja åtkomst till den här posttypen** lägger du till de användare, team, grupper, företag eller jobbroller som du vill ge en annan behörighetsnivå till.
   1. Välj en behörighetsnivå.


   >[!IMPORTANT]
   >
   >* Du kan aldrig ge användare större behörigheter för en posttyp än de har på en arbetsyta.
   >* Du kan inte ge användare mindre behörighet än Hantera till en posttyp, om de har Hantera-behörighet till arbetsytan.
   >* Du kan ge användarna mindre behörighet till posttypen om de har Contribute-behörighet till arbetsytan.
   > Mer information finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Om du vill ge användare som inte har behörighet till arbetsytan åtkomst för att visa posttypen, kan du börja skriva namnet på en användare, en grupp, ett team, ett företag eller en jobbroll i fältet **Bevilja åtkomst till den här vyn** och sedan klicka på den när den visas i listan.

   Den entitet du har valt läggs till i posttypen och på arbetsytan med **Visa**-behörigheter.

   Systemadministratörer får alltid behörigheten Hantera för att registrera typer som delas med dem, och det finns en indikation på att en användare är systemadministratör.

1. Klicka på **Kopiera länk** om du vill kopiera en länk till posttypen till Urklipp.
1. Klicka på **Spara**.

   Posttypen delas nu med andra användare.

1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt posttypssidan och visa den i den valda vyn.

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

## Ta bort behörigheter till en posttyp

<!-- take this section out - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

{{step1-to-planning}}

1. Öppna arbetsytan vars posttyper du vill sluta dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.

1. Klicka på **Dela** i det övre högra hörnet av posttypen på fliken i valfri vy.

   Rutan **Dela** öppnas.
1. Hitta den användare, grupp, team, företag eller jobbroll vars behörigheter du vill ta bort, utöka den nedrullningsbara menyn Behörigheter till höger om namnet och klicka sedan på **Ta bort**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Ta bort alternativ i listrutan för posttypsdelning](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Klicka på **Spara**.

   Personer har inte längre åtkomst till posttypen. De kan fortfarande ha behörigheter till arbetsytan, såvida du inte också tar bort dem från arbetsytebehörigheterna.

   Användarna som har tagits bort från vyn får inget meddelande om att de inte längre har åtkomst till den.


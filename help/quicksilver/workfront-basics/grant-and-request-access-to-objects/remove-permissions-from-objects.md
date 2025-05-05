---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Ta bort behörigheter från objekt
description: Du kan ta bort andra användares behörigheter för objekt som du har åtkomst till Dela. Att ta bort behörigheter från objekt är identiskt för alla objekt som kan delas.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: ce7b475dbd11f9cfd7fcf9879c0f34bf993f9113
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Ta bort behörigheter från objekt

<!--Audited: 01/2024-->

Du kan ta bort andra användares behörigheter för objekt som du har åtkomst till Dela. Att ta bort behörigheter från objekt är identiskt för alla objekt som kan delas.

Liknande överväganden som för att dela objekt gäller för borttagning av behörigheter från objekt. Mer information finns i avsnittet [Att tänka på när du delar objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) i artikeln [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

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
   <td role="rowheader">Workfront-licens*</td> 
   <td> <p>Ny licens: Medarbetare eller högre</p>
   eller  
   <p>Aktuell licens: Begär eller högre</p>
   <p><b>ANMÄRKNING</b></p>

<p>Vissa objekt kräver högre åtkomst än Request. </p>

<p>För den nya licensen kan till exempel en medarbetare dela problem, men bara standardlicensanvändare kan dela ett projekt.</p>

<p>För den aktuella licensen kan en begärande dela utgåvor, men bara arbetare eller planerare kan dela ett projekt.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p> <p>Hantera behörigheter för att ta bort ärvda behörigheter för objekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort enheter från delningslistan för ett objekt {#remove-entities-from-the-sharing-list-of-an-object}

Du kan ta bort enheter (användare, jobbroller, team, grupper, företag) från delningslistan för ett objekt. Detta tar bort deras behörigheter till objektet.

1. Gå till objektet som du vill ta bort behörigheter från.

   Mer information om vilka objekt som kan delas finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Villkorligt) Gör följande för program, portföljer och dokument:

   1. Klicka på ikonen **Mer** ![Mer](assets/more-icon.png)bredvid objektnamnet och klicka sedan på **Dela** eller **Dela.**

      ![dela](assets/share-a-document-350x160.png)

   1. Klicka på **x** bredvid namnet på en användare, ett team, en grupp, ett företag eller en jobbroll för att ta bort dem i rutan för objektåtkomst.

      ![ta bort behörighet](assets/remove-permissions-on-portfolio.png)

   1. I listrutan **för**&#x200B;[ användarnamnet]s åtkomst till Workfront tas bort. Välj om du vill att deras åtkomst ska tas bort från det markerade objektet eller från alla underordnade objekt som är kopplade till det.

1. (Villkorligt) Gör följande för projekt, uppgifter och ärenden:

   1. Klicka på **Dela** till höger om objektets namn.

      ![dela](assets/new-share-button.png)
   1. Hitta den användare, roll, det team, den grupp eller det företag som du vill ta bort från objektet.
   1. Klicka på **Ta bort**.
I listrutan **Ta bort &lt; användarnamn > från** väljer du om du vill att deras åtkomst ska tas bort från det markerade objektet eller från alla underordnade objekt som är kopplade till det.

      ![ta bort](assets/remove-permissions-on-project-nwe-350x479.png)

   Följande scenarier finns:

   * Om du bara tar bort entiteten från objektet förlorar entiteten sina behörigheter för objektet och deras ärvda behörigheter till de underordnade objekten. Om de tidigare beviljats behörigheter till de underordnade objekten individuellt behåller de samma behörigheter för alla underordnade objekt som är kopplade till dem när du väljer det här alternativet.
   * Om du tar bort entiteten från objektet och alla underordnade objekt förlorar entiteten sina behörigheter till objektet och alla underordnade objekt, även när de tidigare fått individuell behörighet för varje underordnat objekt.

1. Klicka på **Spara**.

<!--
## Remove permissions from several objects in bulk

You can remove entities (users, job roles, teams, groups, companies) from several objects at a time when you bulk select them in a list.

>[!NOTE]
>
>You cannot view what access entities have for all the objects selected when you select them in bulk. You must know which entity you want to remove from the sharing of the objects selected before removing their permissions.

1. Go to the list of objects that you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Select several objects in the list, then click the **Share** icon ![share icon](assets/share-icon.png)at the top of the list. 
1. Type the name of the user, role, team, group, or company for which you want to remove the access in the **Edit `<Object Name>` access to** field. 
1. From the access drop-down menu, select **No Access**.

   ![remove in bulk](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the objects that you have selected, or from all other children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.

   **Example:** Select whether to remove permissions to just the tasks you selected in a list, or to the issues and documents attached to the tasks as well.

   ![access](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) To change permissions in bulk for several objects, select another level of sharing for the selected entity.

   For example, if they have Manage permissions, select Contribute or View instead. 

1. Click **Save**.

-->

## Ta bort ärvda behörigheter

Ärvda behörigheter kan tas bort från objekt, vilket gör det möjligt för ägare att specifikt identifiera vem som får åtkomst till underordnade objekt oavsett om en användare har åtkomst till ett överordnat objekt.

>[!IMPORTANT]
>
>Endast användare med behörigheten Hantera kan ta bort ärvda behörigheter.

Så här tar du bort ärvda behörigheter:

1. Gå till ett objekt som du har behörigheten Hantera för. Gå till exempel till en uppgift.
1. Gå till åtkomstrutan för objekt enligt beskrivningen i avsnittet [Ta bort entiteter från delningslistan för ett objekt](#remove-entities-from-the-sharing-list-of-an-object) i den här artikeln.
1. Välj **Inaktivera** bredvid **Ärvd behörighet** för att inaktivera.

   Detta garanterar att ingen som har behörighet till det överordnade objektet (till exempel projektet) har behörighet till den här uppgiften som standard. Du måste lista enskilda enheter i delningslistan för uppgiften för att kunna bevilja behörigheter för uppgiften.

   >[!TIP]
   >
   >Du kan inte ta bort enskilda enheter från listan Ärvda behörigheter. Du kan bara inaktivera ärvda behörigheter för alla enheter i listan.

1. Klicka på **Spara**. 

## Gör ett objekt privat

Om du har delat ett objekt i hela systemet, eller om du har delat det med externa användare genom att göra det offentligt, kan du göra det privat igen genom att ta bort behörigheten för hela systemet eller för offentliga användare. 

Mer information om hur du gör ett objekt tillgängligt för hela systemet, eller för allmänheten, finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Så här gör du ett objekt privat:

1. Gå till det objekt som du vill göra privat.\
   Navigera till exempel till en rapport.
1. Klicka på **Rapportera åtgärder** och sedan på **Dela**.

   ![gör privat](assets/report-permissions-make-private-nwe-350x477.png)

1. Klicka på kugghjulsikonen och avmarkera sedan **Gör den offentlig för externa användare**.
1. I listrutan **Vem har åtkomst** klickar du på **Endast inbjudna personer har åtkomst** för att sluta dela den med alla Workfront-användare.
1. Klicka på **Spara**.

---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Ta bort behörigheter från objekt
description: Du kan ta bort andra användares behörigheter för objekt som du har åtkomst till Dela. Att ta bort behörigheter från objekt är identiskt för alla objekt som kan delas.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Ta bort behörigheter från objekt

Du kan ta bort andra användares behörigheter för objekt som du har åtkomst till Dela. Att ta bort behörigheter från objekt är identiskt för alla objekt som kan delas. 

Liknande överväganden som för att dela objekt gäller för borttagning av behörigheter från objekt. Mer information finns i avsnittet [Att tänka på när du delar objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) i artikeln [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td role="rowheader">Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p>
   <p><b>ANMÄRKNING</b></p>

Vissa objekt kräver högre åtkomst än Request. En begärande kan till exempel dela problem, men bara arbetare eller planerare kan dela ett projekt.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p> <p>Hantera behörigheter för att ta bort ärvda behörigheter för objekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Ta bort enheter från delningslistan för ett objekt {#remove-entities-from-the-sharing-list-of-an-object}

Du kan ta bort enheter (användare, jobbroller, team, grupper, företag) från delningslistan för ett objekt. Detta tar bort deras behörigheter till objektet.

1. Gå till objektet som du vill dela.

   Mer information om vilka objekt som kan delas finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicka på **Mer** icon ![](assets/more-icon.png)bredvid objektnamnet och klicka sedan på **Delning** eller **Dela.**

   ![](assets/share-a-document-350x160.png)

1. Klicka på **x** bredvid namnet på en användare, ett team, en grupp, ett företag eller en jobbroll som ska tas bort i rutan för objektåtkomst.

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. I `<User Name>`Den här menyn kommer att ta bort Workfront-åtkomst. Välj om du vill att deras åtkomst ska tas bort från det markerade objektet eller från alla underordnade objekt som är kopplade till det.\
   Följande scenarier finns:

   * Om du bara tar bort entiteten från objektet förlorar entiteten sina behörigheter för objektet och deras ärvda behörigheter till de underordnade objekten. Om de tidigare beviljats behörigheter till de underordnade objekten individuellt behåller de samma behörigheter för alla underordnade objekt som är kopplade till dem när du väljer det här alternativet. 
   * Om du tar bort entiteten från objektet och alla underordnade objekt förlorar entiteten sina behörigheter till objektet och alla underordnade objekt, även när de tidigare fått individuell behörighet för varje underordnat objekt. 

1. Klicka **Spara**.

## Ta bort behörigheter från flera objekt samtidigt

Du kan ta bort entiteter (användare, jobbroller, team, grupper, företag) från flera objekt samtidigt när du markerar dem gruppvis i en lista. 

>[!NOTE]
>
>Du kan inte visa vilka åtkomstentiteter som har för alla markerade objekt när du markerar dem gruppvis. Du måste veta vilken enhet du vill ta bort från delningen av de markerade objekten innan du tar bort deras behörigheter.

1. Gå till listan med objekt som du vill dela.

   Mer information om vilka objekt som kan delas finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Markera flera objekt i listan och klicka sedan på **Dela** icon ![](assets/share-icon.png)högst upp i listan.
1. Skriv namnet på användaren, rollen, teamet, gruppen eller företaget som du vill ta bort åtkomsten för i **Redigera `<Object Name>` behörighet till** fält.
1. Välj **Ingen åtkomst**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. I `<User Name>`När Workfront-åtkomst tas bort från den här listrutan väljer du om du vill att deras åtkomst ska tas bort från de objekt du har markerat eller från alla andra underordnade objekt som är kopplade till den.\
   Följande scenarier finns:

   * Om du bara tar bort entiteten från objektet förlorar entiteten sina behörigheter för objektet och deras ärvda behörigheter till de underordnade objekten. Om de tidigare beviljats behörigheter till de underordnade objekten individuellt behåller de samma behörigheter för alla underordnade objekt som är kopplade till dem när du väljer det här alternativet. 
   * Om du tar bort entiteten från objektet och alla underordnade objekt förlorar entiteten sina behörigheter till objektet och alla underordnade objekt, även när de tidigare fått individuell behörighet för varje underordnat objekt.

   **Exempel:** Välj om du bara vill ta bort behörigheter för de uppgifter som du har valt i en lista eller för de utgåvor och dokument som är kopplade till uppgifterna.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Valfritt) Om du vill ändra flera behörigheter gruppvis för flera objekt väljer du en annan nivå för delning för den valda entiteten.

   Om de till exempel har behörigheten Hantera väljer du Contribute eller Visa i stället.

1. Klicka **Spara**.

## Ta bort ärvda behörigheter

Ärvda behörigheter kan tas bort från objekt, vilket gör det möjligt för ägare att specifikt identifiera vem som får åtkomst till underordnade objekt oavsett om en användare har åtkomst till ett överordnat objekt.

>[!IMPORTANT]
>
>Endast användare med behörigheten Hantera kan ta bort ärvda behörigheter.

Så här tar du bort ärvda behörigheter:

1. Gå till ett objekt som du har behörigheten Hantera för. Gå till exempel till en uppgift.
1. Gå till objektåtkomstrutan enligt beskrivningen i [Ta bort enheter från delningslistan för ett objekt](#remove-entities-from-the-sharing-list-of-an-object) i den här artikeln.
1. Välj **x** nästa **Ärvd behörighet** i delningsrutan om du vill ta bort någon som visas där.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Detta garanterar att ingen som har behörighet till det överordnade objektet (till exempel projektet) har behörighet till den här uppgiften som standard. Du måste lista enskilda enheter i delningslistan för uppgiften för att kunna bevilja behörigheter för uppgiften.

   >[!TIP]
   >
   >Du kan inte ta bort enskilda enheter från listan Ärvda behörigheter. Du kan bara inaktivera ärvda behörigheter för alla enheter i listan.

1. Klicka **Spara**. 

## Gör ett objekt privat

Om du har delat ett objekt i hela systemet, eller om du har delat det med externa användare genom att göra det offentligt, kan du göra det privat igen genom att ta bort behörigheten för hela systemet eller för offentliga användare. 

Mer information om hur du gör ett objekt tillgängligt för hela systemet, eller för allmänheten, finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Så här gör du ett objekt privat:

1. Gå till det objekt som du vill göra privat.\
   Navigera till exempel till en rapport.
1. Klicka **Rapportåtgärder** sedan **Delning**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Klicka **Ta bort offentlig åtkomst** för att ta bort externa användares åtkomst till rapporten.
1. Klicka **Ta bort systemomfattande åtkomst** för att sluta dela det med alla Workfront-användare. 
1. Klicka **Spara**.

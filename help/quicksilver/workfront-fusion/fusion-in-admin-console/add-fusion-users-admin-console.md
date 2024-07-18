---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till användare i Adobe Workfront Fusion via Adobe Admin Console
description: Du kan lägga till en användare i Adobe Admin Console och tilldela dem till Adobe Workfront Fusion, eller tilldela en befintlig användare i Adobe Admin Console till Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Lägg till användare i [!DNL Adobe Workfront Fusion] via [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>De procedurer som beskrivs på den här sidan gäller endast för organisationer som har anslutit till [!DNL Adobe Admin Console].
>
>Om din organisation ännu inte har anslutit sig till [!DNL Adobe Admin Console] kan du läsa [Lägga till en användare i en organisation i [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till [!DNL Adobe Admin Console] finns i [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Du kan lägga till en användare i [!DNL Adobe Admin Console] och tilldela dem till [!DNL Adobe Workfront Fusion], eller tilldela en befintlig användare i [!DNL Adobe Admin Console] till [!DNL Workfront Fusion].

En videofilm som beskriver [!DNL Workfront Fusion] i [!DNL Adobe Admin Console], inklusive hur du lägger till användare, finns i [[!DNL Fusion]  på Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] administratörsrättigheter</td> 
   <td>Du måste vara en [!UICONTROL Product Configuration Administrator] av [!DNL Adobe] produkter för din organisation.</td> 
  </tr>
  </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Förutsättningar

Innan du använder [!DNL Admin Console] för [!DNL Workfront] bör du få ett e-postmeddelande med en inbjudan till konsolen.

1. Om du inte har använt [!DNL Adobe] tidigare och du har fått ett e-postmeddelande om att du nu har administratörsbehörighet för att hantera [!DNL Adobe]-programvara och tjänster för din organisation klickar du på knappen i e-postmeddelandet för att skapa ett [!DNL Adobe]-konto och öppna [!DNL Admin Console].

   eller

   Om du redan har ett Adobe-konto går du till [[!DNL Adobe Admin Console] sidan](https://adminconsole.adobe.com/).


## Lägg till en ny användare i [!DNL Adobe Admin Console] och [!DNL Workfront Fusion]

1. Välj fliken **[!UICONTROL Products]** i det övre navigeringsfältet på [[!DNL Adobe Admin Console] sidan](https://adminconsole.adobe.com/) och välj sedan produktpanelen **[!DNL Workfront Fusion]**.

   ![Fusion i Admin Console](assets/fusion-product-admin-console.png)

1. I listan som visas väljer du den organisation där du vill lägga till en användare.

   ![Fusion-instans i Admin Console](assets/fusion-instances-admin-console.png)

1. Klicka på namnet på länken [!DNL Workfront Fusion] [!UICONTROL Product Profile] i listan som visas med fliken **[!UICONTROL Product Profiles]** markerad.

   ![Workfront Fusion - produktprofil](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Gör inga ändringar i själva [!UICONTROL Product Profile].

1. Klicka på **[!UICONTROL Add User]** med fliken **[!UICONTROL Users]** markerad ovanför listan.

1. I rutan **[!UICONTROL Add users to this product profile]** anger du e-postadressen eller namnet på en användare som du vill lägga till och markerar sedan användaren i listan som visas.

1. Klicka på **[!UICONTROL Save]**.

   Användaren har skapats i [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Valfritt) Fortsätt till [Ändra en användares åtkomstnivå i  [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Ändra en användares åtkomstnivå i Workfront Fusion

### Ändra en användares roll till Admin

En användare måste ha en administratörsroll i [!DNL Adobe Admin Console].

1. Välj fliken **[!UICONTROL Admins]** på sidan [!DNL Workfront Fusion] [!UICONTROL Product Profile] där du lade till användaren.

1. Klicka på **[!UICONTROL Add Admin]**.

1. I rutan **[!UICONTROL Add product profile administrators]** anger du e-postadressen eller namnet på en användare som du vill lägga till och markerar sedan användaren i listan som visas.

1. Klicka på **[!UICONTROL Save]**.

   Den här användaren är nu administratör i [!DNL Workfront Fusion].

### Ändra en användares roll till [!UICONTROL Member], [!UICONTROL Accountant] eller [!UICONTROL App Developer].

Roller [!UICONTROL Member], [!UICONTROL Accountant] och [!UICONTROL App Developer] hanteras inuti [!DNL Workfront Fusion].

Instruktioner finns i [Visa eller redigera användarroller](../organizations/manage-fusion-users.md#view-or-edit-user-roles) i artikeln [Hantera [!DNL Adobe Workfront Fusion] användare i din organisation](../organizations/manage-fusion-users.md)

## Tilldela en befintlig användare i [!DNL Adobe Admin Console] till [!DNL Workfront Fusion]

1. Börja redigera användaren enligt beskrivningen i avsnittet Redigera användarinformation i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) i [!DNL Adobe Admin Console]-dokumentationen.

1. Lägg till **[!DNL Adobe Workfront Fusion]** i de produkter som tilldelats användaren.

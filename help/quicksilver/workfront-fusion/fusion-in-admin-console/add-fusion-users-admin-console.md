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
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Lägg till användare i [!DNL Adobe Workfront Fusion] via [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>De förfaranden som beskrivs på denna sida gäller endast organisationer som har anslutit sig till [!DNL Adobe Admin Console].
>
>Om din organisation ännu inte har anslutit sig till [!DNL Adobe Admin Console], se [Lägga till en användare i en organisation i [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>För en lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till [!DNL Adobe Admin Console], se [Plattformsbaserade administrationsskillnader ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Du kan lägga till en användare i [!DNL Adobe Admin Console] och tilldela dem [!DNL Adobe Workfront Fusion]eller tilldela en befintlig användare i [!DNL Adobe Admin Console] till [!DNL Workfront Fusion].

För en videobeskrivning [!DNL Workfront Fusion] i [!DNL Adobe Admin Console], inklusive hur du lägger till användare, se [[!DNL Fusion] på Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] administratörsrättigheter</td> 
   <td>Du måste vara en [!UICONTROL Product Configuration Administrator] av [!DNL Adobe] produkter för er organisation.</td> 
  </tr>
  </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

&#42;&#42;För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Förutsättningar

Innan du använder [!DNL Admin Console] for [!DNL Workfront]bör du få ett e-postmeddelande med en inbjudan till konsolen.

1. Om du inte har använt [!DNL Adobe] och du har fått ett e-postmeddelande som säger att du nu har administratörsrättigheter för att hantera [!DNL Adobe] programvara och tjänster för din organisation, klicka på knappen i e-postmeddelandet för att skapa en [!DNL Adobe] konto och öppna [!DNL Admin Console].

   eller

   Om du redan har ett Adobe-konto går du till [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/).


## Lägg till en ny användare i [!DNL Adobe Admin Console] och [!DNL Workfront Fusion]

1. Från [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/)väljer du **[!UICONTROL Products]** i det övre navigeringsfältet och välj sedan **[!DNL Workfront Fusion]** produktpanel.

   ![Fusion i Admin Console](assets/fusion-product-admin-console.png)

1. I listan som visas väljer du den organisation där du vill lägga till en användare.

   ![Fusion-instans i Admin Console](assets/fusion-instances-admin-console.png)

1. I listan som visas med **[!UICONTROL Product Profiles]** klickar du på namnet på [!DNL Workfront Fusion] [!UICONTROL Product Profile] länk.

   ![Workfront Fusion - produktprofil](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Gör inga ändringar i [!UICONTROL Product Profile] själv.

1. Med **[!UICONTROL Users]** som är markerad ovanför listan, klicka på **[!UICONTROL Add User]**.

1. I **[!UICONTROL Add users to this product profile]** anger du e-postadressen eller namnet på en användare som du vill lägga till och markerar sedan användaren i listan som visas.

1. Klicka på **[!UICONTROL Save]**.

   Användaren skapas i [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Valfritt) Fortsätt till [Ändra en användares åtkomstnivå i [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Ändra en användares åtkomstnivå i Workfront Fusion

### Ändra en användares roll till Admin

En användare måste ha en administratörsroll i [!DNL Adobe Admin Console].

1. På [!DNL Workfront Fusion] [!UICONTROL Product Profile] sidan där du lade till användaren väljer du **[!UICONTROL Admins]** -fliken.

1. Klicka på **[!UICONTROL Add Admin]**.

1. I **[!UICONTROL Add product profile administrators]** anger du e-postadressen eller namnet på en användare som du vill lägga till och markerar sedan användaren i listan som visas.

1. Klicka på **[!UICONTROL Save]**.

   Den här användaren är nu administratör i [!DNL Workfront Fusion].

### Ändra en användares roll till [!UICONTROL Member], [!UICONTROL Accountant], eller [!UICONTROL App Developer].

[!UICONTROL Member], [!UICONTROL Accountant]och [!UICONTROL App Developer] roller hanteras inuti [!DNL Workfront Fusion].

Instruktioner finns i [Visa eller redigera användarroller](../organizations/manage-fusion-users.md#view-or-edit-user-roles) i artikeln [Hantera [!DNL Adobe Workfront Fusion] användare i din organisation](../organizations/manage-fusion-users.md)

## Tilldela en befintlig användare i [!DNL Adobe Admin Console] till [!DNL Workfront Fusion]

1. Börja redigera användaren enligt beskrivningen i avsnittet Redigera användarinformation i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) i [!DNL Adobe Admin Console] dokumentation.

1. Lägg till **[!DNL Adobe Workfront Fusion]** till de produkter som tilldelats användaren.

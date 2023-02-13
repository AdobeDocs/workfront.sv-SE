---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Hantera [!DNL Adobe Workfront Fusion] användare i din organisation
description: Hantera [!DNL Adobe Workfront Fusion] användare i din organisation
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Hantera [!DNL Adobe Workfront Fusion] användare i din organisation

[!DNL Adobe Workfront Fusion] administratörer kan hantera användarroller inuti [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> 
     <p>Du måste vara en [!DNL Workfront Fusion] administratör för din organisation.</p>
     <p>Du måste vara en [!DNL Workfront Fusion] administratör för ditt team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visa eller redigera användarroller {#view}

[!DNL Adobe Workfront Fusion] administratörer kan visa och uppdatera användarroller.

1. När du är inloggad som en [!DNL Workfront Fusion] administratör, välja **[!UICONTROL Users]** i den vänstra navigeringen.
1. Klicka **[!UICONTROL Details]** på raden för den användare som du vill visa.
1. (Valfritt) Om du vill uppdatera användarens roll klickar du på listrutan i dialogrutan **[!DNL Role]** i raden i organisationen där du vill ändra användarens roll och sedan välja den nya rollen.

## Visa eller redigera användarinformation {#view2}

[!DNL Adobe Workfront Fusion] administratörer kan visa och uppdatera användarinformation.

1. När du är inloggad som en [!DNL Workfront Fusion] administratör, välja **[!UICONTROL Users]** i den vänstra navigeringen.
1. Klicka **[!UICONTROL Details]** på raden för den användare som du vill visa.
1. (Valfritt) Om du vill uppdatera användarens information klickar du på **[!UICONTROL Options]** i skärmens övre högra hörn och välj **[!UICONTROL Change Details]**.

## Ta bort en användare {#delete}

[!DNL Adobe Workfront Fusion] administratörer kan ta bort användare.

1. När du är inloggad som en [!DNL Workfront Fusion] administratör, välja [!UICONTROL Users] i den vänstra navigeringen.
1. Klicka **[!UICONTROL Details]** på raden för den användare som du vill visa.
1. (Valfritt) Om du vill uppdatera användarens information klickar du på **[!UICONTROL Options]** i skärmens övre högra hörn och välj **[!UICONTROL Delete]**.

### Att tänka på när du tar bort en användare i Workfront Fusion

* När en användare tas bort tas användarens anslutningar, nycklar och webbböcker bort. Alla scenarier som tillhör användaren överförs till organisationsägaren. Anslutningarna i dessa scenarier måste uppdateras eftersom anslutningarna som tillhör användaren inte längre är giltiga.
* Om den borttagna användaren äger något program eller publika mallar överförs programmen eller de publika mallarna till organisationens ägare. Om det inte finns någon organisationsägare överförs programmen eller de offentliga mallarna till en annan användare.

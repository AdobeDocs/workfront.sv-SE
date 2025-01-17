---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Lägga till en användare i en organisation i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Lägga till en användare i en organisation eller ett team i Adobe Workfront Fusion

>[!IMPORTANT]
>
>Den här artikeln kommer att tas bort inom en snar framtid eftersom alla organisationer flyttas till Adobe Admin Console.

>[!IMPORTANT]
>
>Den procedur som beskrivs på den här sidan gäller endast för organisationer som ännu inte har anslutit till [!DNL Adobe Admin Console]. Om din organisation har anslutit sig till [!DNL Adobe Admin Console] måste du utföra den här åtgärden via [!DNL Adobe Admin Console].
>
>Instruktioner om hur du lägger till en användare när din organisation har flyttats till [!DNL  Adobe Admin Console] och Adobe Unified Experience finns i [Lägg till användare till [!DNL Adobe Workfront Fusion] via  [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> 
     <p>Du måste vara administratör för [!DNL Workfront Fusion] för din organisation.</p>
     <p>Du måste vara administratör för [!DNL Workfront Fusion] för ditt team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Lägga till användare i en organisation


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->
>[!NOTE]
>
>Om din organisation håller på att övergå till Adobe Admin Console kan du inte hantera användare i Workfront (lägga till eller ta bort användare). Du kan utföra dessa åtgärder i Adobe Admin Console när migreringen är klar.

Om du vill lägga till användare i organisationen måste du vara administratör för den organisation som du vill lägga till användare i. Mer information om roller finns i [Organisationsroller i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Så här lägger du till en användare i organisationen:

1. Navigera till **[!UICONTROL Organizations]** på menyn och markera den organisation du vill lägga till en användare i.
1. Öppna fliken **[!UICONTROL Users]** i din instrumentpanel.
1. Klicka på **[!UICONTROL Invite a new user]** och skicka inbjudan genom att klicka på **[!UICONTROL Send]**.

   >[!NOTE]
   >
   >   
   >Om du inte ser knappen [!UICONTROL Invite a new user] har din organisation anslutit till [!DNL Adobe Business Platform.]
   >
   >  Instruktioner om hur du lägger till en användare i en organisation som har anslutit till [!DNL Adobe Business Platform] finns i [Lägg till användare i [!DNL Adobe Workfront Fusion] via  [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

1. Fyll i formuläret.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Email address]</td>
      <td>
        Ange användarens e-postadress
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>Ange användarens fullständiga namn</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Role] </td>
      <td>Välj användarens roll. Mer information om roller finns i <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Organisations- och teamroller.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Team</td>
      <td>Välj alla team som du vill att användaren ska vara medlem i.</td>
    </tr>
    <tr>
      <td role="rowheader">Anteckning</td>
      <td>Ange en anteckning för användaren. Den här anteckningen visas i användarens e-postmeddelande med en inbjudan.</td>
    </tr>
  </tbody>
</table>

Användaren får ett e-postmeddelande med en inbjudan där han/hon kan acceptera inbjudan.

## Lägg till en användare i ett team

Dina användare tilldelas team när du skapar dem. Om en befintlig användare måste läggas till i ett team kan du lägga till dem på teamets användarsida.

Att lägga till en användare i ett team hanteras från sidan för det teamet.

1. Gå till det team du vill lägga till användaren i genom att välja **Organisationer** i den vänstra panelen, klicka på fliken **Team** på organisationssidan och sedan välja teamet.

   eller

   Om du är på sidan för ett annat team klickar du på grupplistrutan överst på sidan.

1. På teamets sida (med teamnamnet längst upp på sidan) väljer du fliken **Användare**.
1. Leta reda på användaren på sidan. Användare i din organisation visas på den här sidan även om de inte är medlem i gruppen.
1. Klicka på **Ingen** till höger om användarens namn och välj sedan den roll du vill att de ska ha i teamet.

Användaren läggs till i teamet.
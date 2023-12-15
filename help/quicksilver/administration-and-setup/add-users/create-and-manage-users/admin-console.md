---
title: Hantera användare i Adobe Admin Console
description: Som Adobe-administratör kan du skapa Adobe Workfront-användare och systemadministratörer med Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 0%

---

# Hantera användare i Adobe Admin Console

>[!IMPORTANT]
>
>Funktionerna i den här artikeln är bara tillgängliga om din organisations instans av Workfront har anslutits till Adobe Business Platform.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Som Adobe-administratör kan du skapa Adobe Workfront-användare och systemadministratörer med Adobe Admin Console. Konsolen är en central plats för att hantera Adobe i hela organisationen. Mer information finns i [Översikt över Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Administratörsrättigheter för Adobe</td> 
   <td> <p>Du måste vara produktkonfigurationsadministratör för Adobe-produkter för din organisation</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar

Innan du använder Admin Console för Workfront bör du få ett e-postmeddelande med en inbjudan till konsolen.

1. Om du inte har använt Adobe tidigare och du har fått ett e-postmeddelande om att du nu har administratörsbehörighet för att hantera program och tjänster för Adobe i din organisation klickar du på knappen i e-postmeddelandet för att skapa ett Adobe-konto och öppna Admin Console.

   eller

   Om du redan har ett Adobe-konto går du till [Adobe Admin Console page](https://adminconsole.adobe.com/).

## Mer information om Adobe Admin Console

* Workfront systemadministratörer kan inaktivera en Workfront-användare i Workfront, men detta inaktiverar inte användaren i Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* Användaren **Hemgrupp** bestäms utifrån den användare som skapade dem. Det går inte att anpassa inifrån Admin Console.
* Åtkomstnivån för Workfront-systemadministratören kan bara redigeras inifrån Adobe Admin Console.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* Om du vill ändra en användares åtkomst från systemadministratören till någon annan åtkomstnivå måste du först gå via Admin Console.

  <!--
   This is not clear
  -->

* Om du vill ta bort systemadministratörsåtkomst från en användare i Workfront måste du använda Adobe Admin Console för att ta bort användaren som produktprofiladministratör. Detta ändrar användarens Workfront-åtkomstnivå från systemadministratör till begärande.

  >[!IMPORTANT]
  >
  >Gör inga ändringar i själva produktprofilen.

## Gå till användar- och administratörsområdet för din Production-instans av Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Från [Adobe Admin Console page](https://adminconsole.adobe.com/)väljer du **Produkter** i det övre navigeringsfältet och välj sedan **Workfront** produktpanel.

   ![](assets/admin-product-1.png)

1. I listan som visas väljer du länken längst upp.

   Det här är din produktionsinstans där dina användare arbetar.

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >Den andra länken i listan, din Preview-instans, är en testmiljö som replikerar din produktionsmiljö. Mer information finns i [Sandlådemiljön Adobe Workfront Preview](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Du kan också se länkar till sandlådemiljöer i listan. Mer information finns i [Sandlådemiljön Adobe Workfront Preview](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. I listan som visas med **Produktprofiler** klickar du på namnet på länken Workfront produktprofil.

   ![](assets/prod-profile-1.png)

   Den här listan innehåller alla användare som redan är tilldelade till din Production-instans av Workfront.

   >[!IMPORTANT]
   >
   >Gör inga ändringar i själva produktprofilen.

1. Fortsätt till ett av följande avsnitt i den här artikeln:

   * [Skapa användare i Workfront med Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Skapa systemadministratörer i Workfront med Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Skapa användare i Workfront med Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

Workfront-användare måste läggas till i Adobe Admin Console. En administratör kan skapa användaren direkt i Adobe Admin Console. Gruppadministratörer skapar användare i Workfront som sedan skickas in för godkännande. När det är godkänt läggs användaren till i Adobe Admin Console.

* [Skapa användare i Workfront direkt i Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Skapa användare i Workfront och godkänn dem för Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Skapa användare i Workfront direkt i Adobe Admin Console

1. Gå till användar- och administratörsområdet i Admin Console, enligt beskrivningen i avsnittet [Gå till användar- och administratörsområdet för din Production-instans av Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) i den här artikeln.
1. Med **Användare** som är markerad ovanför listan, välj **Lägg till användare**.
1. I **Lägg till användare i den här produktprofilen** anger du e-postadressen eller namnet på en användare som du vill lägga till och väljer **Spara**.

   Användaren skapas i Workfront med åtkomstnivån Begärande.

   >[!IMPORTANT]
   >
   >Gör inga ändringar i själva produktprofilen.

1. Ändra användarens åtkomstnivå i Workfront.

   Instruktioner om hur en Workfront-administratör kan ändra användarens åtkomstnivå finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Upprepa steg 3 och 4 för att lägga till fler användare.

   >[!NOTE]
   >
   >För nya användare av Adobe skickar Admin Console ett e-postmeddelande med en inbjudan om att slutföra registreringsprocessen. Alla användare måste slutföra registreringsprocessen för att få tillgång till alla Adobe-program.
   >
   >För användare som redan har Adobe kan användaren få ett e-postmeddelande om att Workfront är tillgängligt eller inte. Detta är en inställning som styrs av Adobe-administratören för produkten.

### Skapa användare i Workfront och godkänn dem för Adobe Admin Console

Med det här arbetsflödet kan gruppadministratörer som inte har tillgång till Adobe Admin Console skapa användare.

Först skapar gruppadministratören användaren i Workfront. Detta skapar användaren med statusen Inaktiverad och Väntande godkännande.

Sedan godkänner en Workfront-administratör användaren. Detta aktiverar användaren i Workfront och lägger till dem i Adobe Admin Console.

#### Skapa användaren i Workfront (gruppadministratör)

Instruktioner om hur du skapar en användare i Workfront finns i [Lägg till användare](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### Godkänn användaren (Workfront-administratör)

Godkänna en användare:

{{step-1-to-users}}

1. Markera användaren och klicka sedan på M **o** re, ikon ![](assets/more-icon.png).

1. Klicka på **Godkänn** och sedan klicka **Skicka**.

   eller

   Om du vill avvisa användaren och ta bort den från Workfront klickar du på **Avvisa** och sedan klicka **Skicka**.

   Godkända användare läggs automatiskt till i Adobe Admin Console.

   Avvisade användare tas automatiskt bort från Workfront.



## Skapa systemadministratörer i Workfront med Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

Åtkomstnivån för systemadministratören ges endast på Adobe Admin Console. Du kan inte bevilja eller ta bort administratörsåtkomst inifrån Workfront.

Du måste lägga till en användare i din Production-instans av Workfront innan du kan göra användaren till Workfront-systemadministratör. Instruktioner finns i avsnittet [Skapa användare i Workfront med Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console) i den här artikeln.

1. Gå till användar- och administratörsområdet i Admin Console, enligt beskrivningen i avsnittet [Gå till användar- och administratörsområdet för din Production-instans av Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) i den här artikeln.
1. Välj **Administratörer** -fliken ovanför listan med användare.
1. Välj **Lägg till administratör**.
1. I **Lägg till produktprofiladministratörer** anger du e-postadresserna eller namnen på de administratörer som du vill lägga till och väljer **Spara**.

   ![](assets/add-admin-1.png)

   Systemadministratörerna skapas i Workfront.

   >[!IMPORTANT]
   >
   >Gör inga ändringar i själva produktprofilen.



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->

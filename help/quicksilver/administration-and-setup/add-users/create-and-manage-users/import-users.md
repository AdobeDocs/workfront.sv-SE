---
title: Importera användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan importera användare till Adobe Workfront-platsen genom att synkronisera användare från en nätverkskatalogtjänst (till exempel Active Directory eller en annan LDAP-katalog) eller importera användare med hjälp av en kalkylbladsimportfil.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Importera användare

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Du kan importera användare med hjälp av en kalkylbladsimportfil.

Innan du skapar en ny användare måste du se till att du har skapat alla objekt som du vill associera med användaren. Om du till exempel inte har skapat ett schema kan du inte tilldela det till den nya användaren ett schema, och fältet som du använder för att associera ett schema med den nya användaren visas inte på skärmen Ny användare.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> ange din åtkomstnivå som <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst en av de två <b>Användaradministratör</b> alternativ aktiverade under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>av dessa två alternativ, om användaren <b>Administratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om <b>Användare</b> ange en åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Använd en kalkylbladsimportfil för att importera användare

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).

1. Klicka på **Ny användare** nedrullningsbar pil och klicka sedan på **Importera användare**.

1. I **Importera användare** som visas hämtar du exempelfilen och uppdaterar sedan exempelfilen så att den innehåller din egen användares personliga information.

   Varje rad innehåller följande fält:

   * **Förnamn**
   * **Efternamn**
   * **E-postadress**

     E-postadresser måste vara unika.

   * **Åtkomstnivå**

     Åtkomstnivåer är skiftlägeskänsliga.

   * **Inloggnings-ID för enkel inloggning**

     Det här fältet inkluderas bara om enkel inloggning är aktiverat i systemet. Du måste lägga till Federations-ID i det här fältet för varje användare. När du skapar en användare från fliken Personer kan du ange ett lösenord för användaren om du vill tillåta användare att logga in utan enkel inloggning. Importfunktionen tillåter dock inte att du lämnar SSO-LOGIN-ID:t tomt.

   * Kontrollera att det inte finns några extra blanksteg före eller efter en användares e-postadress.

   När du är klar med en rad bör den se ut så här:

   ![importing-new-users.png](assets/importing-new-users.png)

1. Spara filen på en plats på din arbetsstation.
1. Klicka **Välj fil** i **Importera användare** box.

1. Navigera till och markera filen som du har sparat.
1. (Valfritt) Välj **Skicka en inbjudan via e-post till den här användaren** möjlighet att skicka en e-postinbjudan till användaren, meddela dem att ett Workfront-konto har skapats och be dem att ange sitt lösenord.

   Avmarkera det här alternativet om du vill ange lösenordet för användaren.

1. Klicka **Importera**.

   Du får ett bekräftelsemeddelande högst upp på skärmen om att användaren har importerats.

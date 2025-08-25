---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,sparkstart,kickstarter,sparkstarter
navigation-topic: use-kick-starts
title: 'Scenario med snabb start: Förberedelser för företag, grupper, roller och användare har startats'
description: När du börjar implementera Adobe Workfront, i stället för att ange data manuellt, kan du importera kundlistan, interna avdelningar, jobbroller och användarinformation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# Fast-Starts-scenario: Förberedelser för företag, grupp, roll och användare

När du börjar implementera Adobe Workfront, i stället för att ange data manuellt, kan du importera kundlistan, interna avdelningar, jobbroller och användarinformation.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td>
   <p> Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vad du kan importera

I följande tabell visas de företag, grupper och roller som ska importeras:

| Företag | Grupper | Roller |
|---|---|---|
| Acme, Co <p>Workfront, Inc. <p>_Ditt företag_ <p>XYZ, Inc. | Ekonomi <p>IT <p>Marknadsföring <p>Försäljning | Affärsanalytiker <p>Creative <p>Designer <p>Resurshanteraren <p>Scrum Master <p>Teknikskribent <p>Webbutvecklare |

{style="table-layout:auto"}

Rollnamn måste vara unika. Befintliga jobbroller kan inte importeras.

I följande tabeller visas vilka användare som ska importeras och olika användarattribut för varje:

### Användare 1

| Attribut | Värde |
|---|---|
| **Förnamn** | Chris |
| **Efternamn** | Manning |
| **Användarnamn/e-postadress** | mailto:cmanning@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Teammedlem |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Marknadsföring |
| **Jobbroll** | Affärsanalytiker |

{style="table-layout:auto"}

### Användare 2

| Attribut | Värde |
|---|---|
| **Förnamn** | Jennifer |
| **Efternamn** | Campbell |
| **Användarnamn/e-postadress** | jcampbell@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Projektledare |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Marknadsföring |
| **Jobbroll** | Projektledare |

{style="table-layout:auto"}

### Användare 3

| Attribut | Värde |
|---|---|
| **Förnamn** | Jill |
| **Efternamn** | Sullivan |
| **Användarnamn/e-postadress** | jsullivan@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Help Desk |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Försäljning |
| **Jobbroll** | Säljare |

{style="table-layout:auto"}

### Användare 4

| Attribut | Värde |
|---|---|
| **Förnamn** | Marc |
| **Efternamn** | Lewis |
| **Användarnamn/e-postadress** | mlewis@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Portfolio Manager |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Ekonomi |
| **Jobbroll** | Styrenhet |

{style="table-layout:auto"}

### Användare 5

| Attribut | Värde |
|---|---|
| **Förnamn** | Pam |
| **Efternamn** | Reynolds |
| **Användarnamn/e-postadress** | preynolds@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Projektledare |
| **Företag** | *Ditt företag>* |
| **Hemgrupp** | Marknadsföring |
| **Jobbroll** | IT |

{style="table-layout:auto"}

### Användare 6

| Attribut | Värde |
|---|---|
| **Förnamn** | Ray |
| **Efternamn** | Andrews |
| **Användarnamn/e-postadress** | randrews@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Administratör |
| **Företag** | *Ditt företag>* |
| **Hemgrupp** | Resurshanteraren |
| **Jobbroll** | ingen |

{style="table-layout:auto"}

## Ladda ned en snabbstartsmall

{{step-1-to-setup}}

1. Klicka på **System** > **Snabbstart** > **Importera data.**

1. Klicka på **Fler alternativ** om du vill se en fullständig lista över importalternativ.
1. Markera de åtkomstnivå, företag, grupper, jobbroller och användarobjekt som du vill importera.
1. Klicka på **Hämta**.

## Ange företagsinformation

1. Öppna filen **Workfront.xlsx** som du just laddat ned.

   >[!TIP]
   >
   >När du arbetar med mycket breda datablad kanske du vill använda verktygen Frys ruta (eller motsvarande) i kalkylbladet för att göra kalkylbladet enklare att arbeta med.

1. Gå till bladet **CMPY Company**.

   Den ska vara tom om inte företagen redan finns i systemet.

   ![Företagsblad](assets/cmpysheet-350x16.png) ![Företag-ID](assets/companyid--1--350x78.png)

1. Ange **TRUE** i kolumnen **isNew**.

   Upprepa den här åtgärden för varje företag som läggs till. (I det här exemplet slutför du den här åtgärden för raderna 3-6 eftersom fyra företag läggs till.)

   ![Företaget är nytt](assets/cmpyisnew-350x86.png)

1. Ange ett unikt **ID**.

   Du måste ange ett ID för varje rad. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![Företaget är nytt](assets/cmpyisnew-350x86.png)

1. Ange namnen på varje kund i kolumnen **setName**.

   ![Företag-ID](assets/companyid-350x78.png)

1. Gå till bladet **GRUPPgrupp**.

   Om du inte redan har skapat grupper i Workfront ska det här bladet endast visa standardgruppen som har etablerats med alla Workfront-konton.

   ![Gruppblad](assets/groupsheet-350x15.png) ![Tomt gruppblad](assets/emptygroupsheet-350x85.png)

1. Ange **TRUE** i kolumnen **isNew**.

   Enligt scenariot importeras fyra grupper, så ange **TRUE** i kolumnen **isNew** för raderna 4 till 7.

1. Ange ett unikt **ID**.

   Du måste ange ett ID för varje rad. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![Grupp-ID](assets/groupids-350x85.png)

1. Ange namnen på varje avdelning i kolumnen **setName**.

   ![Gruppnamn](assets/groupnames-350x85.png)

1. Gå till bladet **ROLE Role**.

   Om du inte redan har skapat eller tagit bort roller i ditt konto, ska det här bladet innehålla 8 roller som har tilldelats med alla Workfront-konton.

   ![Gruppnamn](assets/groupnames-350x85.png)

1. Ange **TRUE** i kolumnen **isNew**.

   Enligt scenariot kommer 7 jobbroller att importeras, så ange **TRUE** i kolumnen **isNew** för raderna 12 till 18.

   ![Rollen är ny](assets/roleisnew-350x104.png)

1. Ange ett unikt **ID**.

   Du måste ange ett ID för varje rad. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![Rollen är ny](assets/roleisnew--1--350x104.png)

1. Ange ett namn för varje roll i kolumnen **setName**.

   ![Rollen är ny](assets/roleisnew-350x104.png)

1. Ange ytterligare information efter behov.

   Inkludera faktureringstariffer, kostnadstariffer och beskrivningar för de roller du skapar efter behov.

1. Gå till bladet **ANVÄNDARE**.

   Om du inte redan har skapat användare i ditt konto ska det här bladet endast visa den Admin User som har etablerats med alla Workfront-konton.

   ![Användarblad](assets/usersheet-350x16.png) ![Tomt användarblad](assets/emptyusersheet-350x52.png)

1. Ange **TRUE** i kolumnen **isNew**.

   Enligt scenariot importeras 6 användare, så ange **TRUE** i kolumnen **isNew** för raderna 4 till 9.

   ![Användaren är ny](assets/userisnew-350x52.png)

1. Ange ett unikt **ID**.

   Du måste ange ett ID för varje rad. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![Användaren är ny](assets/userisnew-350x52.png)

1. Ange namnen på varje användare i kolumnerna **setFirstName** och **setLastName**.

   ![Användarnamn](assets/usernames-350x52.png)

1. Ange detaljvärden genom att ange värden i kolumnerna **setEmail**, **setPassword** och **setUsername**.

   ![Användarautentiseringsuppgifter](assets/usercredentials-350x52.png)

1. Ange åtkomstnivåvärden.

   Chris Manning är till exempel en teammedlem. Leta upp ID:t på **ACSLVL-åtkomstnivån** för teammedlemmens åtkomstnivå. Kopiera ID:t och klistra in det på bladet **ANVÄNDARE** i kolumnen **setAccessLevelID** på användarens rad.

   Upprepa det här steget för varje användare och åtkomstnivå.

   ![Kopiera åtkomstnivå-ID](assets/copyalid-350x171.png) ![Klistra in åtkomstnivå-ID](assets/pastealid-350x59.png)

1. Ange information om användarens hemgrupp.

   Enligt scenariot tillhör Chris Manning marknadsföringsgruppen. På bladet **GRUPPgrupp** letar du reda på ID:t för marknadsföringsgruppen, kopierar det och klistrar in det på bladet **ANVÄNDARE** i kolumnen **setHomeGroupID** på användarens rad. &#x200B;Upprepa det här steget för varje användare och grupptilldelning.

   ![Kopiera grupp-ID](assets/copygroupid-1-350x133.png) ![Klistra in grupp-ID](assets/pastegroupid-350x59.png)

1. Ange användarens företagsinformation.

   Alla användare i det här scenariot tillhör samma företag. På bladet **CMPY Company** letar du reda på ID:t för företaget **Ditt eget företag**, kopierar ID:t och klistrar in det här värdet på fliken **ANVÄNDARE** på varje rad i kolumnen **setCompanyID** &#x200B;.

   Upprepa det här steget för varje användare och grupptilldelning.

   ![Företag-ID](assets/companyid--1--350x78.png) ![Klistra in företags-ID](assets/pastecompanyid-350x84.png)

1. Ange information om användarens jobbroll.

   Enligt scenariot har Chris Manning rollen Business Analyst. På bladet **ROLE Role** letar du reda på ID:t för Business Analyst-rollen, kopierar det och klistrar in det på bladet **USER User** i kolumnen **setRoleID** på användarens rad. &#x200B;Upprepa det här steget för varje användare och grupptilldelning.

   ![Kopiera roll-ID](assets/copyroleid-350x149.png) ![Klistra in roll-ID](assets/pasteroleid-350x95.png)

1. Fyll i annan användarinformation efter behov och spara sedan filen.
1. Importera Excel-filen.

   Följ anvisningarna i [Importera data till Adobe Workfront med en snabbstartmall](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

>[!NOTE]
>
>Användare som importeras till Workfront skapas med statusen Inaktiverad och Väntande godkännande.
> 
>Om din organisation har migrerats till Adobe Admin Console och en användare inte går ut ur statusen Inaktiverat och Väntande godkännande inom några minuter, kan du lägga till gruppen med användare direkt till Adobe Admin Console.
>
>Instruktioner finns i [Hantera flera användare | Massöverföring av CSV ](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) i Adobe-dokumentationen.

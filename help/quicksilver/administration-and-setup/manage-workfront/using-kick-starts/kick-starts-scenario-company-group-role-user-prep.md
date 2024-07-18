---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,sparkstart,kickstarter,sparkstarter
navigation-topic: use-kick-starts
title: 'Spark-Starts-scenario: Förberedelser för företag, grupp, roll och användare har startats'
description: När du börjar implementera Adobe Workfront, i stället för att ange data manuellt, kan du importera kundlistan, interna avdelningar, jobbroller och användarinformation.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 0%

---

# Scenario med snabb start: Förberedelser för företag, grupper, roller och användare har startats

När du börjar implementera Adobe Workfront, i stället för att ange data manuellt, kan du importera kundlistan, interna avdelningar, jobbroller och användarinformation.

## Åtkomstkrav

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vad du kan importera

I följande tabell visas de företag, grupper och roller som ska importeras:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Företag</strong> </th> 
   <th><strong>Grupper</strong> </th> 
   <th><strong>Roller</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>Ditt företag</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Ekonomi</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marknadsföring </p> <p valign="top" rowspan="7">Försäljning</p> </td> 
   <td valign="top"> <p valign="top">Affärsanalytiker</p> <p valign="top">Kreativ styrenhet</p> <p valign="top">Designer</p> <p valign="top">Resurshanteraren</p> <p valign="top">Scrum Master</p> <p valign="top">Teknikskribent</p> <p valign="top">Webbutvecklare</p> </td> 
  </tr> 
 </tbody> 
</table>

Rollnamn måste vara unika. Befintliga jobbroller kan inte importeras.

I följande tabeller visas vilka användare som ska importeras och olika användarattribut för varje:

### Användare 1

| **Förnamn** | Chris |
|---|---|
| **Efternamn** | Manning |
| **Användarnamn/e-postadress** | mailto:cmanning@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Teammedlem |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Marknadsföring |
| **Jobbroll** | Affärsanalytiker |

{style="table-layout:auto"}

### Användare 2

| **Förnamn** | Jennifer |
|---|---|
| **Efternamn** | Campbell |
| **Användarnamn/e-postadress** | jcampbell@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Projektledare |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Marknadsföring |
| **Jobbroll** | Projektledare |

{style="table-layout:auto"}

### Användare 3

| **Förnamn** | Jill |
|---|---|
| **Efternamn** | Sullivan |
| **Användarnamn/e-postadress** | jsullivan@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Help Desk |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Försäljning |
| **Jobbroll** | Säljare |

{style="table-layout:auto"}

### Användare 4

| **Förnamn** | Marc |
|---|---|
| **Efternamn** | Lewis |
| **Användarnamn/e-postadress** | mlewis@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Portfolio Manager |
| **Företag** | &lt;*Ditt företag>* |
| **Hemgrupp** | Ekonomi |
| **Jobbroll** | Styrenhet |

{style="table-layout:auto"}

### Användare 5

| **Förnamn** | Pam |
|---|---|
| **Efternamn** | Reynolds |
| **Användarnamn/e-postadress** | preynolds@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Projektledare |
| **Företag** | *Ditt företag>* |
| **Hemgrupp** | Marknadsföring |
| **Jobbroll** | IT |

{style="table-layout:auto"}

### Användare 6

| **Förnamn** | Ray |
|---|---|
| **Efternamn** | Andrews |
| **Användarnamn/e-postadress** | randrews@foo.com |
| **Lösenord** | updateMe |
| **Åtkomst** | Administratör |
| **Företag** | *Ditt företag>* |
| **Hemgrupp** | Resurshanteraren |
| **Jobbroll** | ingen |

{style="table-layout:auto"}

## Ladda ned en snabbstartsmall

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **System** > **Snabbstart** > **Importera data.**

1. Klicka på **Fler alternativ** om du vill se en fullständig lista över importalternativ.
1. Markera de åtkomstnivå, företag, grupper, jobbroller och användarobjekt som du vill importera.

## Ange företagsinformation

1. Öppna filen **Workfront.xlsx** som du just laddat ned.

   >[!TIP]
   >
   >När du arbetar med mycket breda datablad kanske du vill använda verktygen Frys ruta (eller motsvarande) i kalkylbladet för att göra kalkylbladet enklare att arbeta med.

1. Gå till&quot;CMPY Company&quot;.

   Den ska vara tom om inte företagen redan finns i systemet. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Ange TRUE i kolumnen **isNew**.
1. Upprepa den här åtgärden för varje företag som läggs till. (I det här exemplet slutför du den här åtgärden för raderna 3-6 eftersom fyra företag läggs till.)

   ![](assets/cmpyisnew-350x86.png)

1. Ange ett unikt ID.

   Detta måste göras för varje rad för ID-kolumnen. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![](assets/cmpyisnew-350x86.png)

1. Ange ett namn.

   Ange namnen på varje kund i kolumnen **setName**.

   ![](assets/companyid-350x78.png)

1. Gå till GROUP Group-arket.

   Om du inte redan har skapat grupper i Workfront ska det här bladet endast visa standardgruppen som har etablerats med alla Workfront-konton.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Ange kolumnen **isNew**.Enligt scenariot importeras fyra grupper, så ange TRUE i raderna 4 till 7 för kolumnen &#39;isNew&#39;.
1. Ange ett unikt ID.

   Detta måste göras för varje rad för ID-kolumnen. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![](assets/groupids-350x85.png)

1. Ange ett namn.

   Ange namnen på varje avdelning i kolumnen **setName**.

   ![](assets/groupnames-350x85.png)

   Ange rollinformation. Gå till ROLLrollbladet.

1. Om du inte redan har skapat eller tagit bort roller i ditt konto, ska det här bladet innehålla 8 roller som har tilldelats med alla Workfront-konton.

   ![](assets/groupnames-350x85.png)

1. Ange programsatsen True.

   Sju jobbroller importeras, ange TRUE i raderna 12 till 18 för kolumnen &#39;isNew&#39;.

   ![](assets/roleisnew-350x104.png)

1. Ange ett unikt ID.

   Detta måste göras för varje rad för ID-kolumnen. Heltal som börjar vid 1 fungerar bra när du skapar nya poster.

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. Ange ett namn för varje roll genom att skriva in den i kolumnen setName.

   ![](assets/roleisnew-350x104.png)

1. Ange ytterligare information efter behov.

   Inkludera faktureringstariffer, kostnadstariffer och beskrivningar för de roller du skapar efter behov.

1. Gå till användarbladet för ANVÄNDARE om du vill ange användarinformation.

   Om du inte redan har skapat användare i ditt konto ska det här bladet endast visa den Admin User som har etablerats med alla Workfront-konton.

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. Ange True-värdet genom att ange TRUE i raderna 4 till 9 för kolumnen &#39;isNew&#39; eftersom 6 användare importeras.

   ![](assets/userisnew-350x52.png)

1. Ange ett unikt ID genom att ange ett unikt ID i varje rad för ID-kolumnen. Vanligtvis fungerar heltal med början vid 1 bra för nya poster.

   ![](assets/userisnew-350x52.png)

1. Ange namnen för varje användare i kolumnerna setFirstName och setLastName.

   ![](assets/usernames-350x52.png)

1. Ange detaljvärden genom att ange värden i kolumnerna setEmail, setPassword och setUsername.

   ![](assets/usercredentials-350x52.png)

1. Ange åtkomstnivåvärden.

   Chris Manning, som är teammedlem, kan till exempel slå upp ID:t på ACSLVL-åtkomstnivåbladet för teammedlemmens åtkomstnivå. Kopiera ID:t till Urklipp och klistra in det på användarbladet i kolumnen **setAccessLevelID** på raden Chris.

   Upprepa det här steget för varje användare och åtkomstnivå.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Ange hemgruppsinformation.

   Enligt scenariot tillhör Chris Manning marknadsföringsgruppen. På GROUP Group-bladet letar du reda på ID:t för marknadsföringsgruppen, kopierar det till Urklipp och klistrar in det i kolumnen **setHomeGroupID** på raden Chris i användarbladet. &#x200B;Upprepa det här steget för varje användare och grupptilldelning.

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. Ange företagsinformation.

   Alla användare i det här scenariot tillhör samma företag. På CMPY Company-bladet letar du reda på ID:t för *Ditt eget företag *företag, kopierar ID:t till Urklipp och klistrar in det här värdet på varje rad i kolumnen setCompanyID på fliken ANVÄNDARE. &#x200B;

   Upprepa det här steget för varje användare och grupptilldelning.

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. Ange information om jobbroll.

   Enligt scenariot har Chris Manning rollen Business Analyst. På ROLE Role-bladet letar du reda på ID:t för Business Analyst-rollen, kopierar det till Urklipp och klistrar in det i kolumnen setRoleID på raden Chris på användarbladet. &#x200B;Upprepa det här steget för varje användare och grupptilldelning.

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. Fyll i annan användarinformation efter behov och spara sedan filen.
1. Importera Excel-filen.

   Följ anvisningarna i avsnittet **Importera snabbstartsfiler** i den här artikeln.

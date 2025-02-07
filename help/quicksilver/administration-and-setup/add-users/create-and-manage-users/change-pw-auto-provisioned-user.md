---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ändra lösenordet för en automatiskt tilldelad användare
description: Vi rekommenderar att du ändrar en ny användares användarnamn till e-postadressen för Workfront och sedan låter användaren ändra sitt lösenord.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Ändra lösenordet för en användare som har tilldelats automatiskt

När du skapar användare med automatisk etablering tilldelar Adobe Workfront dem ett GUID (Global Unique Identifier) för ett användarnamn. Ett GUID är en unik sträng med slumpmässiga siffror och bokstäver, till exempel *5489cb430012526e1ea635e8c29f377f*.

När en ny användare försöker ändra sitt tillfälliga lösenord anger han/hon ofta sin e-postadress som användarnamn och får ett felmeddelande om ett felaktigt användarnamn. För att användaren ska kunna ändra sitt lösenord måste användaren ange sitt systemtilldelade användarnamn, som är ett GUID.

Eftersom det kan vara svårt att använda GUID-användarnamn rekommenderar vi att du först ändrar en användares användarnamn till sin Workfront-e-postadress och sedan låter användaren ändra sitt lösenord.

>[!TIP]
>
>Du kan hitta användarens GUID på följande sätt:
>
>* Gå till användarens profil och kopiera GUID från webbadressen i webbläsaren.
>
>  I URL:en `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details` skulle du till exempel kopiera strängen med siffror och bokstäver mellan de två sista snedstrecken: `61941ab1000af22d7104628efa1c738b`.
>
>  Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Skapa en användarrapport med kolumnen Användare > GUID. Mer information finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Fråga Workfront API.
>

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändra lösenordet för en användare som har tilldelats automatiskt

1. Ta reda på en användares GUID-användarnamn genom att skicka en API-begäran, vilket visas i följande exempel:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Var *`<domain>`* är företagets domän och *`<ID of User>`* är användarens Workfront-ID.

   Du får ett svar som liknar följande:

   ![Hämta GUID](assets/get-guid.png)

   Returvärdet för &quot;username&quot; är användarens GUID.

1. Ändra användarens lösenord med användarens GUID som användarnamn.

   Mer information om hur du ändrar ditt lösenord finns i [Återställ ditt lösenord](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Om din organisation använder ett SSO-system kan bara en Workfront-systemadministratör ändra en användares lösenord. Mer information finns i [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Med användaren inloggad på Workfront går du till:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Kontrollera att användarens e-postadress är korrekt i rutan **Din e-postadress för inloggning** och klicka sedan på **Uppdatera konto**.

   ![Användarnamn](assets/guidusername-350x272.png)

   Användarnamnet ändras till e-postadressen för Workfront.

>[!TIP]
>
>Så här söker du efter en användares ID:
>
>1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ikonen **Användare** ![Användare](assets/users-icon-in-main-menu.png) .
>
>1. Markera användaren.
>
>   Användarens profilsida öppnas och användar-ID:t visas i URL:en.
>

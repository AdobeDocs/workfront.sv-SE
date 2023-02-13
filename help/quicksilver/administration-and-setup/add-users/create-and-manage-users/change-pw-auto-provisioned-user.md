---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ändra lösenordet för en automatiskt tilldelad användare
description: När en ny användare försöker ändra sitt tillfälliga lösenord anger han/hon ofta sin e-postadress och får ett felmeddelande om ett felaktigt användarnamn. De måste ange sitt systemtilldelade användarnamn, som är deras GUID (Global Unique Identifier). Eftersom det är svårt att komma ihåg och använda ett GUID rekommenderar vi att du ändrar en ny användares användarnamn till e-postadressen i Workfront och sedan tillåter att användaren ändrar sitt lösenord.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Ändra lösenordet för en automatiskt tilldelad användare

När du skapar användare med automatisk etablering tilldelar Adobe Workfront dem ett GUID (Global Unique Identifier) för ett användarnamn. Ett GUID är en unik sträng med slumpmässiga siffror och bokstäver, till exempel *5489cb430012526e1ea635e8c29f377f*.

När en ny användare försöker ändra sitt tillfälliga lösenord anger han/hon ofta sin e-postadress som användarnamn och får ett felmeddelande om ett felaktigt användarnamn. För att användaren ska kunna ändra sitt lösenord måste användaren ange sitt systemtilldelade användarnamn, som är ett GUID.

Eftersom det kan vara svårt att använda GUID-användarnamn rekommenderar vi att du först ändrar en användares användarnamn till sin Workfront-e-postadress och sedan låter användaren ändra sitt lösenord.

>[!TIP]
>
>Du kan hitta användarens GUID på följande sätt:
>
>* Gå till användarens profil och kopiera GUID från webbadressen i webbläsaren.
>
>  I URL:en `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`kopierar du strängen med siffror och bokstäver mellan de två sista snedstrecken: `61941ab1000af22d7104628efa1c738b`.
>
>  Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Skapa en användarrapport med kolumnen Användare > GUID. Mer information finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Fråga Workfront API.
>


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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändra lösenordet för en automatiskt tilldelad användare

1. Ta reda på en användares GUID-användarnamn genom att skicka en API-begäran, vilket visas i följande exempel:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Plats *`<domain>`* är företagets domän och *`<ID of User>`* är användarens Workfront-ID.

   Du får ett svar som liknar följande:

   ![](assets/get-guid.png)

   Returvärdet för &quot;username&quot; är användarens GUID.

1. Ändra användarens lösenord med användarens GUID som användarnamn.

   Mer information om hur du ändrar ditt lösenord finns i [Återställ lösenordet](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Om din organisation använder ett SSO-system kan bara en Workfront-systemadministratör ändra en användares lösenord. Mer information finns i [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Med användaren inloggad på Workfront går du till:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. I **Din e-postadress för inloggning** bekräfta att användarens e-postadress är korrekt och klicka sedan på **Uppdatera konto**.

   ![](assets/guidusername-350x272.png)

   Användarnamnet ändras till e-postadressen för Workfront.

>[!TIP]
>
>Så här söker du efter en användares ID:
>
>1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).
>
>1. Markera användaren.
>
>   Användarens profilsida öppnas och användar-ID:t visas i URL:en.

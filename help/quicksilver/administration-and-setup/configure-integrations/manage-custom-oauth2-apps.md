---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Visa och hantera anpassade OAuth2-program
description: Som Adobe Workfront-administratör kan du visa och hantera OAuth2-program för din instans av Workfront, som ger andra program åtkomst till Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Visa och hantera anpassade OAuth2-program

Som en [!DNL Adobe Workfront] kan du visa och hantera OAuth2-program för din instans av [!DNL Workfront]som ger andra program åtkomst [!UICONTROL Workfront].

>[!NOTE]
>
>I OAuth2-sammanhang avser &quot;Oauth2-program&quot; den här typen av åtkomstlänk mellan en app och en server som [!DNL Workfront]. Mer information finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* Mer information om hur du skapar anpassade OAuth2-program finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med inloggningsuppgifter (auktoriseringskodflöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med hjälp av ett auktoriseringskodsflöde](../../wf-api/api/oauth-app-code-token-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med serverautentisering (JWT-flöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](../../wf-api/api/oauth-app-jwt-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med PKCE finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med PKCE-flöde](../../wf-api/api/oauth-app-pkce-flow.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td> <p>[!UICONTROL Plan] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> Du måste vara en [!DNL Workfront] administratör. </p>
    <p>För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Du måste skapa [!UICONTROL OAuth2] program för din organisation innan du kan visa eller hantera dem.

Mer information finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Hantera anpassade OAuth2-program

* [Visa och redigera anpassade OAuth2-program](#view-and-edit-custom-oauth2-applications)
* [Ta bort anpassade OAuth2-program](#delete-custom-oauth2-applications)

### Visa och redigera anpassade OAuth2-program {#view-and-edit-custom-oauth2-applications}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL System]** väljer **[!UICONTROL OAuth Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
1. Håll muspekaren över programmet och klicka **[!UICONTROL Edit]** ![](assets/edit-icon.png) när den visas längst till höger.
1. (Valfritt) Redigera information om programmet.

   Fälten för OAuth2- och JWT-program finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Ta bort anpassade OAuth2-program {#delete-custom-oauth2-applications}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL System]** väljer **[!UICONTROL OAuth Applications]**.
1. Klicka på **  **.
1. Håll muspekaren över programmet och klicka **[!UICONTROL Delete]** ![](assets/delete.png) när den visas längst till höger.

## Hantera klienthemligheter i OAuth2-program

* [Visa information om klienthemlighet](#view-client-secret-details)
* [Lägga till eller redigera anteckningar för Klienthemlighet](#add-or-edit-notes-for-client-secret)
* [Ta bort klienthemlighet](#delete-client-secret)

### Visa information om klienthemlighet {#view-client-secret-details}

>[!IMPORTANT]
>
>Du kan inte visa själva klienthemligheten. Om du har förlorat din klienthemlighet måste du ta bort den och skapa en ny.
>
>* Information om hur du tar bort en klienthemlighet finns i [Ta bort klienthemlighet](#delete-client-secret) i den här artikeln.
>* Information om hur du skapar en ny klienthemlighet finns i [Skapa ett OAuth2-program](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. Klicka på *[!UICONTROL *Main Menu]** ikon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL System]** väljer **[!UICONTROL OAuth Applications]**.
1. Håll pekaren över programmet och klicka på knappen **[!UICONTROL Edit]** -ikonen när den visas längst till höger.
1. Visa information i området Klienthemlighet:

   * Skapad den
   * Senast använt den
   * Anteckningar

      Information om hur du lägger till anteckningar i en klienthemlighet finns i [Lägga till eller redigera anteckningar för Klienthemlighet](#add-or-edit-notes-for-client-secret).

### Lägga till eller redigera anteckningar för Klienthemlighet {#add-or-edit-notes-for-client-secret}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL System]** väljer **[!UICONTROL OAuth Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
1. Håll pekaren över programmet och klicka på knappen **[!UICONTROL Edit]** -ikonen när den visas längst till höger.
1. Leta reda på den klienthemlighet som du vill lägga till eller redigera en anteckning för.
1. Klicka på rutan som innehåller information om klienthemligheten.

   Nu kan du lägga till anteckningstext eller redigera befintlig anteckningstext.

   >[!NOTE]
   >
   >Anteckningstexten får innehålla högst 64 tecken.

1. Klicka utanför rutan eller tryck på **[!UICONTROL Enter]** om du vill spara anteckningstexten.

### Ta bort klienthemlighet {#delete-client-secret}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL System]** väljer **[!UICONTROL OAuth Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
1. Håll pekaren över programmet och klicka på knappen **[!UICONTROL Edit]** -ikonen när den visas längst till höger.
1. Leta reda på den klienthemlighet som du vill ta bort.
1. Klicka på **[!UICONTROL Delete]** icon ![](assets/delete.png) bredvid Klienthemligheten.

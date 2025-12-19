---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Visa och hantera anpassade OAuth2-program
description: Som Adobe Workfront-administratör kan du visa och hantera OAuth2-program för din instans av Workfront, som ger andra program åtkomst till Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Visa och hantera anpassade OAuth2-program

Som [!DNL Adobe Workfront]-administratör kan du visa och hantera OAuth2-program för din instans av [!DNL Workfront], som ger andra program åtkomst till [!UICONTROL Workfront].

>[!NOTE]
>
>* I OAuth2-kontexten hänvisar Oauth2-programmet till den här typen av åtkomstlänk mellan ett program och en server som [!DNL Workfront]. Mer information finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Du kan ha upp till totalt tio OAuth2-program samtidigt.

* Mer information, instruktioner och information om hur du skapar anpassade OAuth2-program finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Mer information, instruktioner och information om hur du konfigurerar och använder OAuth2-programmet med inloggningsuppgifter (auktoriseringskodflöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med hjälp av auktoriseringskodflöde](../../wf-api/api/oauth-app-code-token-flow.md).
* Mer information, instruktioner och information om hur du konfigurerar och använder OAuth2-programmet med serverautentisering (JWT-flöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](../../wf-api/api/oauth-app-jwt-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med PKCE finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med PKCE-flöde](../../wf-api/api/oauth-app-pkce-flow.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara Workfront-administratör. </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste skapa [!UICONTROL OAuth2] program för din organisation innan du kan visa eller hantera dem.

Mer information finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Hantera anpassade OAuth2-program

* [Visa och redigera anpassade OAuth2-program](#view-and-edit-custom-oauth2-applications)
* [Ta bort anpassade OAuth2-program](#delete-custom-oauth2-applications)

### Visa och redigera anpassade OAuth2-program {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
1. Hovra över programmet och klicka på ikonen **[!UICONTROL Edit]** ![Redigera](assets/edit-icon.png) när den visas längst till höger.
1. (Valfritt) Redigera information om programmet.

   Fälten för OAuth2- och JWT-program finns i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Ta bort anpassade OAuth2-program {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth Applications]**.
1. Hovra över programmet och klicka på **[!UICONTROL Delete]** ![Ta bort](assets/delete.png) när det visas längst till höger.

## Hantera klienthemligheter i OAuth2-program

* [Visa information om klienthemlighet](#view-client-secret-details)
* [Lägga till eller redigera anteckningar för Klienthemlighet](#add-or-edit-notes-for-client-secret)
* [Ta bort klienthemlighet](#delete-client-secret)

### Visa information om klienthemlighet {#view-client-secret-details}

>[!IMPORTANT]
>
>Du kan inte visa själva klienthemligheten. Om du har förlorat din klienthemlighet måste du ta bort den och skapa en ny.
>
>* Om du vill ta bort en klienthemlighet läser du [Ta bort klienthemlighet](#delete-client-secret) i den här artikeln.
>* Information om hur du skapar en ny klienthemlighet finns i [Skapa ett OAuth2-program](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) i [Skapa OAuth2-program för [!DNL Workfront] integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth Applications]**.
1. Håll pekaren över programmet och klicka på ikonen **[!UICONTROL Edit]** när den visas längst till höger.
1. Visa information i området Klienthemlighet:

   * Skapad den
   * Senast använt den
   * Anteckningar

     Mer information om hur du lägger till anteckningar i en klienthemlighet finns i [Lägga till eller redigera anteckningar för Klienthemlighet](#add-or-edit-notes-for-client-secret).

### Lägga till eller redigera anteckningar för Klienthemlighet {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
1. Håll pekaren över programmet och klicka på ikonen **[!UICONTROL Edit]** när den visas längst till höger.
1. Leta reda på den klienthemlighet som du vill lägga till eller redigera en anteckning för.
1. Klicka på rutan som innehåller information om klienthemligheten.

   Nu kan du lägga till anteckningstext eller redigera befintlig anteckningstext.

   >[!NOTE]
   >
   >Anteckningstexten får innehålla högst 64 tecken.

1. Klicka utanför rutan eller tryck på **[!UICONTROL Enter]** för att spara anteckningstexten.

### Ta bort klienthemlighet {#delete-client-secret}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
1. Håll pekaren över programmet och klicka på ikonen **[!UICONTROL Edit]** när den visas längst till höger.
1. Leta reda på den klienthemlighet som du vill ta bort.
1. Klicka på ikonen **[!UICONTROL Delete]** ![Ta bort](assets/delete.png) intill klienthemligheten.

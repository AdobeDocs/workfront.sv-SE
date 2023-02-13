---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fel: SSO-användare kan inte logga in på [!DNL Adobe Workfront] På grund av olika fel'
description: När du får ett inloggningsfel om federerad enkel inloggning, din kombination av användarnamn och lösenord eller din åtkomst till [!DNL Workfront], the problem might be that your [!DNL Workfront] -instansen använder enkel inloggning och du försöker logga in med en felaktig URL. Kontrollera att du loggar in med rätt URL utan något efter ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Fel: SSO-användare kan inte logga in på [!DNL Adobe Workfront] På grund av olika fel

## Problem

Jag kan inte logga in på [!DNL Workfront] och fick ett av följande fel:

* Du kan tyvärr inte komma åt [!DNL Workfront] via inloggningsskärmen. [!DNL Workfront] har konfigurerats för enkel federerad inloggning med SAML 2.0. Kontakta [!DNL Workfront] administratör.
* Kombinationen av användarnamn och lösenord var inte helt rätt. Kontrollera att du inte har aktiverat ändlåset och försök igen.
* Du har tyvärr inte åtkomst till [!DNL Workfront]. Kontakta [!DNL Workfront] administratör för att få ett användarnamn och lösenord.

## Lösning

Dina [!DNL Workfront] -instansen använder enkel inloggning, och du försöker logga in via en felaktig URL. Kontrollera att du loggar in med rätt URL utan något efter &quot;.com&quot;

>[!TIP]
>
>Ta bort alla befintliga bokmärken som har ogiltiga URL-adresser.

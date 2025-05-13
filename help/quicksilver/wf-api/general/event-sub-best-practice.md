---
content-type: api
navigation-topic: general-api
title: Bästa praxis för händelseteckning
description: Bästa praxis för händelseteckning
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 19e0b792bc49ede0504af479952fdbdf384dc73c
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Bästa praxis för händelseteckning

Meddelanden om Adobe Workfront Event-prenumerationer skickas automatiskt från Workfront när du har konfigurerat tjänsten korrekt och skapat en Event-prenumeration som utlöser dessa meddelandeleveranser. Mer information om hur du konfigurerar händelseprenumerationer finns i [Leveranskrav för händelseprenumeration](../../wf-api/general/setup-event-sub-endpoint.md).


Nedan beskrivs några tips på hur du effektivt kan skapa händelseteckningar.

## Ange alla obligatoriska fält för begärandeinnehåll

Kontrollera att alla obligatoriska fält för begärandeinnehåll har skickats till API:t. Mer information om alla obligatoriska attribut för begäran finns i [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

## Undvik att ta med extra innehållsfält

Inkludera inte extra innehållsfält i begäran eftersom detta leder till att API:t inte kan skapa en prenumeration.

## Fullständig testning inom respitperioden

Försök att få alla prenumerationstester gjorda inom 100-meddelandets respitperiod. Mer information om den här respitperioden finns i [Vanliga frågor och svar - Händelseprenumerationer](../../wf-api/general/event-subs-faq.md).

## Uppfyll standardkraven för leverans av prenumerationsmeddelanden för händelse

Kontrollera att prenumerationens slutpunkt uppfyller leveransvillkoren för standardprenumerationsmeddelanden. Mer information om de här kraven finns i [Leveranskrav för händelseteckning](../../wf-api/general/setup-event-sub-endpoint.md).

## Tillåtslista IP-adresser efter global region

För att kunna ta emot händelseprenumerationsnyttolaster via din brandvägg måste du lägga till IP-adresserna i tillåtelselista efter global region. Mer information finns i [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

## ha rätt åtkomstnivå och autentisering

För att skapa, fråga efter eller ta bort en händelseprenumeration behöver din Workfront-användare:

* Åtkomstnivån **Systemadministratör**
Mer information finns i [Bevilja en användare fullständig administrativ åtkomst](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) eller [Bevilja användare administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) .

* Ett `sessionID`-huvud krävs för att använda API:t för händelseprenumerationer

  Mer information finns i [Autentisering](api-basics.md#authentication) i [API-grunder](api-basics.md).

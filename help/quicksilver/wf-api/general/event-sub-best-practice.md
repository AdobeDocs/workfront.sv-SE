---
content-type: api
navigation-topic: general-api
title: Bästa praxis för händelseteckning
description: Bästa praxis för händelseteckning
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Bästa praxis för händelseteckning

Meddelanden om Adobe Workfront Event-prenumerationer skickas automatiskt från Workfront när du har konfigurerat tjänsten korrekt och skapat en Event-prenumeration som utlöser dessa meddelandeleveranser. Mer information om hur du konfigurerar händelseprenumerationer finns i [Leveranskrav för evenemangsprenumeration](../../wf-api/general/setup-event-sub-endpoint.md).


Nedan följer några tips om hur du effektivt kan skapa händelseteckningar.

## Ange alla obligatoriska fält för begärandeinnehåll

Kontrollera att alla obligatoriska fält för begärandeinnehåll har skickats till API:t. Mer information om alla obligatoriska attribut finns i [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

## Undvik att ta med extra innehållsfält

Inkludera inte extra innehållsfält i begäran eftersom detta leder till att API:t inte kan skapa en prenumeration.

## Fullständig testning inom respitperioden

Försök att få alla prenumerationstester gjorda inom 100-meddelandets respitperiod. Mer information om denna respitperiod finns i [Frågor och svar - Evenemangsprenumerationer](../../wf-api/general/event-subs-faq.md).

## Uppfyll standardkraven för leverans av prenumerationsmeddelanden för händelse

Kontrollera att prenumerationens slutpunkt uppfyller leveransvillkoren för standardprenumerationsmeddelanden. Mer information om dessa krav finns i [Leveranskrav för evenemangsprenumeration](../../wf-api/general/setup-event-sub-endpoint.md).

## Tillåtslista IP-adresser efter global region

För att kunna ta emot händelseprenumerationsnyttolaster via din brandvägg måste du lägga till IP-adresserna i tillåtelselista efter global region. Mer information finns på [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

## ha rätt åtkomstnivå och en API-nyckel

För att skapa, fråga efter eller ta bort en händelseprenumeration behöver din Workfront-användare:

* En åtkomstnivå på **Systemadministratör**
Mer information finns på [Bevilja användaren fullständig administrativ åtkomst](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) eller [Ge användarna administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* En API-nyckel

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->

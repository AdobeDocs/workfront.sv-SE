---
content-type: reference
navigation-topic: notifications
title: 'Meddelanden: Delegering'
description: I följande meddelanden får du information om vilka uppgifter du har gjort och vilka delegeringar du har gjort åt dig i Adobe Workfront.
author: Courtney
feature: Get Started with Workfront
exl-id: bd329c5a-4440-4bb7-96f1-30e83c213851
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Meddelanden: Delegering

I följande meddelanden får du information om uppgifter och om de delegeringar du gjort eller andra som gjorts åt dig i [!DNL Adobe Workfront].

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Ändra dina egna e-postmeddelanden](activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](event-notifications.md).

>[!NOTE]
>
>Dessa meddelanden är aktiverade som standard. Du kan inte konfigurera de här meddelandena för ett dagligt e-postmeddelande med sammandrag.

| Delegering | Fält som visas i e-postmeddelandet | Typ av e-postmeddelande |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|----------------------------|
| **Jag delegerar mina uppgifter och ärenden (bekräftelse)**: Den användare som delegerar sina uppgifter och ärenden får en bekräftelse på att de har konfigurerat delegeringen. Ämnet för e-postmeddelandet är: *[!UICONTROL You delegated your tasks and issues to] (namn) från (startdatum till slutdatum)*. | Delegeringsnamnet Start- och slutdatum för delegeringen | **Direkt** |
| **Jag avbryter delegeringen av mina aktiviteter och ärenden (bekräftelse)**: Den användare som avbryter delegeringen av sina aktiviteter och ärenden får en bekräftelse på att de har stoppat delegeringen. Ämnet för e-postmeddelandet är: *[!UICONTROL You stopped your delegation of tasks and issues to] (namn)*. | Delegatnamn | **Direkt** |
| **Någon delegerar sina uppgifter och utgåvor till mig**: Den användare som har delegerats till någon persons uppgifter och utgåvor får ett e-postmeddelande när delegeringen startas. Ämnet för e-postmeddelandet är: *(Namn) [!UICONTROL delegated tasks and issues to you from] (Startdatum till slutdatum)*. | Den tilldelades namn Start- och slutdatum för delegeringen | **Direkt** |
| **Någon stoppar delegeringen av sina uppgifter och utgåvor till mig**: Den användare som delegerats till någon annans uppgifter och utgåvor får ett e-postmeddelande när delegeringen avbryts. Ämnet för e-postmeddelandet är: *(Namn) [!UICONTROL stopped task and issue delegation to you.]* | Uppgiftslämnarens namn | **Direkt** |

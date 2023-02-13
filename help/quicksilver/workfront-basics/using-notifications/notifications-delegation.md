---
content-type: reference
navigation-topic: notifications
title: '''Meddelanden: Delegering'
description: I följande meddelanden får du information om vilka uppgifter du har gjort och vilka delegeringar du har gjort åt dig i Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: bd329c5a-4440-4bb7-96f1-30e83c213851
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Meddelanden: Delegering

I följande meddelanden får du veta mer om uppgifter och de delegeringar du gjort eller andra som gjorts åt dig i [!DNL Adobe Workfront].

Mer information om hur du konfigurerar vilka meddelanden du får finns i [Aktivera eller inaktivera egna händelsemeddelanden](activate-or-deactivate-your-own-event-notifications.md).

Se även [Händelsemeddelanden](event-notifications.md).

>[!NOTE]
>
>Dessa meddelanden är aktiverade som standard. Du kan inte konfigurera de här meddelandena för ett dagligt e-postmeddelande med sammandrag.

| Delegering | Fält som visas i e-postmeddelandet | Typ av e-postmeddelande |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|----------------------------|
| **Jag delegerar mina uppgifter och ärenden (bekräftelse)**: Användaren som delegerar sina uppgifter och ärenden får en bekräftelse på att de har konfigurerat delegeringen. Ämnet för e-postmeddelandet är: *[!UICONTROL You delegated your tasks and issues to](Namn) från (startdatum till slutdatum)*. | Delegeringsnamnet Start- och slutdatum för delegeringen | **Direkt** |
| **Jag avbryter delegeringen av mina uppgifter och frågor (bekräftelse)**: Användaren som avbryter delegeringen av sina uppgifter och utgåvor får en bekräftelse på att de har stoppat delegeringen. Ämnet för e-postmeddelandet är: *[!UICONTROL You stopped your delegation of tasks and issues to](Namn)*. | Delegatnamn | **Direkt** |
| **Någon delegerar sina uppgifter och ärenden till mig**: Användaren som delegeras till någon annans uppgifter och ärenden får ett e-postmeddelande när delegeringen startar. Ämnet för e-postmeddelandet är: *(Namn) [!UICONTROL delegated tasks and issues to you from] (Startdatum till slutdatum)*. | Den tilldelades namn Start- och slutdatum för delegeringen | **Direkt** |
| **Någon stoppar delegeringen av deras uppgifter och ärenden till mig**: Användaren som delegerats till någon annans uppgifter och ärenden får ett e-postmeddelande när delegeringen avbryts. Ämnet för e-postmeddelandet är: *(Namn)[!UICONTROL stopped task and issue delegation to you.]* | Uppgiftslämnarens namn | **Direkt** |

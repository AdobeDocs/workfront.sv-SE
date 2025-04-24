---
content-type: overview
navigation-topic: notifications
title: Händelsemeddelanden
description: Händelsemeddelanden är e-postmeddelanden som utlöses av olika typer av händelser för objekt som projekt, uppgifter eller problem. De skickas när något händer i projektet som andra behöver känna till. Beroende på händelsen får användarna e-postmeddelanden om händelsen direkt, dagligen eller både direkt och dagligen.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Händelsemeddelanden

<!-- Audited: 4/2025 -->

Händelsemeddelanden är e-postmeddelanden som utlöses av olika typer av händelser för objekt som projekt, uppgifter eller problem. De skickas när något händer i projektet som andra behöver känna till. Beroende på händelsen får användarna e-postmeddelanden om händelsen direkt, dagligen eller både direkt och dagligen.

>[!NOTE]
>
>Händelsemeddelanden är en av flera typer av [!DNL Adobe Workfront]-meddelanden. Mer information om alla meddelandetyper i [!DNL Workfront] finns i [Översikt över meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

## Konfigurera händelsemeddelanden

E-postmeddelanden om händelser kan konfigureras på följande nivåer:

* **Systemnivå**: En [!DNL Workfront]-administratör kan aktivera och inaktivera händelsemeddelanden på systemnivå, vilket förklaras i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Alla grupper ärver systemmeddelanden som standard, men gruppadministratörer kan eventuellt ändra vissa konfigurationer på gruppnivån om det tillåts av [!DNL Workfront]-administratören.

* **Gruppnivå**: En gruppadministratör kan konfigurera ett händelsemeddelande för grupper som de hanterar efter att en [!DNL Workfront]-administratör har låst upp den här funktionen för grupper. Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för [!DNL Workfront]-administratörer (för alla grupper). Mer information finns i [Visa och konfigurera händelsemeddelanden för en grupp](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

* **Användarnivå**: Alla händelsemeddelanden som aktiveras i hela systemet visas i varje användares [!UICONTROL Notifications] -avsnitt i den enskilda profilen. Användarna kan aktivera och inaktivera sina enskilda händelsemeddelanden där.

  [!DNL Workfront] administratörer och användare med behörighet att redigera andra användare kan också aktivera och inaktivera meddelanden i en enskild användares profil.

  Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Meddelanden på användarnivå innehåller även [!DNL Workfront Goals] meddelanden. Administratören [!DNL Workfront] eller gruppadministratören kan dock inte konfigurera meddelanden för [!DNL Workfront Goals]. Varje användare måste konfigurera sina egna [!DNL Workfront Goals]-meddelanden i sin profil. Om du har behörighet att redigera användare kan du även ändra dessa meddelanden för andra. Information om hur du aktiverar [!DNL Workfront Goals]-meddelanden för din profil eller för andra användare som du har behörighet att redigera finns i [Meddelanden: Mål](../../workfront-basics/using-notifications/notifications-goals.md).

  Mer information om vilka meddelanden [!DNL Workfront]-administratören kan konfigurera finns i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Innehåll för händelsemeddelanden

Ett e-postmeddelande med en händelse innehåller information om händelsen som inträffade och en länk till [!DNL Workfront] där du kan se händelsen i systemet. Mer information om hur du tar emot e-postmeddelanden finns i [Översikt över meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

En [!DNL Workfront]-administratör kan inte ändra e-postmeddelandeinnehåll som det har konfigurerats av [!DNL Workfront], men de kan ändra ämnesrader för e-postaviseringar. Mer information finns i [Anpassa e-postavsnitt för händelsemeddelanden](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

En lista över alla [!DNL Workfront]-händelsemeddelanden, tillsammans med en kort beskrivning av varje händelse och om den är aktiv eller inaktiv som standard, finns i [Händelsemeddelandetyper](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

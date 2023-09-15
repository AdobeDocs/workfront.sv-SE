---
content-type: overview
navigation-topic: notifications
title: Händelsemeddelanden
description: Händelsemeddelanden är e-postmeddelanden som utlöses av olika typer av händelser för objekt som projekt, uppgifter eller problem. De skickas när något händer i projektet som andra behöver känna till. Beroende på händelsen får användarna e-postmeddelanden om händelsen direkt, dagligen eller både direkt och dagligen.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Händelsemeddelanden

Händelsemeddelanden är e-postmeddelanden som utlöses av olika typer av händelser för objekt som projekt, uppgifter eller problem. De skickas när något händer i projektet som andra behöver känna till. Beroende på händelsen får användarna e-postmeddelanden om händelsen direkt, dagligen eller både direkt och dagligen.

>[!NOTE]
>
>Händelsemeddelanden är en av flera typer [!DNL Adobe Workfront] meddelanden. Mer information om alla [!DNL Workfront] meddelandetyper, se [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

## Konfigurera händelsemeddelanden

E-postmeddelanden med händelsemeddelanden kan konfigureras på följande nivåer i listan nedan. Konfigurationen av ett händelsemeddelande består av att aktivera eller inaktivera det.

* **Systemnivå**: A [!DNL Workfront] administratören kan aktivera och inaktivera händelsemeddelanden på systemnivå, vilket förklaras i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Alla grupper ärver systemmeddelanden som standard, men gruppadministratörer kan eventuellt ändra vissa konfigurationer på gruppnivån om det tillåts av [!DNL Workfront] administratör, enligt beskrivningen i nästa punkt nedan.

* **Gruppnivå**: En gruppadministratör kan konfigurera ett händelsemeddelande för grupper som de hanterar efter en [!DNL Workfront] administratören låser upp den här funktionen för grupper. Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller [!DNL Workfront] administratörer (för alla grupper). Mer information finns i [Visa och konfigurera händelseaviseringar för en grupp](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Den här funktionaliteten är inledningsvis bara tillgänglig för kunder i kluster 4 som en del av en fasad utrullning. Det kommer att bli tillgängligt för andra kluster kort därefter. Artikeln uppdateras när detta inträffar.

* **Användarnivå**: Alla händelsemeddelanden som aktiveras i hela systemet visas i varje användares [!UICONTROL Notifications] i respektive profil. Användarna kan aktivera och inaktivera sina enskilda händelsemeddelanden där.

  [!DNL Workfront] administratörer och användare med behörighet att redigera andra användare kan också aktivera och inaktivera meddelanden i profilen för enskilda användare.

  Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Meddelanden på användarnivå innehåller även [!DNL Workfront Goals] meddelanden. Men [!DNL Workfront] administratören eller gruppadministratören kan inte konfigurera meddelanden för [!DNL Workfront Goals]. Varje användare måste konfigurera sina egna [!DNL Workfront Goals] meddelanden i sin profil. Om du har behörighet att redigera användare kan du även ändra dessa meddelanden för andra. För aktivering [!DNL Workfront Goals] meddelanden om din profil eller om andra användare som du har behörighet att redigera finns i [Meddelanden: Mål](../../workfront-basics/using-notifications/notifications-goals.md).

  Om du vill ha mer information om vilka meddelanden [!DNL Workfront] administratörer kan konfigurera, se [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] är bara tillgängliga i den nya [!DNL Adobe Workfront] upplevelse.

## Innehåll för händelsemeddelanden

Ett e-postmeddelande med en händelse innehåller information om händelsen som inträffade och en länk till [!DNL Workfront] där du kan se händelsen i systemet. Mer information om hur du tar emot e-postmeddelanden finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] administratören kan inte ändra innehållet i e-postmeddelandena eftersom de har konfigurerats av [!DNL Workfront]. De kan dock ändra ämnesraderna i e-postmeddelanden om händelser. Mer information finns i [Anpassa e-postämnen för händelsemeddelanden](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

En lista över alla [!DNL Workfront] händelsemeddelanden, tillsammans med en kort beskrivning av varje händelse och om den är aktiv eller inaktiv som standard, finns i [Händelsemeddelanden är tillgängliga i [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

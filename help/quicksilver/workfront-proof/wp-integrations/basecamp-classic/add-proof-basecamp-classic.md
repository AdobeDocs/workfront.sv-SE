---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Lägga till ett korrektur i ett Classic-projekt
description: När du har konfigurerat [!DNL Basecamp Classic] integration kan du börja lägga till korrektur i projekt i [!DNL Basecamp Classic] konto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: fbca81fb-97c4-449a-9c64-cfd902ea1e19
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Lägg till ett korrektur i en [!DNL Basecamp Classic] Projekt

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

När du har konfigurerat [!DNL Basecamp Classic] integration kan du börja lägga till korrektur i projekt i [!DNL Basecamp Classic] konto.

När du har lagt till ett korrektur i en [!DNL Basecamp Classic] kommer dina granskare att få ett e-postmeddelande med en länk för att visa korrekturet i [!DNL Workfront Proof] och en länk för att öppna meddelandet i deras [!DNL Basecamp Classic] konto.

När de har öppnat meddelandet kan de kommentera och fatta beslut i korrekturet inifrån de [!DNL Basecamp] konto.

Mer information finns i [Granska ett korrektur i [!DNL Basecamp Classic]](../../../workfront-proof/wp-integrations/basecamp-classic/review-proof-basecamp-classic.md).

## Lägga till ett nytt korrektur i en [!DNL Basecamp Classic] Projekt

>[!NOTE]
>
>Innan du lägger till ett korrektur i [!DNL Basecamp Classic]måste du se till att [!DNL Basecamp] integreringen är aktiverad och att du har rätt [!DNL Basecamp] konto som valts i dina personliga inställningar (eftersom du kan integrera med fler än ett [!DNL [!DNL Basecamp]]-konto, men lägg bara till korrektur i ett [!DNL Basecamp] konto åt gången). Mer information om dina inställningar finns i [Personliga inställningar.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Skapa ett korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Om du vill meddela granskarna via e-post måste du se till att **[!UICONTROL Notify people by mail]** är markerat.\
   Observera att [!DNL Basecamp] granskarna får ytterligare [!DNL Basecamp] meddelande.

1. I **[!UICONTROL Organize]** avsnitt, klicka **[!UICONTROL Add proof to a [!DNL Basecamp] project]**.

1. I **[!UICONTROL Add to [!DNL Basecamp]]** visas klickar du på **[!UICONTROL Refresh the data]** synkronisera med [!DNL Basecamp Classic].

1. Ange om du vill att det här beviset ska vara privat i [!DNL Basecamp] (alternativ inte tillgängligt i Nytt [!DNL Basecamp]).
1. Välj [!DNL Basecamp Classic] projekt.
1. Välj [!UICONTROL [!DNL Basecamp Classic] Message Category].
1. Under **[!UICONTROL People on the project]** markerar du kryssrutorna för granskarna i [!DNL Basecamp Classic] konto som du vill lägga till i korrekturet.\
   Granskarna visas i sin standardroll/e-postavisering. De valda granskarna får ett meddelande i [!DNL Basecamp] för det här korrekturet och även ett e-postmeddelande från [!DNL Workfront Proof].

1. Om granskarnas standardinställningar har ändrats måste du uppdatera [!DNL Basecamp] data innan de nya standardvärdena används. Så här uppdaterar du [!DNL Basecamp] klickar du på &quot;[!UICONTROL refresh]&quot; på [!DNL Basecamp] popup-fönster [!DNL Workfront Proof]. Inkludera ditt eget namn om du även vill få meddelandet i [!DNL Basecamp].
1. Klicka på **[!UICONTROL OK]**.
1. Använd eventuella andra inställningar som du behöver för korrekturet (som vanligt) och klicka på **[!UICONTROL Save]** för att skicka in bevis.

## Lägga till ett befintligt korrektur i en [!DNL Basecamp Classic] Projekt

1. I [!DNL Workfront Proof], går till [!UICONTROL Proof details] sida, enligt beskrivning i  [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. I **[!UICONTROL Workflow]** öppnar du **[!UICONTROL More sharing options]** -avsnitt.

1. Se till att **[!UICONTROL Proof URL]** och **[!UICONTROL Embed code]** är inställda på **[!UICONTROL Enable]**.

1. Klicka på **[!UICONTROL Add proof to a [!DNL Basecamp] project]**.
1. I [!UICONTROL Add to [!DNL Basecamp]] gör följande i den ruta som visas:

   1. Klicka **[!UICONTROL Refresh the data]** synkronisera med [!DNL Basecamp Classic] innan du fortsätter.
   1. Ange om du vill att det här korrekturet ska vara [!UICONTROL Private] in [!DNL Basecamp] (alternativ inte tillgängligt i Nytt [!DNL Basecamp]).
   1. Välj [!DNL Basecamp Classic] projekt.
   1. Välj [!UICONTROL [!DNL Basecamp Classic] Message Category].
   1. Under **[!UICONTROL People on the project]** markerar du kryssrutorna för granskarna i [!DNL Basecamp Classic] konto som du vill lägga till i korrekturet.
   1. Granskarna visas i sin standardroll/e-postavisering. De valda granskarna får ett meddelande i [!DNL Basecamp] för det här korrekturet och även ett e-postmeddelande från [!DNL Workfront Proof].

      >[!NOTE]
      >
      > Om granskarnas standardinställningar har ändrats måste du uppdatera [!DNL Basecamp] data innan de nya standardvärdena används. Så här uppdaterar du [!DNL Basecamp] klickar du på &quot;[!UICONTROL refresh]&quot; på [!DNL Basecamp] popup-fönster [!DNL Workfront Proof]. Inkludera ditt eget namn om du även vill få meddelandet i [!DNL Basecamp].

1. Klicka på **[!UICONTROL OK]**.

När du har lagt till korrekturet i [!DNL Basecamp Classic] visas ytterligare alternativ i [!UICONTROL More sharing options] i [!UICONTROL Proof details] sida (för information om den här sidan, se [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md). Du kan:

* Redigera [!DNL Basecamp Classic] projektinformation.
* Gå till meddelandet i [!DNL Basecamp Classic] genom att klicka på projektets URL längst ned i rutan (URL:en innehåller en identifierare för korrekturet).

>[!NOTE]
>
> Om du inte har en [!DNL Basecamp Classic] session öppnad i ett annat webbläsarfönster måste du logga in på [!DNL Basecamp Classic] innan du kan se meddelandet i [!DNL Basecamp].

Se även [Granska ett korrektur i [!DNL Basecamp Classic]](../../../workfront-proof/wp-integrations/basecamp-classic/review-proof-basecamp-classic.md).

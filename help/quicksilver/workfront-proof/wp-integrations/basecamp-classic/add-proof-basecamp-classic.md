---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Lägga till ett korrektur i ett Classic-projekt
description: När du har konfigurerat  [!DNL Basecamp Classic] integreringen kan du börja lägga till korrektur i projekt på ditt [!DNL Basecamp Classic] konto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: fbca81fb-97c4-449a-9c64-cfd902ea1e19
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Lägg till ett korrektur i ett [!DNL Basecamp Classic]-projekt

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

När du har konfigurerat din [!DNL Basecamp Classic]-integrering kan du börja lägga till korrektur i projekt på ditt [!DNL Basecamp Classic]-konto.

När du har lagt till ett korrektur i ett [!DNL Basecamp Classic]-projekt får granskarna ett e-postmeddelande som innehåller en länk för att visa korrekturet i [!DNL Workfront Proof] och en länk för att öppna meddelandet i deras [!DNL Basecamp Classic]-konto.

När de öppnar meddelandet kan de kommentera och fatta beslut i korrekturet från sitt [!DNL Basecamp]-konto.

Mer information finns i [Granska ett korrektur i [!DNL Basecamp Classic]](../../../workfront-proof/wp-integrations/basecamp-classic/review-proof-basecamp-classic.md).

## Lägger till ett nytt korrektur i ett [!DNL Basecamp Classic]-projekt

>[!NOTE]
>
>Innan du lägger till ett korrektur i [!DNL Basecamp Classic] måste du se till att din [!DNL Basecamp]-integrering är aktiverad och att du har valt det relevanta [!DNL Basecamp]-kontot i dina personliga inställningar (eftersom du kan integrera med mer än ett [!DNL [!DNL Basecamp]]-konto, men bara lägga till korrektur i ett [!DNL Basecamp]-konto åt gången). Mer information om dina inställningar finns i [Personliga inställningar.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Skapa ett korrektur enligt beskrivningen i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Om du vill meddela granskarna via e-post kontrollerar du att **[!UICONTROL Notify people by mail]** är markerat.\
   Observera att dina [!DNL Basecamp]-granskare får ytterligare ett [!DNL Basecamp]-meddelande.

1. Klicka på **[!UICONTROL Add proof to a [!DNL Basecamp] project]** i avsnittet **[!UICONTROL Organize]**.

1. I rutan **[!UICONTROL Add to [!DNL Basecamp]]** som visas klickar du på **[!UICONTROL Refresh the data]** för att synkronisera med [!DNL Basecamp Classic].

1. Ange om du vill att det här korrekturet ska vara privat i [!DNL Basecamp] (alternativet är inte tillgängligt i Nytt [!DNL Basecamp]).
1. Välj ditt [!DNL Basecamp Classic]-projekt.
1. Välj din [!UICONTROL [!DNL Basecamp Classic] Message Category].
1. Under **[!UICONTROL People on the project]** markerar du kryssrutorna för de granskare i ditt [!DNL Basecamp Classic]-konto som du vill lägga till i korrekturet.\
   Granskarna visas i sin standardroll/e-postavisering. De valda granskarna får ett meddelande i [!DNL Basecamp] om detta korrektur och även ett e-postmeddelande från [!DNL Workfront Proof].

1. Om granskarens standardinställningar har ändrats måste du uppdatera [!DNL Basecamp]-data innan de nya standardvärdena används. Uppdatera [!DNL Basecamp]-data genom att klicka på länken [!UICONTROL refresh] på popup-menyn [!DNL Basecamp] i [!DNL Workfront Proof]. Inkludera ditt eget namn om du även vill ta emot meddelandet i [!DNL Basecamp].
1. Klicka på **[!UICONTROL OK]**.
1. Använd eventuella andra inställningar som du behöver för korrekturet (som vanligt) och klicka på **[!UICONTROL Save]** för att skicka in korrekturet.

## Lägger till ett befintligt korrektur i ett [!DNL Basecamp Classic]-projekt

1. Gå till sidan [!UICONTROL Proof details] i [!DNL Workfront Proof], enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Öppna avsnittet **[!UICONTROL More sharing options]** i avsnittet **[!UICONTROL Workflow]**.

1. Kontrollera att **[!UICONTROL Proof URL]** och **[!UICONTROL Embed code]** är inställda på **[!UICONTROL Enable]**.

1. Klicka på **[!UICONTROL Add proof to a [!DNL Basecamp] project]**.
1. Gör följande i rutan [!UICONTROL Add to [!DNL Basecamp]] som visas:

   1. Klicka på **[!UICONTROL Refresh the data]** om du vill synkronisera med [!DNL Basecamp Classic] innan du fortsätter.
   1. Ange om du vill att det här korrekturet ska vara [!UICONTROL Private] i [!DNL Basecamp] (alternativet är inte tillgängligt i Nytt [!DNL Basecamp]).
   1. Välj ditt [!DNL Basecamp Classic]-projekt.
   1. Välj din [!UICONTROL [!DNL Basecamp Classic] Message Category].
   1. Under **[!UICONTROL People on the project]** markerar du kryssrutorna för de granskare i ditt [!DNL Basecamp Classic]-konto som du vill lägga till i korrekturet.
   1. Granskarna visas i sin standardroll/e-postavisering. De valda granskarna får ett meddelande i [!DNL Basecamp] om detta korrektur och även ett e-postmeddelande från [!DNL Workfront Proof].

      >[!NOTE]
      >
      > Om granskarens standardinställningar har ändrats måste du uppdatera [!DNL Basecamp]-data innan de nya standardvärdena används. Uppdatera [!DNL Basecamp]-data genom att klicka på länken [!UICONTROL refresh] på popup-menyn [!DNL Basecamp] i [!DNL Workfront Proof]. Inkludera ditt eget namn om du även vill ta emot meddelandet i [!DNL Basecamp].

1. Klicka på **[!UICONTROL OK]**.

När du har lagt till korrekturet i ditt [!DNL Basecamp Classic]-projekt visas ytterligare alternativ i avsnittet [!UICONTROL More sharing options] på sidan [!UICONTROL Proof details] (mer information om den här sidan finns i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md). Du kan:

* Redigera projektinformationen för [!DNL Basecamp Classic].
* Gå till meddelandet i [!DNL Basecamp Classic] genom att klicka på projekt-URL:en längst ned i rutan (URL:en innehåller en identifierare för det här korrekturet).

>[!NOTE]
>
> Om du inte har en [!DNL Basecamp Classic]-session öppen i ett annat webbläsarfönster måste du logga in på ditt [!DNL Basecamp Classic]-konto innan du kan se meddelandet i [!DNL Basecamp].

Se även [Granska ett korrektur i [!DNL Basecamp Classic]](../../../workfront-proof/wp-integrations/basecamp-classic/review-proof-basecamp-classic.md).

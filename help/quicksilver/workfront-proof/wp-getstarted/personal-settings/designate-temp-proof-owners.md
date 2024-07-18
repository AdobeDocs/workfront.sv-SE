---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: personal-settings
title: Tillfälliga korrekturägare utses i  [!DNL Workfront Proof]
description: Om du inte kommer att vara på kontoret under en längre period kan du delegera ägarskap av dina korrektur till en annan användare på ditt konto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d00636d7-1eb1-4aac-9663-6335e7675836
source-git-commit: bf6c6c497d98d91ca78f892606a52f82ee4b5666
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Tillfälliga korrekturägare utses i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du inte kommer att vara på kontoret under en längre period kan du delegera ägarskap av dina korrektur till en annan användare på ditt konto.

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i [!DNL Workfront Proof].

Så här anger du tillfällig äganderätt till dina korrektur:

1. Gå till **[!UICONTROL Personal settings]** inom [!DNL Workfront Proof].\
   ![personal-settings.png](assets/personal-settings-350x83.png)

1. Klicka på fliken **[!UICONTROL Out of office]**. Följande inställningar är tillgängliga:

   * **[!UICONTROL Delegate your proofs to]** en annan användare i ditt konto.
   * Aktivera och inaktivera funktionen **[!UICONTROL Out of office]** genom att markera eller avmarkera kryssrutan.
   * Välj **[!UICONTROL Start date]**.

     Om alternativet **[!UICONTROL Start immediately]** väljs delegeras ägarskapet av korrektur till den valda användaren omedelbart efter att du har aktiverat funktionen.

     Om ett visst startdatum och en viss starttid anges aktiveras funktionen den valda dagen och vid den valda tidpunkten.

   * Välj **[!UICONTROL End date]**.

     Om inget slutdatum har valts delegeras ägandet av korrektur tills funktionen inaktiveras manuellt.

     Om ett visst slutdatum och en viss sluttid anges inaktiveras funktionen den valda dagen och vid den valda tidpunkten.

     ![out-of-office-options.png](assets/out-of-office-options-350x234.png)

1. När korrektur delegeras visas den delegerade ägaren i avsnittet **[!UICONTROL Details]** på sidan med korrekturinformation. Anteckningen om delegering av ägarskap visas i avsnittet **[!UICONTROL Activity]** på sidan med korrekturinformation.

   ![activity-section-Delegated.png](assets/activity-section-delegated-350x318.png)

   Ett [!UICONTROL Out of Office]-meddelande visas också i det ursprungliga korrekturägarkontot när funktionen aktiveras. Detta fungerar som en påminnelse till den ursprungliga ägaren och gör det även möjligt för dem att avsluta delegeringen direkt eller gå till [!UICONTROL Personal settings] för att justera detta.

   ![notification-on-account.png](assets/notification-on-account-350x15.png)

   När ägarskapet för dina korrektur återtas av den ursprungliga ägaren, försvinner den delegerade ägaren från avsnittet [!UICONTROL Details] på sidan med korrekturinformation och meddelandet [!UICONTROL Out of Office] visas inte längre på den ursprungliga korrekturägarens konto. En anteckning som visar att korrekturägarskap har återställts visas i avsnittet [!UICONTROL Activity] på sidan med korrekturinformation.

   >[!NOTE]
   >
   >Den delegerade ägaren finns kvar i korrekturarbetsflödet om du inte tar bort dem manuellt.

   ![[!UICONTROL activity-section-taken-back].png](assets/activity-section-taken-back-350x99.png)

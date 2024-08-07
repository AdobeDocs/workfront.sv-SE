---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Konfigurera alternativ för godkännandebeslut i  [!DNL Workfront Proof]
description: Du kan konfigurera beslutsalternativ för godkännande för alla korrektur som skapats av  [!DNL Workfront Proof] användare i din organisation.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Konfigurera alternativ för godkännandebeslut i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Som [!DNL Workfront Proof]-administratör med en Select- eller Premium-utgåva-plan kan du konfigurera beslutsalternativ för godkännande på följande sätt för alla korrektur som skapats av [!DNL Workfront Proof] -användare i din organisation:

* Ändra namnet på beslutet
* Ändra ordningen på besluten som visas i korrekturläsaren
* Bestäm vilka beslut som ska visas

I den här artikeln förklaras följande:

## Konfigurerar beslutsinställningar

1. Klicka på **[!UICONTROL Account Settings]**.
1. Öppna fliken **[!UICONTROL Decisions]**.
1. Gör någon av följande ändringar:

   * Om du vill dölja ett beslut klickar du på **[!UICONTROL Hide]** till höger om det beslut du inte behöver.
   * Om du vill byta namn på ett beslut klickar du på beslutsnamnet, redigerar det och klickar sedan utanför rutan (eller trycker på Retur). [!DNL Workfront Proof] uppdaterar namnet på beslutet för alla befintliga korrektur i systemet.

     >[!IMPORTANT]
     >
     >Behåll logiken för ett beslut när du byter namn på det. Standardbeslutet&quot;Avvisat&quot; kan till exempel ändras till&quot;Ny version krävs&quot;, men det bör inte ändras till&quot;Skicka till skrivare&quot;.)

     Om du vill gå tillbaka till standardinställningarna för [!DNL Workfront Proof] kan du klicka på Återställ standardbeslut.

>[!NOTE]
>
>* Logiken bakom besluten används för att beräkna den övergripande statusen för ett korrekturarbetsflöde om det finns flera beslut på olika nivåer.
>* Besluten&quot;Godkänd&quot; och&quot;Godkänd med ändringar&quot; utlöser nästa steg i ett automatiskt arbetsflöde.
>* Om du byter namn på ett beslut och vill verifiera logiken, kan du klicka på **[!UICONTROL Activity]** i den vänstra navigeringspanelen och kontrollera aktivitetsloggen där de ursprungliga besluten visas inom hakparentes.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Skapa beslutsorsaker

Beslutsskäl är ett bra sätt att samla in ytterligare beslutsinformation om ett bevis.

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**.

1. Öppna fliken **[!UICONTROL Decisions]**.
Som standard är anledningar tillgängliga för alla beslutsfattare i dina korrektur, men du kan begränsa det till enbart primära beslutsfattare.
Beroende på dina behov kan du välja flera anledningar eller göra det till en enda urvalslista. Du kan också göra skäl obligatoriska, vilket innebär att granskarna måste välja en anledning innan de kan spara sitt beslut om ett bevis.
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. Klicka på **[!UICONTROL New reason]** i avsnittet **[!UICONTROL Reasons]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. Skriv en titel för anledningsavsnittet i rutan som visas under **[!UICONTROL Reason]**.
1. Om du vill inkludera en textruta väljer du **[!UICONTROL Include text box]**.
1. Klicka på **[!UICONTROL Save]**.
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
Det viktigaste steget är att välja beslut som anledningarna ska visas på. Om du glömmer att göra det kommer orsaken inte att visas på korrekturet.

1. Markera rutorna i kolumnen **[!UICONTROL Display reasons]** i beslutslistan högst upp på sidan. Du kan välja ett eller flera beslut av dina skäl.
   ![reasons_-_Decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Skapa ett meddelande efter beslut

Du kan skapa ett meddelande som ska visas efter att en granskare har sparat sitt beslut på korrekturet.

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**.

1. Öppna fliken **[!UICONTROL Decisions]**.
1. Klicka på **[!UICONTROL Edit]** i slutet av raden **[!UICONTROL Message]** i avsnittet **[!UICONTROL Post decision message]**.
Du kan också bestämma om du vill att meddelandet ska visas för alla beslutsfattare eller om du vill begränsa det till den primära beslutsfattaren.
   ![post_Decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. I kolumnen **[!UICONTROL Display message]** anger du vilka beslut det här meddelandet ska visas på.
Om du inte väljer minst ett beslut visas inte meddelandet på korrekturet. Kontrollera minst en ruta i kolumnen.
   ![post_Decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)

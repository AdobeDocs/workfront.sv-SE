---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Nytt korrekturmeddelande
description: Få den här artikeln att fungera bättre för PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Nytt korrekturmeddelande

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

När du skapar ett nytt korrektur eller en ny version av ett korrektur, lägger till nya personer i ett korrektur eller lägger till ett arbetsflöde till ett korrektur, kan du bestämma om du vill skicka e-post till granskarna enligt följande artiklar:

* [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

E-postmeddelandet som mottagarna får kallas [!UICONTROL New Proof] e-post. Det är bara den som har skapat korrekturet och de användare som har behörighet att lägga till granskare i ett korrektur som kan kontrollera det här e-postmeddelandet. Mottagarna kan inte inaktivera det.

E-postmeddelandet Nytt korrektur innehåller:

* Ditt personliga meddelande (om du väljer att ta med ett)
* Om du alltid skickar samma anpassade meddelande till granskarna kan det vara bra att spara det i [!UICONTROL Personal settings] under [!UICONTROL Proofing defaults] -fliken. Mer information finns i .
* Personlig länk till beviset
* **[!UICONTROL View details]** länk som tar dig till associerad [!DNL Workfront] objekt (t.ex. ett projekt, en uppgift eller ett ärende)
* Miniatyrbild av korrekturbilden
* Följande korrekturinformation:

   * Korrekturnamn
   * Versionsnummer

      Mer information finns i .

   * Lista över granskarna och deras framsteg med korrekturet
   * En länk för att dela beviset med någon annan

      På så sätt kan du dela korrektur-URL:en och/eller hämtningslänken för originalfilen. Detta gör att du inte uttryckligen kan lägga till granskare i korrekturet, du delar bara det offentliga korrektur-URL:en och mottagaren får skrivskyddad åtkomst till korrekturet.

      Se [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) för mer information.

      Om du inte vill att den här länken ska visas i mottagarens e-post kan du inaktivera [!UICONTROL Public Sharing] inställningar på korrekturet

      (Hämta originalfil och offentlig URL). Se [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) för mer information.

## Aktivitetsloggen

Skicka en [!UICONTROL New Proof] e-post till en granskare loggas i [!UICONTROL Activity] avsnitt i [!UICONTROL Proof details] sida. Se  [Hantera[!UICONTROL  Proof Details] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) för mer information. Du kan kontrollera om [!UICONTROL New Proof] e-post aktiverades när ett korrektur skapades.

![New_Version_email_-_acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Om korrekturets skapare eller ägare har [!UICONTROL Proof Made] e-postmeddelanden som är inaktiverade som standard (i deras personliga inställningar) får de inga [!UICONTROL Proof made] eller [!UICONTROL New proof] e-postmeddelanden även om [!UICONTROL Notify people by email] är markerad på sidan Nytt korrektur. Mer information finns i .
>* Om e-postmeddelanden är inaktiverade som standard i [!UICONTROL Account settings] Bevisets skapare/ägare kommer inte att få något [!UICONTROL Proof made] eller [!UICONTROL New proof] e-postmeddelanden även om detta är aktiverat i deras personliga inställningar och [!UICONTROL Notify] Personen via e-post är markerad på sidan Nytt korrektur. Mer information finns i [The [!UICONTROL Proof Made] e-post](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) och se .
>




## Aktivera [!UICONTROL New Proof] e-post och inkludera ett anpassat meddelande

Du kan ange om du vill skicka en e-postavisering till granskarna om ett korrektur när du skapar det eller när du lägger till någon i det.

* [När du skapar ett korrektur](#when-you-create-a-proof)
* [När du lägger till en granskare i ett korrektur](#when-you-add-a-reviewer-to-a-proof)

### När du skapar ett korrektur {#when-you-create-a-proof}

När du skapar ett nytt korrektur i [!UICONTROL New proof] sida, under **[!UICONTROL Share]** kan du välja om du vill skicka e-postaviseringar:

* Här kan du bestämma om du vill [!UICONTROL Notify people by email] (1). Om du avmarkerar det här alternativet får ingen av dina granskare ett e-postmeddelande om att korrekturet är klart för granskning.
* Du kan även inkludera ett anpassat meddelande i e-postmeddelandet (2).
* Om du bestämmer dig för att lägga till ett eget anpassat meddelande kan du placera i en anpassad ämnesrad (3) och ett meddelande i e-postmeddelandets brödtext (4).
* Klicka på länken (5) om du vill ignorera det anpassade meddelandet.

   >[!NOTE]
   >
   >Om du alltid skickar samma anpassade meddelande till dina granskare kan det vara bra att spara det i dina personliga inställningar under [!UICONTROL Proofing defaults] -fliken. Mer information finns i .

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### När du lägger till en granskare i ett korrektur {#when-you-add-a-reviewer-to-a-proof}

Du kan välja om en ny granskare som läggs till i ett befintligt korrektur ska meddelas om korrekturet (liknande ovan).

* Lägg först till nya granskare genom att klicka på **[!UICONTROL Share this Version]** på **[!UICONTROL Proof details]** sidan (1).

![Korrektur_detaljer_sida_1.png](assets/proof-details-page-1-350x118.png)

* En ruta visas där du kan lägga till nya granskare. Du kan sedan bestämma om du vill att de ska meddelas via e-post (2) och välja att lägga till ett anpassat meddelande i e-postmeddelandet (3).

![Korrektur_detaljer_sida_2.png](assets/proof-details-page-2-350x174.png)

* Om du väljer att lägga till ett anpassat meddelande expanderar rutan och du kan lägga in en anpassad ämnesrad (4) och anpassad text i e-postmeddelandets brödtext (5). Du kan också ignorera det anpassade meddelandet genom att klicka på länken (6).

![Korrektur_detaljer_sida_3.png](assets/proof-details-page-3-350x258.png)

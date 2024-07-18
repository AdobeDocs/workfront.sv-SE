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
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Nytt korrekturmeddelande

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

När du skapar ett nytt korrektur eller en ny version av ett korrektur, lägger till nya personer i ett korrektur eller lägger till ett arbetsflöde till ett korrektur, kan du bestämma om du vill skicka e-post till granskarna enligt följande artiklar:

* [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Generera korrektur i  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

Det e-postmeddelande som dina mottagare får kallas [!UICONTROL New Proof]-e-post. Det är bara den som har skapat korrekturet och de användare som har behörighet att lägga till granskare i ett korrektur som kan kontrollera det här e-postmeddelandet. Mottagarna kan inte inaktivera det.

E-postmeddelandet Nytt korrektur innehåller:

* Ditt personliga meddelande (om du väljer att ta med ett)
* Om du alltid skickar samma anpassade meddelande till granskarna kan det vara bra att spara det i [!UICONTROL Personal settings] under fliken [!UICONTROL Proofing defaults]. Mer information finns i .
* Personlig länk till beviset
* **[!UICONTROL View details]**-länk som tar dig till det associerade [!DNL Workfront]-objektet (till exempel ett projekt, en aktivitet eller ett problem)
* Miniatyrbild av korrekturbilden
* Följande korrekturinformation:

   * Korrekturnamn
   * Versionsnummer
   * Lista över granskarna och deras framsteg med korrekturet
   * En länk för att dela beviset med någon annan

     På så sätt kan du dela korrektur-URL:en och/eller hämtningslänken för originalfilen. Detta gör att du inte uttryckligen kan lägga till granskare i korrekturet, du delar bara det offentliga korrektur-URL:en och mottagaren får skrivskyddad åtkomst till korrekturet.

     Mer information finns i [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

     Om du inte vill att den här länken ska visas i mottagarens e-post kan du inaktivera inställningarna för [!UICONTROL Public Sharing] i korrekturet

     (Hämta originalfil och offentlig URL). Mer information finns i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Aktivitetsloggen

Om du skickar ett [!UICONTROL New Proof]-e-postmeddelande till en granskare loggas det i [!UICONTROL Activity] -avsnittet på sidan [!UICONTROL Proof details]. Mer information finns i [Hantera[!UICONTROL  Proof Details] i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md). Du kan kontrollera om e-postmeddelandet [!UICONTROL New Proof] var aktiverat när ett korrektur skapades.

![New_Version_email__acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Om den som skapat eller äger korrekturet har [!UICONTROL Proof Made] e-postmeddelanden inaktiverade som standard (i sina personliga inställningar) får de inga [!UICONTROL Proof made]- eller [!UICONTROL New proof]-e-postmeddelanden, även om kryssrutan [!UICONTROL Notify people by email] är markerad på sidan Nytt korrektur. Mer information finns i .
>* Om e-postmeddelandena är inaktiverade som standard i [!UICONTROL Account settings] får inte författaren/ägaren av beviset några [!UICONTROL Proof made]- eller [!UICONTROL New proof]-e-postmeddelanden, även om detta är aktiverat i deras personliga inställningar, och kryssrutan [!UICONTROL Notify] personer via e-post är markerad på sidan Nytt korrektur. Mer information finns i [[!UICONTROL Proof Made] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) och i .
>



## Aktivera e-postmeddelandet [!UICONTROL New Proof] och inkludera ett anpassat meddelande

Du kan ange om du vill skicka en e-postavisering till granskarna om ett korrektur när du skapar det eller när du lägger till någon i det.

* [När du skapar ett korrektur](#when-you-create-a-proof)
* [När du lägger till en granskare i ett korrektur](#when-you-add-a-reviewer-to-a-proof)

### När du skapar ett korrektur {#when-you-create-a-proof}

När du skapar ett nytt korrektur på sidan [!UICONTROL New proof], under avsnittet **[!UICONTROL Share]**, kan du välja om du vill skicka e-postaviseringar:

* Här kan du bestämma om du vill [!UICONTROL Notify people by email] (1). Om du avmarkerar det här alternativet får ingen av dina granskare ett e-postmeddelande om att korrekturet är klart för granskning.
* Du kan även inkludera ett anpassat meddelande i e-postmeddelandet (2).
* Om du bestämmer dig för att lägga till ett eget anpassat meddelande kan du placera i en anpassad ämnesrad (3) och ett meddelande i e-postmeddelandets brödtext (4).
* Klicka på länken (5) om du vill ignorera det anpassade meddelandet.

  >[!NOTE]
  >
  >Om du alltid skickar samma anpassade meddelande till dina granskare kan det vara bra att spara det i dina personliga inställningar på fliken [!UICONTROL Proofing defaults]. Mer information finns i .

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### När du lägger till en granskare i ett korrektur {#when-you-add-a-reviewer-to-a-proof}

Du kan välja om en ny granskare som läggs till i ett befintligt korrektur ska meddelas om korrekturet (liknande ovan).

* Lägg först till nya granskare genom att klicka på knappen **[!UICONTROL Share this Version]** på sidan **[!UICONTROL Proof details]** (1).

![Korrektur_details_page_1.png](assets/proof-details-page-1-350x118.png)

* En ruta visas där du kan lägga till nya granskare. Du kan sedan bestämma om du vill att de ska meddelas via e-post (2) och välja att lägga till ett anpassat meddelande i e-postmeddelandet (3).

![Korrektur_details_page_2.png](assets/proof-details-page-2-350x174.png)

* Om du väljer att lägga till ett anpassat meddelande expanderar rutan och du kan lägga in en anpassad ämnesrad (4) och anpassad text i e-postmeddelandets brödtext (5). Du kan också ignorera det anpassade meddelandet genom att klicka på länken (6).

![Korrektur_details_page_3.png](assets/proof-details-page-3-350x258.png)

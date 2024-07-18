---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Hantera korrekturversioner i  [!DNL Workfront Proof]
description: Det kan vara en stor utmaning att hantera feedback i flera versioner eller revisioner av ett verk. [!DNL Workfront Proof] förenklar den här processen genom att du kan skapa och jämföra flera versioner av ett korrektur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# Hantera korrekturversioner i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Det kan vara en stor utmaning att hantera feedback i flera versioner eller revisioner av ett verk. [!DNL Workfront Proof] förenklar den här processen genom att du kan skapa och jämföra flera versioner av ett korrektur.

Det finns ingen gräns för hur många versioner av ett korrektur du kan skapa. Om du behöver gå igenom många revisioner med en klient för att få ett slutligt godkännande kan alla versioner som skapas visas och enkelt hanteras i [!DNL Workfront Proof].

Behörigheterna är specifika för en version, så du kan ge en person behörighet att se en version men inte en annan. Omvänt gäller att om du delar en senare version med en person kommer personen inte att kunna se tidigare versioner såvida du inte går tillbaka och uttryckligen lägger till dem även i de tidigare versionerna.

Om du vill skapa en ny version av ett korrektur måste du ha redigeringsbehörighet för korrekturet.

Se [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) om du vill ha mer information om vem som har redigeringsbehörighet för ett korrektur. Mer information om hur du skapar versioner finns i.

## Visa korrekturversioner i korrekturläsaren

Det fullständiga namnet på den version du visar visas längst upp till vänster i korrekturläsaren. Alla andra versioner av korrekturet visas endast som versionsnummer.

1. Öppna ett korrektur i korrekturläsaren enligt beskrivningen i [Öppna ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. Klicka i korrekturläsaren på versionsnumret till höger om korrekturnamnet.
1. Om du vill visa den andra versionen klickar du på dess namn på menyn som visas när du klickar på versionsnumret.
1. Klicka på ikonen **[!UICONTROL Compare proofs]** om du vill jämföra två versioner.\
   ![Jämför_korrektur_knapp.png](assets/compare-proofs-button.png)\
   Om det finns flera versioner av korrekturet kan du välja vilken två versioner du vill jämföra genom att klicka på det relevanta versionsnumret på varje sida av delskärmen i jämförelseläget.

Mer information om hur du granskar korrektur i ett korrekturläsare finns i [Granska ett korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Åtkomst till korrekturversioner via sidan Korrekturinformation

Du kommer åt alla versioner av ett korrektur via sidan Korrekturinformation.

1. Öppna sidan Korrekturinformation om du vill ha ett korrektur, vilket beskrivs i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Klicka på fliken för versionflikarna högst upp på sidan och klicka på **[!UICONTROL Go to proof]** för att öppna den version du vill ha i korrekturläsaren.\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Länkar korrekturversioner

Om korrekturet har flera versioner kallas den tidigare versionen av korrekturet för det överordnade korrekturet.

Om du vill ändra det överordnade korrekturet (föregående version) till ett annat korrektur i ditt konto, eller koppla ett enskilt korrektur till ett annat korrektur i ditt konto (som en ny version av det andra korrekturet), kan du göra det enkelt genom att följa de här stegen:

1. Öppna sidan Korrekturinformation om du vill ha ett korrektur, vilket beskrivs i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Change previous version]**.

1. I rutan **[!UICONTROL Change previous version]** som visas väljer du det korrektur som du vill ange som överordnat korrektur (tidigare version).\
   Om du behöver hjälp med att hitta korrekturet i listan kan du sortera kolumnerna genom att klicka på kolumnrubriken.

1. Klicka på **[!UICONTROL Change previous version]** längst ned i rutan för att ansluta versioner.

>[!NOTE]
>
>När du ansluter ett korrektur till ett annat korrektur i ditt konto (som en ny version), låser [!DNL Workfront Proof] korrekturet som nu är den föregående versionen.

## Bryta länkar till korrekturversioner

Du kan ta bort länken mellan det korrektur som du för närvarande visar från det överordnade korrekturet (tidigare version) utan att länka det till ett annat korrektur i ditt konto:

1. Öppna sidan Korrekturinformation om du vill ha ett korrektur, vilket beskrivs i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Remove link to previous version]**.

   * Det är bara den senaste versionen som kan kopplas från (kopplas från) från hela versionsuppsättningen. Sedan blir det ett enda bevis.
   * Om du behöver infoga en version mellan två befintliga versioner kan du bryta länken mellan alla versioner av samma korrektur och länka om dem i rätt ordning.

## Om Versionsuppsättningar och korrekturgränser

Varje uppsättning om fem versioner räknas som ett korrektur i förhållande till den totala korrekturgränsen.

Om du till exempel överför fem versioner av en design (inklusive originalversionen) räknas det som ett korrektur. Om du överför sex versioner av en design räknas det som två korrektur. Elva versioner räknas som tre korrektur och så vidare.

För visuella ljudfiler räknas varje ny version som ett nytt korrektur.

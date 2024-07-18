---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: Frågor och svar - Skapa och dela korrektur och filer
description: Ett korrektur är en statisk fil, ljudfil eller videofil som är tillgänglig för granskning i korrekturläsaren. Granskare som läggs till i ett korrektur har en uppsättning verktyg tillgängliga för dem för att göra kommentarer och beslut om korrekturet.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 0%

---

# Frågor och svar - Skapa och dela korrektur och filer

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

## Vad är ett bevis?

### Svar

Ett korrektur är en statisk fil, ljudfil eller videofil som är tillgänglig för granskning i korrekturläsaren. Granskare som läggs till i ett korrektur har en uppsättning verktyg tillgängliga för dem för att göra kommentarer och beslut om korrekturet.

## Vilka filtyper stöds?

### Svar

Du kan skapa korrektur från statiska filer, ljud- och videofiler. Du kan inte överföra filer som är större än 4 GB. [!DNL Workfront] har stöd för över 150 filtyper (se [Översikt över filtyper och storleksbegränsningar som stöds](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) för en fullständig lista).

## Vad är skillnaden mellan ett korrektur och en fil?

### Svar

När du överför en fil till [!DNL Workfront Proof] lagrar systemet filen på ditt [!DNL Workfront Proof]-konto. När du delar den skickar [!DNL Workfront Proof] ett e-postmeddelande till mottagarna med en länk som de kan klicka på för att hämta filen. Du kan dela vilken filtyp du vill.

När du skapar ett korrektur från en fil som du har överfört till [!DNL Workfront Proof] kan du göra filen tillgänglig för granskning i korrekturläsaren. Granskarna får ett mejl med en länk till korrekturet. När de öppnar korrekturet ser de korrekturbilden och kan lägga till kommentarer och fatta beslut i den. Du kan skapa korrektur med hjälp av filer i listan över filtyper som stöds. Du kan också skapa korrektur med URL:er för webbplatser och annat webbinnehåll.

En fullständig lista över de filtyper som stöds finns i [Översikt över filtyper och storleksbegränsningar som stöds](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Hur skapar jag ett bevis?

### Svar

Du kan skapa korrektur av statiska filer, ljudfiler, videofiler och URL:er (se ).

Om du vill skapa ett korrektur i kontot måste du vara en användare med rätt behörighetsprofil (se [[!UICONTROL Proof Permissions Profiles] i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Om du överför flera filer samtidigt kan du skapa flera korrektur som du kan skicka till samma grupp med granskare via ett och samma e-postmeddelande. Om din organisation har ett [!UICONTROL Enterprise]- eller [!UICONTROL Unlimited]-konto kan du kombinera filer till ett enda korrektur (se [Skapa ett flersidigt korrektur](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## Vad är korrekturroller och e-postaviseringar?

### Svar

Korrekturroller definierar vilka åtgärder en granskare behöver utföra på ett korrektur. Det finns olika rollalternativ som du kan använda för granskare när du skapar ett korrektur, beroende på om du vill att de ska kunna göra kommentarer, fatta beslut och så vidare. Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

E-postaviseringar uppdaterar granskarna om korrekturens förlopp (de skiljer sig från nya korrektur- och korrekturmeddelanden). Du kan välja olika alternativ för olika granskare, beroende på vilken roll respektive granskare har på korrekturet. Mer information finns i [Skapa ett avancerat korrektur med en [!UICONTROL Automated workflow]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Kan jag skapa ett korrektur av flera filer?

### Svar

Att kombinera flera filer till ett enda korrektur är en funktion som är tillgänglig i [!UICONTROL Enterprise]- och [!UICONTROL Unlimited]-versionsplanerna. Det här alternativet är bara möjligt för statiska filer, inte för videofiler. Mer information finns i [Skapa ett flersidigt korrektur](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Kan jag skapa korrektur från URL:er?

### Svar

Ja, du kan skapa korrektur av webbplatser och annat webbinnehåll. När du lägger till en URL för att skapa ett korrektur kan du ange om du vill ha ett statiskt korrektur eller ett interaktivt korrektur:

* I ett interaktivt korrektur kan granskarna navigera och interagera som vanligt med webbplatsen eller annat webbinnehåll som annonser med direktuppspelad video eller ljud, [!DNL Flash] element i en annons, HTML-animeringar och interaktiva banners. Mer information finns i [Skapa ett korrektur för interaktivt innehåll i en ZIP-fil](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).
* För ett statiskt korrektur tar [!DNL Workfront] en uppsättning skärmbilder av de sidor och undersidor som du anger. Hyperlänkar finns direkt i korrekturet, så du kan testa om de leder till rätt mål eller inte. Mer information finns i [Skapa ett statiskt korrektur för en webbplats eller annat webbinnehåll](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Du kan lägga till flera URL-adresser samtidigt om du separerar dem med ett mellanslag. Observera att kombinationen bara är tillgänglig för [!UICONTROL Enterprise]- och [!UICONTROL Unlimited]-versionsplanerna.

## Kan personer som inte har någon inloggning skapa korrektur i mitt konto?

### Svar

Du behöver inloggningsuppgifter för att skapa korrektur direkt i ett [!DNL Workfront Proof]-konto.

## Vad innebär att dela ett bevis?

### Svar

Genom att dela ett korrektur får granskarna tillgång till det så att de kan lägga till kommentarer och markeringar och fatta beslut i det. Gästgranskarna får åtkomst till korrektur från e-postmeddelanden de får. Granskare med ett eget [!DNL Workfront Proof]-konto har åtkomst till korrektur på [!UICONTROL Dashboard].

## Hur delar jag ett bevis?

### Svar

När du skapar ett korrektur kan du lägga till granskare i avsnittet [!UICONTROL Workflow] på sidan [!UICONTROL New Proof]. När korrekturet är klart skickar [!DNL Workfront Proof] ett e-postmeddelande till granskarna med en länk till korrekturet.

Om du har tillräcklig behörighet för ett korrektur kan du använda korrekturläsaren, [!UICONTROL Dashboard] eller någon av listvyerna för att lägga till granskare i ett befintligt korrektur (se [Dela ett korrektur på  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] sidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)).

Att lägga till granskare är det vanligaste sättet att dela korrektur. Om du vill utforska andra tillgängliga alternativ kan du läsa:

* [Dela korrekturlänkar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Dela den offentliga URL:en i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Prenumerera på ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Skapa ett minikorrektur i  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## Måste du vara användare för att granska ett bevis?

### Svar

Nej. Gästgranskare (personer utan inloggningsuppgifter för [!DNL Workfront Proof]) kan få åtkomst till ett korrektur från det e-postmeddelande som de får. Du kan dela ett bevis med så många gäster du vill.

Det går att begränsa delning av korrektur till personer med inloggningsuppgifter för [!DNL Workfront Proof]. Då läggs ytterligare ett säkerhetsskikt till i korrekturet. För förbättrad säkerhet kan systemadministratörer för organisationer med [!UICONTROL Enterprise]- och [!UICONTROL Unlimited]-planer konfigurera det här kravet för alla korrektur som skapats i organisationen.

Mer information om inloggningskrav finns i [Korrekturskydd i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Om din organisation kräver att granskare signerar korrektur elektroniskt, vilket kräver inloggning på [!DNL Workfront Proof], kan användare bara dela korrektur med registrerade användare. Det här är tillgängligt för [!UICONTROL Enterprise]- och [!UICONTROL Unlimited]-versionsplanerna. Mer information finns i [Förstå elektroniska signaturer i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Kan jag sätta en deadline för mina granskare?

### Svar

Du kan ange en deadline för ett nytt korrektur eller en ny korrekturversion när du skapar korrekturet. Det gör du i avsnittet [!UICONTROL Workflow] på sidan [!UICONTROL New Proof]. Om du använder [!UICONTROL Automated Workflow] kan du ange olika tidsgränser för varje fas i granskningen.

Du kan också ange eller uppdatera en deadline för ett befintligt korrektur med sidan [!UICONTROL Proof Details]. Mer information finns i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Hur skapar jag en ny version av mitt bevis?

### Svar

Granskarna begär ofta ändringar i sina kommentarer på ett korrektur och vill se en ny version av korrekturet. Du kan skapa nya versioner av ett korrektur. [!DNL Workfront Proof] kommer ihåg korrekturinställningarna från den tidigare versionen. Du kan fortfarande redigera de här inställningarna om du behöver göra något som att lägga till eller ta bort granskare för korrekturet.

Du måste dela varje version med de specifika granskare som behöver visa den. Om du t.ex. bara delar version 3 med en granskare kan den personen inte se version 1 och 2. Tillsynsmyndigheter och administratörer på ditt konto övervakar alla projekt på kontot så att de kan se och redigera alla versioner av korrekturet.

Mer information finns i .

## Kan jag dela filer med [!DNL Workfront Proof]?

### Svar

Ja. Om du vill dela något med andra personer, men du inte behöver dem för att visa det som ett korrektur (eller om det är en filtyp som inte stöds av [!DNL Workfront Proof]), kan du överföra den som en fil till ditt [!DNL Workfront Proof]-konto. Precis som med korrektur kan du ordna dina filer i mappar, tagga filer och lägga till ett eget meddelande i e-postmeddelandet när du delar filen. Mer information finns i [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

När mottagarna får ett e-postmeddelande om en fil som du delar kan de hämta filen genom att klicka på länken i meddelandet.

[!DNL Workfront Proof] användare kan konvertera filer till korrektur när de har sparat dem i sitt konto.

<!--Is there a limit-->

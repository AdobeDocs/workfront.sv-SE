---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: Frågor och svar - Granska korrektur
description: Gästgranskare som inte har egna inloggningar på Korrektur får åtkomst till sina korrektur via [!UICONTROL Go to proof] i de e-postmeddelanden de får. Användarna kan få åtkomst till sina korrektur via e-post och kan även dra nytta av att använda sin kontrollpanel i kontot. I kontrollpanelsvyn kan de ta en titt på en lista med korrektur som kräver deras beslut och komma åt dem med ett klick genom att klicka på den blå [!UICONTROL Go to proof] ikon.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d8bcddf8-0586-4263-8445-26615fdf07f7
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Frågor och svar - Granska korrektur

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

## Hur får jag åtkomst till ett intyg som delats med mig

Gästgranskare som inte har egna inloggningar på [!DNL ProofHQ], kan du få tillgång till deras korrektur med *[!UICONTROL Go to proof]* i de e-postmeddelanden de får. Användarna kan få åtkomst till sina korrektur via e-post och kan även dra nytta av att använda sin kontrollpanel i kontot. I kontrollpanelsvyn kan de ta en titt på en lista med korrektur som kräver deras beslut och komma åt dem med ett klick genom att klicka på den blå *[!UICONTROL Go to proof]* ikon.

## Hur lägger jag in kommentarer i ett korrektur?

Om du vill lägga till en kommentar i ett korrektur klickar du på *[!UICONTROL Add a comment]* som finns längst upp på sidan. Om du inte kan se den knappen kontaktar du ägaren av beviset. Det är möjligt att du har tilldelats fel korrekturroll (mer information om korrekturroller finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

A [!UICONTROL comment] öppnas till höger på skärmen. Här kan du skriva din kommentar och spara den på korrekturet. Detta lämnar en allmän kommentar på korrekturet som inte hör till något visst område i korrekturet. Om du vill kommentera något specifikt använder du markeringsverktygen som finns längst upp på sidan.

Om du vill svara på någons kommentar på korrekturet klickar du på kommentaren i kommentarlistan och skriver in svaret i dialogrutan [!UICONTROL reply] box. När du sparar bokförs svaret på korrekturet.

Alla kommentarer och beslut visas på korrekturet nästan direkt, så om någon annan tittar på beviset samtidigt som du ser dem ser de dina kommentarer direkt.

Det här är mycket grundläggande instruktioner som hjälper dig att komma igång med [!DNL ProofHQ]. Om du vill veta mer om korrektur kan du gå till  [Granska korrektur](https://support.workfront.com/hc/en-us/sections/200054044-Reviewing-proofs) i hjälpcentret för mer detaljerade hjälpartiklar.

## Hur kommenterar jag upp ett bevis?

[!DNL ProofHQ] innehåller en uppsättning ritverktyg som hjälper dig att ge korrektur precis feedback. Du kan välja färg och opacitet för varje markering som du lämnar i korrekturet, och för linjeverktyg kan du även ändra linjens tjocklek.

Om du vill visa de tillgängliga verktygen klickar du på [!UICONTROL Add a comment] överst på sidan. Ritverktygen i verktygsfältet är:

* rektangel
* frihandslinje
* rät linje
* anslutna linjer
* pil
* markera
* maskform

Om du vill rita väljer du bara det verktyg du vill använda, markeringens färg och linjens tjocklek (för linjeverktyg). Du kan bifoga flera markeringar till en kommentar. När du sparar kommentaren tas ett häftstift med numret på kommentaren bort mitt i gruppen med markeringar. Med punkter kan du snabbt visa markeringar som finns kvar i korrekturet. Om du klickar på det visas markeringen och kommentaren som är kopplad till markeringen.

## Vilka verktyg kan jag använda för att markera text i ett korrektur?

Textanteckningsverktyget som finns i [!UICONTROL Proof Viewer] kan du snabbt markera text i korrekturet. Du öppnar den genom att klicka på *[!UICONTROL Add a comment]* överst på sidan. Anteckningsverktyget är den första ikonen till vänster i verktygsfältet. Du kan markera text i korrekturet. Du kan välja mellan fyra alternativ:

* markera - markerar texten och kopierar den till kommentarsrutan
* replace - kopierar texten och lägger till [[!UICONTROL REPLACE]] och [[!UICONTROL WITH]] i kommentarsrutan, så att du enkelt kan föreslå ersättningstext
* delete - stryker över texten och lägger till [[!UICONTROL DELETE]] till kommentarsrutan
* infoga efter - gör att du enkelt kan föreslå text som behöver infogas efter den markerade frasen

Om texten du vill använda sparas i ett separat dokument kan du använda kortkommandona (Ctrl+C och Ctrl+V på en dator, cmd+c och cmd+v på en [!DNL Mac]) för att kopiera och klistra in den i [!UICONTROL comment] box.

## Vad innebär det att fatta ett beslut om ett bevis?

Att fatta ett beslut om ett bevis kan ha två betydelser i [!DNL ProofHQ]. Å ena sidan kan det vara ett formellt godkännande när någon måste skriva på ett bevis. Ett annat tillvägagångssätt är att fatta ett beslut om att meddela andra granskare att du är klar med att kommentera korrekturet.

Standardalternativ för beslut finns i [!DNL ProofHQ] är *Godkänd*, *Godkänd med ändringar*, *Ändringar krävs* och *Ej relevant*. Administratörer i [!UICONTROL Enterprise] och [!UICONTROL Unlimited] kan anpassa dessa alternativ (ändra namn på dem eller dölja dem). Mer information finns på [Konfigurera alternativ för godkännandebeslut i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Måste alla fatta beslut om bevis?

Nej, det beror på vilken korrekturroll varje granskare har tilldelats i ett korrektur (mer information om korrekturroller finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)). *[!UICONTROL Approver]*, *[!UICONTROL Reviewer and Approver]*, *[!UICONTROL Moderator]* och *[!UICONTROL Author]* är roller som kräver ett beslut om beviset.

Vanligtvis behöver den person som skapar beviset inte fatta något beslut, men det beror på arbetsflödet i organisationen. Om en granskare inte behöver fatta ett beslut om ett bevis måste du se till att deras roll är inställd på granskare, annars väntar systemet på att de ska fatta sitt beslut innan korrekturens övergripande status uppdateras.

Om du skickar ett bevis till en grupp granskare, men bara behöver en person för att signera och det inte spelar någon roll vem som fattar beslutet, kan du aktivera [!UICONTROL Only one decision required]. Den totala bevisutvecklingen kommer att uppdateras efter det att det första beslutet om beviset har fattats, oavsett vem som fattar beslutet.

## Kan jag generera en lista med alla kommentarer som gjorts på ett bevis?

Ja, du kan generera en *[!UICONTROL Print summary]* av de kommentarer som finns kvar på korrekturet. Det här dokumentet kan genereras för en enstaka version eller för alla versioner som delats med den här granskaren. Här visas en lista med alla kommentarer, markeringar och beslut som har fattats på beviset. Mer information om den här funktionen finns på [Skriv ut och exportera kommentarer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

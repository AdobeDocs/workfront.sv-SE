---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Dela mappar i  [!DNL Workfront Proof]
description: Du kan dela en mapp med användare och hela företag som har  [!DNL Workfront Proof] konton (inte med gäster).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 57f846a1-f315-42c1-911a-cfbc8b4879ba
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Dela mappar i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan dela en mapp med användare och hela företag som har [!DNL Workfront Proof] konton (inte med gäster).

Om du delar en hel mapp:

* Du kan inte ange roller för de personer som du delar mappen med (roller och e-postaviseringar gäller bara för mottagare när du delar enskilda korrektur).
* Mottagarna har skrivskyddad åtkomst till alla objekt i mappen (befintliga och senare tillagda objekt).
* Mottagarna får ett e-postmeddelande med en personlig URL till mappen.
* Mottagarna får inga e-postmeddelanden när nya objekt läggs till i mappen.
* Mottagarna kan hämta originalfilerna för objekten i mappen (observera att varje korrektur måste ha alternativet [!UICONTROL Download original file] aktiverat för att mottagaren ska kunna hämta originalfilen).
* Ägare och skapare av mappar kan alltid visa mappen och kan inte tas bort från mappen.
* Om du delar en privat mapp med en Manager-användare på ditt konto kan du bestämma om du vill att de ska ha redigeringsbehörighet för mappen.

Du kan också dela objekt i en mapp (i stället för själva mappen). Mer information finns i [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) och [Dela filer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-files.md).

## Dela en enskild mapp

1. Klicka på fliken **[!UICONTROL Folders]** i den vänstra navigeringssidlisten.
1. Håll pekaren över en enskild mapp som du vill dela och klicka sedan på knappen **[!UICONTROL More]** som visas till höger om mappen.
1. Klicka på **[!UICONTROL Share folder]**.
1. Gör något av följande på sidan som visas:

   * Lägg till användare i mappen genom att skriva in deras e-postadress (1).
   * Om du delar en privat mapp med en hanterare kan du bestämma om du vill att de ska kunna skapa, redigera och ta bort mappobjekt genom att klicka på ett alternativ under **[!UICONTROL Allow on folder]**.
   * Om du ändrar dig kan du ta bort en användare genom att hålla markören över personens e-postadress och klicka på **[!UICONTROL Remove person]** (papperskorgsikonen längst till höger). Du kan ta bort alla personer som du just har lagt till genom att hålla markören över namnen och sedan klicka på **[!UICONTROL Remove all people]** (den övre papperskorgsikonen).

1. När du är klar klickar du på **[!UICONTROL Share folder]**.

1. Om du delar mappen med en grupp eller partner visas alla kontakter i den gruppen eller partnerorganisationen i delningsavsnittet på sidan.

## Dela flera mappar

1. Klicka på fliken **[!UICONTROL Folders]** i den vänstra navigeringssidlisten.
1. Klicka på namnet på mappen som innehåller de mappar som du vill dela.
1. I listan med mappar till höger klickar du på kryssrutan till vänster om varje mapp som du vill dela.\
   eller\
   Markera kryssrutan ovanför listan med mappar om du vill markera alla mappar i listan.

1. Klicka på **[!UICONTROL Share selected items]**.\
   ![Share_button-small.png](assets/share-button-small.png)

1. Gör något av följande på sidan som visas:

   * Lägg till användare i mappen genom att skriva in deras e-postadress.
   * Om du delar en privat mapp med en hanterare kan du bestämma om du vill att de ska kunna skapa, redigera och ta bort mappobjekt genom att klicka på ett alternativ under **[!UICONTROL Allow on folder]**.
   * Om du ändrar dig kan du ta bort en användare genom att hålla markören över personens e-postadress och klicka på **[!UICONTROL Remove person]** (papperskorgsikonen längst till höger). Du kan ta bort alla personer som du just har lagt till genom att hålla markören över namnen och sedan klicka på **[!UICONTROL Remove all people]** (den övre papperskorgsikonen).

1. När du är klar klickar du på **[!UICONTROL Share folder]**.

## Åtkomst till en mapp som har delats med dig

När någon delar en mapp med dig visas den i sidofältet för sitt [!DNL Workfront Proof]-konto under namnet på mappens ägare. Du får ett e-postmeddelande med mappinformation och en personlig länk till mappen.

1. Klicka på länken i det e-postmeddelande du får.
1. Logga in på [!DNL Workfront Proof].\
     [!DNL  Workfront Proof] visar sidan Mappinformation. Mer information finns i [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

## Om delning av undermappar

Om en överordnad mapp som innehåller undermappar delas och sedan en undermapp flyttas från under den överordnade mappen (till exempel till översta nivån), behålls inte den ursprungliga resursen i undermappen. Detta beror på att själva undermappen inte delades explicit, eftersom den överordnade mappen inte delades. Om du i det här fallet vill att undermappen ska delas med de ursprungliga mottagarna bör du dela undermappen igen med dessa mottagare.

Om en privat överordnad mapp delas med en hanterare och redigeringsbehörighet för mappen ges till den här användaren, ärvs den här inställningen av alla undermappar i den privata mappen.

## Om undermappar som delas med dig

När en undermapp har delats med någon visas den i sidofältet för ditt [!DNL Workfront Proof]-konto under namnet på mappens ägare.

Om den överordnade mappen, eller objekt från den, redan har delats med samma person, visas undermappen automatiskt under den överordnade mappen i sidofältet och på den överordnade mappens informationssida.

## Om att dela en mapp med ett företag

Om du vill dela en mapp med en partnerorganisation måste det finnas en befintlig partnerrelation mellan ditt konto och deras.

Att dela en mapp med en partner innebär:

* Alla användare i den organisationen har skrivskyddad åtkomst till mappen (och mappobjekten).
* Alla nya användare som läggs till i organisationen får automatiskt skrivskyddad åtkomst till mappen (och alla objekt i mappen).

Mer information finns i [Dela objekt med en partner i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/share-items-partner-in-wp.md).

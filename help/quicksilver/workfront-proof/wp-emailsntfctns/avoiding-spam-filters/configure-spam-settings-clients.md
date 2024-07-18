---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Konfigurera skräppostinställningar för vanliga e-postklienter
description: Du kan konfigurera din e-postklient så att  [!DNL Workfront Proof] e-postmeddelanden inte skickas till skräppostmappen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 41517540-c5a8-4bf5-997b-e7a605337e73
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# Konfigurera skräppostinställningar för vanliga e-postklienter

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan konfigurera din e-postklient så att [!DNL Workfront Proof] e-postmeddelanden inte skickas till skräppostmappen.

I följande avsnitt beskrivs den här processen för olika e-postklienter:

## [!DNL Gmail]

I det här avsnittet:

* Lägg till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i [!UICONTROL Contacts]-listan i [!DNL Gmail] eller skapa filter för att förhindra att [!UICONTROL Gmail] dirigerar e-postmeddelanden från adresserna till din [!UICONTROL Spam]-mapp
* Ta bort befintliga [!DNL Workfront Proof]-e-postmeddelanden från mappen [!UICONTROL Spam] och ändra eventuella filter som dirigerar [!DNL Workfront Proof]-meddelanden till papperskorgen

### För nya [!DNL Workfront Proof] e-postmeddelanden

Lägg antingen till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i [!UICONTROL Contacts]-listan i [!DNL Gmail] eller skapa e-postfilter för att hindra att [!DNL Workfront Proof] e-postmeddelanden dirigeras till din [!UICONTROL Spam]-mapp av [!DNL Gmail]. Så här lägger du till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i [!UICONTROL Contacts]-listan:

1. Klicka på **[!UICONTROL Contacts]** nedanför **[!UICONTROL Mail]** i det övre vänstra hörnet på en Gmail-sida.

1. Du kan behöva klicka på ett plustecken (+) efter [!UICONTROL Mail] för att visa [!UICONTROL Contacts] och [!UICONTROL Tasks]. Om plustecknet inte visas flyttar du markören till [!UICONTROL Mail] så visas plustecknet.
1. Klicka på knappen **[!UICONTROL Add to "My Contacts"]** ovanför din lista över kontakter och deras e-postadresser.
1. Kopiera och klistra in den första [!UICONTROL from]-adressen i den omärkta e-postadressdialogrutan.
1. Klicka på **[!UICONTROL Add]** nedanför dialogrutan. Adressen läggs till i din lista över kontakter.
1. Upprepa steg 2-4 för den andra [!UICONTROL from]-adressen.

Du kan också skapa ett e-postfilter för var och en av de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna:

1. Klicka på **[!UICONTROL Create a filter]** bredvid knapparna **[!UICONTROL Search]** högst upp på en Gmail-sida.

1. Kopiera och klistra in den första [!UICONTROL from]-adressen i fältet **[!UICONTROL From]** i rutan **[!UICONTROL Create a Filter]**.

1. Klicka på knappen **[!UICONTROL Next Step]**.
1. Välj **[!UICONTROL Never send it to Spam]** i listan **[!UICONTROL Choose action]**.

1. Klicka på knappen **[!UICONTROL Create Filter]**. Filtret läggs till i din lista med filter på sidan [!UICONTROL Settings].
1. För den andra [!UICONTROL from]-adressen klickar du på **[!UICONTROL Create a filter]** längst ned på inställningssidan och upprepar steg 2-5.

### För befintliga [!DNL Workfront Proof]-e-postmeddelanden

Så här tar du bort alla [!DNL Workfront Proof] e-postmeddelanden som [!DNL Gmail] har placerat i mappen [!UICONTROL Spam] sedan den senast rensades:

1. Klicka på **[!UICONTROL Spam]** i mapplistan till vänster på en Gmail-sida.
1. Välj eventuella [!DNL Workfront Proof]-e-postmeddelanden i mappen [!UICONTROL Spam].
1. Klicka på knappen **[!UICONTROL Not Spam]** ovanför listan [!UICONTROL Spam].\
   Du hittar nu de [!DNL Workfront Proof] e-postmeddelandena i din inkorg.

Så här ändrar du eventuella filter som skickar [!DNL Workfront Proof] e-postmeddelanden till papperskorgen:

1. Klicka på **[!UICONTROL Create a filter]** bredvid knapparna [!UICONTROL Search] högst upp på en Gmail-sida.
1. Klicka på **[!UICONTROL Show current filters]** längst ned i dialogrutan [!UICONTROL Create a filter]. De befintliga filtren visas på sidan Inställningar efter fält (från) och namn eller adress.
1. Om filtret [!UICONTROL Do this action for an existing [!DNL Workfront Proof] address] är [!UICONTROL Delete it] klickar du på **[!UICONTROL edit]**.
1. Klicka på knappen **[!UICONTROL Next Step]**.
1. Avmarkera alternativet **[!UICONTROL Delete it]** och markera **[!UICONTROL Never send it to Spam]**.

1. Klicka på knappen **[!UICONTROL Update Filter]**.\
   Sidan [!UICONTROL Settings] visas igen.

1. Om det finns ytterligare [!DNL Workfront Proof] adressfilter i listan upprepar du steg 3-6 för vart och ett av dem.

## [!DNL Microsoft Outlook] 2003 - 2007

I det här avsnittet:

* Lägg till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i listan [!UICONTROL Safe Senders] i [!DNL Outlook]
* Ta bort befintliga [!DNL Workfront Proof]-e-postmeddelanden från mappen [!UICONTROL Junk E-mail] och eventuella [!UICONTROL from]-adresser från listan [!UICONTROL Blocked Senders]

### För nya [!DNL Workfront Proof] e-postmeddelanden

Så här lägger du till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i listan Betrodda avsändare i Outlook:

1. Klicka på **[!UICONTROL Options]** på menyn **[!UICONTROL Tools]**.

1. Klicka på **[!UICONTROL Junk E-mail]** under **[!UICONTROL E-mail]** på fliken **[!UICONTROL Preferences]**.

1. Klicka på **[!UICONTROL Add]** på fliken **[!UICONTROL Safe Senders]**.

1. Kopiera och klistra in den första [!UICONTROL from]-adressen eller bara domännamnet (resten av namnet efter @-tecknet) i rutan **[!UICONTROL Add Address or domain]**.
1. Klicka på **[!UICONTROL OK]**. Adressen läggs till i listan.
1. Upprepa steg 3-5 för den andra [!UICONTROL from]-adressen.

### För befintliga [!DNL Workfront Proof]-e-postmeddelanden

Så här tar du bort alla [!DNL Workfront Proof] e-postmeddelanden som [!DNL Outlook] har placerat i mappen [!UICONTROL Junk E-mail] sedan den senast rensades:

1. Klicka på mappen **[!UICONTROL Junk E-mail]** i navigeringsfönstret.
1. Om det finns [!DNL Workfront Proof] e-postmeddelanden i mappen högerklickar du på varje e-post, väljer [!UICONTROL Junk E-mail] och klickar sedan på **[!UICONTROL Mark as Not Junk]**.
1. Du hittar nu de [!DNL Workfront Proof] e-postmeddelandena i din inkorg.

Så här kontrollerar du om det finns några [!DNL Workfront Proof] [!UICONTROL from]-adresser i listan Spärrade avsändare:

1. Klicka på **[!UICONTROL Options]** på menyn **[!UICONTROL Tools]**

1. Klicka på **[!UICONTROL Junk E-mail]** under **[!UICONTROL E-mail]** på fliken **[!UICONTROL Preferences]**.

1. Klicka på fliken **[!UICONTROL Blocked Senders]**.
1. Om det finns några [!DNL Workfront Proof]-adresser i listan klickar du på var och en av dem och sedan på **[!UICONTROL Remove]**.

## [!DNL Windows Live Hotmail]

I det här avsnittet:

* Lägg till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i listan [!UICONTROL Safe Senders] i [!DNL Windows Live Hotmail]
* Ta bort befintliga [!DNL Workfront Proof]-e-postmeddelanden från mappen Skräppost och eventuella [!UICONTROL from]-adresser från listan [!UICONTROL Blocked Senders]

### För nya [!DNL Workfront Proof] e-postmeddelanden

Så här lägger du till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i [!UICONTROL Safe Senders]-listan i [!DNL Windows Live Hotmail]:

1. Klicka på **[!UICONTROL Options]** i det övre högra hörnet på din postlådesida.
1. Klicka på **[!UICONTROL More options]**.
1. Klicka på **[!UICONTROL Safe and blocked senders]** under **[!UICONTROL Junk e-mail]**.

1. Klicka på **[!UICONTROL Safe Senders]**.
1. Kopiera och klistra in den första [!UICONTROL from]-adressen eller bara domännamnet (resten av namnet efter @-tecknet) i [!UICONTROL Sender] eller domänen för att markera som säkert fält.
1. Klicka på knappen **[!UICONTROL Add to list]**. Adressen visas i listan.
1. Upprepa steg 4-6 för den andra [!UICONTROL from]-adressen.

### För befintliga [!DNL Workfront Proof]-e-postmeddelanden

Så här tar du bort alla [!DNL Workfront Proof] e-postmeddelanden som [!DNL Windows Live Hotmail] har placerat i din [!UICONTROL Junk]-e-postmapp sedan den senast rensades:

1. Klicka **[!UICONTROL Junk]** under **[!UICONTROL Folders]** till vänster på sidan.

1. Om det finns [!DNL Workfront Proof] e-postmeddelanden i den här mappen öppnar du varje e-postmeddelande och klickar på länken **[!UICONTROL Not junk]**.
1. Du hittar nu de [!DNL Workfront Proof] e-postmeddelandena i din inkorg.

Så här kontrollerar du om det finns några [!DNL Workfront Proof] [!UICONTROL from]-adresser i listan [!UICONTROL Blocked Senders]:

1. Klicka på **[!UICONTROL Options]** i det övre högra hörnet på din postlådesida.
1. Klicka på **[!UICONTROL More options]**.
1. Klicka på **[!UICONTROL Safe and blocked senders]** under **[!UICONTROL Junk e-mail]**.

1. Klicka på **[!UICONTROL Blocked Senders]**.
1. Om det finns [!DNL Workfront Proof] adresser i listan markerar du var och en av dem och klickar på knappen **[!UICONTROL Remove from list]** .

## [!DNL Yahoo Mail]

I det här avsnittet:

* Lägg till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna till filter så att [!DNL Yahoo Mail] skickar [!DNL Workfront Proof] e-post till din inkorg
* Ta bort befintliga [!DNL Workfront Proof]-e-postmeddelanden från mappen [!UICONTROL Spam]

### För nya [!DNL Workfront Proof] e-postmeddelanden

Så här skapar du ett nytt filter i [!DNL Yahoo Mail] för varje [!DNL Workfront Proof] [!UICONTROL from]-adress:

1. Klicka på **[!UICONTROL Options]** i det övre högra hörnet på e-postsidan.
1. Klicka på **[!UICONTROL More options]**.
1. Klicka på **[!UICONTROL Filters]** till vänster på sidan.
1. Klicka på **[!UICONTROL Create or edit filters]**.
1. Klicka på **[!UICONTROL Add]** på sidan Filter.
1. Ge filtret ett namn.
1. För regeln [!UICONTROL From header] väljer du alternativet **[!UICONTROL contains]** och kopierar och klistrar in den första [!UICONTROL from]-adressen eller bara domännamnet (resten av namnet efter @-tecknet).
1. Klicka på **[!UICONTROL Choose Folder]** och välj **[!UICONTROL Inbox]**.

1. Klicka på knappen *[!UICONTROL *Add Filter]**. Filtret visas i filterlistan.
1. Upprepa steg 5-9 för den andra [!UICONTROL from]-adressen.

### För befintliga [!DNL Workfront Proof]-e-postmeddelanden

Så här tar du bort alla [!DNL Workfront Proof] e-postmeddelanden som [!DNL Yahoo Mail] har dirigerat till din [!UICONTROL Spam]-mapp sedan den senast rensades:

1. Välj mappen **[!UICONTROL Spam]** till vänster på sidan [!UICONTROL Mail].
1. Om det finns [!DNL Workfront Proof] e-postmeddelanden i mappen markerar du varje e-postmeddelande och klickar på knappen **[!UICONTROL Not Spam]**.
1. Du hittar nu dessa e-postmeddelanden i din inkorg.

Så här tar du bort [!DNL Workfront Proof] [!UICONTROL from]-adresser från listan över blockerade adresser:

1. Klicka på **[!UICONTROL Options]** i det övre högra hörnet på e-postsidan.
1. Klicka på **[!UICONTROL More options]**.
1. Klicka på **[!UICONTROL Spam]** till vänster på sidan.
1. Om några [!DNL Workfront Proof]-adresser eller domännamn visas i avsnittet **[!UICONTROL Blocked Email Addresses]** på skräppostsidan, markerar du varje post och klickar på knappen **[!UICONTROL Remove]** .

## [!DNL Aol]

I det här avsnittet:

* Lägg till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i din [!DNL Aol] [!UICONTROL Address Book]
* Ta bort befintliga [!DNL Workfront Proof]-e-postmeddelanden från mappen [!DNL Aol] [!UICONTROL Spam] och eventuella [!DNL Workfront Proof] [!UICONTROL from]-adresser från listan över blockerade adresser i filtret [!DNL Aol] [!UICONTROL Spam]

### För nya [!DNL Workfront Proof] e-postmeddelanden

Så här lägger du till de två [!DNL Workfront Proof] [!UICONTROL from]-adresserna i din [!DNL Aol] [!UICONTROL Address Book]:

1. Klicka på menyn **[!UICONTROL Mail]**.
1. Välj **[!UICONTROL Address Book]**.
1. Klicka på knappen [!UICONTROL Add] längst ned i fönstret [!UICONTROL Address Book].
1. I fönstret **[!UICONTROL Address Card for New Contact]** kopierar och klistrar du in den första [!UICONTROL from]-adressen i fältet [!UICONTROL Other E-Mail] och kontrollerar alternativknappen [!UICONTROL Primary E-Mail] bredvid fältet.
1. Klicka på **[!UICONTROL Save]**.
1. Upprepa steg 3-5 för den andra [!UICONTROL from]-adressen.

### För befintliga [!DNL Workfront Proof]-e-postmeddelanden

Så här tar du bort alla [!DNL Workfront Proof] e-postmeddelanden som [!DNL Aol] har dirigerat till din [!UICONTROL Spam]-mapp sedan den senast rensades:

1. Klicka på menyn [!UICONTROL Mail].
1. Välj mappen **[!UICONTROL Spam]**.
1. Om det finns [!DNL Workfront Proof] e-postmeddelanden i mappen öppnar du varje e-postmeddelande i taget och klickar på knappen **[!UICONTROL This Is Not Spam]** .
1. Du hittar nu de [!DNL Workfront Proof] e-postmeddelandena i din inkorg.

Så här kontrollerar du om några [!DNL Workfront Proof] [!UICONTROL from]-adresser är blockerade i filtret [!DNL Aol] [!UICONTROL Spam]:

1. Gå till **[!UICONTROL [!DNL Aol] Keyword: Mail controls]** om du vill visa sidan [!UICONTROL Spam Settings].

1. [!DNL Aol] [!UICONTROL Keyword] är bara en funktion i [!DNL Aol]. Om du behöver instruktioner för att få åtkomst till sidan [!UICONTROL Spam Settings] från [!DNL Aol] [!UICONTROL Webmail] eller [!DNL Aol] [!UICONTROL Desktop] kan du läsa hjälpen för [!DNL Aol].
1. Om **[!UICONTROL Block mail from addresses I specify]** har valts i fältet **[!UICONTROL Sender Filter]** och eventuella [!DNL Workfront Proof] adresser eller domännamn finns med i listan över blockerade adresser, tar du bort de adresserna från listan.

1. Klicka på **[!UICONTROL Save]**.

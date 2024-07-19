---
title: Exempel på det externa sökfältet i ett anpassat formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Ett externt uppslagsfält i ett anpassat formulär anropar ett externt API och returnerar värden som alternativ i ett nedrullningsbart fält. I den här artikeln finns exempel på hur du använder fältet för extern sökning för att anropa samma instans av Workfront eller ett offentligt API.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 101a5a80d00a8113ce31222b92f77300a5b0ce8a
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Exempel på det externa sökfältet i ett anpassat formulär

Ett externt uppslagsfält i ett anpassat formulär anropar ett externt API och returnerar värden som alternativ i ett nedrullningsbart fält. Användare som arbetar med objektet som det anpassade formuläret är kopplat till kan välja ett eller flera av dessa alternativ i listrutan.

I den här artikeln finns exempel på hur du använder fältet för extern sökning för att anropa samma instans av Workfront eller ett offentligt API. Du kan också använda den externa sökningen för att kommunicera med ett externt system som Jira, Salesforce eller ServiceNow.

Externa sökfält är bara tillgängliga i den nya formulärdesignern, inte i den gamla formulärbyggaren. Mer information om hur du lägger till ett externt uppslagsfält i ett anpassat formulär och ytterligare definitioner för de externa uppslagskomponenterna finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Konfigurera ett externt sökfält för samma instans av Workfront

Du kan använda den externa sökningen för att hämta data från din Workfront-instans till det anpassade formuläret.

I det här exemplet visas hur du anropar Workfront API och hämtar data från det befintliga statusfrågefältet till det externa sökfältet.

1. Öppna det anpassade formuläret.
1. Leta upp **extern sökning** till vänster på skärmen och dra den till ett avsnitt på arbetsytan.
1. Ange fältets **etikett** och **namn**.
1. Välj **Format** för fältet.
1. Ange API-URL-anropet i fältet **Bas-API URL**.

   * Du kan lägga till $$HOST för att referera till samma instans.
   * Du kan lägga till $$QUERY om du vill filtrera resultaten baserat på en fråga i ett annat fält.

   **Exempel**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Granska **beroendena** för fälten som det här sökfältet refererar till i API:t.

   Ett beroendefält kan vara vilket anpassat eller inbyggt fält som helst som finns på objektets informationssida.

   I det här exemplet ersätts `{DE:StatusQuery}` med värdet för det anpassade statusfrågefältet.

1. Välj **HTTP-metod**.

   Detta kommer troligtvis att vara **Get**.

1. Ange **JSON-sökvägen** för att få resultat från ditt API-anrop.

   **Exempel**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Rubrik** krävs inte för ett anrop till samma Workfront-instans.

1. Klicka på **Använd**.

   ![Konfigurera API-anrop till Workfront i anpassat format](assets/external-lookup-to-workfront.png)

   När det anpassade formuläret läggs till i ett Workfront-objekt (i det här exemplet ett projekt) ser det ut ungefär så här.

   ![Anpassat formulär med externt sökfält](assets/external-lookup-project-status-example1.png)

   ![Alternativ för extern sökning baserat på status](assets/external-lookup-project-status-example2.png)

## Konfigurera ett externt sökfält för ett offentligt API

Du kan använda den externa sökningen för att anropa ett externt, offentligt API och hämta data.

I det här exemplet visas hur du anropar ett API med länder (till exempel <https://api.first.org/data/v1/countries>) så att du inte behöver hårdkoda alla landsnamn i listrutan.

1. Öppna det anpassade formuläret.
1. Leta upp **extern sökning** till vänster på skärmen och dra den till ett avsnitt på arbetsytan.
1. Ange fältets **etikett** och **namn**.
1. Välj **Format** för fältet.
1. Ange API-URL-anropet i fältet **Bas-API URL**.

   * Du kan lägga till $$QUERY för att implementera frågefiltrering för slutanvändarna.

   **Exempel**
Visar alla länder: <https://api.first.org/data/v1/countries>

   Tillåter användaren att söka efter ett land i listrutan: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Låter användaren söka efter ett land i en region: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * De tillgängliga områdena definieras i ett separat anpassat fält i Workfront.
   * När användaren väljer en region i formuläret visar fältet för extern sökning endast länderna i den regionen (i vilket land som regionen definieras i API:t). Användaren kan också söka efter ett land i den valda regionen.

1. Granska **beroendena** för fälten som det här sökfältet refererar till i API:t.

   Ett beroendefält kan vara vilket anpassat eller inbyggt fält som helst som finns på objektets informationssida.

   I det här exemplet ersätts `{DE:Region}` med värdet för det anpassade fältet Region.

1. Välj **HTTP-metod**.

   Detta kommer troligtvis att vara **Get**.

1. Ange **JSON-sökvägen** för att få resultat från ditt API-anrop.

   Med det här alternativet kan data extraheras från den JSON som returneras av API-URL:en. Det är ett sätt att välja vilka värden från JSON som ska visas i listrutealternativen.

   **Exempel**
   `$.data[*].country`

1. (Valfritt) Klicka på **Lägg till huvud** och skriv eller klistra in det nyckel/värde-par som krävs för autentisering med API:t.

   >[!NOTE]
   >
   >Rubrikfälten är inte ett säkert ställe att lagra inloggningsuppgifter på och du bör vara försiktig med vad du anger och sparar.

1. (Valfritt) Välj **Flervalslistruta** om du vill att användaren ska kunna välja mer än ett värde i listrutan.

1. Klicka på **Använd**.

   ![Konfigurera API-anrop till publikt API i anpassat format](assets/external-lookup-to-api-for-countries.png)

   När det anpassade formuläret läggs till i ett Workfront-objekt (i det här exemplet ett projekt) ser det ut ungefär så här.

   ![Anpassat formulär med externt sökfält](assets/external-lookup-countries-example1.png)

   ![Alternativ för extern sökning för ett land baserat på region](assets/external-lookup-countries-example2.png)

---
title: Exempel på det externa sökfältet i ett anpassat formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Ett fält för extern sökning i ett anpassat formulär anropar ett externt API och returnerar värden som alternativ i ett nedrullningsbart fält. I den här artikeln finns exempel på hur du använder fältet för extern sökning för att anropa samma instans av Workfront eller ett offentligt API.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 40d9455fe3b14006817c784a4d3c8dea8a601839
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# Exempel på det externa sökfältet i ett anpassat formulär

Ett fält för extern sökning i ett anpassat formulär anropar ett externt API och returnerar värden som alternativ i ett nedrullningsbart fält. Användare som arbetar med objektet som det anpassade formuläret är kopplat till kan välja ett eller flera av dessa alternativ i listrutan.

I den här artikeln finns exempel på hur du använder fältet för extern sökning för att anropa samma instans av Workfront eller ett offentligt API. Du kan också använda den externa sökningen för att kommunicera med ett externt system som Jira, Salesforce eller ServiceNow.

Mer information om hur du lägger till ett externt sökfält i ett anpassat formulär och ytterligare definitioner för de externa sökningskomponenterna finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Konfigurera ett externt sökfält för samma instans av Workfront

Du kan använda den externa sökningen för att hämta data från din Workfront-instans till det anpassade formuläret.

### Använd inbyggda Workfront-fältvärden i den externa sökningen

I det här exemplet visas hur du anropar Workfront API och hämtar data från det befintliga statusfrågefältet till det externa sökfältet.

1. Öppna det anpassade formuläret.
1. Leta upp **extern sökning** till vänster på skärmen och dra den till ett avsnitt på arbetsytan.
1. Ange fältets **etikett** och **namn**.
1. Välj **Format** för fältet.
1. Ange API-anropet i fältet **Bas-API URL**.

   * Om du vill referera till samma instans av Workfront som det anpassade formuläret finns i använder du $$HOST som URL.
   * Om du vill filtrera resultaten baserat på en fråga i ett annat fält lägger du till $$QUERY.

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

### Använd anpassade fältvärden i extern sökning

I det här exemplet visas hur du anropar Workfront API och hämtar data från ett anpassat fält till det externa sökfältet. Det anpassade exempelfältet heter&quot;Egna färger&quot;.

1. Öppna det anpassade formuläret.
1. Leta upp **extern sökning** till vänster på skärmen och dra den till ett avsnitt på arbetsytan.
1. Ange fältets **etikett** och **namn**.
1. Välj **Format** för fältet.
1. Ange API-URL-anropet i fältet **Bas-API URL**.

   **Exempel**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Granska **beroendena** för fälten som det här sökfältet refererar till i API:t.

   Ett beroendefält kan vara vilket anpassat eller inbyggt fält som helst som finns på objektets informationssida.

1. Välj **HTTP-metod**.

   Detta kommer troligtvis att vara **Get**.

1. Ange **JSON-sökvägen** för att få resultat från ditt API-anrop.

   **Exempel**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * &quot;parameterValues&quot; refererar till alla anpassade fält i Workfront för det objekt du är på.
   * I det här exemplet är&quot;DE:Combo Colors&quot; det specifika anpassade fältet som innehåller de värden som du vill hämta.

   >[!NOTE]
   >
   >**Rubrik** krävs inte för ett anrop till samma Workfront-instans.

1. Klicka på **Använd**.

   När det anpassade formuläret läggs till i ett Workfront-objekt visas alla värden i fältet&quot;Kombinationsfärger&quot; i listrutan Extern sökning.

## Konfigurera ett externt sökfält för Workfront Planning API

Det finns en slutpunkt i Workfront Planning API för att söka efter poster efter posttyp-ID med metoden Get. Du kan använda den här slutpunkten för att referera till planeringsposter i externa sökfält.

* **Bas-API-URL:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **HTTP-metod:** Hämta
* **JSON-sökväg:** `$.records[*].data.{fieldID}`

  **{fieldID}** är det fält som ska visas i sökresultaten för extern sökning i det anpassade formuläret för slutanvändare.

Mer information finns i [Workfront Planning API](/help/quicksilver/planning/general/planning-api-basics.md).

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

## Fler användningsexempel för externa sökfält

Det finns många andra användningsområden för att skapa en extern sökning.

**Använd skiftläge:** Ersätt typsnittsfält eftersom de kan orsaka problem med rapporteringen.
**Lösning:** Använd ett API-anrop till befintliga objekt i systemet.

Exempel på bas-API-URL för mallar som ersätter ett typsnittsfält:
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Använd skiftläge:** Skapa listrutefält med fler funktioner (det finns t.ex. radbrytning i fältet Extern sökning).
**Lösning:** Använd ett API-anrop till befintliga objekt i systemet eller skapa ett nytt objekt och använd ett API-anrop till det här objektet.

**Använd skiftläge:** Definiera ett sätt för användare att behålla sina egna fält utanför det anpassade formulärområdet. Konfigurera fältet Extern sökning så kan du ge användarna till de objekt som fältet består av. Det här alternativet passar bra för underhållsområden och team.
**Lösning:** Skapa ett nytt objekt och använd ett API-anrop till det här objektet.

**Använd skiftläge:** Integrering med objekt utanför Workfront. Du kan till exempel få åtkomst till ett annat system för att få namnet på varje användare, i stället för att begränsas i ett typsnittsfält.
**Lösning:** Webkrok-/Fusion-automatisering för att ansluta till andra system.


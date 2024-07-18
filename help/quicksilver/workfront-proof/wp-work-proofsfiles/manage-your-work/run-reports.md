---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Kör rapporter i  [!DNL Workfront Proof]
description: Med Workfront Proof kan du visa rapporter så att du kan följa upp hur arbetet fortskrider och hur effektivt era team är.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Kör rapporter i [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">Rapporteringsfunktionen är inte längre tillgänglig i [!DNL Workfront Proof]. Rapporteringsfliken visas fortfarande, men data är inte korrekta.</span>
> 
>* Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Med Workfront Proof kan du visa rapporter så att du kan följa upp hur arbetet fortskrider och hur effektivt era team är.

Du kan enkelt visa antalet korrektur som har skapats i ditt [!DNL Workfront Proof]-konto, hur många versioner som är associerade med varje korrektur, hur lång tid det tar att gå runt och mycket annat.

## Förutsättningar

Vilka rapporter som är tillgängliga beror på vilken typ av [!DNL Workfront Proof]-konto du har och vilken behörighet användaren har.

* [Kontokrav](#account-prerequisites)
* [Förutsättningar](#user-prerequisites)

### Kontokrav {#account-prerequisites}

Rapporteringsinformation är bara tillgänglig med Premium-planer.

### Förutsättningar {#user-prerequisites}

Rapporteringsinformation är bara tillgänglig för användare med fullständig åtkomst till alla korrektur på ditt konto (d.v.s. användare med minst [behörighetsprofiler för korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

På den här panelen kan du

* Styr tidsrymden för visade data
* Analysera förändringar i mätvärden över tid
* Kontrollera informationen om en markerad tidpunkt genom att hålla markören över den
* Kontrollera det totala antalet korrektur som skapats under den valda tidsperioden
* Kontrollera det genomsnittliga antalet versioner som ingår i de färdiga korrekturuppsättningarna

## Visa rapporter {#viewing-reports}

1. Gå till sidan **[!UICONTROL Dashboards]**.
1. Klicka på fliken **[!UICONTROL Reports]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. I listrutan **[!UICONTROL Time frame]** väljer du om du vill visa information om korrektur som skapats under de senaste 24 timmarna, 7 dagarna, 30 dagar, 90 dagarna eller en anpassad tidsperiod.\
   Om du väljer en anpassad tidsperiod väljer du start- och slutdatum och klickar sedan på **[!UICONTROL Apply]**.\
   Följande information visas för den valda tidsperioden:\
   **Korrektur har skapats:** Antal korrektur som har skapats under den valda tidsperioden.\
   **Versioner per korrektur:** Genomsnittligt antal versioner per korrektur för alla slutförda korrektur (Godkänd eller Godkänd med ändringar) under den valda tidsperioden.\
   **Vänd om tid:** Genomsnittlig tid från det att den första versionen skapades till den tidpunkt då beslutet fattades om den slutliga versionen.\
   **Första aktivitetstid:** Genomsnittlig tid från det att korrekturet skapades till tidpunkten för den första aktiviteten i korrekturet.\
   **Sena korrektur:** Genomsnittligt antal slutförda korrektur (Godkänd eller Godkänd med ändringar) som hade minst en version som var sen inom den valda tidsperioden.\
   **Kommentarer och svar:** Genomsnittligt antal kommentarer och svar som gjordes på alla korrektur under den valda tidsperioden.

1. (Valfritt) Markera eller avmarkera alternativet **[!UICONTROL Show min-max range]** för att avgöra om lägsta och högsta värden visas i diagrammet.\
   När det här alternativet är markerat visas blå skuggning mellan det lägsta och högsta registrerade värdet.

1. (Valfritt) Du kan filtrera de data som visas enligt beskrivningen i [Filtreringsrapporter](#filtering-reports).

## Filtrera rapporter {#filtering-reports}

Som standard innehåller data som visas i rapporter all information från ditt [!DNL Workfront Proof]-system. Du kan använda filter för att endast visa information som är relevant för dina behov.

Så här filtrerar du rapportinformation:

1. Gå till sidan **[!UICONTROL Dashboards]**.
1. Klicka på fliken **[!UICONTROL Reports]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Kör en rapport enligt beskrivningen i [Visa rapporter](#viewing-reports).
1. Klicka på **[!UICONTROL Filter]**.

1. Till vänster på sidan väljer du bland följande filteralternativ:\
   **[!UICONTROL Proof Type]:** Välj den typ av korrektur som du vill ska ingå i rapporten.\
   **[!UICONTROL Decisions]:** Välj alternativ för att avgöra om endast korrektur som innehåller vissa beslut har gjorts.\
   **[!UICONTROL Recipients]:** Välj enskilda användare om du vill visa information om korrektur som delas med de valda användarna.\
   **[!UICONTROL Proof Owners]:** Välj enskilda användare om du vill visa information om korrektur som ägs av de valda användarna.\
   **[!UICONTROL Proof Creators]:** Välj enskilda användare om du vill visa information om korrektur som har skapats av de valda användarna.\
   **[!UICONTROL Accounts]:** Välj vilka konton du vill inkludera i rapporten.

1. Klicka på **[!UICONTROL Apply]**.
1. (Valfritt) Markera eller avmarkera alternativet **[!UICONTROL Show min-max range]** för att avgöra om lägsta och högsta värden visas i diagrammet.\
   När det här alternativet är markerat visas blå skuggning mellan det lägsta och högsta registrerade värdet.

## Utskriftsrapporter

1. Gå till sidan **[!UICONTROL Dashboards]**.
1. Klicka på fliken **[!UICONTROL Reports]** och sedan på **[!UICONTROL Print]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Välj bland de olika utskriftsalternativen som är tillgängliga.\
   Utskriftsalternativen varierar beroende på vilken webbläsare och webbläsarversion du använder.

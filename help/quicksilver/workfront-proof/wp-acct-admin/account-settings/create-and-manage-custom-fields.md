---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Skapa och hantera anpassade fält i [!DNL Workfront Proof]
description: A Select or Premium [!DNL Workfront] Planering krävs för att använda den här funktionen. Mer information om olika planer finns i Workfront Planer.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Skapa och hantera anpassade fält i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

A Select or Premium [!DNL Workfront] Planering krävs för att använda den här funktionen. Mer information om olika planer finns i [Workfront-planer](https://www.workfront.com/plans).

Med anpassade fält kan du samla in ytterligare data när du skapar ett nytt korrektur, en ny användare eller en ny gäst.

Användare som skapar ett nytt korrektur kan till exempel vilja inkludera ytterligare ett avsnitt där de kan hämta ett jobbnummer, en avdelningskod eller en leverantörsreferens.

>[!NOTE]
>
>* Genom att hämta in den här typen av information på sidan Nytt korrektur via anpassade fält kan du också minska längden på korrekturnamnet, eftersom dessa uppgifter inte behöver inkluderas i namnet. Mer information om sidan Nytt korrektur finns i&quot;Skapa korrektur i [!DNL Workfront Proof].&quot;
>
>När ett anpassat fält har använts på ett korrektur, en användare eller en kontakt, kan du inte ta bort det eller redigera fälttypen. Du kan dock dölja den (via [!UICONTROL Custom field Settings] sida) så att den inte används för nya objekt.
>
>Om du döljer ett anpassat fältavsnitt döljs även alla fält i avsnittet, även om de enskilda fälten är synliga.

I den här artikeln beskrivs hur du gör följande:

## Skapa anpassade fält

Först måste du ställa in avsnittet Anpassat fält där du ska lägga till anpassade fält.

1. Klicka **[!UICONTROL Settings]** >**[!UICONTROL Account Settings]**&#x200B;öppnar du **[!UICONTROL Custom fields]** -fliken.

1. Klicka **[!UICONTROL Add custom field section]** i den relevanta modulen (Korrektur, Användare eller Kontakter).
1. Skriv a **Namn** för anpassade fältavsnitt och klicka sedan på **[!UICONTROL Save]**.

   Nu kan du skapa anpassade fält i avsnittet:

1. Klicka på **[!UICONTROL Custom fields settings]** för att uppdatera sidan.
1. Klicka på namnet på det nya anpassade fältavsnittet för att öppna **[!UICONTROL Custom field]section** sida för det nya avsnittet.
1. Klicka på **[!UICONTROL New custom field]** nära det övre högra hörnet.
1. I **[!UICONTROL New custom field]** anger du information om det anpassade fältet på sidan som visas:

   | **Obligatoriskt** | Workfront kräver att användaren fyller i fältet. |
   |---|---|
   | **Sökbart** | Gör att användare kan hitta objekt genom att söka efter data i det anpassade fältet. |
   | **Dold** | Döljer det anpassade fältet på [!UICONTROL New proof], ny gäst och [!UICONTROL New user] sidor |

   {style=&quot;table-layout:auto&quot;}

1. Klicka på **[!UICONTROL Save]**.
1. I **Anpassat fält** som visas klickar du på **[!UICONTROL Custom fields settings]** för att uppdatera sidan.

1. Gör ytterligare ändringar av fältets inställningar:

   * Dölja eller visa det anpassade fältavsnittet genom att klicka på **[!UICONTROL More]** (tre punkter) meny till höger om namnet på det anpassade fältavsnittet och klicka sedan på **[!UICONTROL Hide section]** eller **[!UICONTROL Unhide section]**.

   * Dölj eller visa det anpassade fältet genom att klicka på **[!UICONTROL More]** (tre punkter) meny till höger om namnet på det anpassade fältavsnittet och klicka sedan på **[!UICONTROL Hide custom field]** eller **[!UICONTROL Unhide custom field]**.

   * Ändra fältordningen med upp-/nedpilarna som visas till höger om fältnamnen (om du har lagt till flera fält i ett avsnitt).

1. Öppna **[!UICONTROL Visibility rules]** -fliken.\
   Med synlighetsregler kan du ange vilka ytterligare fält som ska visas, baserat på det inledande anpassade fältet. Om det beroende fältet till exempel är A och kontrollfältet är X, innebär det att fält A bara är synligt om fält X är ifyllt.

   Du kan använda kontrollvärden för att bestämma värdena i kontrollfältet som, om de väljs, leder till att det beroende fältet visas. Föreställ dig till exempel att det beroende fältet är A och att kontrollfältet är X, och du anger att kontrollvärdena i X endast är alternativ 1 och 2. Det innebär att fält A bara visas om fält X alternativ 1 eller 2 är markerat. Det innebär att fält A inte visas om fält X alternativ 3 eller 4 är markerade. Öppna **[!UICONTROL Visibility rules]** -fliken.

   Så här lägger du till en synlighetsregel:

   1. Klicka **[!UICONTROL New visibility rule]** för den modul där du vill lägga till regeln.
   1. Välj önskade inställningar för regeln och klicka sedan på **[!UICONTROL Save]**.

1. Öppna **[!UICONTROL Dependency rules]** -fliken.

   Med beroenderegler kan du bestämma vilka alternativ som är tillgängliga i det beroende fältet när vissa alternativ är markerade i kontrollfältet. Om det beroende fältet till exempel är &quot;B&quot; och kontrollfältet är &quot;Y&quot;, kan du ställa in det på följande sätt:

   Om alternativ 1 väljs i fält Y visas endast alternativen 1 och 2 i fält B.

   Om alternativ 2 väljs i fält Y visas endast alternativen 3 och 4 i fält B.

   Så här lägger du till en beroenderegel:

   1. Klicka **[!UICONTROL New dependency rule]** för modulen som du vill lägga till regeln i.
   1. Välj inställningar för beroendet och klicka sedan på **[!UICONTROL Save]**.

## Hantera anpassade fält

Du kan visa och redigera information om anpassade fältavsnitt eller enskilda anpassade fält.

1. Klicka **[!UICONTROL Settings]** >**[!UICONTROL Account Settings]**&#x200B;öppnar du **[!UICONTROL Custom fields]** -fliken.

1. Klicka på namnet på det anpassade fältavsnittet eller enskilda anpassade fält.
1. (Villkorligt) Om du hanterar ett anpassat fältavsnitt gör du någon av följande ändringar i **[!UICONTROL Custom field section]** sida:

   * Redigera avsnittets namn.
   * Flytta den till en annan modul.
   * Dölj/visa avsnittet.

1. (Villkorligt) Om du hanterar ett anpassat fält gör du något av följande på **[!UICONTROL Custom field]** sida:

   * Flytta fältet till ett annat avsnitt.
   * Redigera fältets namn.
   * Inmatningshjälptext (en frågeteckenikon visas bredvid fältavsnittet och texten visas när du håller muspekaren över den).
   * Aktivera/inaktivera **[!UICONTROL Mandatory]** på fältet.
   * Aktivera/inaktivera **[!UICONTROL Searchable]** på fältet.
   * Dölj/visa fältet.
   * Redigera fälttypen.
   * Ange/redigera ett standardvärde för fältet.
   * Ställ in synlighets- och beroenderegler (som beskrivs ovan i steg 11 och 12).

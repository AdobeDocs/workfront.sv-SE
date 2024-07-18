---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Skapa och hantera anpassade fält i  [!DNL Workfront Proof]
description: En Select- eller Premium [!DNL Workfront] Plan krävs för den här funktionen. Mer information om olika planer finns i Workfront Planer.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Skapa och hantera anpassade fält i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

En Select- eller Premium [!DNL Workfront]-plan krävs för den här funktionen. Mer information om olika tillgängliga planer finns i [Workfront-planer](https://www.workfront.com/plans).

Med anpassade fält kan du samla in ytterligare data när du skapar ett nytt korrektur, en ny användare eller en ny gäst.

Användare som skapar ett nytt korrektur kan till exempel vilja inkludera ytterligare ett avsnitt där de kan hämta ett jobbnummer, en avdelningskod eller en leverantörsreferens.

>[!NOTE]
>
>* Genom att hämta in den här typen av information på sidan Nytt korrektur via anpassade fält kan du också minska längden på korrekturnamnet, eftersom dessa uppgifter inte behöver inkluderas i namnet. Mer information om sidan Nytt korrektur finns i&quot;Skapa korrektur i [!DNL Workfront Proof]&quot;.
>
>När ett anpassat fält har använts på ett korrektur, en användare eller en kontakt, kan du inte ta bort det eller redigera fälttypen. Du kan emellertid dölja den (via sidan [!UICONTROL Custom field Settings]) så att den inte används för nya objekt.
>
>Om du döljer ett anpassat fältavsnitt döljs även alla fält i avsnittet, även om de enskilda fälten är synliga.

I den här artikeln beskrivs hur du gör följande:

## Skapa anpassade fält

Först måste du ställa in avsnittet Anpassat fält där du ska lägga till anpassade fält.

1. Klicka på **[!UICONTROL Settings]** >**[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Custom fields]**.

1. Klicka på **[!UICONTROL Add custom field section]** i relevant modul (Korrektur, Användare eller Kontakter).
1. Ange ett **namn** för det anpassade fältavsnittet och klicka sedan på **[!UICONTROL Save]**.

   Nu kan du skapa anpassade fält i avsnittet:

1. Klicka på fliken **[!UICONTROL Custom fields settings]** för att uppdatera sidan.
1. Klicka på namnet på det nya anpassade fältavsnittet för att öppna sidan **[!UICONTROL Custom field]section** för det nya avsnittet.
1. Klicka på **[!UICONTROL New custom field]** i det övre högra hörnet.
1. På sidan **[!UICONTROL New custom field]** som visas anger du information för det anpassade fältet:

   | **Obligatoriskt** | Workfront kräver att användaren fyller i fältet. |
   |---|---|
   | **Sökbar** | Gör att användare kan söka efter objekt genom att söka efter data i det anpassade fältet. |
   | **Dold** | Döljer det anpassade fältet på sidorna [!UICONTROL New proof], Ny gäst och [!UICONTROL New user] |

   {style="table-layout:auto"}

1. Klicka på **[!UICONTROL Save]**.
1. Klicka på fliken **[!UICONTROL Custom fields settings]** på sidan **Anpassat fält** som visas för att uppdatera sidan.

1. Gör ytterligare ändringar av fältets inställningar:

   * Dölj eller visa det anpassade fältavsnittet genom att klicka på menyn **[!UICONTROL More]** (tre punkter) till höger om det anpassade fältavsnittsnamnet och sedan klicka på **[!UICONTROL Hide section]** eller **[!UICONTROL Unhide section]**.

   * Dölj eller visa det anpassade fältet genom att klicka på menyn **[!UICONTROL More]** (tre punkter) till höger om namnet på det anpassade fältavsnittet och sedan klicka på **[!UICONTROL Hide custom field]** eller **[!UICONTROL Unhide custom field]**.

   * Ändra fältordningen med upp-/nedpilarna som visas till höger om fältnamnen (om du har lagt till flera fält i ett avsnitt).

1. Öppna fliken **[!UICONTROL Visibility rules]**.\
   Med synlighetsregler kan du ange vilka ytterligare fält som ska visas, baserat på det inledande anpassade fältet. Om det beroende fältet till exempel är A och kontrollfältet är X, innebär det att fält A bara är synligt om fält X är ifyllt.

   Du kan använda kontrollvärden för att bestämma värdena i kontrollfältet som, om de väljs, leder till att det beroende fältet visas. Föreställ dig till exempel att det beroende fältet är A och kontrollfältet är X, och du ställer in kontrollvärdena i X till att endast vara alternativ 1 och 2. Det innebär att fält A bara visas om fält X alternativ 1 eller 2 är markerat. Det innebär att fält A inte visas om fält X alternativ 3 eller 4 är markerade. Öppna fliken **[!UICONTROL Visibility rules]**.

   >[!NOTE]
   >
   >Endast anpassade fälttyper för List och Radio kan användas för kontrollfältet i en synlighetsregel, medan det beroende fältet kan vara vilken fälttyp som helst.

   Så här lägger du till en synlighetsregel:

   1. Klicka på **[!UICONTROL New visibility rule]** för den modul där du vill lägga till regeln.
   1. Välj önskade inställningar för regeln och klicka sedan på **[!UICONTROL Save]**.

1. Öppna fliken **[!UICONTROL Dependency rules]**.

   Med beroenderegler kan du bestämma vilka alternativ som är tillgängliga i det beroende fältet när vissa alternativ är markerade i kontrollfältet. Om det beroende fältet till exempel är &quot;B&quot; och kontrollfältet är &quot;Y&quot;, kan du ställa in det på följande sätt:

   Om alternativ 1 väljs i fält Y visas endast alternativen 1 och 2 i fält B.

   Om alternativ 2 väljs i fält Y visas endast alternativen 3 och 4 i fält B.

   >[!NOTE]
   >
   >Endast anpassade fälttyper List och Radio kan användas för beroende och styrande fält i en beroenderegel.

   Så här lägger du till en beroenderegel:

   1. Klicka på **[!UICONTROL New dependency rule]** för den modul som du vill lägga till regeln i.
   1. Välj inställningar för beroendet och klicka sedan på **[!UICONTROL Save]**.

## Hantera anpassade fält

Du kan visa och redigera information om anpassade fältavsnitt eller enskilda anpassade fält.

1. Klicka på **[!UICONTROL Settings]** >**[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Custom fields]**.

1. Klicka på namnet på det anpassade fältavsnittet eller enskilda anpassade fält.
1. (Villkorligt) Om du hanterar ett anpassat fältavsnitt gör du någon av följande ändringar på sidan **[!UICONTROL Custom field section]**:

   * Redigera avsnittets namn.
   * Flytta den till en annan modul.
   * Dölj/visa avsnittet.

1. (Villkorligt) Om du hanterar ett anpassat fält gör du någon av följande ändringar på sidan **[!UICONTROL Custom field]**:

   * Flytta fältet till ett annat avsnitt.
   * Redigera fältets namn.
   * Inmatningshjälptext (en frågeteckenikon visas bredvid fältavsnittet och texten visas när du håller muspekaren över den).
   * Aktivera/inaktivera inställningen **[!UICONTROL Mandatory]** för fältet.
   * Aktivera/inaktivera inställningen **[!UICONTROL Searchable]** för fältet.
   * Dölj/visa fältet.
   * Redigera fälttypen.
   * Ange/redigera ett standardvärde för fältet.
   * Ställ in synlighets- och beroenderegler (som beskrivs ovan i steg 1 och 12).

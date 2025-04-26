---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Skapa och hantera anpassade fält i  [!DNL Workfront Proof]
description: En Select- eller Premium [!DNL Workfront] Plan krävs för den här funktionen. Mer information om olika planer finns i Workfront Planer.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Skapa och hantera anpassade fält i [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

En Select- eller Premium [!DNL Workfront]-plan krävs för den här funktionen. Mer information om olika tillgängliga planer finns i [Workfront-planer](https://business.adobe.com/products/workfront/pricing.html).

Med anpassade fält kan du samla in ytterligare data när du skapar ett nytt korrektur, en ny användare eller en ny gäst. Användare som skapar ett nytt korrektur kan till exempel vilja inkludera ytterligare ett avsnitt där de kan hämta ett jobbnummer, en avdelningskod eller en leverantörsreferens.

>[!NOTE]
>
>* Genom att hämta in den här typen av information på sidan Nytt korrektur via anpassade fält kan du också minska längden på ditt korrekturnamn, eftersom dessa uppgifter inte behöver inkluderas i namnet.
>
>* När ett anpassat fält har använts på ett korrektur, en användare eller en kontakt, kan du inte ta bort det eller redigera fälttypen. Du kan emellertid dölja det via sidan Inställningar för anpassat fält så att det inte används för nya objekt.
>
>* Om du döljer ett anpassat fältavsnitt döljs även alla fält i avsnittet, även om de enskilda fälten är synliga.

## Skapa anpassade fält

{{step1-to-proofing}}

1. Klicka på **Kontoinställningar** i det övre högra hörnet på sidan.

1. På sidan **Kontoinställningar** väljer du fliken **Anpassade fält** .

1. Klicka på **[!UICONTROL Add custom field section]** till höger om den modul (**Korrektur**, **Användare** eller **Kontakter**) som du vill lägga till det anpassade fältet i. Fliken **Avsnittsinformation** öppnas.

1. Ange ett **namn** för det anpassade fältavsnittet och klicka sedan på **[!UICONTROL Save]**.

1. Klicka på fliken **[!UICONTROL Custom fields settings]** för att uppdatera sidan. Det nya anpassade fältavsnittet visas under den tilldelade modulen.

   ![Fliken Inställningar för anpassade fält](assets/custom-field-settings-tab.png)

1. Klicka på namnet på det nya anpassade fältavsnittet för att öppna fliken **Anpassade fält**.

1. Klicka på knappen **[!UICONTROL New custom field]** längst upp till höger på sidan. Sidan **Nytt anpassat fält** visas.

1. Ange **fältinformation**:

   * **Namn**: Ange det anpassade fältnamnet.
   * **Hjälp**: Ange hjälptext som ska visas i ett verktygstips.
   * **Obligatoriskt**: Markera den här kryssrutan om du vill att användaren ska fylla i fältet.
   * **Sökbart** (villkorligt): Markera den här rutan om du vill att det anpassade fältet ska vara sökbart.
   * **Dold**: Markera den här rutan om du vill dölja det anpassade fältet på sidorna **Nytt korrektur**, **Ny gäst** och **Ny användare**.

1. Ange **fälttyp** och information:

   * **Typ**: Välj den anpassade fälttypen.
   * **Listobjekt**: (Villkorligt) Lägg till listobjekten som ska visas i det anpassade fältet.
   * **Standardvärde**: Välj standardvärde för det här anpassade fältet. Det här alternativet varierar beroende på vilken anpassad fälttyp som är vald.

1. Klicka på **[!UICONTROL Save]**.

1. Gör ytterligare ändringar av fältets inställningar:

   * Dölj eller visa det anpassade fältavsnittet genom att klicka på menyn **Mer** ![Mer](assets/more-button-small.png) till höger om det anpassade fältavsnittets namn och sedan klicka på **[!UICONTROL Hide section]** eller **[!UICONTROL Unhide section]**.
   * Dölj eller visa det anpassade fältet genom att klicka på menyn **Mer** ![Mer](assets/more-button-small.png) till höger om det anpassade fältavsnittets namn och sedan klicka på **[!UICONTROL Hide custom field]** eller **[!UICONTROL Unhide custom field]**.
   * Ändra fältordningen med upp-/nedpilarna som visas till höger om fältnamnen (om du har lagt till flera fält i ett avsnitt).

1. Klicka på fliken **[!UICONTROL Visibility rules]**.

   Med synlighetsregler kan du ange vilka ytterligare fält som ska visas baserat på det ursprungliga anpassade fältet. Om det beroende fältet till exempel är A och kontrollfältet är X, innebär det att fält A bara är synligt om fält X är ifyllt.

   Du kan använda kontrollvärden för att bestämma värdena i kontrollfältet som, om de väljs, leder till att det beroende fältet visas. Föreställ dig till exempel att det beroende fältet är A och kontrollfältet är X, och du ställer in kontrollvärdena i X till att endast vara alternativ 1 och 2. Det innebär att fält A bara visas om fält X alternativ 1 eller 2 är markerat. Om fältalternativ X 3 eller 4 är markerade visas inte fält A.

   >[!NOTE]
   >
   >Endast anpassade fälttyper för List och Radio kan användas för kontrollfältet i en synlighetsregel, medan det beroende fältet kan vara vilken fälttyp som helst.

   Så här lägger du till en synlighetsregel:

   1. Klicka på **[!UICONTROL New visibility rule]** för den modul som du vill lägga till regeln i.

   1. Välj önskade inställningar för regeln och klicka sedan på **[!UICONTROL Save]**.

1. Öppna fliken **[!UICONTROL Dependency rules]**.

   Med beroenderegler kan du bestämma vilka alternativ som är tillgängliga i det beroende fältet när vissa alternativ är markerade i kontrollfältet. Om det beroende fältet till exempel är &quot;B&quot; och kontrollfältet är &quot;Y&quot;, kan du ställa in det på följande sätt:

   * Om alternativ 1 väljs i fält Y visas endast alternativen 1 och 2 i fält B.

   * Om alternativ 2 väljs i fält Y visas endast alternativen 3 och 4 i fält B.

   >[!NOTE]
   >
   >Endast anpassade fälttyper List och Radio kan användas för beroende och styrande fält i en beroenderegel.

   Så här lägger du till en beroenderegel:

   1. Klicka på **[!UICONTROL New dependency rule]** för den modul som du vill lägga till regeln i.

   1. Välj inställningar för beroendet och klicka sedan på **[!UICONTROL Save]**.

## Hantera anpassade fält

Du kan visa och redigera information om anpassade fältavsnitt eller enskilda anpassade fält.

{{step1-to-proofing}}

1. Klicka på **Kontoinställningar** i det övre högra hörnet på sidan.

1. På sidan **Kontoinställningar** väljer du fliken **Anpassade fält** .

1. Klicka på namnet på det anpassade fältavsnittet eller enskilda anpassade fält.

1. (Villkorligt) Om du hanterar ett anpassat fältavsnitt gör du någon av följande ändringar på sidan **[!UICONTROL Custom field section]**:

   * Redigera avsnittets namn.
   * Flytta den till en annan modul.
   * Dölj/visa avsnittet.

1. (Villkorligt) Om du hanterar ett anpassat fält gör du någon av följande ändringar på sidan **[!UICONTROL Custom field]**:

   * Flytta fältet till ett annat avsnitt.
   * Redigera fältets namn.
   * Redigera hjälptext.
   * Aktivera/inaktivera inställningen **[!UICONTROL Mandatory]** för fältet.
   * (Villkorligt) Aktivera/inaktivera inställningen **[!UICONTROL Searchable]** i fältet.
   * Dölj/visa fältet.
   * Redigera fälttypen.
   * Ange/redigera ett standardvärde för fältet.
   * Ställ in synlighets- och beroenderegler.

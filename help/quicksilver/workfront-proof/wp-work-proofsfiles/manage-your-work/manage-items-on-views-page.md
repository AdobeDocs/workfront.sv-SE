---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Hantera objekt på sidan [!UICONTROL Views] i [!DNL Workfront Proof]
description: På sidan [!UICONTROL Views] kan du visa och arbeta med alla dina korrektur, filer och mappar på ett och samma ställe.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 56556d16-9aab-4b0e-b08c-ac5f1703e082
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 0%

---

# Hantera objekt på sidan [!UICONTROL Views] i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

På sidan [!UICONTROL Views] kan du visa och arbeta med alla dina korrektur, filer och mappar på ett och samma ställe.

## Visar sidan [!UICONTROL Views]

1. Klicka på **[!UICONTROL Views]** i den vänstra sidlisten.
1. I listrutan (2) klickar du på den vy (3) som du vill se.

![Vyer.png](assets/views-350x297.png)

## Ändra sidlayouten [!UICONTROL Views]

Standardsidlayouten [!UICONTROL Views] är miniatyrlistan. I den här layouten kan du se en miniatyrbild av varje korrektur, fil (om det går att generera) och mappar (om det är inställt), med annan information i separata kolumner.

1. Klicka på ikonen **[!UICONTROL Page Layout]** (1) och välj sedan önskad layout.

![Views_Page_Layout.png](assets/views-page-layout-350x140.png)

## Ändra listan [!UICONTROL Views]

Så här ändrar du det du ser i listan [!UICONTROL Views]:

1. Klicka på knappen **[!UICONTROL Change view]**.\
   Namnet som visas på den här knappen beror på vilken vy du valde senast du använde den.\
   ![Views-Change_view_button.png](assets/views-chnge-view-button-350x205.png)

1. Klicka på en annan vy i listrutan:

   * **[!UICONTROL All items]**: Innehåller alla korrektur, filer och mappar som du har behörighet att se. Det är standard när du öppnar sidan [!UICONTROL Views]. Du kan välja att inkludera/exkludera arkiverade korrektur i den här vyn.
   * **[!UICONTROL Active items]**: Alla aktiva korrektur, filer och mappar.
   * **[!UICONTROL Active proofs]**: Alla aktiva (inte arkiverade) korrektur som du har behörighet att se.
   * **[!UICONTROL Locked proofs]**: Endast låsta korrektur.
   * **[!UICONTROL Archived proofs]**: Endast arkiverade korrektur (se [Arkivera i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/archive.md)).

   * **[!UICONTROL My Proofs]**: Visar endast korrektur som du är ägare till och som har delegerats till dig. Mer information finns i [Ange tillfälliga korrekturägare i [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).

   * **[!UICONTROL Proofs awaiting decision]**: Visar endast korrektur som du måste fatta ett beslut om
   * **[!UICONTROL Late proofs]**: Visar endast korrektur som deadline har passerat
   * **[!UICONTROL Files]**: Visar endast filer

   I var och en av dessa vyer ingår följande kolumner

   * **Typ**: Ikon för objektet med ikonen för korrektur, fil eller mapp
   * **Namn**: Namn på korrektur, fil eller mapp
   * **Förlopp**: S=Skickat, O=Öppnat, C=Kommentar, D=Beslut (se förloppsindikator)
   * **Status**: [!UICONTROL Pending, Changes required, Approved]
   * **Beslut**: Antal beslut som fattats och antal som krävs
   * **Ägare**: Namnet på den person som äger beviset\

     Mina korrektur, korrektur som väntar på beslut och sen korrekturvy har en extra kolumn som heter Min deadline. I den här kolumnen visas dina egna deadlines på korrektur där du uttryckligen har lagts till som granskare/godkännare.

     >[!NOTE]
     >
     >Om du navigerar bort från sidan Vyer och återgår till den senare under samma session, visas den senast markerade vyn.

     Du kan också skapa egna vyer. Mer information finns i [Skapa och hantera anpassade vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).



## Filtrera objekt

Du kan filtrera informationen som visas i en vy.

1. Klicka på ikonen **Visa filter** längst upp på sidan (1).\
   ![Filters.png](assets/filters-350x107.png)

1. Filterfältet (2) visas och varje kategori har en listruta för filtrering (3) där du kan välja önskat värde. Standardvärdet för varje kategori är Alla.
1. Filterfältet visas inte i anpassade vyer som du skapar. För dessa vyer kan du använda och redigera filter på fliken [!UICONTROL Filters]. Mer information finns i [Skapa och hantera anpassade vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
1. Om du vill använda alla valda filter klickar du på ikonen [!UICONTROL Filter] (4) i slutet av filtreringsfältet.\
   ![Filters_2.png](assets/filters-2-350x102.png)

De filtervärden som du väljer fortsätter att gälla tills du ändrar dem. Om du vill visa och komma åt den fullständiga listan med objekt igen måste du ändra alla filtervärden tillbaka till standardvärdet, som är **[!UICONTROL All]**.

>[!NOTE]
>
>Om du anger filtreringsalternativ och sedan döljer filtreringsfältet genom att klicka på ikonen [!UICONTROL Hide filters] (5), visas fältet automatiskt igen om du byter vy. Om du döljer filtreringsfältet medan alla filter är inställda på standardalternativet för alla, förblir filtreringsfältet dolt när du ändrar vyer.

## Sortera objekt

När du skapar ett nytt korrektur (eller en ny version) eller överför en ny fil visas det högst upp i listan [!UICONTROL All items]. Det äldsta objektet visas längst ned i listan.

Så här visar du listan i en annan sorteringsordning:

1. Gör något av följande:

   * Klicka på en av kolumnrubrikerna i listan: Typ, Namn, Status, Beslut eller Ägare.\

     Om du till exempel vill se korrektur/filer i alfabetisk ordning klickar du på rubriken Namn en gång (1) för att sortera listan efter namn i stigande ordning (A - Z).\
      Du kan klicka på rubriken Korrekturnamn igen (2) om du vill kasta om ordningen och visa korrektur i fallande ordning (Z - A).

   * Klicka på nedpilen i det övre högra hörnet på sidan [!UICONTROL Views] om du vill sortera efter skapandedatum (senaste eller äldsta) eller efter typ, namn, status, beslut eller ägare.\

     ![Views-Sort_down_arrow.png](assets/views-sort-down-arrow-350x124.png)\
      Om kolumnen är sorterad i stigande ordning visas en uppåtpil bredvid kolumnnamnet i kolumnrubriken. Om du vill ändra ordningen (till fallande) klickar du på den relevanta kolumnrubriken (då visas en nedåtpil bredvid kolumnnamnet).

   * Ändringar som du gör i sorteringsordningen för objekten är bara de sista medan du är kvar på sidan Alla objekt. Om du navigerar bort från sidan Alla objekt och återgår till den senare, listas objekten igen i den omvända kronologiska standardordningen.

## Visa en korrektursammanfattning

Så här visar du mer detaljerad information om ett korrektur:

1. Klicka på pilen till vänster om korrekturbilden.\
   Pilen pekar nedåt och korrektursammanfattningen visas under den grundläggande informationen om korrekturet. I korthet:

   * **Korrektursammanfattning**: Korrekturens övergripande status
   * **Steg**: Anger deadline för korrektur och antalet beslut som fattas och krävs
   * **Granskare**: Namn, roll och förlopp för varje granskare visas
   * **Versioner**: Versionen av det korrektur som visas och det totala antalet tillgängliga versioner
   * **Mapp**: Mappen där korrekturet finns
   * **Läge**: Aktiv, Låst, Utkast eller Skickat

1. (Valfritt) Om du har redigeringsbehörighet för korrekturet och korrekturet har faser klickar du på menyn **[!UICONTROL More]** (tre punkter) till höger om scenen för att få tillgång till följande alternativ:

   * **[!UICONTROL Message all]**: Skicka e-post till alla granskare på scenen.
   * **[!UICONTROL Share]**: Lägg till nya granskare
   * **[!UICONTROL Delete stage]**

1. (Valfritt) Klicka på en granskares **[!UICONTROL More]**-meny (tre punkter) till höger om namnet om du vill göra något av följande:

   * Skicka en påminnelse till granskaren.
   * Redigera granskarens inställningar på korrekturet.\

     I rutan Redigera granskare som visas kan du ändra både roll- och e-postvarningar och visningsnamnet för granskaren. Observera att visningsnamnet bara kan ändras på det aktuella korrekturet, inte i granskarens information på sidan Kontakter. Mer information finns i [Kontakter](https://support.workfront.com/hc/en-us/sections/115000920808-Contacts).

   * Välj granskaren som ska vara primär beslutsfattare på korrekturet.
   * Ta bort granskaren från korrekturet.
   * Du kan också ändra rollmeddelanden och e-postaviseringar för en granskare som har lagts till i korrekturet.

## Inkludera och exkludera arkiverade korrektur

I vyn [!UICONTROL All Items] visas som standard alla aktiva och låsta korrektur, filer och mappar. Här finns också möjlighet att inkludera eller exkludera arkiverade korrektur i vyn.\
Så här inkluderar du arkiverade korrektur:

1. Klicka på **[!UICONTROL Include archived proofs]** när du väljer en vy.\
   ![Views-include_archived_proofs.png](assets/views-include-archived-proofs-350x188.png)\
   Arkiverade korrektur visas med en arkiverad ikon för att skilja dem från andra korrektur.\
   ![Views-Archived_icon.png](assets/views-archived-icon.png)

## Öppna ett objekt från en listvy

1. Gör något av följande:

   * Om du vill visa information om ett korrektur, en fil eller en mapp klickar du på dess namn.
   * Om du vill öppna ett korrektur i korrekturläsaren klickar du på **[!UICONTROL Go to Proof]**.\

     Mer information om korrekturläsaren finns i [Granska ett korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Utföra åtgärder på flera objekt

Så här markerar du flera objekt:

1. Klicka i kryssrutan ovanför listan.\
   ![Vyer-select_all_items_checkbox.png](assets/views-select-all-items-checkbox-350x193.png)

1. Gör något av följande i de extra alternativen som visas ovanför visningslistan för de filer som du har markerat:

   * Klicka på **[!UICONTROL Tags]** om du vill lägga till en tagg i objekten.
   * Klicka på **[!UICONTROL Move to]** om du vill flytta de markerade objekten till en annan mapp (eller flytta objekten från mappen om du väljer (ingen mapp har valts).
   * Klicka på **[!UICONTROL Share selected items]** om du vill dela alla dessa objekt med andra granskare.\

     ![Share_button-small.png](assets/share-button-small.png)

   * Klicka på **[!UICONTROL Delete]** om du vill flytta de markerade objekten till papperskorgen.\

     ![Trash_button.png](assets/trash-button.png)

   * Klicka på menyn **[!UICONTROL More]** om du vill se fler tillgängliga åtgärder.

   * Åtgärderna tillämpas bara på de av de markerade objekten som har det särskilda alternativet tillgängligt. Om du t.ex. markerar filer och korrektur och väljer [!UICONTROL Lock] låses bara korrektur (eftersom du inte kan låsa filer)

## Flytta ett objekt till en mapp

Om du har redigeringsbehörighet att göra det kan du flytta korrektur, filer och mappar till specifika mappar på sidan [!UICONTROL Views].

1. Öppna mappträdet i sidlisten genom att klicka på pilen till vänster om mappen längst upp.
1. Gör något av följande:

   * Om du vill flytta ett objekt klickar du och håller ned det, drar och släpper det i den mapp där du vill placera det.
   * Om du vill flytta flera objekt samtidigt kan du markera kryssrutorna till vänster om objekten, klicka på **[!UICONTROL Move to]**ovanför listan och sedan markera den mapp där du vill placera dem eller skapa en ny mapp för dem.

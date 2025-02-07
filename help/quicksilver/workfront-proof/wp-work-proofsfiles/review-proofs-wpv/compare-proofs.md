---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: Jämför korrektur i korrekturläsaren
description: Du kan visa jämförelser sida vid sida av två korrektur. Det kan vara två versioner av samma korrektur eller två helt separata korrektur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 0%

---

# Jämför korrektur i korrekturläsaren

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan visa jämförelser sida vid sida av två korrektur. Det kan vara två versioner av samma korrektur eller två helt separata korrektur.

## Jämför korrekturversioner {#compare-proof-versions}

1. Öppna korrekturet med flera versioner som du vill jämföra.
1. Klicka på korrekturets namn i det övre vänstra hörnet i det korrekturläsare som visas. Klicka sedan på ikonen **Jämför** bredvid den version du vill öppna och jämföra i listan över versioner som visas.

   ![Jämför korrektur och välj version](assets/compare-proofs-choose-version-350x115.jpg)

   Språkversionerna visas sida vid sida, med den nyare versionen till vänster.

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. Fortsätt med [Använd jämförelseverktygen](#use-the-compare-tools).

## Jämför separata korrektur {#compare-separate-proofs}

Du kan jämföra två separata korrektur.

* [Jämför separata korrektur i  [!DNL Workfront]](#compare-separate-proofs-in-workfront)
* [Jämför separata korrektur i  [!DNL Workfront Proof]](#compare-separate-proofs-in-workfront-proof)

### Jämför separata korrektur i [!DNL Workfront] {#compare-separate-proofs-in-workfront}

Mer information om hur du jämför separata korrektur från dokumentlistan i [!DNL Workfront] finns i avsnittet [Jämför två olika korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list) i artikeln [Jämför korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

### Jämför separata korrektur i [!DNL Workfront Proof] {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>De korrektur du jämför måste finnas i samma mapp och på samma hierarkinivå i mappstrukturen. Mer information om hur du använder mappar för att gruppera korrektur som du vill jämföra finns i [Arbeta med flera korrektur i korrekturläsaren](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)

1. Öppna ett av de korrektur som du vill jämföra i korrekturläsaren.
1. Klicka på ikonen **[!UICONTROL Compare Mode]**.

   ![proof_compare_icon.png](assets/proof-compare-icon.png)\
   Visningsområdet delas upp i två delar och korrekturet visas både till vänster och till höger om korrekturläsaren.

   ![Compare_proofs-versions.png](assets/compare-proofs-versions-350x180.png)

1. Klicka på ikonen [!UICONTROL folder] ovanför korrekturet till vänster eller höger om du vill visa de andra korrekturen i samma mapp.

   ![Folder_icons_when_comparing_in_proofing_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. Klicka i listan på namnet på det korrektur som du vill jämföra med det korrektur som är öppet i korrekturläsaren.

   ![Comparing_proofs-list_of_proofs_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   Båda korrektur visas.

1. Fortsätt med [Använd jämförelseverktygen](#use-the-compare-tools).

## Använda jämförelseverktygen {#use-the-compare-tools}

Språkvisningsprogrammet har olika verktyg för att jämföra korrektur effektivt.

* [Jämför korrektur automatiskt](#auto-compare-proofs)
* [Jämför korrektur i en övertäckning](#compare-proofs-in-an-overlay)
* [Samtidig navigeringsjämförelse](#simultaneous-navigation-comparison)

### Jämför korrektur automatiskt {#auto-compare-proofs}

Vid automatisk jämförelse görs en pixel-för-pixel-jämförelse mellan två statiska korrektur eller videoklipp. Eventuella skillnader som upptäcks markeras med rött i korrekturet till vänster.

Automatisk jämförelse är inte tillgängligt när du jämför interaktiva korrektur.

Så här jämför du två korrektur automatiskt:

1. Börja jämföra korrektur på något av följande sätt:

   * Jämför två versioner av samma korrektur (se [Jämför korrekturversioner](#compare-proof-versions) i den här artikeln).
   * Jämför två separata korrektur (se [Jämför separata korrektur](#compare-separate-proofs) i den här artikeln).

1. Klicka på ikonen **[!UICONTROL Autocompare]**.

   ![proof_autocompare_icon.png](assets/proof-autocompare-icon-31x32.png)

   Eventuella skillnader mellan de två korrekturen markeras med rött i korrekturet till vänster.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch]** om du vill ändra den aktiva sidan så att skillnader visas på korrekturet till höger. Som standard visas skillnader i korrekturet på den vänstra sidan.

   ![proof_autocompare_changeactive.png](assets/proof-autocompare-changeactive.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Color]** om du vill ändra färg och opacitet som används när skillnaderna ska markeras.

   ![proof_compare_color.png](assets/proof-compare-color.png)

### Jämför korrektur i en övertäckning {#compare-proofs-in-an-overlay}

Med hjälp av en jämförelse av övertäckningar kan du visa skillnader mellan två statiska korrektur genom att visa de två korrektur som ett enda korrektur, samtidigt som du får en lodrät avdelare nedåt i mitten av korrekturet. När du panorerar korrekturet över den lodräta avgränsaren visas skillnaderna.

>[!NOTE]
>
>Övertäckningsjämförelse är inte tillgängligt när du jämför video eller interaktiva korrektur.

Så här aktiverar du jämförelse av övertäckning:

1. Börja jämföra korrektur på något av följande sätt:

   * Jämför två versioner av samma korrektur (se [Jämför korrekturversioner](#compare-proof-versions) i den här artikeln).
   * Jämför två separata korrektur (se [Jämför separata korrektur](#compare-separate-proofs) i den här artikeln).

1. Klicka på ikonen **[!UICONTROL Overlay]**.

   ![proof_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   De två korrekturen visas som ett enda korrektur med en lodrät avdelare nedåt i mitten av korrekturet.

1. Gör något av följande:

   * Panorera korrekturet över den lodräta avgränsaren. När du panorerar ser du korrekturet till vänster på den lodräta delarens vänstra sida, medan korrekturet till höger visas på den högra sidan.
   * Flytta den lodräta avgränsaren åt vänster och höger. När du flyttar avgränsaren ser du korrekturet till vänster på den lodräta delarens vänstra sida, medan korrekturet till höger visas på den högra sidan.

### Samtidig navigeringsjämförelse {#simultaneous-navigation-comparison}

Samtidig navigering är aktiverat som standard när korrektur jämförs. Det är tillgängligt när du jämför ett statiskt korrektur och ett statiskt korrektur, eller när du jämför ett videokorrektur och ett videokorrektur. Det är inte tillgängligt när du jämför ett statiskt korrektur och ett videoklipp.

**Statiska korrektur:** När det är aktiverat för statiskt korrektur låses zoomnivån och positionen för de två korrektur när du panorerar eller rullar samtidigt. När ett korrektur innehåller flera sidor och samtidig navigering är aktiverat, ändras sidan i det andra korrekturet om sidorna ändras i ett korrektur.

**Videokorrektur:** När det är aktiverat på videoklipp kommer samtidig navigering att komma ihåg tidsskillnaden på tidslinjerna för de två korrektur.

Så här aktiverar du samtidig navigering om den inte redan är aktiverad:

1. Börja jämföra korrektur på något av följande sätt:

   * Jämför två versioner av samma korrektur (se [Jämför korrekturversioner](#compare-proof-versions) i den här artikeln).
   * Jämför två separata korrektur (se [Jämför separata korrektur](#compare-separate-proofs) i den här artikeln).

1. Klicka på ikonen **[!UICONTROL Simultaneous Navigation]**.

   ![proof_compare_samtidig_icon.png](assets/proof-compare-simultaneous-icon.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Reset]** när du vill återställa zoomnivån och placeringen (för statiskt korrektur) eller tidslinjen (för videokorrektur).

   ![proof_compare_samtidig_reset.png](assets/proof-compare-simultaneous-reset.png)

## Avsluta jämförelseläge

1. Stäng korrekturet som du inte längre vill visa genom att klicka på ikonen (x) i det övre vänstra hörnet av korrekturet.

   ![proof_compare_exit.png](assets/proof-compare-exit-350x163.png)

   Beviset som du inte stänger är öppet i korrekturläsaren.

---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Vanliga frågor om miljökampanjer
description: Frågor och svar om Workfront marknadsföring.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Vanliga frågor om miljökampanjer

Följande frågor ställs ofta om miljökampanjer:

## Stöds korsdomänsmarknadsföring?

### Svar

Marknadsföring över domäner stöds inte för närvarande. Du måste uppgradera mellan miljöer i samma domän.—>

<!--DELETE THIS SECTION MARCH 2026-->

<!--## Is the Adobe Business Platform / IMS a prerequisite for environment promotion?

### Answer

No. Environment Promotion is available for both IMS-enabled and non-IMS Workfront instances.-->

## Hur kan vi ta reda på om Workfront finns i en licens för Prime eller Ultimate?

### Svar

* En Workfront-administratör kan hitta din organisations licens.

   1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
   1. Klicka på **System** i den vänstra panelen
   1. Om du vill visa din Workfront-plan väljer du **licenser**.
Din plan visas i det övre högra hörnet på sidan.
      ![Hitta plan](assets/locate-plan.png)

  eller
* Kontakta din Workfront-kontorepresentant.

## Är miljökampanjen dubbelriktad?

### Svar

Ja. Du kan till exempel befordra från Sandox till Production eller från Production till Sandbox.

## Stöds delning?

### Svar

Nej, delning stöds inte för närvarande.

## Är paketåterställning tillgängligt?

### Svar

Paketåterställningen är tillgänglig för det senaste paketet inom 24 timmar efter paketinstallationen.

## Finns det något alternativ för att hoppa över befordran av enskilda komponenter? Var alternativen `Use Existing`, `Overwrite` och `Save with a new Name` finns, kan `Skip` läggas till så att du kan hoppa över befordran av enskilda parametrar?

### Svar

* &quot;Använd befintlig&quot; är detsamma som att&quot;hoppa över&quot; eller ignorera distributionen, eftersom den mappar till det befintliga objektet i målmiljön och inte gör några ändringar.
* Om du vill hoppa över objekt rekommenderar vi att du tar bort objekt som du inte vill installera från erbjudandepaketet eller från källmiljön direkt. När du har tagit bort objekten sätter du ihop paketet igen.

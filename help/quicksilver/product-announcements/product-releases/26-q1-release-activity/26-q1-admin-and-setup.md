---
title: Förbättringar av första kvartalet 2026 för administratörer
description: Förbättringar av första kvartalet 2026 för administratörer
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 5a1af10b7e3e59eb203c0507aeea15db5689e24b
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Förbättringar av första kvartalet 2026 för administratörer

Den här sidan beskriver administratörsförbättringar som gjorts i första utgåvan av kvartalet 2026 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den första utgåvan av kvartal 2026 finns i [Översikt över utgåvan första kvartalet 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Hantera prioriteringar i layoutmallen

>[!NOTE]
>
>Den här funktionen är inte tillgänglig för tillfället i förhandsvisningsmiljön
>Förhandsgranska: 2 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026


Du kan nu aktivera eller inaktivera prioriteter för specifika användare i layoutmallen. Om du tidigare har inaktiverat prioriteter för din organisation förblir den inaktiverad i layoutmallen med den här ändringen.

Prioriteringarna inkluderas automatiskt för licenstyper som har standardbehörighet för begäranden. En Contributor-licens kommer som standard att visa begäranden, anslagstavlor och prioriteter på huvudmenyn, medan en extern licens endast kommer att visa dokument och anslagstavlor eftersom den inte har tillgång till begäranden om att visa eller skicka.


Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Kontrollera om det finns flera formulärkonflikter för beräknade anpassade fält

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Samma beräkningsfält kan ha olika formler när de kopplas till olika anpassade formulär. Om två eller flera formulär som innehåller samma beräkningsfält är kopplade till ett objekt, måste formlerna vara identiska i alla formulären. Det är inte tillåtet att redigera formeln om ändringen kan orsaka en konflikt.

Vi har lagt till ett alternativ för att kontrollera om det finns konflikter, så att du kan se vilka objekt som kan påverkas när du redigerar ett uttryck i anpassade fält. I den här dialogrutan visas alla objekt som kan påverkas av att formeln ändras, grupperade efter objekttyp. Du kan navigera till informationen för varje objekt och granska fälten för att bestämma om fältet ska tas bort från något av formulären eller om uttrycket ska förbli oförändrat.

Mer information finns i [Lägga till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Anmälningsdatum och Anges av ID som lagras på anpassade objekt

>[!NOTE]
>
>Förhandsgranska: 13 november 2025
>Production fast release: 13 november 2025
>Produktion för alla: 13 november 2025

Anmälningsdatumet och det angivna ID:t lagras nu i anpassade formulär, fält och avsnitt. Du kan använda dessa dataalternativ i rapporter som filter, vyer eller grupperingar. Om du vill visa dem i listan med anpassade formulär, fält eller avsnitt i installationsprogrammet lägger du till anmälningsdatum och anges av: Namnge som kolumner i en ny eller befintlig vy.

>[!NOTE]
>
>Anmälningsdatumet och det angivna ID:t är bara tillgängligt för anpassade formulär, fält och avsnitt som skapades den 13 november 2025 eller senare.

## Uppdateringar av knappnamn vid redigering av en layoutmall

>[!NOTE]
>
>Förhandsgranska: 30 oktober 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

För att skapa större enhetlighet med andra områden i installationsprogrammet, t.ex. den anpassade formulärdesignern, har knapparna som visas när du redigerar en layoutmall ändrats till **Använd**, **Spara och stäng** och **Avbryt**. Med det nya alternativet **Använd** kan du spara ändringarna i layoutmallen och fortsätta redigera. Tidigare var de tillgängliga alternativen **Spara** och **Avbryt**.

Mer information finns i [Skapa och hantera layoutmallar](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Förbättrad fälthantering med aktiv flagga i anpassade fält

>[!NOTE]
>
>Förhandsgranska: 30 oktober 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

När du har ett stort antal anpassade fält i systemet kan det vara svårt att hantera dessa fält i anpassade formulär och rapporter. Du kan nu markera anpassade fält som inaktiva med den nya flaggan **Aktiv**. Den här flaggan är tillgänglig när du arbetar med ett fält i ett anpassat formulär eller när du lägger till eller redigerar ett fält från fältlistan.

Om du markerar ett fält som inaktivt:

* Den tas inte med i rapporter, filter, vyer eller på andra ställen i Workfront där du kan lägga till ett eget fält
* Det är inte tillgängligt i fältbiblioteket att lägga till i andra anpassade formulär

>[!NOTE]
>
>Uteslutningen från rapporter, filter, vyer och grupperingar sker när fältet har inaktiverats. Befintliga rapportelement som använder fältet ändras eller tas inte bort när fältet har markerats som inaktivt.

Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).





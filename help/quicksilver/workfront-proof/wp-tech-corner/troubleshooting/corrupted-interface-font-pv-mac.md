---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Felsökning - skadat gränssnittsteckensnitt i korrekturläsare på Mac
description: Felsöka skadat gränssnittsteckensnitt i korrekturläsaren i Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Felsökning - skadat gränssnittsteckensnitt i korrekturläsare på Mac

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du märker att korrekturläsaren inte visar gränssnittsteckensnitt på rätt sätt kan det bero på vissa problem med teckensnitten på din Mac-dator. Du kan lösa problemet genom att försöka med följande lösningar:

## Ta bort teckensnittsdubbletter

Kontrollera om det finns några dubbletter av teckensnitt i systemet.

1. Stäng webbläsaren som du använder.
1. Öppna programmet Teckensnittsbok i mappen Program.
1. Klicka **[!UICONTROL All Fonts]** (1)
1. Klicka på **[!UICONTROL Edit]** > **[!UICONTROL Look for Enabled Duplicates]**.

1. Klicka **[!UICONTROL Yes]** för att lösa dubbletter.
1. Om du ser en varning om skadade teckensnitt klickar du på **[!UICONTROL Yes]**.
1. Starta om datorn.
1. Försök med korrekturet igen.

## Rensa teckensnittscachen

Ibland blir cacheminnen för teckensnitt i Mac OS X skadade. Om ett teckensnitt eller en teckensnittsfamilj installeras om ett antal gånger eller om ett program har uppdaterats eller installerats om. Förutom teckensnittscachefilerna i operativsystemet kan vissa program ha en egen teckensnittscache. Om du tar bort de här teckensnittscachefilerna kan du lösa problem med felaktig text.

Först måste du starta Teckensnittsbok, välja det teckensnitt eller den familj som du har problem med och sedan trycka på knappen Ta bort på tangentbordet. Du kan också högerklicka och välja [!UICONTROL Remove Family]. Om du är osäker på vilket teckensnitt eller vilken familj som orsakar problemen kan du prova att först ta bort dubbletter enligt beskrivningen ovan.

Det andra steget är att rensa teckensnittscachen och det finns flera sätt att uppnå detta.

Det första är att helt enkelt starta om i felsäkert läge genom att hålla ned Skift-tangenten omedelbart när du hör startchimerna vid start. När det här läget läses in bör en förloppsindikator visas, där systemet kör olika kontroller- och underhållsrutiner, varav en är att rensa teckensnittscachen.

Det andra sättet är att använda terminalen, vilket kan göras genom att köra följande kommando från ett administratörskonto: *sudo atsutil databaser -remove*

>[!NOTE]
>
>Det här kommandot kräver att du anger ditt lösenord, som inte visas när du skriver. Vi rekommenderar att du kontaktar din IT-avdelning eftersom det kan kräva administratörsbehörighet på din dator.

Ett annat sätt är att använda ett teckensnittscache-verktyg som t.ex. FontNuke och rensa cacheminnet med hjälp av det.

Många prepress- och designstudior använder också Universal Type Server för att hantera licensiering och distribution av teckensnitt. Ibland kan ett problem uppstå med Universal Type Server-teckensnittscachen, vilket kan orsaka [!DNL Workfront Proof] anteckningar som ska försvinna.

Åtgärda problemet genom att rensa Universell Type Server-teckensnittscachen och starta om Universal Type Server.

## Korrigera [!DNL Flash] teckensnittskonflikt

Du kanske inte har åtkomst till den här funktionen eftersom den stöds av [!DNL Flash], som har tagits bort i de flesta miljöer.

Det äldre korrekturläsaren baseras på [!DNL Flash Player] och ibland kan det finnas en teckensnittskonflikt mellan OS X och [!DNL Flash Player]. Försök med följande:

1. Öppna Finder och öppna **[!UICONTROL Go]** -fliken.
1. Tryck på Option-tangenten ( ⌥ Alt) för att öppna [!UICONTROL Library] i listrutan.
1. Håll ned Option-tangenten och klicka på [!UICONTROL Library] mapp.
1. Efter [!UICONTROL Library] mapp öppnas, gå till [!UICONTROL Fonts] i.
1. Flytta alla teckensnitt som finns i [!UICONTROL Fonts] till en annan mapp, kanske på skrivbordet (skapa inte en annan mapp i mappen Fonts).
1. Den här åtgärden döljer alla anpassade teckensnitt. Du bör fortfarande ha standardsystemteckensnitten sparade på sin separata plats.
1. Avsluta och starta om [!DNL Safari].
1. Öppna korrekturet igen.

Du borde se teckensnitten nu. Om du inte behöver något av teckensnitten som du har tagit bort från din arbetskatalog kan du ta bort dem. Annars går du igenom dem gruppvis, kopierar dem tillbaka till mappen Bibliotek/Teckensnitt och ser vilken som orsakar problemet.
